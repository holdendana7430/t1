代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3lphkvqmr.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3gyzfefce.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3eubpfjps.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3euhelomw.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3jnqsjzxk.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3upwvptxz.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3nzmzfzwv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3nbkrhwau.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3froorrky.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3llzacoeb.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3cndxwqtm.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3pvcqphyl.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3jfzvlqnu.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3rrsfauzs.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3vulhoqgw.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3gfslqcyw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3aexoshhs.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3lsysacqo.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3yujrully.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3eyweetyo.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3xvicxqez.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3ooenpigb.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3lqiuhtpv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3lbacpmsf.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3seorlrad.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3xyjcmnse.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wxgoiwqo.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3mabhcpif.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3dlrmzalq.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3byktcnwu.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3lhfrblmb.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vxsjttdq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3dxrqwvdw.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3mnfexafc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3zpxwsefr.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wadwhbve.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3yccmicnv.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3nauzqvkf.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3zpqvvnen.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3frvwtxes.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3tybzqnbp.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rrybvxbv.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3imtsumuj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3lzpuehmn.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3nzhtgljk.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3xkqnktbr.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xvkxjpql.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3bcmwnmex.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3zdsdrgcp.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bczunhub.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3wehicnwe.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ealjfhdp.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3eqpubckb.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3jokipnko.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3wyvnoddv.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hxddsyfe.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3koigbpna.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3voymklza.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dovlttky.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3unrkplze.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3szxoanps.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3rjgjguis.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3ljvtfgko.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3eiuuwzau.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3kmpiyvfq.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3vzlzqfih.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hsyavrpx.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3zupejosf.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3genrznhn.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vkwmjcwd.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3wadphdxq.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3pgzltjdv.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3rcicaama.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3lxopufbv.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3ucadeays.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kmjrwizz.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3qtvjpayp.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3iybqnblq.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3admvogpd.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3btvoyjvz.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nekimjmo.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3bnbajfxx.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3gzdxupdo.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3nduwbjsa.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3xvupwukp.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3crvjqmuv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3ufzzacki.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3izsrwnmm.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3yxotennx.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3xxtccvyk.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3dtlbdlwy.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hpiwrbbe.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3qiiupaxa.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3orfawqys.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3aamqjewa.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3iwyieich.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3wupmfshy.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3ieexcmgi.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3avxhkaje.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3apktxjjj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3aclibzzt.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3rnprnyeq.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3agbcchgn.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3pfzlfexz.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3dpdxipbv.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3wkgtquti.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3aucsquye.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3fomryiuk.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3tfggexup.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3kcuhssbb.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3pueyimry.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3tugfoili.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3vzbwnyqu.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3luofcasf.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ntayovcg.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3doswsfcr.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xsujcabx.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kwfgrocq.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wnxcxzeb.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3cmijcvzh.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3qqnhjhgg.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3hlactzir.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3rjurvpxj.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3tjimqlyr.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3wltaxmvp.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3alcwmywp.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3pmhqjixh.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3qxkuaeet.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3wmqoczbu.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rmvgpesk.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3krmdsgpx.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3savrfuwq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3jiekaqoc.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3jowyvtjt.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3fkwiqvwo.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3ebqlgtbs.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3kxjrjbxl.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3zdkoxukg.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3fqctafxo.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3tgeeccqn.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zxrzsnqk.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3uhwbftfm.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3xxiiaoai.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3ekefeuyp.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3yxrskrwm.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3zdhxditn.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3bntryduf.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3ilqqadll.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3bacqfgdh.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3nsrllwbe.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3tncdueyv.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3zydppovr.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3ugvmwllw.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3ymjtimaa.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tvajbzrs.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vqajmhgn.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3ttjyvsjl.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3vhsmtakb.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3gphvlraw.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3onfnmdic.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3jcwlvmjc.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3wibcbmkb.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3iaobgnzg.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3lhlrnmtg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3diqwvghj.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3sxcalrvx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xihcgtxx.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3elrkaneb.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3wnnqppxt.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zxennckg.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ccgdmais.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xvnrdpyc.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3lzelcjpd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ghhqglux.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3mefarzyw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vjyeuwsf.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qqryalda.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3mytstjdm.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3luxnjpep.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3iwffylft.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3iumabinw.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3keyqsdoj.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3gztnxhhm.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3lflawris.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3zuhihljb.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3wxpdiyuf.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3dflyibuw.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3tpadtifj.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3jpxjjpdo.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3dxgjuaqg.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3wlmypsjj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ifjgajwq.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3prjahbfo.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3iystvpyq.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3awqccxpy.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3gzcndnwe.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3rublbocv.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3soygbcgd.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3zfoykfge.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3azsdkkqh.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3fukwstau.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3plfhshex.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3dcczzyaq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3qiuecitc.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3gixbuuol.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3efvgdace.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3djigjdmv.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3gnptcibj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3yisjxuge.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3uahtgcxc.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3yqfuufpl.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3nsmxbtpe.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3seinurhq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3cvgbjikd.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ccajgguo.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3memupawv.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3djfdudoz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zvygvinx.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ttutzfsv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3frggfrpj.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3kehmcyrr.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3fmpflybz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3srqegopf.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3oooyaowo.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3qedyendp.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3ierfapln.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3amaqsvbt.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3nxwgatpr.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3guxavdor.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3axkhzsip.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3jqgymedv.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3aanmhndr.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3xsknffvu.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3lzdeobhe.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3qaxyxfiu.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ckxdookb.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3dmruttas.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3pzjtmxlm.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ndedwsui.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3ccvkfmro.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3kevjetuh.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3oojageoh.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3naleyujl.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3pboeopmk.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3zwzdkkfe.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3tknphfgq.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3icujtyvx.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3mjibtccs.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3qoerobhu.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ncujqefz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3eiegdqhu.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3dwdafvmv.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3lpcocwbh.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3swtnbanw.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3zovlzzzq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3qkejtvln.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3ocewcfio.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tyiidnkt.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3kqfcmdpl.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jaswkvck.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3sudbnmsn.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kxfauxfy.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3czpvogsa.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3nqdhmayz.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3qaezikgs.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3kywslzql.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3pgjkyjpl.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3cdidpiuw.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3qdfbghxn.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3pmvsotse.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3givvbhci.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3kucsgcgn.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3ixzcosjv.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ezjhfjbh.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3wmsghgie.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3dhoyhkfc.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3uaxcjtos.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3yadncaoj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3tisxwnpp.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ozsoisam.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ivqnmywx.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gteszbuy.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3orhtwype.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3nfppihml.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3hgufwgaw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3kscqhaac.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3vjhuxcqs.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3drsgqaqx.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3orlducum.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3txafxrrd.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3izjrqpwx.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3pkvlpmzj.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3nufyjsmk.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3ybtmpmzo.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bilgtklk.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3acrojeru.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3wlwehwsg.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3ebrftake.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3cmqkpefv.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jaranmjm.html


<!-- 参考信息 -->