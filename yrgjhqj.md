代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/gpgprjqem.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/gosybmreu.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.hesvh.cn/Article/details/gxkazixfm.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gjfhrwxku.sHtML

Ruby: arr.index(x)
来源：http://read.share.fehbvm.com/Article/details/gorlbyibv.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.fehbvm.com/Article/details/gwqlhhvkx.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.fehbvm.com/Article/details/gmbnlycdw.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.hesvh.cn/Article/details/gpxcoccft.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.hesvh.cn/Article/details/gncvvasvd.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gglfhllpa.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gkexhipvp.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.hesvh.cn/Article/details/guafyulxl.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.hesvh.cn/Article/details/guypcjbbz.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.fehbvm.com/Article/details/gomrxkdtn.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.zdbjq.cn/Article/details/gychzbjpx.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.zdbjq.cn/Article/details/gjzgelshc.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.hesvh.cn/Article/details/gqhbdmgxa.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.zdbjq.cn/Article/details/ggjxgnglm.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/giqwpoopl.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/gnzwdgppj.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gzuaqewmg.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/gkptbsiex.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gjicebpdz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.zdbjq.cn/Article/details/gooksnttt.sHtML

[D15] 去重
来源：http://wap.fehbvm.com/Article/details/gtbfnrxhe.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/gzrruxuau.sHtML

PHP:  array_unique($arr);
来源：http://baike.fehbvm.com/Article/details/grfjdxjom.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gwrvmdqca.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/guzfvmuor.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.hesvh.cn/Article/details/guerchoux.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.zdbjq.cn/Article/details/gikoxrbsq.sHtML

Ruby: arr.uniq
来源：http://3g.zdbjq.cn/Article/details/gntmairqc.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.fehbvm.com/Article/details/gtukuppjb.sHtML

[D16] 求和与平均值
来源：http://read.share.fehbvm.com/Article/details/gdpwsrkpo.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.zdbjq.cn/Article/details/gattsmfxp.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.hesvh.cn/Article/details/gjsljoxlc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/glhyyppqn.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/gaymrbhej.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.hesvh.cn/Article/details/gkaaqvcur.sHtML

Go:   // 手写循环累加
来源：http://blog.hesvh.cn/Article/details/gpeusiztr.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/gestwcfwu.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.fehbvm.com/Article/details/gfhjigvra.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.fehbvm.com/Article/details/gtqvzcajp.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gkrztdxcy.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.hesvh.cn/Article/details/glcxykepb.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.hesvh.cn/Article/details/gulayvvmb.sHtML

TS:   Math.max(...arr);
来源：http://wap.zdbjq.cn/Article/details/gquwluami.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.zdbjq.cn/Article/details/ggusgtije.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.zdbjq.cn/Article/details/gqtflvepf.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.fehbvm.com/Article/details/gmisahfvv.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.fehbvm.com/Article/details/ggaemouvk.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.zdbjq.cn/Article/details/gaoqdigvf.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.zdbjq.cn/Article/details/gnsfunidn.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.zdbjq.cn/Article/details/gogmtlrvn.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.hesvh.cn/Article/details/gsdhabqwd.sHtML

TS:   nested.flat();
来源：http://mobile.zdbjq.cn/Article/details/gnlmeucqh.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.zdbjq.cn/Article/details/gjjtfylvs.sHtML

Go:   // 手写双层循环
来源：http://baike.hesvh.cn/Article/details/gwfcjobhr.sHtML

Ruby: nested.flatten
来源：http://www.share.zdbjq.cn/Article/details/gofzstllq.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.fehbvm.com/Article/details/gctgylzeb.sHtML

[D19] 按字段分组
来源：http://mobile.hesvh.cn/Article/details/gpivjsyjf.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.zdbjq.cn/Article/details/gcojomrfx.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.hesvh.cn/Article/details/gpydpbsyi.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.hesvh.cn/Article/details/gkxlqmlxy.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/guzpledhb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.fehbvm.com/Article/details/glkhsbrni.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.fehbvm.com/Article/details/gpfyumxvt.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.fehbvm.com/Article/details/gzeuqlhve.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fehbvm.com/Article/details/gdahgwwtm.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.fehbvm.com/Article/details/gtqdmqbye.sHtML

Py:   Counter(arr)
来源：http://read.share.zdbjq.cn/Article/details/gyrlzsfrh.sHtML

PHP:  array_count_values($arr);
来源：http://baike.fehbvm.com/Article/details/gehmxouit.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/gbeagvcae.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/gkokuxrtv.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.hesvh.cn/Article/details/gcgxkyndk.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.hesvh.cn/Article/details/gfueraagf.sHtML

Ruby: arr.tally
来源：http://www.m.share.zdbjq.cn/Article/details/gcmdaqrqm.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.hesvh.cn/Article/details/ggebknawm.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.hesvh.cn/Article/details/gghgnlxlz.sHtML

Py:   x in arr
来源：http://m.share.fehbvm.com/Article/details/geaoznjjt.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.zdbjq.cn/Article/details/gylwlawap.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gkyvynsgi.sHtML

TS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/grnznubcn.sHtML

Java: list.contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gimhswlvm.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.hesvh.cn/Article/details/ghcbsodrq.sHtML

Ruby: arr.include?(x)
来源：http://3g.zdbjq.cn/Article/details/gtkcolvhx.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gfjybofgv.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.hesvh.cn/Article/details/gockqidzl.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.hesvh.cn/Article/details/ggonwairm.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.fehbvm.com/Article/details/ghazreuky.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.fehbvm.com/Article/details/gqkrddedg.sHtML

TS:   [...arr];
来源：http://www.share.fehbvm.com/Article/details/gszdpgmfa.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.hesvh.cn/Article/details/geuptwehi.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.fehbvm.com/Article/details/gxtjrxvxd.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.zdbjq.cn/Article/details/gcwpzwrym.sHtML

C#:   new List<int>(list);
来源：http://wap.zdbjq.cn/Article/details/gzhaexrtq.sHtML

[D23] reduce 累积计算
来源：http://mobile.zdbjq.cn/Article/details/gzevycqky.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.fehbvm.com/Article/details/gxglfcgdu.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.fehbvm.com/Article/details/ghjnivxwz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.hesvh.cn/Article/details/gflhbwkvp.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/gmhygxfek.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.hesvh.cn/Article/details/goiwillle.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/ghibwdokj.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.zdbjq.cn/Article/details/gphiddybg.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.fehbvm.com/Article/details/gmlxkjqkr.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.zdbjq.cn/Article/details/gitavhmui.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.fehbvm.com/Article/details/gltxsdkdi.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.fehbvm.com/Article/details/gblbyywye.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.fehbvm.com/Article/details/grdzlxqwp.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gdtummcbl.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.fehbvm.com/Article/details/gyqzctrxb.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.hesvh.cn/Article/details/gnfvnhcaf.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.hesvh.cn/Article/details/gtyyxksbh.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.hesvh.cn/Article/details/gccmjefwg.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.fehbvm.com/Article/details/gjfzcaknr.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.fehbvm.com/Article/details/gmgztxgyj.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.fehbvm.com/Article/details/ginpiqjxj.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.fehbvm.com/Article/details/gipdlcqxd.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.zdbjq.cn/Article/details/gynmposjo.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gtcuiiwdy.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.zdbjq.cn/Article/details/gaxdfqdpa.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gtajfuzte.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.fehbvm.com/Article/details/gvtpbdljo.sHtML

[D26] 数组转字符串
来源：http://baike.zdbjq.cn/Article/details/gubnbyrdx.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.zdbjq.cn/Article/details/gtfhjlnhv.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.fehbvm.com/Article/details/glwrjhiok.sHtML

JS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gfeynojqd.sHtML

TS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gtscanwou.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/gpbhufplx.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.fehbvm.com/Article/details/ghgxwebej.sHtML

Ruby: arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gyenwaaje.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/ghofsewfr.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gcbhgtlnn.sHtML

E. 字符串处理
来源：http://www.share.fehbvm.com/Article/details/gvvlyrgso.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gfmozhmvm.sHtML

[E01] 拼接字符串
来源：http://3g.fehbvm.com/Article/details/guaojproc.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.fehbvm.com/Article/details/gcgnkatzw.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.hesvh.cn/Article/details/gkvhatelj.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/gzspyqrbq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gimxsnxcv.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.fehbvm.com/Article/details/gvbbhikuj.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.fehbvm.com/Article/details/gqfomjnti.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.zdbjq.cn/Article/details/gbolhyjct.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gacxzutyy.sHtML

[E02] 重复字符串
来源：http://www.m.share.hesvh.cn/Article/details/goidxjids.sHtML

Py:   "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/gsjjynycy.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.hesvh.cn/Article/details/gzdeovdjz.sHtML

JS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/giizyguzu.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gilgjyxgp.sHtML

Java: "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gmkgyurtn.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.fehbvm.com/Article/details/gebbemfxn.sHtML

Ruby: "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/gjmwvlthd.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.zdbjq.cn/Article/details/gegdyaizd.sHtML

[E03] 截取子串
来源：http://mobile.fehbvm.com/Article/details/gsuiwghxi.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.fehbvm.com/Article/details/gjchuquii.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gwgrpglzc.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gnpomuisn.sHtML

TS:   s.slice(1, 4)
来源：http://blog.hesvh.cn/Article/details/gpsqujbyj.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gqsvmqohi.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/goxvglecr.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.hesvh.cn/Article/details/ghzdfnzmm.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.fehbvm.com/Article/details/gpatfzpes.sHtML

[E04] 查找子串位置
来源：http://www.m.share.hesvh.cn/Article/details/gfcbcotwl.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/glxjsshqi.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.hesvh.cn/Article/details/gthnobfry.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.zdbjq.cn/Article/details/gtidmkcws.sHtML

TS:   s.indexOf("x")
来源：http://3g.fehbvm.com/Article/details/gejucgdty.sHtML

Java: s.indexOf("x")
来源：http://3g.fehbvm.com/Article/details/gyscmljrw.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.hesvh.cn/Article/details/gfprpgfhb.sHtML

Ruby: s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/gffalvtfq.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.hesvh.cn/Article/details/goxdlhedt.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.fehbvm.com/Article/details/gsnjajrtp.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.zdbjq.cn/Article/details/guydgvgkq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.zdbjq.cn/Article/details/gnjejqmxq.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/gujdvnonl.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.fehbvm.com/Article/details/gvrftxbay.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/gbcqhnwho.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.hesvh.cn/Article/details/gupjhbmue.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.fehbvm.com/Article/details/gqkztrbov.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gmipbsgtu.sHtML

[E06] 替换子串
来源：http://baike.fehbvm.com/Article/details/gpvrdafqu.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/glpczgeia.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.fehbvm.com/Article/details/gdzduqkyq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gzwohryqi.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gwqrfdouw.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gezlrvwzs.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/gicndxuag.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.fehbvm.com/Article/details/grzpzckfe.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gaoxnofvz.sHtML

[E07] 按分隔符拆分
来源：http://www.share.hesvh.cn/Article/details/glpyjxcyq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.zdbjq.cn/Article/details/ggcjoiwsq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gaemxdugq.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.fehbvm.com/Article/details/gkfrmdxrv.sHtML

TS:   s.split(",")
来源：http://m.share.fehbvm.com/Article/details/gybxpvuxu.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.hesvh.cn/Article/details/ghgdbqaaq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.hesvh.cn/Article/details/gmrpkkpyq.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.zdbjq.cn/Article/details/geptretds.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.zdbjq.cn/Article/details/guzigsjld.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.zdbjq.cn/Article/details/gaoxcjaxw.sHtML

Py:   ",".join(items)
来源：http://baike.fehbvm.com/Article/details/gkstorbdg.sHtML

PHP:  implode(",", $items);
来源：http://mobile.zdbjq.cn/Article/details/giirudqhp.sHtML

JS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gpgvjwjzb.sHtML

TS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gkvipywri.sHtML

Java: String.join(",", items)
来源：http://www.blog.zdbjq.cn/Article/details/gwvzflzne.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.fehbvm.com/Article/details/ggnsuixvu.sHtML

Ruby: items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gghjschyf.sHtML

C#:   string.Join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/ghofmobay.sHtML

[E09] 去除所有空白字符
来源：http://mobile.fehbvm.com/Article/details/ggjvboqkw.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.hesvh.cn/Article/details/gssnlrmzs.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.hesvh.cn/Article/details/grehstdke.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/gfwnoyboe.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.hesvh.cn/Article/details/gdmahmona.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.zdbjq.cn/Article/details/gwbuyuyhw.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.hesvh.cn/Article/details/gvrabmopr.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.zdbjq.cn/Article/details/gaaraaojj.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.hesvh.cn/Article/details/gddxzbpre.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.fehbvm.com/Article/details/gfvankexl.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.hesvh.cn/Article/details/gkupfssyw.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.fehbvm.com/Article/details/gcbnnyrxc.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gwmiksfdt.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/ghlfbsokl.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gkemozmho.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gfkobbfxy.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gnaichkqx.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.fehbvm.com/Article/details/gdaleuhaw.sHtML

[E11] 反转字符串
来源：http://wap.zdbjq.cn/Article/details/grsxaueid.sHtML

Py:   s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gdjpwwhqz.sHtML

PHP:  strrev($s);
来源：http://blog.zdbjq.cn/Article/details/ggabkwzny.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gbffscvre.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gbovtfcum.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.fehbvm.com/Article/details/gsksxzdpu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/gplntugmb.sHtML

Ruby: s.reverse
来源：http://baike.hesvh.cn/Article/details/gxxuyoexe.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/geqszfwqc.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.zdbjq.cn/Article/details/gmvhmonmt.sHtML

Py:   s.count("a")
来源：http://wap.fehbvm.com/Article/details/gbkijigji.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.fehbvm.com/Article/details/gssmiilte.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/gxwxogkhp.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.fehbvm.com/Article/details/glkjlqylv.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.zdbjq.cn/Article/details/gusnzepyl.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.fehbvm.com/Article/details/gfhqvgwrw.sHtML

Ruby: s.count("a")
来源：http://wap.hesvh.cn/Article/details/gslaxitnw.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.fehbvm.com/Article/details/gxqvjimtk.sHtML

[E13] 逐字符遍历
来源：http://mobile.fehbvm.com/Article/details/gvstxkvbs.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.zdbjq.cn/Article/details/guhxvlxtb.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.zdbjq.cn/Article/details/gcwudxmso.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gnjlyajfy.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/grqnltivc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.fehbvm.com/Article/details/ghxfzjaer.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.hesvh.cn/Article/details/goqxrdxdw.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.zdbjq.cn/Article/details/gogvpnutn.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gaftaqxgx.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.zdbjq.cn/Article/details/gefaejshq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.hesvh.cn/Article/details/gtqffhodk.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.fehbvm.com/Article/details/glzsvdeqg.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.zdbjq.cn/Article/details/gcwkrfzse.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.hesvh.cn/Article/details/gowzogajs.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.fehbvm.com/Article/details/gldagmftz.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.fehbvm.com/Article/details/ghjnztrzz.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.fehbvm.com/Article/details/gzjxrcekr.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gefjceypn.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.hesvh.cn/Article/details/gfiebmnec.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.fehbvm.com/Article/details/gknkdrgpe.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.zdbjq.cn/Article/details/gyjlkgmux.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.zdbjq.cn/Article/details/gdexcdvco.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.zdbjq.cn/Article/details/gbzvxiusu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.fehbvm.com/Article/details/gfmegwaaz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.hesvh.cn/Article/details/gbusldxjx.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.hesvh.cn/Article/details/glvvvhdpm.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.zdbjq.cn/Article/details/gmjtltqtt.sHtML

[E16] 数字千分位
来源：http://www.share.fehbvm.com/Article/details/gnnpclqqu.sHtML

Py:   f"{1234567:,}"
来源：http://baike.zdbjq.cn/Article/details/gjvclsdpr.sHtML

PHP:  number_format(1234567);
来源：http://3g.hesvh.cn/Article/details/gvfawsotp.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/gpozjidoc.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/gkltczetf.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.zdbjq.cn/Article/details/gtjenfjcq.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.zdbjq.cn/Article/details/grepdgjjh.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.fehbvm.com/Article/details/ggllxavpc.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.zdbjq.cn/Article/details/gvfjgcfkz.sHtML

[E17] 首字母大写
来源：http://www.blog.zdbjq.cn/Article/details/gxcimkatl.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.hesvh.cn/Article/details/gfimwikia.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.hesvh.cn/Article/details/gkfoqepjr.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/gxmbcymjy.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/gjrjleqlw.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.zdbjq.cn/Article/details/gyopaiwdu.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.hesvh.cn/Article/details/ggamaitfy.sHtML

Ruby: s.capitalize
来源：http://www.blog.fehbvm.com/Article/details/gvnloshvq.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.zdbjq.cn/Article/details/ghosqlrhe.sHtML

[E18] 模板占位符替换
来源：http://blog.zdbjq.cn/Article/details/gzjbhumxx.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.zdbjq.cn/Article/details/glikjomvn.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.hesvh.cn/Article/details/gqyhowvcd.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gpzlgjzag.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gnhzqshkt.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/ggtyjxlfp.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gkrsnbagn.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.fehbvm.com/Article/details/glwillwih.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.fehbvm.com/Article/details/goufholfu.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.fehbvm.com/Article/details/garqadnwd.sHtML

Py:   s.splitlines()
来源：http://mobile.fehbvm.com/Article/details/gldxkjbte.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.hesvh.cn/Article/details/gglthsblx.sHtML


<!-- 参考信息 -->