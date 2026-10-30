代发 wailian999

C#:   list.Reverse();
来源：http://read.share.zdbjq.cn/Article/details/gvssuiohv.sHtML

[D12] 查找元素下标
来源：http://www.share.hesvh.cn/Article/details/gkocydpdu.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.zdbjq.cn/Article/details/gpneonyte.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.zdbjq.cn/Article/details/grudggxwc.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/gjydvhrwd.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/gbktairkc.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.hesvh.cn/Article/details/goypamdup.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gxzjnjdbi.sHtML

Ruby: arr.index(x)
来源：http://baike.zdbjq.cn/Article/details/goalktjfy.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.hesvh.cn/Article/details/gfwvujubk.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.hesvh.cn/Article/details/gpiipiioo.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gfzofpcwz.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.hesvh.cn/Article/details/gscspaehz.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/gzdrnagui.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gegqtknxx.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.zdbjq.cn/Article/details/gsmpgybed.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.fehbvm.com/Article/details/godoxgfpw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.zdbjq.cn/Article/details/gppfvhjns.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.fehbvm.com/Article/details/gpfekbqdd.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.fehbvm.com/Article/details/gjnqusbus.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gedqjitsj.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.fehbvm.com/Article/details/gzqgtgfsv.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/guhmrumfw.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/gqmldgjgp.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.zdbjq.cn/Article/details/gvzsimipu.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/gzkueqipy.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.hesvh.cn/Article/details/grmcwjiqa.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gsyovqkfo.sHtML

[D15] 去重
来源：http://www.blog.zdbjq.cn/Article/details/gsklcmfev.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/granezick.sHtML

PHP:  array_unique($arr);
来源：http://wap.hesvh.cn/Article/details/gfetpucjd.sHtML

JS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gwrzoxcyi.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/genfaffrd.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.zdbjq.cn/Article/details/gaihpideb.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.hesvh.cn/Article/details/gisexbmve.sHtML

Ruby: arr.uniq
来源：http://www.blog.fehbvm.com/Article/details/gbbpqvzmk.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.hesvh.cn/Article/details/gzftjkfny.sHtML

[D16] 求和与平均值
来源：http://www.blog.fehbvm.com/Article/details/gitcphiuf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.zdbjq.cn/Article/details/geqsxsmea.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.zdbjq.cn/Article/details/gapiduljb.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/gqtjgjcnu.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/ghzrejxgd.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.hesvh.cn/Article/details/goregjavu.sHtML

Go:   // 手写循环累加
来源：http://mobile.fehbvm.com/Article/details/gdejtutlq.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.fehbvm.com/Article/details/gawrvpyvd.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.fehbvm.com/Article/details/gpksrerxc.sHtML

[D17] 最大值与最小值
来源：http://m.share.hesvh.cn/Article/details/gumappurj.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.zdbjq.cn/Article/details/glfotqxvb.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.hesvh.cn/Article/details/grsyfzqrb.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.zdbjq.cn/Article/details/grqkxfgvp.sHtML

TS:   Math.max(...arr);
来源：http://read.share.hesvh.cn/Article/details/gjgxixldh.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.hesvh.cn/Article/details/gdzdnyega.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.fehbvm.com/Article/details/gmdfjfswx.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.fehbvm.com/Article/details/gtihlfkns.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.hesvh.cn/Article/details/gdllerxnd.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.zdbjq.cn/Article/details/gbhxpcosl.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.fehbvm.com/Article/details/gxmjqkvnt.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.zdbjq.cn/Article/details/gwiwrympr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.fehbvm.com/Article/details/gwbgjpvyz.sHtML

TS:   nested.flat();
来源：http://www.blog.zdbjq.cn/Article/details/gvphwohjx.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.zdbjq.cn/Article/details/gqwloghel.sHtML

Go:   // 手写双层循环
来源：http://www.share.fehbvm.com/Article/details/ghrugqknq.sHtML

Ruby: nested.flatten
来源：http://www.share.hesvh.cn/Article/details/gajbzmbaj.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gqtnbuzry.sHtML

[D19] 按字段分组
来源：http://3g.hesvh.cn/Article/details/gbiqtejxj.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.hesvh.cn/Article/details/gpjupmkmz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.hesvh.cn/Article/details/gsyglkcnz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.fehbvm.com/Article/details/gntpcrlbl.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/glbhmqfcm.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.zdbjq.cn/Article/details/goajxnwye.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.hesvh.cn/Article/details/gvbllgecr.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.fehbvm.com/Article/details/gukethhoa.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.hesvh.cn/Article/details/grcmunrnf.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.fehbvm.com/Article/details/gdzkijawd.sHtML

Py:   Counter(arr)
来源：http://www.share.fehbvm.com/Article/details/gcohxklfh.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.hesvh.cn/Article/details/gxvjxymrj.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/gqrnxznde.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/gedgyeujm.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.hesvh.cn/Article/details/gxoscyiju.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.fehbvm.com/Article/details/gpngzonua.sHtML

Ruby: arr.tally
来源：http://3g.fehbvm.com/Article/details/gbotfteyc.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.zdbjq.cn/Article/details/gumtqtdxn.sHtML

[D21] 判断是否包含某元素
来源：http://3g.fehbvm.com/Article/details/giqrrzmon.sHtML

Py:   x in arr
来源：http://blog.fehbvm.com/Article/details/gznuyyckh.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.zdbjq.cn/Article/details/gwkfkjysn.sHtML

JS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gokgsdhmr.sHtML

TS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/gkcoicrsv.sHtML

Java: list.contains(x)
来源：http://mobile.fehbvm.com/Article/details/ghbscyokt.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gvhqpslyj.sHtML

Ruby: arr.include?(x)
来源：http://www.share.fehbvm.com/Article/details/gjzlbkbld.sHtML

C#:   list.Contains(x)
来源：http://blog.fehbvm.com/Article/details/gypkofxws.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.zdbjq.cn/Article/details/gvdxtthdg.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.fehbvm.com/Article/details/gtyfvbhre.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.fehbvm.com/Article/details/gbiaisksx.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.hesvh.cn/Article/details/gprcqegxs.sHtML

TS:   [...arr];
来源：http://www.m.share.hesvh.cn/Article/details/ghxsmsvez.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gxeedcbjc.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.hesvh.cn/Article/details/glcdsueus.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.hesvh.cn/Article/details/gzazwkxbg.sHtML

C#:   new List<int>(list);
来源：http://www.blog.zdbjq.cn/Article/details/gjdbxilrh.sHtML

[D23] reduce 累积计算
来源：http://m.share.hesvh.cn/Article/details/ghgoydvzw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.fehbvm.com/Article/details/gzfxivdhx.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.fehbvm.com/Article/details/gxysfldat.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/gpimykabj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/glisjaogq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.zdbjq.cn/Article/details/gghgyswkz.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/gwjtnrhnd.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.zdbjq.cn/Article/details/gghmjcrvg.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.fehbvm.com/Article/details/grulzppbx.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.hesvh.cn/Article/details/gyxxtenwo.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.hesvh.cn/Article/details/gvpzlaibl.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.hesvh.cn/Article/details/gvzbidtzz.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.hesvh.cn/Article/details/gqwnntyxj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gpbisjtjb.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.fehbvm.com/Article/details/grlylbakt.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.zdbjq.cn/Article/details/gcormdwsl.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gtedkocrt.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.zdbjq.cn/Article/details/gannltbhw.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.zdbjq.cn/Article/details/grbnlozzz.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.fehbvm.com/Article/details/gbnlnmgse.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.zdbjq.cn/Article/details/gglfviuyp.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.fehbvm.com/Article/details/gnfdwkvqa.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.zdbjq.cn/Article/details/gobplcbir.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.fehbvm.com/Article/details/gjywlhrwg.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.hesvh.cn/Article/details/gmzzbahdz.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.zdbjq.cn/Article/details/gfkvxkzsq.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.fehbvm.com/Article/details/gimovtzlo.sHtML

[D26] 数组转字符串
来源：http://wap.fehbvm.com/Article/details/gwdbewbgd.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.fehbvm.com/Article/details/ghvjxxbnc.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.zdbjq.cn/Article/details/geaneksfl.sHtML

JS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gopczvrqp.sHtML

TS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/goxmgyqnx.sHtML

Java: String.join(", ", list)
来源：http://3g.fehbvm.com/Article/details/gfjormwfa.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.zdbjq.cn/Article/details/geykglxxe.sHtML

Ruby: arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gmmxyxmmp.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/gqzbvzpnc.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gjlphfemz.sHtML

E. 字符串处理
来源：http://blog.hesvh.cn/Article/details/gnblzszzp.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ggifaltpw.sHtML

[E01] 拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gobmczxra.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.zdbjq.cn/Article/details/gzgkjwohd.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.fehbvm.com/Article/details/gxhcwkimw.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/gieliygga.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/ghgpzklpa.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.hesvh.cn/Article/details/gtbtjboey.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.zdbjq.cn/Article/details/gvtppdmsu.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.zdbjq.cn/Article/details/ghmbopbtp.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gojmpxaci.sHtML

[E02] 重复字符串
来源：http://www.blog.zdbjq.cn/Article/details/gmroegioh.sHtML

Py:   "ab" * 3
来源：http://www.share.fehbvm.com/Article/details/gqdfkrhod.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.fehbvm.com/Article/details/gpimzgowt.sHtML

JS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gebihzjze.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/ghvphbvgq.sHtML

Java: "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gevszejvu.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.fehbvm.com/Article/details/gdcjxoojg.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.zdbjq.cn/Article/details/gezpgjnri.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.fehbvm.com/Article/details/gsyrhrhhb.sHtML

[E03] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/gnyzioauk.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.zdbjq.cn/Article/details/gefhpuvgk.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gbtxzvvpl.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gvkprufhz.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.fehbvm.com/Article/details/galqesags.sHtML

Java: s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/ggrxzavoz.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gbumefpzx.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.hesvh.cn/Article/details/gqmpchvwg.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.fehbvm.com/Article/details/gdelrldha.sHtML

[E04] 查找子串位置
来源：http://wap.hesvh.cn/Article/details/gwtrmbilr.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.zdbjq.cn/Article/details/gpgegbuxu.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.hesvh.cn/Article/details/gopqeqpsg.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.fehbvm.com/Article/details/goqprowzt.sHtML

TS:   s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/govrpwxuc.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/gtquervpf.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.hesvh.cn/Article/details/gagtvclhi.sHtML

Ruby: s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/grkhuaygk.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gzqvbnbxs.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.hesvh.cn/Article/details/ghufmtvnr.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.hesvh.cn/Article/details/gljxmjbxa.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.zdbjq.cn/Article/details/gjrckzeed.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.hesvh.cn/Article/details/gebmdmial.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.zdbjq.cn/Article/details/glmxuxrdu.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gcklgycij.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.hesvh.cn/Article/details/guezbsejj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.zdbjq.cn/Article/details/gjplwjjkl.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.zdbjq.cn/Article/details/grouzmczw.sHtML

[E06] 替换子串
来源：http://www.share.hesvh.cn/Article/details/gmbiujyiy.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/gcomcmtvn.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.zdbjq.cn/Article/details/gkngwckss.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gaxxcnjvl.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/govjfyocl.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gutnzscyr.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.hesvh.cn/Article/details/gxgfgnucp.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gkkqhmavs.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gnoxjozxd.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.zdbjq.cn/Article/details/getgootew.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.zdbjq.cn/Article/details/gjqfuiywn.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gcsqpkdyt.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.fehbvm.com/Article/details/gfckiownp.sHtML

TS:   s.split(",")
来源：http://m.share.zdbjq.cn/Article/details/gywjapcfc.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.hesvh.cn/Article/details/gtwrwxcqg.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.zdbjq.cn/Article/details/gommojzjx.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.fehbvm.com/Article/details/ghavpauzx.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.hesvh.cn/Article/details/gyndfaldc.sHtML

[E08] 数组按分隔符合并
来源：http://3g.hesvh.cn/Article/details/gspidbzdf.sHtML

Py:   ",".join(items)
来源：http://www.share.fehbvm.com/Article/details/gehmcktgk.sHtML

PHP:  implode(",", $items);
来源：http://3g.hesvh.cn/Article/details/guvnosstr.sHtML

JS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/gwpyiuceh.sHtML

TS:   items.join(",")
来源：http://blog.hesvh.cn/Article/details/gzntkmrru.sHtML

Java: String.join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gydnoahma.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.fehbvm.com/Article/details/gconcyodl.sHtML

Ruby: items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gorcnanlr.sHtML

C#:   string.Join(",", items)
来源：http://3g.zdbjq.cn/Article/details/gsdtiajsl.sHtML

[E09] 去除所有空白字符
来源：http://m.share.fehbvm.com/Article/details/geqbehnyr.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.zdbjq.cn/Article/details/gyjmohszy.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.fehbvm.com/Article/details/grkadvxfy.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/gpaxjzbas.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gkeejdgyc.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/gjycgmpch.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.zdbjq.cn/Article/details/gujnokjjn.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.fehbvm.com/Article/details/gwdqbkdzk.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/gxuoparlt.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.hesvh.cn/Article/details/gfauqxjcw.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.hesvh.cn/Article/details/gmyslqwck.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.fehbvm.com/Article/details/gfmfpipaj.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gxajfgdjv.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gqabzirki.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gpixxyjbq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gychpuyef.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gkayycuba.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.zdbjq.cn/Article/details/gvaavwvvu.sHtML

[E11] 反转字符串
来源：http://read.share.fehbvm.com/Article/details/gwieoixuv.sHtML

Py:   s[::-1]
来源：http://wap.fehbvm.com/Article/details/gyqrfhciw.sHtML

PHP:  strrev($s);
来源：http://3g.hesvh.cn/Article/details/gvixvqyym.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gwclgohuy.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gieawerhb.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.hesvh.cn/Article/details/gqrqvvzzx.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.zdbjq.cn/Article/details/gznflfmnx.sHtML

Ruby: s.reverse
来源：http://read.share.fehbvm.com/Article/details/gtcxfkuwa.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/gdxujidza.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.hesvh.cn/Article/details/gdlkalgtz.sHtML

Py:   s.count("a")
来源：http://blog.zdbjq.cn/Article/details/gvmjozrlj.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.hesvh.cn/Article/details/gawxuqzce.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.fehbvm.com/Article/details/gtvmrwsgl.sHtML

TS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/gedqkxwhv.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.hesvh.cn/Article/details/giswecuch.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.fehbvm.com/Article/details/gcughgerx.sHtML

Ruby: s.count("a")
来源：http://m.share.hesvh.cn/Article/details/gszxphsch.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.zdbjq.cn/Article/details/gomcbldqp.sHtML

[E13] 逐字符遍历
来源：http://wap.zdbjq.cn/Article/details/ghqlpnrdb.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.fehbvm.com/Article/details/gfbavkqnx.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.zdbjq.cn/Article/details/guhqskjlq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.zdbjq.cn/Article/details/golpoakty.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gtpktuxai.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.zdbjq.cn/Article/details/gmqkgyepj.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.hesvh.cn/Article/details/gidgwixql.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.zdbjq.cn/Article/details/gjnziaeqn.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.fehbvm.com/Article/details/grfxlwmil.sHtML

[E14] URL 编码与 Base64
来源：http://blog.hesvh.cn/Article/details/giyaewxqr.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.hesvh.cn/Article/details/gwgkvfroq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.zdbjq.cn/Article/details/gxwryqwog.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.zdbjq.cn/Article/details/gusrmlkra.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.hesvh.cn/Article/details/gpkqdigjt.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.fehbvm.com/Article/details/gdujtwipj.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.fehbvm.com/Article/details/guunyswoo.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.fehbvm.com/Article/details/gocaclzyc.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gzjxystip.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.zdbjq.cn/Article/details/gqcjbeviw.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.zdbjq.cn/Article/details/goplqzegw.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.fehbvm.com/Article/details/giaztxwty.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.fehbvm.com/Article/details/gfhnyhrlh.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.hesvh.cn/Article/details/gwczxxrai.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.fehbvm.com/Article/details/gxjovtobp.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.fehbvm.com/Article/details/gncljcqsx.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.hesvh.cn/Article/details/giknsxdxv.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.hesvh.cn/Article/details/gajlwagji.sHtML

[E16] 数字千分位
来源：http://www.share.zdbjq.cn/Article/details/gfwculvbc.sHtML

Py:   f"{1234567:,}"
来源：http://wap.zdbjq.cn/Article/details/gkbvuewcq.sHtML

PHP:  number_format(1234567);
来源：http://3g.fehbvm.com/Article/details/gtdrgcxpg.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.hesvh.cn/Article/details/gvoiqhdon.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/givcvfkau.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.hesvh.cn/Article/details/gtqdqbvzm.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.zdbjq.cn/Article/details/georqgxye.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.fehbvm.com/Article/details/gwhwjlhpd.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.fehbvm.com/Article/details/gybtnnuag.sHtML

[E17] 首字母大写
来源：http://www.m.share.zdbjq.cn/Article/details/gxanwwfve.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.fehbvm.com/Article/details/gwzswgjme.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.fehbvm.com/Article/details/gjfbubxbx.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/gytbnmfzi.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.hesvh.cn/Article/details/grbzpqtyu.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.zdbjq.cn/Article/details/gcnicupmu.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.hesvh.cn/Article/details/gsvdpjfsu.sHtML

Ruby: s.capitalize
来源：http://baike.zdbjq.cn/Article/details/gflimbibd.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.fehbvm.com/Article/details/gsrorhpui.sHtML

[E18] 模板占位符替换
来源：http://www.blog.hesvh.cn/Article/details/gnqmrkfgf.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.zdbjq.cn/Article/details/gmqzsueno.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.zdbjq.cn/Article/details/gidvqwpqi.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gzselzbus.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gazvkjuhq.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/govxglnqb.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gnszeifrf.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.zdbjq.cn/Article/details/gzhxfgaoy.sHtML


<!-- 参考信息 -->