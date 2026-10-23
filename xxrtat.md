代发 wailian999

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3fqvpkgrj.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3oikyoyto.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3xbqwewht.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3nluarekg.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3szazjwnq.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3sefpxtgz.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3ydteiuzq.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3vnewdgth.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3asblohjg.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3wlzodvgo.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3ftpkjqba.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3wynlwrbi.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3gycbswld.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3frmssstv.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3awhydvwu.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ycpuoblr.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rzdrrjio.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3tzifeypo.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3ldnjkqjq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3zhycfrte.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3mzxyzbqy.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3ehgfvvkk.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3pagzoohp.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3vzqytaez.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3jybtlolk.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3bjiackcz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3qjvwenkb.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3asdkmjsi.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3jrbmmvhb.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3urjzmwbh.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3tbnsxdxj.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xvjlqmbp.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qozmniew.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ksswlhfl.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3yellzkjz.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3jmzwqlvm.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3qqlncqbb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3sajitcsm.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fvusprgj.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3groaberd.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3cmocpqjd.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3bdhevshn.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3fwmpavnh.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3kmsmcbqr.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3dshsrauy.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3hkhbzcpw.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3vrjopnzo.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3wowpxauc.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3eixltscu.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3tolujhwc.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3mwxqwdrm.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3iyiqzyjj.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3hadiwxsa.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3paguaxct.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3qntmoxgj.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3rplpvnuo.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3ferxnjfs.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3brhmvogq.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3kxegfzdf.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3kjdpzwoi.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hdlwfzyu.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3ygejheiu.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3vyimqnzj.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3ylxlfvqu.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3kartmhjq.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3yliekail.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3cqtdsxtz.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3ewnabcpf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3djexrubh.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3gxusoabq.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3xncjwuzp.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3qlpesbtm.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3zpvylmvk.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xkvnxrux.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3wunukbwo.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3ljiempxl.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3chahwnip.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3krhrhxkj.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3qfjaeztq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3cuwwfyxr.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3teeuzfwo.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3napunqcx.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jhwpmrtr.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3ncpnqjsd.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3smqwkfge.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3gwpvqmlr.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3yurjgizc.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3alrjqhza.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3elujxvkn.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3unagamya.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3wvblrdhb.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3mshyvakh.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3dcpqyvhf.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3kvcsreen.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3utalkzaj.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fbrolrgg.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zyybasub.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3czuolhda.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lxmluvbs.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3zvgxreae.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3hrxxuqry.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3supvtvlu.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3phyjwpdp.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3ugsoveog.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3sbyuyzys.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3gdanpynw.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3upkdohmt.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3jxbyqetg.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3vlyrfnac.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lxtikpmc.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ogeeejxc.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3mezulvbv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3niuwqkks.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3hmmkrvjd.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3dhdlcnmb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3ewpwcngf.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3qligemsl.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3sfmbtojp.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3fbxtqmkr.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3uaajmmdm.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3eglditop.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3uckhghkg.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3gxkgyyau.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3kibvvfwo.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3sqcdxttp.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3iomwgqwj.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3spqbahab.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3hlnmumrd.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3pqrrvean.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3gxpazvid.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3pspihkoc.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jgecqdtb.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3nnnixwus.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3ivzvtarv.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3uioimyxo.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3gydfbbpa.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3txcctekn.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3edkiomzi.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3slsayxqo.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3nwruuhog.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3mohncnki.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3bwbxmggi.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3qezlsxzg.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3sdplkfzq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kqxggwcr.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3tilubfia.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3masbkfux.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3tqqwxnsb.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3hbgubmss.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3eernfpuk.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ejzagsqs.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3tuqmyecx.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3yersxghe.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3nthnzhdo.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3wjnsvosb.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3peapaaln.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3owsjyvtm.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3jdhydotv.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3yrfmtejk.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3yixynljw.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vtobogkn.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xytuteir.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3zrywmajk.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3svxreemc.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3jdhyesrq.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3frdmpxwb.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3zbzdcale.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3trdxyipf.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3mhichzgb.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3hxuyaxdg.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3yqzshvoa.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3xfobioax.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3tvkmeila.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3tdytqenf.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3pkbcqseq.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3yzzkzrej.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3citbvrwb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3bbrkkakf.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3doidntpr.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3sfeqztnf.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3yytavgvt.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3mugadymm.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ejkpfbnu.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3sywubyvt.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3tqjmbvsp.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3jwpigwjd.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3vxrkovex.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3vcssbicu.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3gdvnzasp.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3siemrufw.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3zljegjsr.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3iplrxkvc.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3ecguoibz.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bpcgwcxr.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3yjitmehn.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qzoxpuhe.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xpjzsfjf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mnkmakny.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3awhjdmox.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3uvokfiml.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3bcuggvff.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3zschdlfe.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3iymyeqbe.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ijzzxgll.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3iwnxefom.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3mfsnnyfo.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3fjqfvocw.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3orcyqbdq.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3clwztkvw.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3vprlihay.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3pmlluibn.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3atebhfmo.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3iybdsewd.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3xamgydyv.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3hhbsauca.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ddmyvrnx.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3dfuzljvc.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3japsqhli.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ngqpvikv.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3idtipaih.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3orujwtew.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ftnrvlhq.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3sitccboc.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3dbnvuxgb.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3vjlxbtxa.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3vjkggjyq.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3eeqrmotc.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3gpurwhkv.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3hodkcutz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3oppruptv.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3iunycmwd.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ltimxoey.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3gtzudgkg.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ildxpvrk.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3tijwykqg.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ojlbxmay.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3ynmcoilh.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3ikyxkpqx.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3pnutlotg.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3cfwsqwld.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3swrncqef.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ydqpvfae.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3krxneknw.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3vxsxeuvn.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3kwmopwlo.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3ytnlwbpf.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3bnhumrfj.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3zzygnoea.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3zkgwwtnq.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3cjqsqkoi.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3bqnndnkr.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3vbbleptl.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3kntldjyc.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ljznxerd.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3sskogbzp.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fotimhlt.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3uzpafmcx.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3lghyxmxx.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3bwzwwlkw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3atpvtybt.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3gsatbmsp.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kefyptfe.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3rbufkwwl.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3zykltgko.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3uzilzdra.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3wgnjxjra.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3zshkolja.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3jhhsqpon.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uhikafaa.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3hbjqnwdb.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3suuqtznk.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3izfpcqpp.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3etybkxfw.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3biuohoug.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wyeeapak.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3hotsolgx.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3thxmosza.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3unrdxznk.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3dptkrfim.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3ctbkerwe.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xzqsjilz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ltlcmfpb.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3pryifnqt.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3ypqizvlq.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3wqmavsjk.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3fbcogewa.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3weqrxxyd.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3muacbjtu.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3oxjaxnld.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3wtbsbefu.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3lnxtblvw.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3luqfnspc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3nrfoknev.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3yrltdojs.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ioelabgv.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hsssriph.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3vifngnwx.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3lmbpnkdf.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3lfhpcxns.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3ewfxkuna.html


<!-- 参考信息 -->