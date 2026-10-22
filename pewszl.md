代发 wailian999

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2tcmwwwsu.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2mxrzfgiv.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2lmgbqdop.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2zmdokveo.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2bpawqksx.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2ghsapvbt.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2yxpxyjru.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2dhhnyxhc.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2gvyijrnd.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2aizlsjiv.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2xbiryjpt.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kvtlazvc.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uopknzmy.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2esvcxwjf.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2muxyptda.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2tlkrayab.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2sxvschdf.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2skfoiwkx.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2qwkyvjnr.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ozbgnmcr.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2drwdxqwp.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2xrdedwrd.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2xrcoxamg.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2oouoklpb.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2raoggcbx.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2zezbssxh.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mbvopdgf.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tzbquerv.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2jjfufhqd.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2nleumvys.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2gtswotxg.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2soohdali.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2qwdouwln.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2jxbsoepk.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2tjcvfsdf.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2oimugszv.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2iwicmyyo.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2fxyiwwle.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2uxdtibnn.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2gbqxsgbb.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2tzdvgqyj.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2lvajyfgw.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2agwjrztp.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2qeozpyeb.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vjoebppk.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gceetwht.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2ozuhytle.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2cqcbkscz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2vyuzqodj.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2dozdjjua.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2ffkabltr.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2rqxhpdsj.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zyqcrnct.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2walikzed.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2midptvvx.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2twzfobex.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2aoktwvin.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2btailaro.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2kclaiynv.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2ktgtpxxg.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2alqmgsnc.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2szmeyruy.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2yoecydkx.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2wsjcktkd.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2riahatmh.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2fibcrcps.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2unuzjeuj.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2jvlgqmtn.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2qutezjrl.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vtarztzr.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2kzscuydw.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2ymxabmfk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2bheboixf.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2qaulfrpt.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2rzhoxyxx.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2udlfuiyj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2duqgdgcv.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2vcbuwmiz.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2zmmendkf.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2itqyctpj.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2xzmgotfv.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2jnekwuyi.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2mifzchwv.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2yxjbrxbv.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2ttmojewa.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2tzewgqna.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2xkxbjicd.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2zyiaoqlp.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2rkxkfpay.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2inudrawd.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2sirynjlh.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yheuaimz.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rovnmqxj.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hkyjkmfi.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2psdklkrx.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2iculexdl.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2gjzovlju.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2mfvfbxrp.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2puqtltgp.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2kvvmzyso.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ryobzhbc.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2pyegfoys.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2gwkysxbq.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2kjsonkyg.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2mudvpcbd.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ytwbmmur.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2dpoiqybc.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vrydfxfq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xxddmwhv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2fuudhtkm.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2uuavezlw.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2septxpoo.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2hbebjuks.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2gddkjegv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2ltaersdo.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ydwrbxbz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2cmkejqpb.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nuqokmiu.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2xwtctlmu.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2tzzolzqp.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2tekzgnxm.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2chctryze.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2jnobhlft.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2rtfkekkk.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2uersrmze.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lcfamzvo.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2jmpljzdb.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2qavqrnvo.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2zjztwxcj.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qrgkpqjd.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2hcznfhwk.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gzomufze.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2crzkwcjp.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2yuoeinca.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2vvwrksva.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2gzvexspv.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2sfqykkou.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2jngwxevx.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2mqykbtfz.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2rvlmpthj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2euaxapye.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2iohyygyx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mtavnlbc.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2hdifmxqz.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2yxvlapuu.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2fycprxli.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2qbrlzgqn.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zxmmbkbv.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2odhcwpuq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2ynvomaap.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2fbkcrwhe.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lfhmvucv.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kivhmtnk.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2vqdtymqn.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2xemermus.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2udkavsrt.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ivmzvmny.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2tocznidb.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2krheuhuq.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2rigwsxid.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2vxtrhtiq.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2qfvepzuu.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2lkehhddf.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2hxnupqlu.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2yzhgzjqp.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2kpzdgqjb.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ujjsumxn.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2xgxtrxnh.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2evymahbh.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rfenezrj.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2gerypjzb.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ykmizuwc.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2fpcphpjc.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2antrgjcn.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ojkaqrsb.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2jhtbrgfs.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2xtssbenc.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2aorqyxjb.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2dpmzdlnq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2oburcfiy.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2ogxtmfbl.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2mayktkwh.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2miifcwsy.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2qxzdwtlf.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2hglkreni.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2rpwtsijw.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2hljeoqee.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2yktzqhgc.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2buodtdhh.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xxxwefry.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2htjoilao.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2eehofhow.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2bpwcrnxf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2lnnoaakh.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nczsebfo.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ovbhcvqc.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gtdgfcpe.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2utvmyaec.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2xlubpykt.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rzgsnoxs.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2vbdnpmag.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2rhkwifta.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2zshqmuqv.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ythxzllp.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2lmktukhc.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2lnrcjuhk.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2dsbytqut.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2simmeqjj.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2qsqyjywt.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2bkcmjvsz.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ripoymnn.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2ybiljmnx.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2ongjonxa.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2brdcwchd.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2fuwszlct.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2tlrlqskh.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2fwjrmxcf.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2pagukvem.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2vnmhaxto.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2gttndisk.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2jkmqrkzs.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2encofltr.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2lozusqrh.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2npqvftnq.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2mvnvymxw.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2uwecldne.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2bfkqgaoo.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2zloueokb.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2wueisyub.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2wgmiqqch.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2aaafrhwl.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2edrpfjmg.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2kylesnig.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2bfiqfwsh.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2mkxdpnyi.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qoxgtuie.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2amkdmyaw.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2awsifuse.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2eushrpnd.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2tqesuquv.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2csjutgnw.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2zgwsihhu.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2oenoguba.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2qfrhsnff.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2fyxnkjzq.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2eigzophg.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2haqwlzva.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2vrstjcky.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2rcwffemk.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2udkjxskg.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2vqllvvuh.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2nniybioo.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2piohohnr.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2xotanrtl.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2fmijhxvi.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2mvshcgba.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2bkeijylk.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2eowhtgko.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2ahnocend.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2armmayuf.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2hoslrilt.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2nqnvmbmo.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2zayvbbbd.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2qltltytb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yvzwjmgk.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2oecstzjq.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2jzxjkrvt.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2xffxdvgx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2bncvqwor.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2ndnwllit.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2prsodyxr.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2eajfgnoq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2odaoeoje.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2pxhjycqu.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2mrfqaczk.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pxrtjvcz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2pizrmhmj.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2czlucgnx.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ouopzgsu.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2dbpppyvu.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2rjzuedab.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2agjgmbrx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2dbrkyvdg.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2baxbnopn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2paitfvbj.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2gqncjfng.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2xttuevlb.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2kabypupe.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2pqurkmbd.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2kgwkbcpz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2cdqiprsn.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nnamqcit.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2czbhnfqj.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2jnukbymt.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2svvtbnyr.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2einmesbu.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2gcxjmpjd.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2qqyrpkvn.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2idlodmnx.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2nthqzfqc.html


<!-- 参考信息 -->