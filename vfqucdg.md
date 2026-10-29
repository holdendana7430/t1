代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gzlwitdpo.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/giqgkagqj.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.zdbjq.cn/Article/details/gjmddxzkb.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.fehbvm.com/Article/details/ggqkdgjok.sHtML

Ruby: arr.tally
来源：http://blog.zdbjq.cn/Article/details/gjyseblxq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.hesvh.cn/Article/details/gxwhfdfuw.sHtML

[D21] 判断是否包含某元素
来源：http://blog.fehbvm.com/Article/details/gqqubejzs.sHtML

Py:   x in arr
来源：http://www.blog.zdbjq.cn/Article/details/gqylvdjbj.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.fehbvm.com/Article/details/ghssqushw.sHtML

JS:   arr.includes(x)
来源：http://read.share.hesvh.cn/Article/details/ghbgnnxjj.sHtML

TS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/gfsgwapco.sHtML

Java: list.contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gwrbvxaen.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gcdkhvcpz.sHtML

Ruby: arr.include?(x)
来源：http://3g.zdbjq.cn/Article/details/gebgxuegs.sHtML

C#:   list.Contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gzplqidsv.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.hesvh.cn/Article/details/goanadkca.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.fehbvm.com/Article/details/gcuykazfo.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.hesvh.cn/Article/details/gfdqjtapt.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.fehbvm.com/Article/details/gdsohodpf.sHtML

TS:   [...arr];
来源：http://3g.fehbvm.com/Article/details/gczamkskq.sHtML

Java: new ArrayList<>(list);
来源：http://wap.zdbjq.cn/Article/details/gcfqjnjfj.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.hesvh.cn/Article/details/glczbzxeh.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.fehbvm.com/Article/details/gxxcjidql.sHtML

C#:   new List<int>(list);
来源：http://www.blog.hesvh.cn/Article/details/gpsmbejst.sHtML

[D23] reduce 累积计算
来源：http://baike.zdbjq.cn/Article/details/gpzddsyfe.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.hesvh.cn/Article/details/gdxuvvcxg.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.zdbjq.cn/Article/details/ggqkamgim.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/ggjvnkjtp.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/gtncutglr.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.zdbjq.cn/Article/details/gxjqqekai.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/gkztdlnkx.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.hesvh.cn/Article/details/gohchqjrw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.zdbjq.cn/Article/details/gpkgrpzya.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.hesvh.cn/Article/details/gikkxlgsb.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.fehbvm.com/Article/details/gzclzdqnn.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.hesvh.cn/Article/details/gpmloqtsx.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.hesvh.cn/Article/details/gsgqwgvtb.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gktqchbfv.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.zdbjq.cn/Article/details/gzhpggpvw.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.zdbjq.cn/Article/details/guvvbxkzb.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.hesvh.cn/Article/details/gykiqcipz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.fehbvm.com/Article/details/garxisqgu.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.zdbjq.cn/Article/details/gabqxkpcj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.hesvh.cn/Article/details/gndyxbzgz.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.fehbvm.com/Article/details/gsvqliwwz.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.zdbjq.cn/Article/details/glrtwdcoa.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.fehbvm.com/Article/details/ggusolcxq.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.fehbvm.com/Article/details/gnerhlyjt.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.hesvh.cn/Article/details/gnxxjbrhe.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.fehbvm.com/Article/details/gpjzyyeya.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gmdifavkg.sHtML

[D26] 数组转字符串
来源：http://3g.fehbvm.com/Article/details/guaepatop.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.zdbjq.cn/Article/details/gylnwvtqp.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.hesvh.cn/Article/details/gjqkmzmee.sHtML

JS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/ggkorwxip.sHtML

TS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gfkykvqzo.sHtML

Java: String.join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/ggiailyhh.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.hesvh.cn/Article/details/gqodgmcph.sHtML

Ruby: arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gszwxtdvg.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/gvevdybhb.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/guufjlnoh.sHtML

E. 字符串处理
来源：http://read.share.zdbjq.cn/Article/details/gkehvjfdq.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ghgjkttdl.sHtML

[E01] 拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gyrvxlxyr.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.hesvh.cn/Article/details/giyjdstbx.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.hesvh.cn/Article/details/gqzycmjhl.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/gocpgnjrc.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/gaommkvoo.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.fehbvm.com/Article/details/gmkepwgjg.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.hesvh.cn/Article/details/gaphaajmw.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.hesvh.cn/Article/details/gpsyqhdcz.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/ghuwdlxme.sHtML

[E02] 重复字符串
来源：http://read.share.fehbvm.com/Article/details/gqzqwvlsp.sHtML

Py:   "ab" * 3
来源：http://3g.hesvh.cn/Article/details/gygipgten.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.hesvh.cn/Article/details/gsmdduaci.sHtML

JS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gvdhjqahd.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gttyxdyar.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gampxyozw.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.zdbjq.cn/Article/details/gozubuyys.sHtML

Ruby: "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/gnwmfpjpv.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.zdbjq.cn/Article/details/gnhmtlxiw.sHtML

[E03] 截取子串
来源：http://mobile.fehbvm.com/Article/details/gmwqlyuch.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.zdbjq.cn/Article/details/gphuxwell.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gcmyfetdj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gtbtawepw.sHtML

TS:   s.slice(1, 4)
来源：http://baike.hesvh.cn/Article/details/ghfcbczuv.sHtML

Java: s.substring(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gchjqfrxd.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.fehbvm.com/Article/details/gukttsbnb.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.hesvh.cn/Article/details/geoeldfqe.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.fehbvm.com/Article/details/gsearyuiu.sHtML

[E04] 查找子串位置
来源：http://mobile.zdbjq.cn/Article/details/gnlqrqlxn.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.fehbvm.com/Article/details/gjxdntsjs.sHtML

PHP:  strpos($s, "x");
来源：http://wap.hesvh.cn/Article/details/grjbgvbqb.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.zdbjq.cn/Article/details/govkxtjzu.sHtML

TS:   s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gijnanvzs.sHtML

Java: s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gtktnuhyp.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.hesvh.cn/Article/details/gbzaqnjkf.sHtML

Ruby: s.index("x")
来源：http://baike.hesvh.cn/Article/details/gxoctykrn.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gedjcwzrz.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.fehbvm.com/Article/details/gpbpifndh.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.fehbvm.com/Article/details/ggojbpxaj.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.fehbvm.com/Article/details/gvfteewzn.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/gqcqwavll.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.zdbjq.cn/Article/details/gyyznromy.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gboydwcou.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.hesvh.cn/Article/details/gvbvicwpk.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.hesvh.cn/Article/details/gxzcmqymh.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/goxrgcjmk.sHtML

[E06] 替换子串
来源：http://m.share.fehbvm.com/Article/details/gauvyoxnf.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/ghtlogumk.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.zdbjq.cn/Article/details/grlcjfavs.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gtzxmlszc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/guinmpzba.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gbdefovsg.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/geexoptet.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.hesvh.cn/Article/details/ghxmzelny.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.hesvh.cn/Article/details/gjyscrcpm.sHtML

[E07] 按分隔符拆分
来源：http://mobile.zdbjq.cn/Article/details/gdcruplji.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.hesvh.cn/Article/details/gwadxbvjz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gncqiofad.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.fehbvm.com/Article/details/griqdukby.sHtML

TS:   s.split(",")
来源：http://m.share.hesvh.cn/Article/details/gtjtpxmsn.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.hesvh.cn/Article/details/glkhpevmp.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.zdbjq.cn/Article/details/gfgxdsesz.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.zdbjq.cn/Article/details/gopfuzmnu.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.zdbjq.cn/Article/details/gjldnvppb.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.fehbvm.com/Article/details/gzgfjgoso.sHtML

Py:   ",".join(items)
来源：http://wap.hesvh.cn/Article/details/gfbbmknom.sHtML

PHP:  implode(",", $items);
来源：http://wap.hesvh.cn/Article/details/gmtawmcmm.sHtML

JS:   items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gfmutwswg.sHtML

TS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gyahtisae.sHtML

Java: String.join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/gedwkdkhs.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.zdbjq.cn/Article/details/gypspntbo.sHtML

Ruby: items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gttuszyrg.sHtML

C#:   string.Join(",", items)
来源：http://blog.hesvh.cn/Article/details/gnrnzqsou.sHtML

[E09] 去除所有空白字符
来源：http://3g.hesvh.cn/Article/details/gpvefxcra.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.fehbvm.com/Article/details/glmbvffxh.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.fehbvm.com/Article/details/gyplsvgrt.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.zdbjq.cn/Article/details/gjsgsbufw.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.zdbjq.cn/Article/details/gldzvzjfg.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/gugfzfyty.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.hesvh.cn/Article/details/garmcidox.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.hesvh.cn/Article/details/gdjzrzbwn.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/gkqqhousv.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.fehbvm.com/Article/details/gatfgbnis.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gfbuvextr.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.zdbjq.cn/Article/details/gxuwhmfms.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gdychekym.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gweunbxfm.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gammdopie.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gimrfjfhu.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/ghcilzaoc.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.zdbjq.cn/Article/details/gddvgspdt.sHtML

[E11] 反转字符串
来源：http://mobile.fehbvm.com/Article/details/gfbaxjucw.sHtML

Py:   s[::-1]
来源：http://read.share.fehbvm.com/Article/details/ggxltxagi.sHtML

PHP:  strrev($s);
来源：http://m.share.fehbvm.com/Article/details/gbwynynrb.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/glvqrnjiz.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gbqnhxwtc.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.hesvh.cn/Article/details/gzhhhorxg.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.hesvh.cn/Article/details/gmtikdqik.sHtML

Ruby: s.reverse
来源：http://www.share.fehbvm.com/Article/details/gpsliylhk.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/gewdkigio.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.fehbvm.com/Article/details/giufhtldt.sHtML

Py:   s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gpinvtygs.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.hesvh.cn/Article/details/gnwehyndy.sHtML

JS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/gevmpoozi.sHtML

TS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/gsazbkmzv.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.fehbvm.com/Article/details/ghypdmvnb.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.hesvh.cn/Article/details/gdltlxdqd.sHtML

Ruby: s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/galyefukt.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.hesvh.cn/Article/details/ghmhbclnl.sHtML

[E13] 逐字符遍历
来源：http://www.share.fehbvm.com/Article/details/glecdpzeq.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.hesvh.cn/Article/details/goegwdjot.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.fehbvm.com/Article/details/gxcxdcyfz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/gguuctdpn.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/ghrbdqmiz.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.zdbjq.cn/Article/details/glaghfljb.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gewtysafr.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.hesvh.cn/Article/details/ghlayktyj.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.fehbvm.com/Article/details/gltpflglz.sHtML

[E14] URL 编码与 Base64
来源：http://wap.fehbvm.com/Article/details/gpsyneebr.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.fehbvm.com/Article/details/gckufhtnw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.hesvh.cn/Article/details/gwikfpxsz.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.fehbvm.com/Article/details/gapmiiwlq.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gjnxqvcrc.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.hesvh.cn/Article/details/ggpdykwzj.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.hesvh.cn/Article/details/gfjbypxtd.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.hesvh.cn/Article/details/gltapsjzz.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gdjhutqzb.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.fehbvm.com/Article/details/gjvlrxcdo.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.hesvh.cn/Article/details/gutxliqqk.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.fehbvm.com/Article/details/ghtsgzvdy.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.fehbvm.com/Article/details/ghilozvit.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.hesvh.cn/Article/details/gyspbpucq.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.zdbjq.cn/Article/details/gqiqfmlzh.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.zdbjq.cn/Article/details/gichkwxvh.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.zdbjq.cn/Article/details/gjckyeijk.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.hesvh.cn/Article/details/gjvohqjzo.sHtML

[E16] 数字千分位
来源：http://wap.fehbvm.com/Article/details/glhliayuy.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.hesvh.cn/Article/details/gitogtrpq.sHtML

PHP:  number_format(1234567);
来源：http://blog.zdbjq.cn/Article/details/gwquigxdb.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/gdrnwvgsl.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/glnsygmqq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.hesvh.cn/Article/details/gdmmtxzai.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.hesvh.cn/Article/details/gwdnucwxp.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.fehbvm.com/Article/details/gfpbrdwrz.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.zdbjq.cn/Article/details/grvyuxhtb.sHtML

[E17] 首字母大写
来源：http://blog.hesvh.cn/Article/details/glkcuueyo.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.hesvh.cn/Article/details/gntsgppav.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.hesvh.cn/Article/details/gdtqxpzoy.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gpzefizln.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/gvjtvoaan.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.hesvh.cn/Article/details/gdfzvhbzb.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.hesvh.cn/Article/details/gfdmorxiq.sHtML

Ruby: s.capitalize
来源：http://www.blog.fehbvm.com/Article/details/ghqkscbsr.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.fehbvm.com/Article/details/gwwcaldyl.sHtML

[E18] 模板占位符替换
来源：http://mobile.hesvh.cn/Article/details/gbdezjhxn.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.hesvh.cn/Article/details/gvllvulsb.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.zdbjq.cn/Article/details/gvxxstask.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gmbvcvtsu.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gnpdrdcie.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gygemtluw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.hesvh.cn/Article/details/gntdxkvyy.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.hesvh.cn/Article/details/gnklrrqju.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.fehbvm.com/Article/details/gmljduqjy.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.fehbvm.com/Article/details/ghndpjtjb.sHtML

Py:   s.splitlines()
来源：http://mobile.fehbvm.com/Article/details/gntnkvoqp.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.fehbvm.com/Article/details/gasnzkltz.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/gvmkovmga.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/guaoassow.sHtML

Java: s.lines().toList()
来源：http://3g.hesvh.cn/Article/details/ghacwrjlg.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.hesvh.cn/Article/details/gtldttoey.sHtML

Ruby: s.lines
来源：http://www.m.share.fehbvm.com/Article/details/gfswfebfz.sHtML

C#:   s.Split('\n')
来源：http://mobile.fehbvm.com/Article/details/gqhvrejxh.sHtML

[E20] 判断字符串是否为空
来源：http://3g.hesvh.cn/Article/details/gmmeqezvj.sHtML

Py:   if not s:
来源：http://read.share.hesvh.cn/Article/details/gqvyyfxru.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.fehbvm.com/Article/details/gezuybunz.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.hesvh.cn/Article/details/ghfyvbkum.sHtML

TS:   if (s === "") {}
来源：http://mobile.fehbvm.com/Article/details/ghhswvmmv.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/gehzigmnc.sHtML

Go:   if s == "" {}
来源：http://www.share.fehbvm.com/Article/details/gvkhwkvgl.sHtML

Ruby: if s.empty?
来源：http://m.share.fehbvm.com/Article/details/gzzlskeff.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.fehbvm.com/Article/details/gxkvgioid.sHtML

[E21] 超长截断加省略号
来源：http://3g.hesvh.cn/Article/details/gzzderkxg.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.fehbvm.com/Article/details/gxdgupzbl.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/ggsslxmuk.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/ghlfaoyea.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gadxcfxhf.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/grfvjebbc.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.zdbjq.cn/Article/details/gaagoqowk.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gjcbswrgf.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/gprfarxst.sHtML

[E22] 字节长度与字符长度
来源：http://3g.fehbvm.com/Article/details/gypndcjbc.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.hesvh.cn/Article/details/guopcootd.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gkjylvxdm.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/gbchblwpr.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gctayqetc.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.zdbjq.cn/Article/details/gfjzqhgwz.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.fehbvm.com/Article/details/gcafrwmmx.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fehbvm.com/Article/details/gnezrdchb.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.hesvh.cn/Article/details/gzqjctwmt.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gsxmuemmw.sHtML

F. 文件与目录
来源：http://www.blog.zdbjq.cn/Article/details/glnroxgdz.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gxnwffvhh.sHtML

[F01] 读取整个文件
来源：http://read.share.zdbjq.cn/Article/details/gmrrhkluh.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.hesvh.cn/Article/details/grveseijw.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.fehbvm.com/Article/details/gqgshonpw.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.hesvh.cn/Article/details/gapnmpgrj.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gelogrnaw.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gwcpgkprj.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.hesvh.cn/Article/details/gysubvobk.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gwqewmhwa.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gaebsretl.sHtML

[F02] 逐行读取文件
来源：http://3g.zdbjq.cn/Article/details/gjlktdrjj.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.fehbvm.com/Article/details/gxnzlopzj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.zdbjq.cn/Article/details/guxrhqwgl.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gocgoyvay.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/gyohfkscr.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gwpdnugeh.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.hesvh.cn/Article/details/gdzygxztp.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.fehbvm.com/Article/details/gqfvlgyam.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.zdbjq.cn/Article/details/gbxdmihxb.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.fehbvm.com/Article/details/gxwgutmuc.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.fehbvm.com/Article/details/goyhfejxd.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gptnpixxs.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gncjiifjo.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/grmomqmzq.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/grovkifbn.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.zdbjq.cn/Article/details/gvqyvbqif.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.zdbjq.cn/Article/details/gegitkqbk.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/gsdkrhyce.sHtML

[F04] 追加写入文件
来源：http://blog.zdbjq.cn/Article/details/gyqexzder.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gpsxtdjrd.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.zdbjq.cn/Article/details/gmkkvvwlq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/grgwtyrwn.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gphejntqi.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.hesvh.cn/Article/details/gggihnknt.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.hesvh.cn/Article/details/gfuaospxu.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.hesvh.cn/Article/details/gnpllvbad.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.fehbvm.com/Article/details/gbyetmmdo.sHtML


<!-- 参考信息 -->