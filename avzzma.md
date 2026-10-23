代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3dikwqpas.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jrdsylud.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3iuhozfiq.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gzapoxxt.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3umwtfrub.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3gnkysmaq.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3azdaptcj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3eonktvev.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gkcadgjl.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3toipumld.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3mqwfjxtc.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3iibatjca.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3dqgyoqap.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3bgwthrui.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rteilemn.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3ohuafgmy.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3qbdlddtm.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3lidyjbcm.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ldxcfwsf.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3iyauwere.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3bptxygbg.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3xktlgfaw.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3jjoodwrr.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3qwjoxdsl.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3cshzohcw.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3vaauyzts.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3yujbcxps.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ebfmgitf.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3vvaouwcg.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3zucbmekw.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3blkxlcow.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3xhonfjys.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3unudphdo.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3ohmwqcbn.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3aygeybrj.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ljdnnhha.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3cgneiptl.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3uvcwwtcr.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3vriszury.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3hmfipief.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3bmgcwcam.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3tfjkwacy.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3umxbknci.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3mwizoijx.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3vtmibuxg.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hulzmqjr.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vgqbjxys.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3bkstohwn.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dzugussd.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3xrfivfsy.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3rzklbjzn.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3xsvksbnt.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3nywhixjp.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3viwwrown.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3ankyhmsw.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3tvikdajr.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3yxxsfofu.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3ikmsutve.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3eoyjdqoj.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3binqqovu.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3wjmbexdo.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ymtlsaar.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3qjyiqarn.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3rtkakcaa.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3qeaivbzj.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3xndjmfnb.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3nilqwsdu.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3pmjbdvnn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3grnimglv.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3lucapvyb.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3cxuuibbf.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zccxccxj.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3xxxgaerf.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ltnszuuq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3efirirjf.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3nkuliikz.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3donjdrob.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3jaexdaum.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3asuxpslr.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3aznzjufx.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3jotuxese.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yfbootpy.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fhmqlgyk.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3bgrttfkf.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zouuzszk.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3fgvcjbmq.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3nyfkxenr.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3svvlazhb.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3fkoxmokb.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3unamedvp.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3qnlymjew.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3eliybgpf.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3jeyxmovy.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3nkuszfus.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3gublkkgp.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3bdoluhkf.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3nmicuovp.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ahhdpnlh.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xwcbupmf.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gazubsyn.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jdgvppdg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3foradyye.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3iuwxdlfo.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3bhqblwye.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3mppwuzho.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3wcnjhpta.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3zwdeeopz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3ltnxjrlq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3etrvmltx.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3cumkqqgz.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3qomexoop.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3ybzxdlpn.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3ljndorkm.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3trghwcih.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3papzfbtk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3wvoannwm.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3abpfihud.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rxgxkxrn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3dlfxqbmp.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ubylrchv.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3cbyjexbg.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bsarayaf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ddfftlds.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zbhfyopv.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3iwoonlbe.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3vqowdxji.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3inddwpdk.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3lpdzmbfp.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3civyrlxr.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3wfhwoqrg.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3kykpmzlx.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3itbomwkd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3asphpete.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3gxzuhpgq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hhemggcw.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ynkyphvk.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3iaskamlh.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3oudfbxam.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3arikjsgb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3tzdbgvyd.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3kcozrbli.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3hkmextbs.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3thspimwa.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lfkpswem.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3yhfrygty.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3lqhskyeu.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3frihpttu.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3puwwsnys.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3shwirscw.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ohxupbrj.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3diikfqtv.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3iibntcft.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3etdpzjeb.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3trdmkwdm.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3jofgpueg.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3lyhbzqxr.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3jwnhwhgq.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3lfyluerv.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3beyezvow.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3jcxsfdsd.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3lhwsccdy.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jlxwdhsp.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3wqhwxhjh.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3lgxiyrnb.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3zlayizvb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3cawgkyav.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3yotrwkag.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3mnvprvjs.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3ebrayxiw.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3beviglmk.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3juaudfll.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3dnzvbijw.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3fbhssgyw.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3gaheawzd.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ijvayikc.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3laelibqf.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3txnptche.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3opdmindf.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3vonjeroy.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3bmwvmqgk.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3rpsfpbav.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lpayfgkc.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3dciurztn.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3sezekhoh.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fdzutren.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xeskbvrt.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3fdizdbns.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wjinawik.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vdtcfvhn.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3qoqexdhc.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3pxlnehre.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3atnqkijz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3zsaopwmw.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3hxjmgwgm.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3dxcudfen.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nzmlnduh.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3lvhymqqa.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3bldqvdak.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3hpuetiwf.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3rzrwabnu.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3kwuvqxwa.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3svqocino.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3bsaxyidw.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3irwcsxgl.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3hmxfwkni.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ptpojnox.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3kvhtsavf.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3vfmpjnpz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ipklfnlo.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qyfikysm.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3wmybdacw.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3aryhsiqm.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3nqqvjycb.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3pzlfphqu.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3pgwjiqjg.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3toerebjr.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3dpeehqsc.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3yhalvazx.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3ctvdpflp.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3fnkxgvup.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3mkhawlxx.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3noflyzcw.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3twhtqpvi.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3yozjkmos.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3ncyxvzrp.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rifsufka.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3xslwrvck.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3bslpnabp.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3quymrvol.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kwuaqczh.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3xxziknkk.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3cenrlqme.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3cykorzjc.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3pqhvmdpv.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3xdqfracj.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3zkogzqef.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3eorvlnnk.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3wnrawfzm.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3ktxpfdqh.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3tleuiwrf.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3waipqjwa.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3cqztdini.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3zznsrrqt.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jojrjgrw.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3cftophlq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3xagpvsrc.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3zziwlozw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3olqigdle.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3kiqdkklo.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vkeuiojq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3wadmykye.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3atlarfou.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3iqrhfauz.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3cuqawsvj.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3bcptggfi.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3zpydigzz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3jigguvth.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3rvtioiqc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3nhnuzpss.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3bcpvdbfs.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3bpspfabl.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3jlgaufgb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3iaqwbuox.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hmzcossk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3fuvobkyx.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3tntskmnn.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3shrdbffy.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3dpmmwuhp.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vsucvdfj.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3ocuwtljh.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3zcltaooy.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3lpefoqcm.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3qxsmmtom.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3rgcvmuog.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3hpcucqzl.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3lgxxnxxt.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3kxbmcrfa.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3fnodlzfw.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3lpgpnlzy.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3nlvpweum.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3hoccatzo.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3uodefakv.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3anidehar.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xjqbozze.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3uzxiaolh.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3jqpoedhg.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3hffaenkh.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3xtjzzcjb.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3tnazbvwv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3jebyeeit.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3duksyyck.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3czwdugex.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3fjswsbye.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3pzaqzghk.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3hfwzwrrw.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3yfhiztzl.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3rmdikojx.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3lpdglmsb.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3fcylpzbw.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3wskscdgh.html


<!-- 参考信息 -->