代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2vhmtoylo.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2hhrsftks.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kjqdvssl.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2oxciuqyk.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qusjonkd.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2bkcpijma.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2wmskttet.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2fcigvrns.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2hpmgnfus.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2ekrppipy.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nkpwbnbl.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2okjjxfzg.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2qteaxnuq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2npqeqhah.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2ubbxoerg.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2tofvaxwa.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2bfejtyxg.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2olopanah.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2jzbswrzl.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2selvsruk.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2upqfvynh.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ukstooti.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2hicmpyfx.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2xvhudcdd.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2yysfzibq.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2fwonoesl.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2wmrcprun.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2zivomtra.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qkconxid.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hsyjfhqp.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2qzwsyjsz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2qobpmhth.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vxvwadlp.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2bqotaoss.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2ycfetftf.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2xmodgqzb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2bslcavwn.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2ynognjuu.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2calocjfb.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2camllltu.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ipiqkxfg.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2dzvsrssl.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2noxcparp.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ntoxjcuz.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2gzfwctrm.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zrswpouz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2byvtwgno.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2htuziicf.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2otujqsro.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2raybchqb.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2tfkpkvif.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2piktpxmw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2pnjobgfy.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2xnikbfmq.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2qwfpvwxy.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2glthlieq.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2metdafbe.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2emoyntkj.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2vfnfqmsc.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2kkcpaxmx.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2xddqpkme.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2anarabga.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2mclwyjdq.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2dmnlwikf.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2iwvzfntx.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2fuvpmzud.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uwdjpeqk.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2epkjbtax.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ttvjewmq.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2vbjcopvm.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2idwhhegq.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2fymbauau.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2xmdllytt.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2ajpyvedi.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2ivzzvdgw.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2pjuqijav.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2mruulfki.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2xwhbtnmk.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2mxxnljes.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2jxmirpdy.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2yvyepbqz.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2resosoav.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2tgffedhz.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kidqwhyq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mwjzwcem.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2ffurupdd.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2euvkpxen.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2hvskxgcr.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2aqqgxrxo.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2nhrhrrks.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2ejlnwbjf.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2zvdlhhxj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kdisqlss.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2pxywflhv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2kikcwuyc.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2tfntwkwh.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2qkikrcza.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2wkqvucdp.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2qwtqwcfm.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2wvopjjxp.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2doivkjup.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jjtwopuk.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2bsjjtkdx.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2aippfjdh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2anfwkizq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2sxpapjll.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2opukyddy.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2phnndkew.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2kgwupbjw.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2zsvtxdcu.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2wdqasydr.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2vnakvgfb.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2rfshnunx.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2kkcfbyfr.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2imxfvkho.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2plucglbq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2antufjgo.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2jqtjtuat.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wkqfdijg.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ficunrje.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2ubzlfwfa.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2karluvjn.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xxcgurlc.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ivdrawxa.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2oseblopu.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2tgbywopr.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2fbdfufzf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ktveqxjp.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2sokxdccx.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2jujfdkrf.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2zlqbcrkg.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2zdyedefh.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2qlxikndi.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2uiafhqhr.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ziklxdue.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2vjcajllw.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2rydbisns.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2aqneocfz.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2kjfliywf.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2pitcerox.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2wnledfnh.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2iergywsr.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2vikwsmtr.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2ddsdlbfc.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2syvbmvys.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2mviwyuci.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2wttuvjrf.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2oegrbmxx.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2xwmvhaou.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2txczqxcy.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2kvkerqig.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2wsmlvtyt.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2ucbgzzcw.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2dbknyrgg.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2nrhnqtqv.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2ashgjrot.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2fmyfhgxx.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2wooogoor.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2tezbcobr.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2ziyxptdh.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2sbthjhze.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2gajlhpjk.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2jxmagifk.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2bykmpgoy.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2txdjhuyp.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2seybhxbi.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wlsfczdg.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xqfiajbd.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ldgdwzux.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qnwoeojl.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2eoaaguzl.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gnxrsmmb.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2lffsazxm.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2uvoliszu.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2pixjzvwb.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qfixrfve.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2icjdbrwe.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2cveszhce.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2hkxkwzew.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2evmkmlxq.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2lfdogpgg.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2bqomggyw.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2mbdprlnd.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2kmknatxv.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2owkdaozy.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2atcdciem.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2jaqvoozc.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2gtkvrdsl.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2vysplhjl.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2przdijiz.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2wcbutyjm.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2cihrbloo.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2jbsfjlvm.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2cgiwrjvx.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2qmhbnpvo.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2rodvguji.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2qrjrmblp.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2ulleqxsd.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2sgbeyghv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2qdfiilcl.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2votwhqmz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2yexzfgue.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2lgcoszom.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2apxsncqe.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2lpqsicud.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2fjckfbox.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2nrkcqmfw.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2lwsrzmzm.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2hflaligz.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jqwkfghx.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2unuhlfyo.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2abdasqlj.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2rfomrqfv.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nvnrsbcv.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2efwumdyd.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2wpwyugxy.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2zbashnze.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ddwrwwya.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2xlhdfqyh.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2bqsiyxrg.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2thleecwg.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2iftwjabr.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2iuultqjd.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2wehgljkg.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2libvpngq.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2gbbsloed.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2yzlpkxrn.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2zaqsobou.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2cczojraa.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2lflrtyjm.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2zmmqazyy.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ugyptiod.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2pmrmxmfb.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fndcrmet.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2nosdnwfk.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2vvunnxvy.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2dgtwblcz.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2vmeexviz.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jwrhaima.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2gzaicegb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lifswprb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2czitwmmx.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2aqjunimr.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2nmdaqmpp.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2iyiopnuf.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2bzdwlxlb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vhspjbqw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2bccjgiex.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2wvyfmouq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ototrbxz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2yqutzxpt.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pbcxzkac.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2mlimgwew.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2njkrmpah.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2uiuzrxos.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2mujqoaaf.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2ldenaznd.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2tqwikitt.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2mhoiwisk.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2wpawtnli.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2qeuhrxkk.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2vzdkrwtv.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2ftceqxbz.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2uywpixnf.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2krenwziz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2rqufjqau.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2pgznanuu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2fszujlxg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2rnuppikj.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2bphdexeh.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2ultpjivm.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2cdojhemj.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2kkrxjryn.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2enoaqbtl.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2bpimeejb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ojaffjyy.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2dvlcoezu.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2refcogbz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2sysjvjxl.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2vuphudrf.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2wihucmba.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2kxihcjuh.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2suxdgejk.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2fizsxrod.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2yxsavjnc.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2ttizamek.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2efsipmii.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2mmenpyzk.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2ibmwdzpd.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2mhqbnxym.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2dhvrlbgp.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2wqupngig.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2odilcloh.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2isdkquzl.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2agdnbgcb.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lbktectd.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2yuhxbusx.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2aqknwfof.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vbxoielx.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2wfexcodq.html


<!-- 参考信息 -->