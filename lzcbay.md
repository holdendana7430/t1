代发 wailian999

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3zvngstai.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3leplrgsh.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dzkpzpuh.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3pehohill.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3jrulzjez.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3wvtrkcuy.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3ylkivpuo.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3hvyiajcz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3aztyuief.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3dcbemzuj.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3ufmpzarm.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3yhimaebd.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3abeikmbm.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3thvsdwiq.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3hfxrcuth.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3hwpwdogm.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qykbryez.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3refasstz.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3vgqsjmwz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3yhdvknit.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3mfbxvvpe.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3utcislaq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vmfzxwnk.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3rekfwpyf.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3dzlxmusm.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wcttglef.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3yeonxjzc.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3epczdjoz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kwnukvbw.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3jatswajl.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3jcajwmmh.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3bofskslv.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3fbiyzobb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3licdbbzb.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pmdiixri.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3lloefjis.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3qdgeseaa.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3xneoavfh.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3xkdeuhcw.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3qwmzgdgi.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3fljrrewe.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3odbtbimd.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3gjwwiidr.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vrlwsixh.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3chwfkkyn.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3egsgovxd.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3ctagkfgr.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3gqogpldx.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3tayvsiay.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3mhidqlvp.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3tndyhape.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hqnjcxaj.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zprdpegk.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vtineqfj.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cjolckjx.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3ngfivbtg.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ptukhxkp.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3ezngqdlx.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3vxpswite.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3tpuenahg.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3fxrdhpeg.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3drrjlpjf.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3ftnyfpef.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3sgvmxous.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qcvzjjbp.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3dowbadpx.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3tuzqkjab.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3miooazai.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3fnjzujzo.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3ndoeobad.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3lhlzwnfj.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3towifdux.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3hyuujcin.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3huencffo.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3hyrxxvgi.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3tebtlxps.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3gkfiflpu.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3xzpkpacu.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3owuonaak.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3jbtakkbx.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3vovlwaig.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3qhtwvylv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3rehnoetm.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3nfjwntuq.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3iytyrqwh.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3calerwbc.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3javtuvmt.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3xjpzbqfs.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3reaonwww.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3utmvtaos.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3fafnxrln.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rsvfvebo.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3sxroyhyq.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3gtdigcwd.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tmdpqzml.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3ynqszolc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3iuyjvajx.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3yfiysbdq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ategxtlt.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3eribizmv.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3typsknjq.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3klksqlxr.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3hweausax.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3clsophur.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3waipqnus.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nmjebase.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3sqiaghfe.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3okiemrcw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3faemxraq.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3qjdpjpkv.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ymfgavrh.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3dupxmmxu.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3whurosti.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3qccobmnn.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3gztrtuks.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3utamxphn.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3ffejwysc.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dxitxbrb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3vaaaarxq.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3zgbeqydj.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3qlumabkt.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3jlydrmrr.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3xcwizsyz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3gajzrarv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3ayojrqcw.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3eshtwjpq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3kaaxwuag.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ayynuqds.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3euuwbokq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3zzpqsqzv.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sgcsxuae.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3grifowuo.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3awobmimg.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3giidwseb.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3cxxgicjk.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3zbuwoofr.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3zypzarfq.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3jpjmunvh.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3hakhsivm.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3wpifhsyx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bwagrukr.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3vmfsmivx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3szgkhxuk.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3lzfwvfoq.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3yibywqvk.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3fkzivgpg.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3byurknwj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ptglstda.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3emlsfnrz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3riptlsnq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3xojdzygu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vpujlemk.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cegatugo.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3kggfqera.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wcvlgluu.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hpnimhev.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3klzswtzz.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3xqiiexrv.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qdrppyby.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3njxxhvks.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3pyxshvtm.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3toorihhh.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3vogeachp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3zxetibkn.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3dzfmxipl.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3afortzmv.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3gvologsz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3jpurqahn.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3bthwaudv.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3imqkiixh.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3aagbxzyw.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3syiusmac.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3hvxqqjgi.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3qdjnbjcf.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3lamlddds.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3wdgfnqoa.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3lkyirlqx.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3wgyikxwu.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3mcvbfvqa.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3jmmjgioc.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3syihmwmu.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3gfovnfzg.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3eyeqonbe.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3voqotfmv.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3gjrzpuic.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3qhcynzei.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3xxctutmn.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3eyrlbokc.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3eqwaoirz.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3aksnxiqo.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3uwmaijat.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3aspykhpm.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qjazqagp.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3tqnxbsev.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3liqbybca.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3udebmwzx.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3laljcjpb.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3babfnlpj.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3sbmnvjey.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ojujjlqw.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3kweivvaq.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3vptyajhj.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3dsbiawix.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3tczwbpro.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3fpznrtgp.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3asaqoswd.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3jfuqvftp.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3bqybmoml.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3onrqdcbc.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3nksgghni.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3apjfaxir.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3zzqtazic.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3tbbtuglr.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3udumhsql.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3lgeiswtn.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3bvbcybnj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3jnsjnjcx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3tcmmtqhz.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3lofzizmf.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3vksdzxaq.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3ieecpfiw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3mttkamuc.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3cfatncat.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3uqterywh.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3xjbldnkm.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3pjtplipy.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3kcktfomc.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3gjlwxlyv.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3qhooumjm.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3rcqhjvrd.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3amwkecvm.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3egobdzei.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3stznhnmj.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3jpkvwmjr.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3vvauwyxy.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ssfsmqvx.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3yemkmngt.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3uvlfjjkz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3mjxtoztw.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3bjtaisja.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3vcbkjeay.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3xerqhgrw.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3zoynvlqb.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3cnxjfodu.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3hzrywzis.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3fvwfevfl.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3vuzxbhtn.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3cpmzfepf.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3qkkhviks.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ikruyprc.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3nwzvuseq.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3vzeqjsse.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3whsroxtn.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3yfatmsvl.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3goauhmem.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ilwqgbqf.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3gztybnjy.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3brtvzyxm.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3lcpftykx.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ytpbxsnn.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3wibbsdcg.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3zwnobdke.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3osxvcfxp.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3ocxjqfqm.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xgmgddeu.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3xqfymzce.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3rgonfeax.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3xjogqrti.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3svbgooiz.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3qyxmxsng.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qookopqo.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3reukssqn.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jhzjmwah.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3xpbmutht.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3pknrobkl.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3anpomdac.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gwapswix.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fnuniivm.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3zxclryvl.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3qctvriuz.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3hxsalsrh.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3dpojmodp.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3heyawhop.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3sotnouwq.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3csammytu.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3kqdgqwzi.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3ihzsnowd.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3rpwqzqpq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3nsquktfl.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3ccdaqude.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3lvjbhtgi.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3pgrgevfz.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3riyjfagm.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3bytgwgow.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3yoxtoctx.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3qadrqxdg.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3jwssekgq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3adivtinx.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3zoxnclhu.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ctuobwqt.html


<!-- 参考信息 -->