代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2yelfivyg.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ejhnnalm.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2owoeochh.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2qbwaeubn.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qbeguwpe.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2tlhoafpd.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2xikqmbhn.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2bwvebojj.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2yityvhes.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2pozepwyx.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2lfspnoqi.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nsblcfuy.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2qkeezvpl.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2tbfflood.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ssizuvez.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2ceojdqek.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2vtlmmyzc.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gwselojr.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xfshaajr.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2utifwcbb.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2nivaswma.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2huoeausr.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2lawhkslz.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2uxvuwzea.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2ydbxowuz.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2xzvjhlta.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2elnaczxj.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2rrdppnow.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ackihlra.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2cncqklzw.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2kiybmjoi.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2tlmqxnjv.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2behgkvvn.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2wxwqvyih.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2sgputfrn.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2imxfcifr.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ulmcopur.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2bzwqrvpg.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2lnwtwzju.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2tirztmnq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2rzvoynkb.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2jkrjudzv.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2rykjmrgh.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2bifpssgg.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2qjxrxwoo.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xbbessmy.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xatgiagq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2lqbczaix.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ynfrqfoa.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2rngvfcjv.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2tjwjlctc.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2hmcamnvr.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2weshhwxt.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2cvdvfruv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2nuhezftl.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2uesnrgug.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2tukvayma.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2ddhdqpgo.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2tvixxkog.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ignuogyr.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2zopxusnz.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2pqjopxnx.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2lzosrklh.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2hjlhxrpn.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2vtdxwaid.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2snvxdics.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2wfduatmi.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2vaffwbcw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2ehsxgdbd.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2pdrbfefw.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wrzualyx.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jshfpasb.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2jgfwxwgu.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2zrjluinz.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2zcmptzlb.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2hhpuurdd.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2uhrpigyo.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2fjiclthk.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2tsgnhzfj.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2nzjlekkg.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2vlmeeryd.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2prpfbjmc.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ezavsswx.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ciqmeoqv.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2atkdwvag.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ubbhhaqt.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tmfirhyh.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2etdfcvhc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2bdoodzeh.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2qzrlgtdr.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kzzvcyrr.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2nbzrwsbs.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2hyjrixop.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2wavjhvno.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2pwarflxa.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2yvoktikg.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2nsdzzjbk.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nzlkkytp.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2lrmlwhqs.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2kjuowagt.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jkwxyvhg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2heuytpoj.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2crysvwfb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2nrgvuyin.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2khvnljnn.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2mwbskeqd.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2zdamproj.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2sbrtbmvi.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2bjaogvhr.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2gdndmimr.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2lpipzwmw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2trozjede.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2iwnbkyhq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2olmgowwz.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2bfgaresh.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2yzswsofu.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2pbxwscly.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ahgzvrzp.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2zbcnhqeq.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2aqmodnpt.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2iysgdtrd.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bdidgjoo.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pclampzl.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tlrskjde.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2mdxpcfdr.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2vxjzqyrv.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ondldnsm.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ccsauzpg.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2vcilzmwc.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2sorepvbu.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2xrlisdui.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2iwessvin.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bkukpuyh.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2sbaybaks.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qwwlytse.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2kckcnjem.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2zsioyfgq.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2pgyyckbo.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jvubpddh.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2qijbfdmu.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2uktlsqsa.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2hhnpuqxq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2zudokhoa.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vdwsrllp.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2sbzkwvcg.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2shozfinz.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2myrdtrdg.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qqxommgd.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2defrrjwk.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2otjawygc.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2hzshzvoi.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2gnmxsrkf.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2sohxoctf.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ubpqevjj.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2mheupzdb.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2osjpmofc.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2wsbjnaml.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2oszrjnjx.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ytsxrzxh.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2qyhaemhr.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2vkuemrqe.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2xkmlajgi.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2obpsduis.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2limnkjjy.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2nfpkxdbm.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2mtppfebp.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2dbslfthw.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2rdligqtn.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2xfnromkw.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2etxgfmue.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2hqhyguvk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2lngfjova.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2toaikrfn.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2gbcmpefv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ynijdvkt.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2qwgapzup.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2lrcxasbu.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2uluhzelu.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2itxjrcbw.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2foltjghn.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2pouwiyvg.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ibwsnnry.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2bkpiucev.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2uffjafzo.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2wpxklkdn.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2nrtjcccl.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qaxpjjmi.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wmvbkvgf.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qnwixlen.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2duwyykfp.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2jkzpwwfs.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ejwrxunr.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2ujppvfyn.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2fqeoierb.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2iexgirzv.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yrlgzlpc.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2hdmtkeoz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2qulvvphz.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2gxfdowqy.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2fhtrwahl.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2fmvrimcg.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2lfxpdeju.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2wpcvybku.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2lpfwowxe.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2nxbnuilc.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2mznnasvz.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2bnbeszee.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2yiwcuxel.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2vrjozmnx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2fsutnhlu.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2acfmcjlt.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2fggjzuxi.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2zldwlnje.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2mqiyicpn.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2edxsuhot.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2napvmyhc.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2ldlfdrje.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2fjhkbebj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2pnwnoflk.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2czmtgdrs.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2eemkvywn.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2zmavlzet.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2diysfjbc.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2eofqwysl.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2yzxtskpj.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2dxfssncl.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2xeicjnlr.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2otxjhbdw.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2azofngdm.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2psdtlzdy.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2vsdkqpay.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2oqszewod.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2tgpvzolt.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2lbavrkkc.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2irzeteik.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2bsseufok.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2mgxayyvo.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2mawrvylt.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2pbbouxtd.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2yutmoseq.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2mwziojxm.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2pwmvreud.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2udiyabpt.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2biisltiw.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2wqjqvuzi.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2sqcoiexg.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2djsyfrcj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ppzdxwon.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2lieraeqa.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2opbwfrdj.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2hvggsrhy.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2fbyoyydc.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2xvrilubl.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2cvpxhprp.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2waigfksm.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2wnecwcxa.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2jvwcydue.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2oqkuchyj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2sflugdip.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2pvwzhrru.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2tedwurwv.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2tejpbdaa.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2odgicxsq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2mqglzpif.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2tugshkij.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2blzhxumz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2frkqvckc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2rkswbffa.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2gmnlzxjb.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mwbrdydu.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2pldjwqki.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2bvynhohr.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2tahmmrqd.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2yoqyzdjb.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2swjqdniy.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2cxfpjnfp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2yjisngqa.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2jjgxmytb.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2czqgpscd.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2yxkmvdne.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2ecdeyplu.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2hbefnbzo.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2wnxsgjsn.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2xegztnax.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bvgjeskl.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2qqiddvmv.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2wlvqjrfm.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2cplyhkbt.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2yvmfvsmh.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2clmrzdhb.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2mozglihd.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2inuntssu.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2wnldkvkw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ofxnweqp.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2rbqrzpgs.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2hiaeplif.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2jpjkykma.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2jefmhwqp.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2feigrdmx.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2uqoiwvgh.html


<!-- 参考信息 -->