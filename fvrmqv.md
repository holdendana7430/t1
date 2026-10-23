代发 wailian999

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3siciokxh.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3lgjlalfu.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3yhkyxaoi.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3qexnnkgu.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3kzzmklru.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3aqupqael.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zfoceyqa.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3wspmmjdj.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3khkluzyd.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3bwbgpplz.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3dfsyuskr.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3eispdccr.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3jqnhvljq.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3syyjkbsj.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3ygqhqyyq.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qkxzdqnr.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3ppvwkjmi.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3lyqfphii.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3gytzqnve.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3mzflyjpd.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3tbanierx.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3lkhsvxfh.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ttcebqpw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3ztaaulpv.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3wigtmelz.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3roctolwp.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3tpccshef.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3rrfuggqu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3argdetdb.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3yktwdqtw.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3kysaunmu.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3rwbkhrwd.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3lpgumsbn.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3qwqegvpe.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3sltzzyvo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3huabbanf.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3frzedfsl.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3migvgvwx.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3kfbioksv.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3cajnozpt.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3rptroxyq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3ybikaeni.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3ohwqoorh.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3viaogjqy.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3ppxbgvpm.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3wesmofgq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3xqtflpuq.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ppnhtiyt.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3wlrctaen.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3akqztbhn.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3izwuxhvf.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3eyhbpgjw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3gkmmkxaj.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3ysfhbrib.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3rvjfxfqr.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3coilgnia.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hrtwtzcj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3omnobyti.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ofsfkvqh.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ytpmqejr.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rklakwjq.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3edgfvdeb.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3tvpleous.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3dcnoxtei.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3mrsdcrld.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3gpnsgfkt.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3izttitgc.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3ipusonou.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nxiteyya.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3bzotydfc.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3kmacabfq.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3mqysaeky.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3xzsuidfg.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3siskfbcw.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3gsawnjuh.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3xraqlvgk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3nkiyxuyo.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3lkiyoueh.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3ypaqginn.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3qmbmysfx.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3pmkitmgn.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3itqalaos.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3foeidvur.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3owpbnvld.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3iucbtvrq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3qmxnjsbd.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3knduazjr.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3towtzows.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3helhqsmu.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3ibrjsdmu.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3wjxqrnwm.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3dvzzfiel.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3frnotbxm.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3tdooiziu.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3hwztadze.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3peardzkz.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hhgwsinh.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3irnyzrpo.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mlvxsxnl.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3stomwzcy.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3mfcryafb.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3vcqwviap.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3mbqdhuie.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3fnnkcbqr.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3lyhwqlpe.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3wsmzdtfj.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3iligbrwi.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3kmeagrmo.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3dsvmedic.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3zgotkhgi.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3xabwiija.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3oquhjxdw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3wphknxgu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3vaxmawtd.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3jusjzmhs.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3lzmiqddi.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3yhtyluat.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3dhwmowaq.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ujsaoiyo.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3yrirkdoc.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qmxpkjyp.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3wcwjijgb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3poodkcvh.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3qpoqprly.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3ipsgaezs.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3fpddxfau.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3hgerisij.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3wvndvaic.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3klnqqpgr.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3drfehywy.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3fbtfhnkw.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mcgswoqx.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3jpqiccjn.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kmuigyjf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fettfhfg.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3xbgcidii.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3meqhakba.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mpnctnnu.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3cpskrdno.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3qcykdhvb.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3axnkksmp.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3euxsvnjk.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3obrnembv.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3mbtobcue.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xruyczbs.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3csiutamj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cjwlkzcv.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tycftlom.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3strdlywv.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qeqdbyrb.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3hhcnodrq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3bpinohgn.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3drhetgrf.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3gwsxcgds.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3lsseaxgp.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3thgiskfh.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3eewbsmxo.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3dsovjnmi.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ohfyapbn.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mqhkwdqu.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3eukxaxkx.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3tywyuojv.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3mlqvhftk.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3karbzwbe.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3grhyanyz.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3ybmawbus.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3ctmbyqts.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3uwkyhjdv.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3zzwqmjoj.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3qclukxlc.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3rghfpbeh.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ztzjechc.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3gxrrszjy.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3esjejnhr.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3cbhpmlci.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3zoyejuhm.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3ejikiaah.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3kfmyukwz.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3tkrbcsec.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3gnyxmegl.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3wzrcvmxh.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3lwzmgufk.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3wusiuees.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3rpedpocg.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3jknqjeox.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3rofdgwta.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3zlyopvkt.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3hiezmava.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3vjfmjecd.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3qmyzwkfz.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3mhqtwspc.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3gfdxjwba.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3xophpkle.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3fkjneztz.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wwabsacn.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3izwikslb.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3chkofbsu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3cghzotud.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3gvrkerhx.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ficzkxzh.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3anynshqz.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3txqqzboq.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3slhkzpot.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3cxvghfmw.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3wehdudow.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3bjhfweey.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3xbpmaljp.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xnwpeypd.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3lijruovg.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3tikqprac.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3rmuirbqc.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3nfwsgwft.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3sldopuif.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3hemywwfj.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3rpniomrd.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3yjofkxcu.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3opuxliyw.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3icfepbiy.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3jmblthqe.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3xakwuzal.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3uzpfdnse.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ibjzqxqh.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3sjuoqnpv.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3nxtccdau.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3mfvyylaz.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3rszwxyuz.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3wxwqhoha.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3eqizurmt.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3oicrccax.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3jjuaipgl.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3oyshvhpc.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3fyyfwodh.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3rfvrwzog.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3papalzcs.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3zeyohpnq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3qtbldarw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3jbhnbroo.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3chufdnbc.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3iwbnntnd.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3dxgjwxre.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3mddhmtoz.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zyqvmaqi.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3tffamlxo.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3wncmefdw.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3zffgbjgy.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3avzwvcms.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3xeihnnmo.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3meayxlmr.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3qfhjyncy.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3ykgllntk.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3iouubsco.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3erscmird.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3dfnyndbo.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3fhejhuey.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3ojoztxls.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3rlkocxdo.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3ttopiwxi.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3mxaihopb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3voihavnl.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3mzkaxyet.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3yjocrtql.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ljtjdwne.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3ipinejqf.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3afsazwtm.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3nscazzjl.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3gtpgduoo.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jncicfht.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3nevujajj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tbvupski.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3wwaibgmj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3mixavynk.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3rqxugbqv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3irbceder.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3buysdjmz.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qxvrwyum.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qrnsjwph.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oukrffpe.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3rsrjnkki.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3basvsiot.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3njvjrzbx.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uwklhzme.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3jtclzuch.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3btkdeiow.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3rlovjglh.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3hpyckwte.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3ygsfqsum.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3uaefufls.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3glmhlkyp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3xrchjjzj.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3rhrsqyqv.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3wxzquycc.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3nyqtnuyr.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3oezjsxwx.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3phtanxqq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lsnlhaxr.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ynbskmqk.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3pyxejeuo.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3rosfyvqc.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3pagxptch.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3esxlndfn.html


<!-- 参考信息 -->