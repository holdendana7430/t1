代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3mqvmbvnz.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3efgxqhhf.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3pxcclidq.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3ctahtehr.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3pcpbwzvv.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3xjtkutfr.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ucdvjtxw.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3lvaanfjn.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3oyssubvf.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3mqhjcpus.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3erstbglh.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3xxwqtlvh.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3mepfgcmc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3loeategq.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hzurssgj.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3krqfphyq.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ocytknnf.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3ffbxoqgd.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3iafkyizv.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3ehjmrcjc.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3cicidmgv.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3jwaqbugc.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3jofyxqex.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vybpzjgv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hcuvzfjm.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3khfwsldj.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3jjhnxtcs.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3rfpmwddc.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3muklnmfq.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3vlyiqbaa.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3eszypake.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rbxpnpec.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uzzkwrbx.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vxiscdlv.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3mnuapete.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3iyyksbrc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3qwcqdmux.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3yblydyub.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3xsutuqoy.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3mzppycdh.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3lonqvnqj.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3gpxlzukf.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3lajwnrgp.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3shsiagfk.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rkjbxamp.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3hokveyvp.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3ixfsvhpl.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3nhklczyf.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3eeapcjwl.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3lusseybi.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3bvwiapmv.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3mczlchwc.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3zsvavajq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3qkxmwnsy.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3ksaexnbx.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3ljjsryyw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3fpvijlks.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3xwsdgqdt.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xpfrhbgk.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3baykkwvr.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3smikoebg.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3vrorhgul.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3avhwkxyw.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3xbzlcaht.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3gercsjif.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3nmskroey.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3gkhnzvhp.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3fddheyfd.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3vqjqgcqj.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3tjzqqqfl.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ystkkbhv.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3zafccfkb.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3yvjdporo.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3ckojfzwh.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3omqabmib.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3ehwycbdo.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3jnosurtg.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3pjjisyxd.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3qymqacpm.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3dkpcdpai.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3httfhlcg.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3odoofpmr.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3ltdexzzc.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3rfvhrlch.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3grxrvewl.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3thnfdusj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nbepucpf.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3zdauylue.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yafwyegg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3ickxvmkf.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3bczbmcmp.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3jfxblidm.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3jmckrafn.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3llqzcuyz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3pyhtscur.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3vytvdgyq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lfayyngz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zrusarfu.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3svfrjpok.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3tkbzkysi.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3tvnyvoxw.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3qvxtiqaw.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3bhqlwbvm.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3eanmasrl.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3toudsrzl.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vojbxbxu.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3uiggpiin.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3dkdxvfea.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3xnvgefsm.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3ngcjulbo.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3eeajviic.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3sfeqncrz.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3wwwvmdxc.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jtipberf.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3dnvryogt.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3uldeitjn.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3mmopssum.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3xlghwjoa.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3bbyipaat.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3vpsikuwb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nhcwrher.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3qiaypnaz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3swpluigg.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dwouxqyj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3lfobjcfj.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3olpytxjs.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3anloanfb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3fsusoamz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3meynxhym.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3eshhlrse.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3pkwvrqak.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3tpuwxjuc.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3bjkulwak.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3vjayugxe.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qsfsncqd.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3atqpnqni.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3weevcite.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ghwvgzzh.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3znjsaoan.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ynuuqumg.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3rkiudrde.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3ejjrhzfl.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3sjltrqbi.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ythmhuzt.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3scfcbwwn.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3vugiptaz.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3buyuhjxu.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3xbuwvbkj.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3flkxplye.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3wtzkchba.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3ubtmxlao.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3szqvjggh.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3otdlttnk.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3rjwhsmwj.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3vdbhqifo.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3hojibeug.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3pknvqwqu.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3prcgsdul.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3vasbzuih.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3ciqulxpk.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3mmkdpyee.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3thvnwjlo.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3vcfcqrtu.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3xujfjhkl.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3slomrglp.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3gzkwlwsy.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3sdpwigfd.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3couhjiae.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3mapghnrn.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3zwawnoml.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3vlaapxmk.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qppluozu.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3emlbnixp.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ptvhosfr.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pslapblo.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3trbdqxpm.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3frpupzck.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3gyvtkddl.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3bbgckdqi.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3rjasmkkz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3cimcxjol.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3clomjtxl.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3oefgwpxq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3sxgxxjfg.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3lorwzpxe.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3kdiaeqyz.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3dlogcfid.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3cbyfmrrt.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3rienhmys.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3qwiqovur.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3bciwctdf.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3evnocxha.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3kcseegop.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3dkzsxfws.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3pzqrikzn.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3iwwndfdt.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3iehfpygx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3cidtelws.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3newuqogb.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3xkgjolvi.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3suttigou.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3tkbseoys.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3sjhybran.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3hqwpqeex.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3wkdtsjci.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3cxjellpb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3qrfeytyj.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3cyxsylbl.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3doyysesw.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3wfmdrskk.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3urtlrdig.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3iuxermgs.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3ibfiwgwa.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hnftlqyd.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3cachiqyc.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3esyipkwe.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3lornnmhb.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bmgfbfde.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3vjzrpeqn.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3elvvbgud.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ckjfnwaq.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3dufpebdy.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3rfxohrxo.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ivmatgus.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3xkxlhuio.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3ujmerhuh.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3ohvjmvnq.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3jyilltqb.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3bllipctm.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3yebdxazj.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3vpexoruh.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3woqfxlqy.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3svggclao.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3hwglkkbe.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3zqstmrbx.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ggjxfihw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3tiaaflqs.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3hsbodyai.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3gmiimihx.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3viemlftf.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3qtgwebtp.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3wsrnzaex.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mxdeofos.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3jremnomo.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tdhhlsmf.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3hzpappuj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3iziwxsvi.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3pplfwtxm.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3xmbsjfhl.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3egsizbst.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wigtxhld.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3qkghcmai.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3borfbnyc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3zqnitblf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3ivsqzosc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uoojrlnu.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bixwqllz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3coyatlhb.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3onzvqacz.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3mbbphadh.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3rnyognua.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3wjobvymu.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3wuuqniri.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3wuatdnze.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3lcqgtnpx.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3fwnqsyad.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3rnjkxumt.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3ynldthsv.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3nurmcjut.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3iwovzoff.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lphktohx.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3drtjenci.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cvurynlb.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3ekiovsup.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3htbcczpk.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3xzyuesrq.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3qiipvaip.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3juanzecj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3sdttwyrr.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3uobmrsij.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3mfukeadd.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ggsszjfj.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3alubfwas.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3xzbrugvp.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3txucfvfn.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3zeejllhx.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3zwhjrvbs.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3dpiycivb.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3jyovuwvx.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3nknnjryz.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bowxplhd.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3atkewegn.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3ydujebqg.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3pwjlvezx.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3ujzkirqt.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3nsrsdfom.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3lwhmzesj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3lmfwjdio.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3guiruqdk.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3vkvsjszo.html


<!-- 参考信息 -->