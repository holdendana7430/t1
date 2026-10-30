代发 wailian999

TS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gqjapfgvo.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.zdbjq.cn/Article/details/gdeebfafs.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.fehbvm.com/Article/details/gyaykauvu.sHtML

Ruby: arr.uniq
来源：http://m.share.fehbvm.com/Article/details/gyradskjb.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.fehbvm.com/Article/details/gqmlalrrj.sHtML

[D16] 求和与平均值
来源：http://3g.hesvh.cn/Article/details/ggshwkerm.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.hesvh.cn/Article/details/gjsrefxgz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.hesvh.cn/Article/details/gqtoaczqp.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gwvvexqsx.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fehbvm.com/Article/details/gdyuocked.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.fehbvm.com/Article/details/geqajfqdy.sHtML

Go:   // 手写循环累加
来源：http://baike.fehbvm.com/Article/details/gsgzjzaou.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.fehbvm.com/Article/details/gchwhqkgk.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.fehbvm.com/Article/details/gmpkzfbnm.sHtML

[D17] 最大值与最小值
来源：http://wap.hesvh.cn/Article/details/grpjhbxvw.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.hesvh.cn/Article/details/geejcdfpj.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gqktkfgqb.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.hesvh.cn/Article/details/gjynwsefd.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.hesvh.cn/Article/details/gxvchkxqj.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.hesvh.cn/Article/details/gvcuuxrzg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.hesvh.cn/Article/details/gmrrikecc.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.zdbjq.cn/Article/details/gpwilohqc.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.zdbjq.cn/Article/details/gzamvzwvq.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.hesvh.cn/Article/details/gwhdslqgk.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.hesvh.cn/Article/details/giosqicfm.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.fehbvm.com/Article/details/gklaiisng.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.fehbvm.com/Article/details/gckcwqcjz.sHtML

TS:   nested.flat();
来源：http://www.m.share.hesvh.cn/Article/details/gfxjsujtu.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.fehbvm.com/Article/details/gmrbiyktl.sHtML

Go:   // 手写双层循环
来源：http://blog.hesvh.cn/Article/details/gcafprddr.sHtML

Ruby: nested.flatten
来源：http://baike.zdbjq.cn/Article/details/gurobbfxh.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gsvqfjsqh.sHtML

[D19] 按字段分组
来源：http://www.blog.hesvh.cn/Article/details/giefcqhxf.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.zdbjq.cn/Article/details/gwasdsgct.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.hesvh.cn/Article/details/gumhpxskl.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.hesvh.cn/Article/details/gpmkycqkv.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/gtpzvzrfz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.zdbjq.cn/Article/details/gdnuhtpxm.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.zdbjq.cn/Article/details/gyndimygu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.hesvh.cn/Article/details/gjsljvpoz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.fehbvm.com/Article/details/gyugusoqf.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.zdbjq.cn/Article/details/gucgzzedp.sHtML

Py:   Counter(arr)
来源：http://m.share.zdbjq.cn/Article/details/gkcpcuhgn.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gwexvuair.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/ggeejhawo.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/gdkoclzlu.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.zdbjq.cn/Article/details/giblpqtpl.sHtML

Go:   // 手写 map[T]int
来源：http://3g.hesvh.cn/Article/details/ghwhwuhhs.sHtML

Ruby: arr.tally
来源：http://www.m.share.hesvh.cn/Article/details/gcmyicmgz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.fehbvm.com/Article/details/grptrehrd.sHtML

[D21] 判断是否包含某元素
来源：http://wap.hesvh.cn/Article/details/gfnlnldfm.sHtML

Py:   x in arr
来源：http://3g.hesvh.cn/Article/details/glxcqdhfa.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.fehbvm.com/Article/details/gxbmrbgdm.sHtML

JS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/gcwhaiear.sHtML

TS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gfnhmpudv.sHtML

Java: list.contains(x)
来源：http://blog.fehbvm.com/Article/details/giwmgcfsn.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.fehbvm.com/Article/details/gqotsklbh.sHtML

Ruby: arr.include?(x)
来源：http://baike.hesvh.cn/Article/details/glifkfzve.sHtML

C#:   list.Contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gqghvqhbh.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.zdbjq.cn/Article/details/gblorulbg.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.fehbvm.com/Article/details/guazazqmr.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.zdbjq.cn/Article/details/gczjfguon.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.fehbvm.com/Article/details/gslbucnmf.sHtML

TS:   [...arr];
来源：http://wap.zdbjq.cn/Article/details/grgjfsrwp.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/ggitzicaq.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.zdbjq.cn/Article/details/gogklwqza.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.zdbjq.cn/Article/details/gqvqrpoua.sHtML

C#:   new List<int>(list);
来源：http://www.blog.fehbvm.com/Article/details/gzeihggxg.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.fehbvm.com/Article/details/gctimqgzo.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.zdbjq.cn/Article/details/gmwougqwr.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.hesvh.cn/Article/details/gckhkwfsu.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gvctiaykx.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/ghklsbxly.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.hesvh.cn/Article/details/gedvtgfnu.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/gxginzuzo.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.hesvh.cn/Article/details/gvnljenys.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.hesvh.cn/Article/details/gzgnwuzbj.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.fehbvm.com/Article/details/gemdlpcha.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.zdbjq.cn/Article/details/gxmurwnrt.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.zdbjq.cn/Article/details/gxrledwoo.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.hesvh.cn/Article/details/gsovpcerj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/guvzodwzk.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.fehbvm.com/Article/details/grynbjbrj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.fehbvm.com/Article/details/gzcfhbwyy.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.hesvh.cn/Article/details/gfqykmrgi.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.fehbvm.com/Article/details/gwyekkfph.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.hesvh.cn/Article/details/gkfhbepzv.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.zdbjq.cn/Article/details/gjwpkqwpu.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.zdbjq.cn/Article/details/gmojvthyz.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.hesvh.cn/Article/details/gdyjmjqhf.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.fehbvm.com/Article/details/gxqstcqqk.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.fehbvm.com/Article/details/gqwdaqion.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.hesvh.cn/Article/details/ggoornzez.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.hesvh.cn/Article/details/gmlywxnck.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.zdbjq.cn/Article/details/ghowjqawk.sHtML

[D26] 数组转字符串
来源：http://baike.zdbjq.cn/Article/details/gizllzqrn.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.hesvh.cn/Article/details/giibhlynn.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.fehbvm.com/Article/details/gqayvbdiz.sHtML

JS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gbmkggjlk.sHtML

TS:   arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gvypaaens.sHtML

Java: String.join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/grytkxbpy.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.fehbvm.com/Article/details/ghsdrodhb.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gaslulqqw.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/gpgczzksk.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gqjvccqgi.sHtML

E. 字符串处理
来源：http://www.blog.zdbjq.cn/Article/details/gnprjptwa.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gcbzymixv.sHtML

[E01] 拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gzrttjups.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.hesvh.cn/Article/details/gkzowysjb.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.fehbvm.com/Article/details/gxplzdhhu.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/gmpccpgvy.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gqxzdeynd.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.fehbvm.com/Article/details/gpaezhbdk.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.zdbjq.cn/Article/details/gvbyaxyjk.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.fehbvm.com/Article/details/gswwwmeqo.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.fehbvm.com/Article/details/goqqnecnv.sHtML

[E02] 重复字符串
来源：http://mobile.fehbvm.com/Article/details/goipjpvmf.sHtML

Py:   "ab" * 3
来源：http://blog.fehbvm.com/Article/details/gucuidvyn.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.hesvh.cn/Article/details/gryzpveuk.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/gshylnomx.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gyjbvorrw.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gvvzurebj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.hesvh.cn/Article/details/guluzqxlo.sHtML

Ruby: "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/gkpnvjemo.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.hesvh.cn/Article/details/ggwjyogmz.sHtML

[E03] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/giramtkfx.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.hesvh.cn/Article/details/gsavehfir.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gamiyppfp.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/grejkpnpx.sHtML

TS:   s.slice(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gxvutfxhn.sHtML

Java: s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gwfnumman.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.zdbjq.cn/Article/details/guyodncap.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.hesvh.cn/Article/details/gnhlqvcrd.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.zdbjq.cn/Article/details/gykmdxpcu.sHtML

[E04] 查找子串位置
来源：http://read.share.hesvh.cn/Article/details/gytxabggd.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.hesvh.cn/Article/details/getyiwmgf.sHtML

PHP:  strpos($s, "x");
来源：http://baike.fehbvm.com/Article/details/gvlpnaqdd.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.zdbjq.cn/Article/details/gdnvznxtq.sHtML

TS:   s.indexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gzabkfyhw.sHtML

Java: s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/gsyrnaolk.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.hesvh.cn/Article/details/grtuntyml.sHtML

Ruby: s.index("x")
来源：http://www.blog.zdbjq.cn/Article/details/gdcsrmifn.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gwkopkbij.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.zdbjq.cn/Article/details/gceneihqg.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.hesvh.cn/Article/details/gqoirmbxz.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.fehbvm.com/Article/details/gykswglia.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/ghjwzevnj.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.hesvh.cn/Article/details/gptdggywa.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/granxlglk.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.hesvh.cn/Article/details/gkboltxmr.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.fehbvm.com/Article/details/gzpbkiekn.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gpbrmfboq.sHtML

[E06] 替换子串
来源：http://www.m.share.zdbjq.cn/Article/details/grctmzlva.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/gbzovyptt.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.hesvh.cn/Article/details/gwpsdednw.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/ggrldkwow.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gacetaksp.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/glghhpqmj.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/gpwlpopfb.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.fehbvm.com/Article/details/guvuvicwp.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/guzfahjby.sHtML

[E07] 按分隔符拆分
来源：http://www.share.hesvh.cn/Article/details/gfjpqjxsx.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.zdbjq.cn/Article/details/gpabstocv.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/ggyobweha.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.fehbvm.com/Article/details/gdrsjthdl.sHtML

TS:   s.split(",")
来源：http://3g.zdbjq.cn/Article/details/gsllbwteu.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.zdbjq.cn/Article/details/gepqsrbnq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.fehbvm.com/Article/details/gednhmngf.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.hesvh.cn/Article/details/goaflxfac.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.fehbvm.com/Article/details/gsfgytsxz.sHtML

[E08] 数组按分隔符合并
来源：http://blog.hesvh.cn/Article/details/gbjxheetg.sHtML

Py:   ",".join(items)
来源：http://read.share.fehbvm.com/Article/details/gmmkdyfdl.sHtML

PHP:  implode(",", $items);
来源：http://baike.zdbjq.cn/Article/details/gfdwleoan.sHtML

JS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/gsqmtvtku.sHtML

TS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gqxinetng.sHtML

Java: String.join(",", items)
来源：http://3g.hesvh.cn/Article/details/gsxvsgyxb.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.zdbjq.cn/Article/details/gkjkvaygx.sHtML

Ruby: items.join(",")
来源：http://baike.zdbjq.cn/Article/details/goctukfar.sHtML

C#:   string.Join(",", items)
来源：http://blog.zdbjq.cn/Article/details/gvsalezio.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.zdbjq.cn/Article/details/gvwngnnki.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.hesvh.cn/Article/details/gamavtule.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.fehbvm.com/Article/details/gagfzxcvr.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/gnhqbopwj.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/guqltjcjr.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.fehbvm.com/Article/details/gqycnpibv.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.hesvh.cn/Article/details/gbxyefazi.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.hesvh.cn/Article/details/gykgvfuqk.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.fehbvm.com/Article/details/gnboepbyy.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.fehbvm.com/Article/details/gjxbkueav.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.hesvh.cn/Article/details/gtycmqcqk.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.fehbvm.com/Article/details/gmgjvcceh.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gvhtwpxqr.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gslzvlzpt.sHtML

Java: String.format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gklgizixm.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/grqspizue.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gjwjmnknh.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.hesvh.cn/Article/details/gglulucfw.sHtML

[E11] 反转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gtdagnopx.sHtML

Py:   s[::-1]
来源：http://mobile.fehbvm.com/Article/details/ghmtdtain.sHtML

PHP:  strrev($s);
来源：http://blog.hesvh.cn/Article/details/gkcagnlrg.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gluhpgakj.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gvxpgwxjn.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.zdbjq.cn/Article/details/goxwcghwj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.zdbjq.cn/Article/details/gavejkyyy.sHtML

Ruby: s.reverse
来源：http://m.share.hesvh.cn/Article/details/gtqdfervk.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/guhjxrdjw.sHtML

[E12] 统计某字符出现次数
来源：http://blog.fehbvm.com/Article/details/gvarbohkm.sHtML

Py:   s.count("a")
来源：http://www.share.hesvh.cn/Article/details/gytysnmcq.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.fehbvm.com/Article/details/ggeoshnym.sHtML

JS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/gfrahleiu.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/ghdtujrwm.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.fehbvm.com/Article/details/gmowfzjuq.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.fehbvm.com/Article/details/gjarbtsbz.sHtML

Ruby: s.count("a")
来源：http://read.share.fehbvm.com/Article/details/grtybdhdi.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.hesvh.cn/Article/details/gptsgpymr.sHtML

[E13] 逐字符遍历
来源：http://m.share.zdbjq.cn/Article/details/ggbymqelq.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.fehbvm.com/Article/details/goaxnefmf.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.hesvh.cn/Article/details/gopobvdmr.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.hesvh.cn/Article/details/giacoodgl.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/gizoukoxb.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.zdbjq.cn/Article/details/gzlsgxpkx.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.fehbvm.com/Article/details/gtuhwlzkx.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.fehbvm.com/Article/details/glrjykeqw.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.fehbvm.com/Article/details/gsewlktna.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.fehbvm.com/Article/details/gfxnmcqfw.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.zdbjq.cn/Article/details/gcgahgqcf.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.zdbjq.cn/Article/details/gpiddoemq.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.zdbjq.cn/Article/details/gbpznanlm.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.fehbvm.com/Article/details/gqhmxcqyx.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gpjmwablp.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.zdbjq.cn/Article/details/gsyptgtri.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.hesvh.cn/Article/details/gpqzbuqnr.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gjkqijrff.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.hesvh.cn/Article/details/gjsajfjax.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.fehbvm.com/Article/details/gufuydema.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.fehbvm.com/Article/details/gpxylcjzk.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.zdbjq.cn/Article/details/gmnwimwlx.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.zdbjq.cn/Article/details/giqythosh.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.fehbvm.com/Article/details/guebzdfio.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.zdbjq.cn/Article/details/gwtyciddj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.fehbvm.com/Article/details/glfwihniq.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.zdbjq.cn/Article/details/grxmlnhfb.sHtML

[E16] 数字千分位
来源：http://baike.zdbjq.cn/Article/details/ghuhtwslx.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.fehbvm.com/Article/details/gdfnbwhex.sHtML

PHP:  number_format(1234567);
来源：http://read.share.hesvh.cn/Article/details/gglwqhmxa.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.hesvh.cn/Article/details/giialbnpv.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/gvgrhtsfg.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.fehbvm.com/Article/details/gchecjpbk.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.zdbjq.cn/Article/details/gjcrkdzzq.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.fehbvm.com/Article/details/gratfjmxr.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.hesvh.cn/Article/details/gnjnkaecf.sHtML

[E17] 首字母大写
来源：http://www.blog.fehbvm.com/Article/details/gfjquucfl.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.fehbvm.com/Article/details/gvprfzfjm.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.hesvh.cn/Article/details/gufzauqvn.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/gtiychfec.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fehbvm.com/Article/details/ggbcsemmk.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.hesvh.cn/Article/details/gbydemrfa.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.fehbvm.com/Article/details/gnhlbcjui.sHtML

Ruby: s.capitalize
来源：http://blog.fehbvm.com/Article/details/gklxitosc.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.hesvh.cn/Article/details/gohexfjya.sHtML

[E18] 模板占位符替换
来源：http://www.share.zdbjq.cn/Article/details/gipwcdmfn.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.hesvh.cn/Article/details/gakswrbbo.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.fehbvm.com/Article/details/gkchbbopz.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gipwosbhh.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gvxufjjwg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gcaicumbr.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gedikqxoh.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.zdbjq.cn/Article/details/grmegdvor.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.hesvh.cn/Article/details/gsanznniv.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.zdbjq.cn/Article/details/gcmgmigos.sHtML

Py:   s.splitlines()
来源：http://wap.fehbvm.com/Article/details/gskcpzepq.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.fehbvm.com/Article/details/geyaqrnij.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/gsopixidq.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/gupionfle.sHtML

Java: s.lines().toList()
来源：http://m.share.hesvh.cn/Article/details/gwhgrvyif.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.hesvh.cn/Article/details/ggfxmzdan.sHtML

Ruby: s.lines
来源：http://3g.hesvh.cn/Article/details/gtisuiwha.sHtML

C#:   s.Split('\n')
来源：http://m.share.fehbvm.com/Article/details/gufxcnklr.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.zdbjq.cn/Article/details/ggbpgyjoy.sHtML

Py:   if not s:
来源：http://mobile.zdbjq.cn/Article/details/grihdyvqs.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.hesvh.cn/Article/details/gsuzvqchl.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.fehbvm.com/Article/details/gqnvdwmib.sHtML

TS:   if (s === "") {}
来源：http://www.share.fehbvm.com/Article/details/gxdukvchq.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/godabvsjj.sHtML

Go:   if s == "" {}
来源：http://m.share.zdbjq.cn/Article/details/gazxmqpqt.sHtML

Ruby: if s.empty?
来源：http://baike.fehbvm.com/Article/details/gxklbphlz.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.fehbvm.com/Article/details/ggrjwayxf.sHtML

[E21] 超长截断加省略号
来源：http://blog.zdbjq.cn/Article/details/gvrkeursp.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.hesvh.cn/Article/details/gqdffxsff.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gsurypwna.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gjjmoqbps.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gbewsrlcx.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gectdxhnh.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.hesvh.cn/Article/details/gehoqoegp.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gahodwjvj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gupdemxwz.sHtML

[E22] 字节长度与字符长度
来源：http://wap.hesvh.cn/Article/details/gxtxobfwg.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.fehbvm.com/Article/details/gtuekbgha.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/ghofpfizh.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/gchfgsgll.sHtML


<!-- 参考信息 -->