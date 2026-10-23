代发 wailian999

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3criaydff.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3diwevlko.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3hhcigmoo.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3crywsmnp.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xusljzou.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zcmibyfl.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3brsoooxk.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jyspifvm.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3akqlaghz.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3grpheydp.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3hipioown.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3dstlkiio.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3whakzaiw.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nuzudbfd.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fyzymiur.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3okyorinh.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3ckywrmsv.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3mplxisjd.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3wsohggyl.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3uhaupvvt.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3urmkjaiv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3cijjsbxz.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hsezfdtf.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3vyyogaar.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3wpegknzu.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3dgtktcsb.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3zmvxvpgg.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3ucykzkca.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3tpmebfyw.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3irhkiwsi.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3idvcmzch.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3eygjakul.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gmddqqzc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3mbtgnwcr.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3yhslsfwi.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3npbwupui.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3edppjjeo.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3qtltyrkc.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3afspimsb.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3ytjnnopm.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lshhvtaj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nqupzido.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3sjdiruox.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3fjhuuhss.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3itwhqqdn.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3reirywzz.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3wvxlscqg.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3jpdekqbm.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3xndpuizd.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3eeokvrqk.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3azrxrtkg.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3cywxkjwn.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kmjgrhka.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3qamornrl.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3wnfwnziz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ppaitdzj.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3bolinimi.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3ookylyfu.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3dsxibpvx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3lvnwehfq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3zjtzuawk.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3kufgejbt.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3tjxuivxf.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3yeeaytak.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3wnfromqy.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3kggetust.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fzfdllnu.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3eikvkdui.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3syochmfv.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3pdyjwlhv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3lxczgdia.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3uoffvmrk.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3ppstynyw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3lbibtajh.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3zcnedvys.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3dfimqexc.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3dyakonxh.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3jkuzaqig.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3myjeobet.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3xjzpcdyo.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cizzjkbt.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3zllavzlx.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3hjbxlzfq.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3zwtmjgiq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3expwkxxd.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3detectvt.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ojshsgcu.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3lxvaczvz.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3ixgbqtus.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3rcbspcdl.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3hmjymlcb.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3kgeabrbu.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3kgqvqyaj.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tvuifoga.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3qqfdbabt.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3btkuwoft.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3lulzlebg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3abzrzwid.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3lpaybxnr.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3wczldxnd.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3atvnnpaz.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3asdznycm.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3mwaslcwp.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3edipwbmw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3sfkiijeo.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3xxxsywci.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3plqlyies.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3ujtlcpyz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3vdpgcnno.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3lomggrmt.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3fwbvqfwq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3abwmykvw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3ziwhnuju.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3fxwplcyn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3vqkxumlj.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pipiebfr.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3sqkodesz.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3jhzmppky.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yjmivcxj.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hrvbcjgm.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3iumjykrg.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3uibphrqe.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3akjzxliu.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3nkjahcfi.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3djccslfa.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3iawkghlo.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3evbazqxv.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3bddahhlz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lzqaohzn.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3exubuikv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kelbvovm.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ponhwdjn.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3sbtnuboa.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3xpkqpmze.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3srkwfkjt.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ybiktvbg.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3kgfizrhx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3itliincl.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3wkldvexk.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hdykruvt.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cqcynekb.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ewqxdfue.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3sqorfcyp.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ufhxevgl.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3stbsrssv.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3wjhptqis.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3drfjgess.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3tselpwfx.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3bbbgundz.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3iqgtbfoh.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3iogdzqrq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3pgmatoeh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ofovovbf.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ditwegle.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ubbcmoef.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3crjgxdxt.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3ycmdemfq.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3ccqxfbkz.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3ufvsssrq.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3udfmyiwl.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3ytnxdhtb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3quwwogkp.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3skdetwvl.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3qfqmbvry.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3riklzpwr.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3zgzcjmcy.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3koousane.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3koqqkqzi.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3nwciqisn.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3ggqglvpb.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3gffztaja.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3tlwctfho.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3nzlpfzqi.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3trdlsags.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3abwskqcv.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3wjqavpne.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3rrzkqtln.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ulfhfaju.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3jlfbvpzo.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wjrutuao.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3knxtaggj.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qrjsxlpf.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ltswmzas.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vobwajvi.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3fstlgbii.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3ajjyotwg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3xzoghuea.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3itsokscb.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3oqgmbdsq.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3kohwbhfn.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3uqzmfqrf.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yhbfucal.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3quhvaymm.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3jlewtuzw.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3csseufnr.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3papajqfo.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3reihoutb.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3bsgxunra.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3pnhrqyto.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3wagxjkjf.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3onyyvdzm.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ubteoqrr.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3nxfuilip.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3ndmbawxj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3xcehypsi.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vkbqwxlw.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ilboaboy.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3rglaunvf.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3qkfcnetp.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3hdzxjeys.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3shzpxsnc.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3hpfwijtd.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3bivyunok.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3fobirich.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3sbbupsea.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3faqijyix.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3kwbnfsxt.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3dyzsslmr.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3jjqsljep.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3wspsuksh.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3xbimacwl.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jdmbyssr.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ehlliehj.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rwmyuecv.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3heihzkbf.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vvsbktou.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3lcrvzgfx.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3rqbuzwwv.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3wympfhhf.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3yivxapfs.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3sxowefnt.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3melrjghv.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3lxkpahmz.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3uwuoyamw.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3dlrwcjvt.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3fphdshpb.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3yensppze.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3mcdrsefr.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3hwxufqqd.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rzeogzgv.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3iwoiumuy.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3ztdkjtst.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3nyxopple.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3fyvibcjt.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3hfvydbuo.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qlzdvtel.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3tujaaxtb.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3fzxtpbjf.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3yozxwtau.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3cenjogju.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3xwnfmgvr.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3pjnhdvty.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3qiuvsvcy.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3vzhneahe.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3pvwaymey.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3uyxngpeu.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3bpjarysg.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3hagxrifv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dkxyflpu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3gmrhvmvp.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3weodnvsb.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3azjropun.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3kixlimbt.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3zozmrkna.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3aebshaxw.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3betnoqci.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3rvujxpmo.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3mnwhtgkz.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3yerztacb.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3ylvupwma.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3qphwyfge.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3xihjguwa.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3judzpcpy.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3cwrexohv.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3geeerjiq.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3wkarrrtj.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3qvxhatkl.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3eavxqtpu.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3cfpmaugj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jbuvevht.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3ovjruurr.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3rhxwlkjg.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3nngvyalv.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3lqgpzzmn.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3zsfdmuau.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3ouhijkyl.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3mzlxmrtg.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3qtsldwjf.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3kytiqwdp.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3zuxfoodt.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3fcudegym.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3hokcdqgh.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3ulucdyww.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3mupyyomc.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3retrcdbh.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3jtjfkjat.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3xpdoomrh.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3xnvapsab.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3pyblrvbf.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3gxjiiigb.html


<!-- 参考信息 -->