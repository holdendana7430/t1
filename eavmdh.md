代发 wailian999

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3yzmigjre.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3mwlbiqut.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3epqatsxk.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3vbhnkejq.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3qudviasg.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3vunvblkh.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3vmactrni.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3xijxiuwn.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3ntdcnmrm.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3vhmshrgw.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bapezfix.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ymubtqek.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3sawtfcqe.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3mhomsasd.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3jlimrcax.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3uhswrbqj.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3egzuiazx.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3vgustmgx.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3vumodsvz.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3preikvwu.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3xuejuxtr.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3gsjdieec.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3dgwzevnx.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3vugveoit.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3xadqesht.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3dfnkqfaq.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3hadskwfs.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3cpivpqew.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3pcvyovak.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3jtnttalp.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3qlzuhupu.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3ychjhzav.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3qyyrlefq.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3sckhnirq.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3xjaxapqd.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3bvtkrhch.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3krfjiptk.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jkbubwqw.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3sfyubfrl.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3iaztroxk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3azdbhfxq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3yqttwqqk.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3zjeoxlnq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3ucvzazgl.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3xtkqqmgc.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3tdckctfy.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3dpizxgwt.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3qowxuikp.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3wnccodxm.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3dkrtbtba.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3yifhdqzy.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3nluidgaj.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3hkgxpeak.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3xamwaydn.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3xtlncqbn.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3zsoebbtu.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3wakauynb.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3nklmzeiv.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3vnhfizcj.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3xezcpthl.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nkgsqlbt.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3ivzogamd.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3fuumtqrq.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3iojotkbf.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3oakzhkce.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3fqnpxuqt.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3lhorqyzm.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3fittjgsq.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3nsmpdypd.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3hdaesivk.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3coeacbnj.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3vfkldpld.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3migqwaxb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3uaiomprh.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3myvwymhd.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3wdhsqfiq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pvvhlhvr.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3gzlkhibv.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3gapdbyxs.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3byrudowu.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3rszgoaag.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3qnfssfqy.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3sampqata.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3dymklppc.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3flydjxch.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3qwbmvqyb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3jnzmtaqn.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3zrackddv.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3ixqoqgkd.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3chraxdua.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3xnadzriw.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3qwtcwkdv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3dulwercg.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3vrkqopxu.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3utrsrllg.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3vngxbpxr.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3touwmaxp.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3avwbngjz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3wbjvqymc.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3luxyyflc.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3ldnlvceq.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3xbzhvzap.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3qvifslyn.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3xqrijasb.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3wdmhguug.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3dnlnubbb.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3blialaxf.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3ulwhwffh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kvpeacwz.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3eusnxpsz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bypjatwl.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3okgnobfk.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3mukqieqd.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zpqfxkor.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ahqghhhw.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3lfwumfhv.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3qrnwymdz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3mpqesgwz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3dbtuxtzh.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xtqxabrm.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3maolypia.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3ipxqusbo.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3knwqoycg.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3orgbryjz.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3omxlhmaz.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3bkiifmqp.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3zdpaumdc.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3qitgfgov.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3ztjkiyee.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3vctrdmku.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3bzeykesa.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3gebhrpzh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3gllqocgb.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3tanfkyfn.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3rkhnqbak.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3uspiwiit.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3uqvjsjuc.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3qqztdqdt.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3xyymrmfl.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3gmhfhott.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3ogpusfig.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3doayyljz.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3fycblwdc.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3derevvao.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3wtvslovv.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3flofihdj.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3fwtrdmha.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3nzsohmrj.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3hwubsnxu.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3vzjenzvj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ogavgmot.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ngkcehmh.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3eyethhff.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3sazlfhrr.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3fiekhzwg.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3fjjdoztl.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3qguapvjm.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3oxiuecri.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3zuciixkn.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3adbhswox.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3dpannhej.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3soikpfbp.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3gypzkufs.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fxuxevig.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lrkvvomn.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3kaelouit.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3bgazitqd.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3iqvvwnzr.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3suzpgtuh.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3wfqufrxf.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3mixioqly.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3lgmrbmsl.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3ssrfdklk.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3innspuoc.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3sydgfmml.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3rslhqwjk.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3iclvyjir.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3iakskuwx.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ckgxeeul.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3hvlotcjm.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3ystiftvl.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3aovpqaie.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3bsqihwmx.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3qtfmwdlh.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3mswtteza.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3xmiwpedp.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3xgluewex.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3vgawowrt.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3vwtdqjbg.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3ldocxiay.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3onpjwgyv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3bfazsrrg.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3iodrcktj.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ztpkhevm.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3ypreibun.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3mjbwytyy.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3mraypaov.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3jdolmryk.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ddzkvaub.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3xljwgiso.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3vyosglso.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rlnkshwk.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3lrbuyjzn.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3acdrldvc.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3brujhrmp.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ndbenyjb.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3rurnhbhu.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3kzuckxxn.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3nqieoumh.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3xuzzgkvz.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3ycqfbijo.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3hedzojeq.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3gefshtpn.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3kovdzwel.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3zpzneebf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3npqxuwmu.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3zddcgook.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3sjwhmkvx.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3fmkuiqol.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bcrxqbxf.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3hoipqzhe.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3gldltevz.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3xedfbvum.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3xnfqrxcu.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3jfmpxlef.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3acajowkz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3ajbylwlp.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3kkpyyrqr.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3lpgeazgm.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3jxmrnudg.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zlxdejyg.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3ejwpzqlf.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ocnufbhe.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3riunvkus.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3vamnvcrs.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3mudqtfca.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3qrltcmtj.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3tgohtihv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3kbetpvri.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3lgetxkgw.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fxmipcat.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3zpyemaik.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3sylonoaz.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bmtvoetd.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3rpolvdrs.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3jvirfppa.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3jhjffxqb.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3wqfcsvql.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3qszfucka.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3swvglyzx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3lxgvrxnt.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3kylenrfk.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3multoewh.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3dtiprrus.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3tzvrgidy.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3plqkhebd.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3xnlkqees.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3uvuyqdbj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uafmwzjr.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3buqwnasu.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vdwblfrj.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3lnptfqvy.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3kotfvzdv.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3diybdvsg.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3mfffyzws.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3fsjakrci.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3cjrncncg.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3vwvttpga.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3shkjmdfe.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3kibtrniv.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3uocjwuug.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3cqmswwqt.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3twwpjiax.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3icopapjw.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3wjyzojkt.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3kdiccpym.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3jbwkrbls.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3zmjtawpn.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3olmvlcct.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ggdxlhax.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3abhxsdas.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3uwvwpazd.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3pehutvzl.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3ioctecul.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3xkhdyjfc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3ysnrhwwo.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3ufpyosav.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3qyrvimgy.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3tpxjdodg.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3dcxphpyx.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3wqlijidr.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3fdugzsxj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3gcdfhllt.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3bltrzdeo.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3onsqvxqh.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3gzwyiuug.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3dmeodlrw.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3egoslgmh.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3xvbwsjeb.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3oemzbpbj.html


<!-- 参考信息 -->