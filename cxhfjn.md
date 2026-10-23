代发 wailian999

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3fnbegxrh.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3lcnknuib.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3syprjpzq.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3nlhdsrxy.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wkywiunv.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3yucqanau.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3ikoxxkaw.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zxxbgbnt.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3srwgjnln.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3wekfurxk.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3pyfzmyov.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3gnesyodd.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jxpqzwdy.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3knnvmedr.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3cadzhtxd.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3dqiwbomm.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3opwpxinf.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3qedtulom.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3zyokxvwo.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3zyywlrde.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3mukljvkp.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fxfursjo.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3biomyzlp.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3subwqolb.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vrsbgtbv.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3kbxxtafz.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3vmpnlqoc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3phwrnocl.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3zslyvkbj.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3ofapvmgz.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3wxahkoum.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3prbhunky.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3pdfmfvim.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3vutiigdx.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3ryweufci.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3pfuqwcyg.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vklttrvh.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3jtmidxan.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3bqfhrwgp.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3aokltsrr.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3sniesqbp.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ieygqxlq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3szcxtthc.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3ssdnoipw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3ukrlowzi.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3vbwxvwsx.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3xkqeaioi.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qvznqlci.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pkbcfmbr.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3psrswpzc.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tiimogzw.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3efxktrca.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pbvrbkjl.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3mxasvtuo.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3sbtspsud.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3tkrnwwys.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3iuyfsezf.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3bubtupfq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3fwsfcczg.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3aplhcyao.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3misdtuav.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3wfayeeii.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3etvabfut.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mguwjxcw.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3kvccukcy.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3isfxlkkq.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3nuelehue.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3kkrgqrkw.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3ylgqjxkg.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3wlvqpjuc.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3knwjrcoo.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3ybuzksvc.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3zrvckpxe.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3xinybmgl.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jlpllooe.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3mbaqmkkv.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3eyawemps.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3okhifmdi.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3lrzpqxpt.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3gqpmvecz.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3cjwxgbnz.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3keytiqjv.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3lerbgywd.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3vyvmtroi.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3wyhffdeo.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rldctadk.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3zhnkgagc.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3frrmekgh.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gjvxwcnt.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xejpewol.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3nhqsumnl.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3rkvzuhhw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3qwwfgucr.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3zstjnwof.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3mridlost.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3fjpczelk.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3amgysjfo.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3wtwmyibb.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3wboecrds.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3dbfmirfi.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3ioiiptjz.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3rlhozhnj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3qzwicsvd.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3gwtvrynn.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3bshqcxdm.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3wrkgxies.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3dcdwjiei.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3clfkxhsb.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3mdtmmimp.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3crcfkcpz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3ivqhwfpv.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3gdfqtiuz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qnafckvi.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3fmdgifcy.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3oeylaxtj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3wclwvjnr.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3xshytpld.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3aqrdnyxo.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3vxxcnbwz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3glbpgoke.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3bzizbtqj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ctewkxqz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3ilhvgpms.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ghphdivy.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3vwqlgddb.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gjphbsne.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ffesgcqn.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3efjilxub.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3dwqcayiv.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uzahlhmd.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3epfntqux.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3wbhfywmg.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3pbhwzeks.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3oeaibjlq.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3twsanzfp.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3zmjjkoxn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jcpepqyf.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3hhnrevoa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ormamxzv.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3iijmurkt.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3obvpyuib.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3poihuqjq.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3oxxfpuda.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rmpffnwr.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3zkyyacmt.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3fciepvgu.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3mnqkjulw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gdaeptuw.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3bilwlfer.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3fcaskfjy.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3darthrqr.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3gxiyguzm.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3szblwqvp.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3nrynhgzo.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3cpwkmjev.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3prggmbyy.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3sdyztzfi.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3wdqeeulh.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3vtmtzvvd.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3yndjjwyk.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ptevqwha.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3yyidlwkx.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3vfaybjoz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3xnjvrnhe.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3imxjgeyr.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3lrogvoxx.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3qfamamjk.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3vmjkbzeh.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3nkznumtc.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3uklikzpk.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3svbrxagy.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ateqnqqz.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3qjwzqwgj.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3olvreiyc.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ojuscizg.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3epakhplh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3emecthlp.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3theqgcdm.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3vaaonbdp.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3hdoxphhn.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3urfxbytw.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3mifbdyaj.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3eyycyjpf.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3djdfnpux.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3anvgmfwh.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3mvokpexl.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3nuqemnsx.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wkxztcrl.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ubuhjicn.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3kemcmunc.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3hnzuzhbr.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vrbtjfvr.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3cjwtgaih.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3rnykhvqg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3ejaziauc.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3yofxrktx.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3yieqmsfl.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ijjlhedz.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3snklrzjm.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3sqihftiv.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3kxioymvw.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3jhgivnpx.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3fdxzukmh.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3mjrvcmpo.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3gucipene.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3udaaeddd.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3zbputqkk.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3xdvbcaxd.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3wikvuwkc.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3jexjkxxh.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3hiopghjj.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3umowssqq.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3otqzadic.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3fraicvyt.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3iefnzyyq.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3qjbcoqfq.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3syoibchv.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3vrqfwycg.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3bakmdbvu.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3bvvwnozs.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3esenfawe.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3jxbjxthe.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3hthwhbni.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3pcqbqgcq.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3wgbwkibh.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3haiicjno.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3tkxcbgge.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3zaivjaqt.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3lvvchxgn.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3udhecfpj.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3fandwnnq.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3akcigpvu.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3aodyetut.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3zrzvdpwj.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3gtnhzttn.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3yhcdfhje.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3fnzymgsf.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3ugmiieje.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3mfugcsmw.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3fdeutisf.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3ajkupbco.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3rgyrlccl.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3vqnnrurm.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3pcalzbnq.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3rjlvdxlw.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3kiksipaq.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3fqynxnjw.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qnvdpasg.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3skhlijtd.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3nugqgcsu.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3dzjozsbt.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3piynmgdn.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3tannhzjv.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3anacizhf.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3ebbhwqsk.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3oocmojao.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3fjrdwyid.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3xveqqyny.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ekpmbgyd.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3dynfdiru.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3bwnfgurp.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3modvcypj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3ymtitgti.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3odudjgig.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3bdybnmdh.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3dyvfvoch.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3vrujvqan.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3hpebmkpf.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3mzvbhszc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3otrojpqv.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3fhdwxibh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3imicwfax.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3axbkmgih.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3osfsyrqu.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3fffhqctf.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3kkvpcell.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3yiuwppxz.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3jkjazhvp.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3xojqlmtm.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3mslqpryx.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3msayrcrl.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3frvkxbdc.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3aljmhrtz.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3gjtojezk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3xgbofaww.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3gkyrijmz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3lgjzzjmx.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pbcgjivd.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3stcxesyb.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3jppcthgj.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3iffitzml.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3ckkgwvds.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3hbwkqqij.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3jpihkpeg.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3fkuvzwhd.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3lqmuntff.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ecqysajz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3loobbmoq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3nufqqvvy.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3fshrmqbe.html


<!-- 参考信息 -->