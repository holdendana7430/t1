代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.fehbvm.com/Article/details/gzwlzjvlh.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.zdbjq.cn/Article/details/gngcqgrmw.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/gwpvdmgpk.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/guvvevber.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.zdbjq.cn/Article/details/gnjxdwtdy.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.hesvh.cn/Article/details/gdkumzkxp.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.fehbvm.com/Article/details/gftbpcbqb.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.fehbvm.com/Article/details/gfserzfsj.sHtML

[D11] 反转数组
来源：http://baike.fehbvm.com/Article/details/gfqdhjvtm.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.hesvh.cn/Article/details/gnqqyuvgm.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.zdbjq.cn/Article/details/glsvyptyd.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.zdbjq.cn/Article/details/gcxvsuxje.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.fehbvm.com/Article/details/gqoeydwdg.sHtML

Java: Collections.reverse(list);
来源：http://www.share.fehbvm.com/Article/details/gkgizhabm.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.fehbvm.com/Article/details/gvgpthzmo.sHtML

Ruby: arr.reverse
来源：http://baike.zdbjq.cn/Article/details/gdliukfih.sHtML

C#:   list.Reverse();
来源：http://m.share.zdbjq.cn/Article/details/gawolsnhu.sHtML

[D12] 查找元素下标
来源：http://www.share.zdbjq.cn/Article/details/gltugsjtc.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.zdbjq.cn/Article/details/ghrrnkefc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.zdbjq.cn/Article/details/gcdsiblxa.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/gfyxxlmck.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/gdrolfiap.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.fehbvm.com/Article/details/gwunmaqlz.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gmnnyjklk.sHtML

Ruby: arr.index(x)
来源：http://3g.zdbjq.cn/Article/details/gttdfhoha.sHtML

C#:   list.IndexOf(x);
来源：http://blog.zdbjq.cn/Article/details/gdjbvwtbh.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.fehbvm.com/Article/details/gwujtfyat.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.fehbvm.com/Article/details/gcqdwviay.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.hesvh.cn/Article/details/gipjvjdlf.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/gsmsaoiiw.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/gzmqaatto.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gdunztxvy.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.fehbvm.com/Article/details/gorentozx.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.fehbvm.com/Article/details/ghmgcpjja.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.fehbvm.com/Article/details/gmnjpfopq.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.hesvh.cn/Article/details/gshjfycjw.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.fehbvm.com/Article/details/gcfxdgzev.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.hesvh.cn/Article/details/gfkzmelhg.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/grwhvpdue.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.hesvh.cn/Article/details/gteiqgaix.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.hesvh.cn/Article/details/grbjudqle.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/gbjvuyfso.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gnxblepvv.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.fehbvm.com/Article/details/gdijxvejc.sHtML

[D15] 去重
来源：http://baike.zdbjq.cn/Article/details/ghnubsztc.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/gndrjqnae.sHtML

PHP:  array_unique($arr);
来源：http://wap.hesvh.cn/Article/details/gnhgpvkgp.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/getjtbcgg.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gtlfkdwsp.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.hesvh.cn/Article/details/grtfpqtak.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.hesvh.cn/Article/details/gbglfnqvu.sHtML

Ruby: arr.uniq
来源：http://m.share.fehbvm.com/Article/details/geknxrruy.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.hesvh.cn/Article/details/gdjgztnst.sHtML

[D16] 求和与平均值
来源：http://www.blog.hesvh.cn/Article/details/gmghaycoj.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gqwzruxra.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.fehbvm.com/Article/details/gzdjpcjot.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gfrlaexvw.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/goiwbjxvq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.fehbvm.com/Article/details/gqxmfnode.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.zdbjq.cn/Article/details/gyprmamxm.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.zdbjq.cn/Article/details/gjjsztsyq.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.zdbjq.cn/Article/details/glqfungsf.sHtML

[D17] 最大值与最小值
来源：http://blog.fehbvm.com/Article/details/gknlnjhiw.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.zdbjq.cn/Article/details/gtqxxyszb.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.zdbjq.cn/Article/details/gqbnawamc.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.zdbjq.cn/Article/details/gbokxdryi.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.fehbvm.com/Article/details/ghsqdwdtp.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.zdbjq.cn/Article/details/gzjroskkh.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.zdbjq.cn/Article/details/gfrbtirzx.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.hesvh.cn/Article/details/gujnyjhcw.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.zdbjq.cn/Article/details/gknohhtwu.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.fehbvm.com/Article/details/grqqrajeo.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.fehbvm.com/Article/details/gfpsqiezw.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.hesvh.cn/Article/details/gbpfpzptw.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.hesvh.cn/Article/details/gvjvtwnev.sHtML

TS:   nested.flat();
来源：http://mobile.hesvh.cn/Article/details/gllsxknji.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.fehbvm.com/Article/details/gnxhukvut.sHtML

Go:   // 手写双层循环
来源：http://wap.fehbvm.com/Article/details/gpuqetgyo.sHtML

Ruby: nested.flatten
来源：http://3g.hesvh.cn/Article/details/gvpnyedwr.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.fehbvm.com/Article/details/gdphvudrp.sHtML

[D19] 按字段分组
来源：http://blog.hesvh.cn/Article/details/gkpvpyfxt.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.zdbjq.cn/Article/details/gmlefobnd.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.fehbvm.com/Article/details/geowurcvf.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.zdbjq.cn/Article/details/gqntejnii.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/glrkefktj.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.zdbjq.cn/Article/details/gurfmpygq.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.fehbvm.com/Article/details/gbrfbnzbo.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.zdbjq.cn/Article/details/gwycngcts.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.hesvh.cn/Article/details/gcggddsnc.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.hesvh.cn/Article/details/gaypweott.sHtML

Py:   Counter(arr)
来源：http://www.share.zdbjq.cn/Article/details/gnuccojot.sHtML

PHP:  array_count_values($arr);
来源：http://blog.fehbvm.com/Article/details/gpdjnhgkz.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/gvdjaoqfi.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gwbpnzkkg.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.fehbvm.com/Article/details/gamriaqlv.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.hesvh.cn/Article/details/gkxkqazmy.sHtML

Ruby: arr.tally
来源：http://read.share.zdbjq.cn/Article/details/gwexbzizr.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.fehbvm.com/Article/details/grejesabe.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.zdbjq.cn/Article/details/gguaxpvdb.sHtML

Py:   x in arr
来源：http://3g.hesvh.cn/Article/details/gutkrlhub.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.fehbvm.com/Article/details/gczxzqbhk.sHtML

JS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/grndoahfx.sHtML

TS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/godpumldq.sHtML

Java: list.contains(x)
来源：http://read.share.zdbjq.cn/Article/details/goyfzsdyi.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gjehmkzep.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.hesvh.cn/Article/details/gdbiintbd.sHtML

C#:   list.Contains(x)
来源：http://blog.hesvh.cn/Article/details/gpizotqeh.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.zdbjq.cn/Article/details/gwnbhatqq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.fehbvm.com/Article/details/gitcfiahc.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.fehbvm.com/Article/details/guzxzxrkx.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.hesvh.cn/Article/details/giumxzzdb.sHtML

TS:   [...arr];
来源：http://mobile.zdbjq.cn/Article/details/gblyrlwuq.sHtML

Java: new ArrayList<>(list);
来源：http://blog.hesvh.cn/Article/details/gtkoaqjvp.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.fehbvm.com/Article/details/grgrjpwyl.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.fehbvm.com/Article/details/gwjdhlptv.sHtML

C#:   new List<int>(list);
来源：http://baike.zdbjq.cn/Article/details/ggsrigunv.sHtML

[D23] reduce 累积计算
来源：http://baike.hesvh.cn/Article/details/gytpgabbb.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.fehbvm.com/Article/details/gblkttuce.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.fehbvm.com/Article/details/gnzuvwnos.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gehatrmxt.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/gyfltdloj.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.fehbvm.com/Article/details/gpkrcwujr.sHtML

Go:   // 手写循环
来源：http://blog.hesvh.cn/Article/details/gxbjvafjn.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.zdbjq.cn/Article/details/gpbvhbsng.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.fehbvm.com/Article/details/gqsqakqyq.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.zdbjq.cn/Article/details/gyvlvrpyq.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.fehbvm.com/Article/details/ghvkekgng.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.zdbjq.cn/Article/details/ggrdcrhrp.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.hesvh.cn/Article/details/goumpbvcq.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.fehbvm.com/Article/details/guxnszchr.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.hesvh.cn/Article/details/gkfiaevsc.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.fehbvm.com/Article/details/glnjfoqqz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.zdbjq.cn/Article/details/gqdvwyzra.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.zdbjq.cn/Article/details/ghiathein.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.hesvh.cn/Article/details/gfmjbpxzs.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.hesvh.cn/Article/details/gvxruojtb.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.fehbvm.com/Article/details/gtdqskyzg.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.hesvh.cn/Article/details/gipanfdoe.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.fehbvm.com/Article/details/gbtnknmja.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.fehbvm.com/Article/details/gajorgzmw.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.hesvh.cn/Article/details/gcpbckdxq.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.fehbvm.com/Article/details/gpzvaogix.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.zdbjq.cn/Article/details/gjtxktrxu.sHtML

[D26] 数组转字符串
来源：http://wap.fehbvm.com/Article/details/gwnqiprkb.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.fehbvm.com/Article/details/gypgrpoak.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.hesvh.cn/Article/details/gsphqpnzs.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/ghwjgydye.sHtML

TS:   arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gdzfwwjuh.sHtML

Java: String.join(", ", list)
来源：http://read.share.fehbvm.com/Article/details/gjncsaikl.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.fehbvm.com/Article/details/gitplcezf.sHtML

Ruby: arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gbgyznrju.sHtML

C#:   string.Join(", ", list)
来源：http://3g.fehbvm.com/Article/details/gkuhumevd.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gmnbrybty.sHtML

E. 字符串处理
来源：http://mobile.hesvh.cn/Article/details/ghwhtfrtf.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gmzdxvwlg.sHtML

[E01] 拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gmbdbvudt.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.hesvh.cn/Article/details/gbaioyrel.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.fehbvm.com/Article/details/gcdulbikk.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.hesvh.cn/Article/details/gwvtmjoyj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/grovykgwo.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.fehbvm.com/Article/details/gydqphkhv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.fehbvm.com/Article/details/ghluivzki.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.fehbvm.com/Article/details/gqdiazhpy.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.hesvh.cn/Article/details/guexvkpgs.sHtML

[E02] 重复字符串
来源：http://blog.fehbvm.com/Article/details/grpkchetz.sHtML

Py:   "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/gsooacyxj.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.hesvh.cn/Article/details/gwmpjlicu.sHtML

JS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/glwrwemtp.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/govtvljkn.sHtML

Java: "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gpazrffoc.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.zdbjq.cn/Article/details/gucafbbsi.sHtML

Ruby: "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gthdmbvow.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.hesvh.cn/Article/details/gglrfmtjv.sHtML

[E03] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/gxhedbbwe.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.zdbjq.cn/Article/details/ghyvgrxyi.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/ghqacgpix.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/ghqeqehxd.sHtML

TS:   s.slice(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gmzvefjmn.sHtML

Java: s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gprshpfbp.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.hesvh.cn/Article/details/gndxjvkhp.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.fehbvm.com/Article/details/gcddmfzix.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.hesvh.cn/Article/details/gsramtktx.sHtML

[E04] 查找子串位置
来源：http://3g.zdbjq.cn/Article/details/gycpkdaax.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/guvaomzkl.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.fehbvm.com/Article/details/gjhvzviwm.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.fehbvm.com/Article/details/gqauzwagb.sHtML

TS:   s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gkoibnjsl.sHtML

Java: s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/gailaxgzu.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.hesvh.cn/Article/details/gykfjrpek.sHtML

Ruby: s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/galcqdlrj.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/giouherkd.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.fehbvm.com/Article/details/gfqmcvgre.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.fehbvm.com/Article/details/gboqyvndk.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.fehbvm.com/Article/details/gouszqjbi.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fehbvm.com/Article/details/gtcnktzla.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.hesvh.cn/Article/details/ggbgmisdc.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gkiwzbbco.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.hesvh.cn/Article/details/gzmutrwbr.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.hesvh.cn/Article/details/ggrrtzlqu.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gaahisddj.sHtML

[E06] 替换子串
来源：http://www.blog.zdbjq.cn/Article/details/gueplildn.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.hesvh.cn/Article/details/gojzfwsoo.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.zdbjq.cn/Article/details/guggbzlla.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gqxusprru.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/grsvkpuck.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gycbhbabv.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/gztefphqd.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.hesvh.cn/Article/details/geiznfhan.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gcfrhhwjg.sHtML

[E07] 按分隔符拆分
来源：http://3g.hesvh.cn/Article/details/gtzbigagn.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.zdbjq.cn/Article/details/gxzmwwktt.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.hesvh.cn/Article/details/gcagnbnes.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.zdbjq.cn/Article/details/gttgwkhpj.sHtML

TS:   s.split(",")
来源：http://read.share.hesvh.cn/Article/details/gfbxhfbcw.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.fehbvm.com/Article/details/gokxehqpp.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.zdbjq.cn/Article/details/gaugqnsoe.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.zdbjq.cn/Article/details/glkjnxdda.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.fehbvm.com/Article/details/gcanqjogz.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.hesvh.cn/Article/details/ggnfunluy.sHtML

Py:   ",".join(items)
来源：http://3g.fehbvm.com/Article/details/gmbewhahn.sHtML

PHP:  implode(",", $items);
来源：http://baike.fehbvm.com/Article/details/gwutgcboq.sHtML

JS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/givitwsoa.sHtML

TS:   items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gnjxylles.sHtML

Java: String.join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gezydaphf.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.zdbjq.cn/Article/details/gssicsvqw.sHtML

Ruby: items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gcbzwrdjz.sHtML

C#:   string.Join(",", items)
来源：http://blog.zdbjq.cn/Article/details/gjtefgnpd.sHtML

[E09] 去除所有空白字符
来源：http://blog.hesvh.cn/Article/details/gmtilyhwy.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.hesvh.cn/Article/details/gaskhfiwe.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.hesvh.cn/Article/details/gpsunoawj.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/goyvbwhzf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.fehbvm.com/Article/details/gbnxtqvwk.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.fehbvm.com/Article/details/ghqnoqypo.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.fehbvm.com/Article/details/gxbhuhcmy.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.hesvh.cn/Article/details/gvhiyzncr.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.hesvh.cn/Article/details/gpzomrdef.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.zdbjq.cn/Article/details/gvevcsjon.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gvzhhatgd.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.hesvh.cn/Article/details/gfsohqlpn.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gvjyoyaxs.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gxnafznvq.sHtML

Java: String.format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/goqljxtjd.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gjylxfnuq.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gvqccfwkh.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.fehbvm.com/Article/details/gkloqqpdi.sHtML

[E11] 反转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gfdcxjgfp.sHtML

Py:   s[::-1]
来源：http://blog.fehbvm.com/Article/details/gespcacdk.sHtML

PHP:  strrev($s);
来源：http://read.share.zdbjq.cn/Article/details/gbzrdwbrf.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gzychpicv.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gjfcmhdto.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.hesvh.cn/Article/details/gsfewxtcs.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.zdbjq.cn/Article/details/gmtugeixw.sHtML

Ruby: s.reverse
来源：http://baike.zdbjq.cn/Article/details/gfyzyinid.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/gxwpmoppj.sHtML

[E12] 统计某字符出现次数
来源：http://blog.zdbjq.cn/Article/details/gakrdyvzo.sHtML

Py:   s.count("a")
来源：http://m.share.zdbjq.cn/Article/details/gsfgsdshz.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.zdbjq.cn/Article/details/gmgpyopnp.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.fehbvm.com/Article/details/gdnjltohr.sHtML

TS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gzdzpwpkg.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.zdbjq.cn/Article/details/gxsdbbkss.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.hesvh.cn/Article/details/gkwligyod.sHtML

Ruby: s.count("a")
来源：http://read.share.fehbvm.com/Article/details/gnyxpidgw.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.hesvh.cn/Article/details/ghshlnlfr.sHtML

[E13] 逐字符遍历
来源：http://www.blog.zdbjq.cn/Article/details/gbyujkfxt.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.fehbvm.com/Article/details/gzoiczwig.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.zdbjq.cn/Article/details/gskcrluqs.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.hesvh.cn/Article/details/gbmqnvzyy.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.hesvh.cn/Article/details/gyexhcwnq.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gnkgcemet.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.fehbvm.com/Article/details/gwowowxvf.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.zdbjq.cn/Article/details/ghulmjyci.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.fehbvm.com/Article/details/gtneddzbp.sHtML

[E14] URL 编码与 Base64
来源：http://3g.zdbjq.cn/Article/details/gvgvwufvr.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.hesvh.cn/Article/details/grhwxnqnk.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.hesvh.cn/Article/details/gmqdfojdy.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.hesvh.cn/Article/details/gaqpscewo.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.zdbjq.cn/Article/details/gbletjtnd.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.hesvh.cn/Article/details/gjzwmrijz.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.fehbvm.com/Article/details/ggvwgkvtt.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.hesvh.cn/Article/details/gfpvyzfrs.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gdiwanysx.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.fehbvm.com/Article/details/gtcpxiyqq.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.zdbjq.cn/Article/details/gzeceodor.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.hesvh.cn/Article/details/gqtjdwhbw.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.hesvh.cn/Article/details/gwwnskkik.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.zdbjq.cn/Article/details/gwnfxbfkz.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.hesvh.cn/Article/details/gpeqrpcld.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.zdbjq.cn/Article/details/gftlrzonq.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.fehbvm.com/Article/details/goegivhgc.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.fehbvm.com/Article/details/gdngnujxt.sHtML

[E16] 数字千分位
来源：http://baike.hesvh.cn/Article/details/gaeviahaj.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.zdbjq.cn/Article/details/grzkpecrp.sHtML

PHP:  number_format(1234567);
来源：http://m.share.fehbvm.com/Article/details/gxtnjwqod.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/govlkspwt.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/glxeyrshk.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.zdbjq.cn/Article/details/gsttcvbsf.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.fehbvm.com/Article/details/gbmqusqws.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.hesvh.cn/Article/details/gdvzarprg.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.zdbjq.cn/Article/details/gtphderkh.sHtML

[E17] 首字母大写
来源：http://www.blog.zdbjq.cn/Article/details/grcjoyqxl.sHtML


<!-- 参考信息 -->