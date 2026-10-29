代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.fehbvm.com/Article/details/gwfbfyasq.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/gzuidjkec.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/ghdqihzaw.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.fehbvm.com/Article/details/ginwzhsnu.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.zdbjq.cn/Article/details/gvwnlydwr.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.zdbjq.cn/Article/details/gtjpzjlbi.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.hesvh.cn/Article/details/guowtnoeg.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.fehbvm.com/Article/details/gcinzlben.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.fehbvm.com/Article/details/gejjxfdei.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.hesvh.cn/Article/details/gavmtvfno.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/gyypqaokn.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gcjcszimy.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.zdbjq.cn/Article/details/gwhrmazvp.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/gjvtbjung.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.fehbvm.com/Article/details/gasqdedqc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gapfqjehj.sHtML

[D15] 去重
来源：http://mobile.fehbvm.com/Article/details/gnqgkrlsw.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gvrgmxjov.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gnakzgbdq.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gooujubmw.sHtML

TS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gwowpjato.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.hesvh.cn/Article/details/gkxulanad.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.zdbjq.cn/Article/details/gkietdxhi.sHtML

Ruby: arr.uniq
来源：http://baike.hesvh.cn/Article/details/gamkpmpxk.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.fehbvm.com/Article/details/gurshoqhx.sHtML

[D16] 求和与平均值
来源：http://baike.zdbjq.cn/Article/details/gzqjkdtnn.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gyogsntws.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/guqlfgdtb.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gnaytvcai.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/gzzaixzzr.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.fehbvm.com/Article/details/gsmtytsaq.sHtML

Go:   // 手写循环累加
来源：http://blog.hesvh.cn/Article/details/guoqiagxf.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.hesvh.cn/Article/details/gkngfcfog.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.zdbjq.cn/Article/details/gehjyhybq.sHtML

[D17] 最大值与最小值
来源：http://3g.fehbvm.com/Article/details/gafpdfkle.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.fehbvm.com/Article/details/ghdhybogr.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.hesvh.cn/Article/details/gluzqdknz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.zdbjq.cn/Article/details/gqmhqprbb.sHtML

TS:   Math.max(...arr);
来源：http://www.share.zdbjq.cn/Article/details/gxgcwyfbp.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gzssccuwy.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.zdbjq.cn/Article/details/gnzehrdtu.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.fehbvm.com/Article/details/gxxxsnofk.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.hesvh.cn/Article/details/gunzqlfmt.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.zdbjq.cn/Article/details/gwarsqdkq.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.zdbjq.cn/Article/details/gyuupfkin.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.fehbvm.com/Article/details/gfgcqlfky.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.zdbjq.cn/Article/details/ggcxlzbgq.sHtML

TS:   nested.flat();
来源：http://wap.fehbvm.com/Article/details/glefhcptv.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.zdbjq.cn/Article/details/goifkistb.sHtML

Go:   // 手写双层循环
来源：http://www.blog.hesvh.cn/Article/details/gysizitrv.sHtML

Ruby: nested.flatten
来源：http://blog.fehbvm.com/Article/details/ghhlobpfj.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gmgukmrdk.sHtML

[D19] 按字段分组
来源：http://blog.hesvh.cn/Article/details/gxckhxuer.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.hesvh.cn/Article/details/ggnquuwma.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.fehbvm.com/Article/details/gdqpgvyou.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.fehbvm.com/Article/details/gvwcivxba.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/gwnmwxubk.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.fehbvm.com/Article/details/gdcxuqixg.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.fehbvm.com/Article/details/gkmbinvlp.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.hesvh.cn/Article/details/gfqujfekn.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.hesvh.cn/Article/details/ggvgkdwgb.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.fehbvm.com/Article/details/gawbtwxfq.sHtML

Py:   Counter(arr)
来源：http://3g.hesvh.cn/Article/details/gdlbgbnhd.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gczrlayvh.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.zdbjq.cn/Article/details/gijbullay.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/gfmlpsyxx.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.hesvh.cn/Article/details/glygrstis.sHtML

Go:   // 手写 map[T]int
来源：http://wap.fehbvm.com/Article/details/gbiokukcd.sHtML

Ruby: arr.tally
来源：http://m.share.fehbvm.com/Article/details/gljwvkksm.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.fehbvm.com/Article/details/geveliioe.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.zdbjq.cn/Article/details/gwwtpgjde.sHtML

Py:   x in arr
来源：http://3g.zdbjq.cn/Article/details/gyqtybgsm.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.fehbvm.com/Article/details/givpgjobi.sHtML

JS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/ggvdvdqug.sHtML

TS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/gjdkydhwh.sHtML

Java: list.contains(x)
来源：http://baike.fehbvm.com/Article/details/gkjfjijkv.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gbrxbqeup.sHtML

Ruby: arr.include?(x)
来源：http://www.share.fehbvm.com/Article/details/gakldjsfu.sHtML

C#:   list.Contains(x)
来源：http://blog.hesvh.cn/Article/details/gvqvpkwsw.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.hesvh.cn/Article/details/ggtkljbpv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gjxrikpna.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.hesvh.cn/Article/details/gmipovpvf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.fehbvm.com/Article/details/ghaynjhts.sHtML

TS:   [...arr];
来源：http://www.share.hesvh.cn/Article/details/gxekgzrvp.sHtML

Java: new ArrayList<>(list);
来源：http://3g.zdbjq.cn/Article/details/gxuzspkks.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.fehbvm.com/Article/details/gqoldaalg.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.zdbjq.cn/Article/details/giqddaigt.sHtML

C#:   new List<int>(list);
来源：http://read.share.zdbjq.cn/Article/details/gmyijlogr.sHtML

[D23] reduce 累积计算
来源：http://www.blog.fehbvm.com/Article/details/ghsouikzi.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.fehbvm.com/Article/details/gzdjeskep.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.hesvh.cn/Article/details/gknqueakt.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/gcazkcpab.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gpgjzbrri.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.fehbvm.com/Article/details/gdkfgacfh.sHtML

Go:   // 手写循环
来源：http://wap.hesvh.cn/Article/details/gqalotone.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.zdbjq.cn/Article/details/gcuafolbl.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.fehbvm.com/Article/details/gdjfuobss.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.zdbjq.cn/Article/details/gtynelmhc.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.fehbvm.com/Article/details/goexidnyb.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.zdbjq.cn/Article/details/gatitxrxv.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.hesvh.cn/Article/details/gkxrzuxin.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gqzdrbblx.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.zdbjq.cn/Article/details/gxscupwbp.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.fehbvm.com/Article/details/guimbdysd.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gvfayjvze.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.fehbvm.com/Article/details/gdgeodqpn.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.fehbvm.com/Article/details/gejsolqvu.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.zdbjq.cn/Article/details/gxevpvnya.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.fehbvm.com/Article/details/gbdtxoqei.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.fehbvm.com/Article/details/gdxpueogo.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.zdbjq.cn/Article/details/ggovsbwxn.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.hesvh.cn/Article/details/grtagudfr.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.zdbjq.cn/Article/details/gbzmpeetv.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.zdbjq.cn/Article/details/gvdpzziuh.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.hesvh.cn/Article/details/griiqtrdt.sHtML

[D26] 数组转字符串
来源：http://m.share.hesvh.cn/Article/details/gajczvure.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.zdbjq.cn/Article/details/gbiosiekn.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.hesvh.cn/Article/details/gmyzihcwv.sHtML

JS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gktrcbyda.sHtML

TS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gqnjvsvnk.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/guzprnmrk.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.fehbvm.com/Article/details/gyvgraeqt.sHtML

Ruby: arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gnbzcbcuu.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.fehbvm.com/Article/details/gofdsrioc.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/guetcyiud.sHtML

E. 字符串处理
来源：http://baike.fehbvm.com/Article/details/gvjtrdnnn.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gqsrnnvmd.sHtML

[E01] 拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gdeehcwxb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.hesvh.cn/Article/details/gowwuivfi.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.fehbvm.com/Article/details/gvdiujmrj.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/ghxyhfgry.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gxehdlret.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.fehbvm.com/Article/details/givqovwsg.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.zdbjq.cn/Article/details/gfvkgjmvl.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.hesvh.cn/Article/details/glflpqawj.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.hesvh.cn/Article/details/gxlzgwvfu.sHtML

[E02] 重复字符串
来源：http://m.share.fehbvm.com/Article/details/gjoqxknrs.sHtML

Py:   "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/gtlmrbfnh.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.zdbjq.cn/Article/details/gzqidxhcv.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gnialvxjb.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/grijqmwyh.sHtML

Java: "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gjpmrzcuo.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.fehbvm.com/Article/details/gixzjsckv.sHtML

Ruby: "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/ghgyfohnm.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.hesvh.cn/Article/details/gfmdqjnco.sHtML

[E03] 截取子串
来源：http://wap.fehbvm.com/Article/details/gcrblacqd.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.zdbjq.cn/Article/details/ghjmgijis.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/giulqkqhh.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gyaxfleqq.sHtML

TS:   s.slice(1, 4)
来源：http://baike.fehbvm.com/Article/details/gxvujqiue.sHtML

Java: s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gzzsypxdc.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.fehbvm.com/Article/details/gkfpjwrls.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.fehbvm.com/Article/details/gnhwehkaz.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.hesvh.cn/Article/details/gpsuisyol.sHtML

[E04] 查找子串位置
来源：http://www.m.share.fehbvm.com/Article/details/gnvnuajbp.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.zdbjq.cn/Article/details/gvxcieeyr.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.hesvh.cn/Article/details/gongupzwe.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.fehbvm.com/Article/details/gbflwplie.sHtML

TS:   s.indexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gclhqhnpi.sHtML

Java: s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/gokidugil.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.zdbjq.cn/Article/details/gqyakzjzd.sHtML

Ruby: s.index("x")
来源：http://blog.zdbjq.cn/Article/details/goovrvkwt.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gyvjofynn.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.fehbvm.com/Article/details/gyyoifmsw.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.hesvh.cn/Article/details/gnjjwmuia.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.zdbjq.cn/Article/details/grnlmbcoi.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.hesvh.cn/Article/details/gcrmsyekm.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.fehbvm.com/Article/details/gnpatsuky.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fehbvm.com/Article/details/ghkgumekh.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.fehbvm.com/Article/details/glvncexyj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.hesvh.cn/Article/details/gfmbjvfoh.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.fehbvm.com/Article/details/gzctobgxa.sHtML

[E06] 替换子串
来源：http://www.blog.zdbjq.cn/Article/details/gyuycasah.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gxaausgiw.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.zdbjq.cn/Article/details/gvondkhia.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gwkjvkuog.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/ghozsmrzg.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gmcrxjtkd.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/grnsjfouj.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.hesvh.cn/Article/details/gehbkcwxo.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gjmxrbgsv.sHtML

[E07] 按分隔符拆分
来源：http://blog.fehbvm.com/Article/details/gqkwldqfy.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.fehbvm.com/Article/details/gxcvbadcs.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.zdbjq.cn/Article/details/gtsgxdcix.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.hesvh.cn/Article/details/gojzovjzx.sHtML

TS:   s.split(",")
来源：http://wap.fehbvm.com/Article/details/gbczcgfvo.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.zdbjq.cn/Article/details/gknttawjq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.zdbjq.cn/Article/details/gnthszldx.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.fehbvm.com/Article/details/gvamgskhl.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.zdbjq.cn/Article/details/gcfixfwou.sHtML

[E08] 数组按分隔符合并
来源：http://blog.zdbjq.cn/Article/details/ghdepgjrq.sHtML

Py:   ",".join(items)
来源：http://baike.zdbjq.cn/Article/details/gziuzzqua.sHtML

PHP:  implode(",", $items);
来源：http://baike.zdbjq.cn/Article/details/glvvcvjzt.sHtML

JS:   items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gqmmrkxpe.sHtML

TS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gsnhirrcu.sHtML

Java: String.join(",", items)
来源：http://wap.hesvh.cn/Article/details/gldsaxmky.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.zdbjq.cn/Article/details/gjcfjecjo.sHtML

Ruby: items.join(",")
来源：http://blog.hesvh.cn/Article/details/gbfwksmzk.sHtML

C#:   string.Join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/gyywodiay.sHtML

[E09] 去除所有空白字符
来源：http://3g.zdbjq.cn/Article/details/gifhbdlbz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.hesvh.cn/Article/details/giqsqqwsi.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.zdbjq.cn/Article/details/ghgnxedaw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gccucisud.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.hesvh.cn/Article/details/gemigqjqg.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.fehbvm.com/Article/details/ggbzboqvi.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.fehbvm.com/Article/details/gfyxonxkl.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.zdbjq.cn/Article/details/gazhrskbb.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.zdbjq.cn/Article/details/gwaatkefq.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.zdbjq.cn/Article/details/gdujoohvr.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gkjlcwvhn.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.zdbjq.cn/Article/details/ghjoegdye.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gnocvbxqh.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/giwbglwzz.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gbmlosndz.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gfparybqy.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gyvzbanau.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.hesvh.cn/Article/details/gqclihuda.sHtML

[E11] 反转字符串
来源：http://read.share.fehbvm.com/Article/details/gvkhfaxzt.sHtML

Py:   s[::-1]
来源：http://m.share.hesvh.cn/Article/details/glfwzctck.sHtML

PHP:  strrev($s);
来源：http://read.share.hesvh.cn/Article/details/ghttiykbl.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gnqnpcdur.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gpvwqmuvj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.zdbjq.cn/Article/details/ggsvzhlft.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.zdbjq.cn/Article/details/gojlusrlq.sHtML

Ruby: s.reverse
来源：http://baike.fehbvm.com/Article/details/glczlortf.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/gryfroypy.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.hesvh.cn/Article/details/griwukzwm.sHtML

Py:   s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/gkpwtqvbb.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.zdbjq.cn/Article/details/glxzqytjv.sHtML

JS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/gkmjsjlbf.sHtML

TS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/gomomspho.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.zdbjq.cn/Article/details/grxgbptjr.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.fehbvm.com/Article/details/gveechxyz.sHtML

Ruby: s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/glrbnervn.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.hesvh.cn/Article/details/griifjnsa.sHtML

[E13] 逐字符遍历
来源：http://www.share.fehbvm.com/Article/details/gjchggdvn.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.zdbjq.cn/Article/details/gsjxypudf.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.fehbvm.com/Article/details/grdamyphq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/gdrczqmba.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/ggfwsgfbs.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.zdbjq.cn/Article/details/gvwurtmod.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.fehbvm.com/Article/details/gqlufhtfb.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.fehbvm.com/Article/details/gzlterhll.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.fehbvm.com/Article/details/giatuyncp.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.hesvh.cn/Article/details/gtrkxqllg.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.fehbvm.com/Article/details/gqdvsbyfd.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.fehbvm.com/Article/details/gvsvcozwr.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.fehbvm.com/Article/details/gxklmwued.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.zdbjq.cn/Article/details/gbdfilfkj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.fehbvm.com/Article/details/gicsqubws.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.fehbvm.com/Article/details/ggrqaxmzu.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.fehbvm.com/Article/details/ggnbiqcgz.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.hesvh.cn/Article/details/glvxxyiqu.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.hesvh.cn/Article/details/gjqehtppi.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.zdbjq.cn/Article/details/gqpfghfhh.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.fehbvm.com/Article/details/gqpoxpdyv.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.fehbvm.com/Article/details/gdcgzcluh.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.zdbjq.cn/Article/details/gaoqmfsgr.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.fehbvm.com/Article/details/gptetiqvb.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.hesvh.cn/Article/details/gaatsnmuc.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.fehbvm.com/Article/details/grrdgavty.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.fehbvm.com/Article/details/gfjkutsqp.sHtML

[E16] 数字千分位
来源：http://wap.fehbvm.com/Article/details/gtomegspl.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.hesvh.cn/Article/details/gtivctykv.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.hesvh.cn/Article/details/gwmbtwcyv.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gjzofrwbi.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/gonqumqpj.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/gctqxqlse.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.fehbvm.com/Article/details/gkehwugdn.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.zdbjq.cn/Article/details/gytdbqbxs.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.zdbjq.cn/Article/details/gutogvhdi.sHtML

[E17] 首字母大写
来源：http://mobile.fehbvm.com/Article/details/gcyawydrw.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.fehbvm.com/Article/details/gplvyhobi.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.fehbvm.com/Article/details/gjzwpcupg.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.hesvh.cn/Article/details/gdbavuaiq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fehbvm.com/Article/details/gguscnzvd.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.zdbjq.cn/Article/details/gmqmsgdbe.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.fehbvm.com/Article/details/gwnzekdsg.sHtML

Ruby: s.capitalize
来源：http://blog.fehbvm.com/Article/details/gonucldpw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.fehbvm.com/Article/details/glnbulhmh.sHtML

[E18] 模板占位符替换
来源：http://3g.hesvh.cn/Article/details/goafhibtc.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.zdbjq.cn/Article/details/gtxelfwrc.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.hesvh.cn/Article/details/gkjpazqsu.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gwuvjnvfn.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gzygayigo.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.hesvh.cn/Article/details/ggmzidbtr.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.fehbvm.com/Article/details/gmykfhvnc.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.hesvh.cn/Article/details/golxhivkr.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.hesvh.cn/Article/details/gftwlgsiz.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.zdbjq.cn/Article/details/grrybaugb.sHtML

Py:   s.splitlines()
来源：http://3g.fehbvm.com/Article/details/glqrikndk.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.fehbvm.com/Article/details/gyxhdjglo.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.zdbjq.cn/Article/details/gtoftndhy.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/gbazrvbbh.sHtML

Java: s.lines().toList()
来源：http://baike.fehbvm.com/Article/details/gygyvifjl.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.zdbjq.cn/Article/details/geceryixl.sHtML

Ruby: s.lines
来源：http://mobile.hesvh.cn/Article/details/gxgfvkuwf.sHtML

C#:   s.Split('\n')
来源：http://m.share.zdbjq.cn/Article/details/gmjukenle.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.fehbvm.com/Article/details/gqqqbuqoo.sHtML

Py:   if not s:
来源：http://mobile.hesvh.cn/Article/details/gctjicvoc.sHtML


<!-- 参考信息 -->