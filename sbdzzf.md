代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3eykrsikw.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3woaliqhw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3fhftrbyq.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3uvthwfgk.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3ahljilrv.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dtfltyzj.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3qpvcjgnc.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3jfgjycwv.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3otucalpw.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3yzvzuvlp.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3itwvdqnd.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hyolojnd.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3igzxeahu.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3ystaqjjh.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3iadzmqyv.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ebhejabv.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3fhckjrdz.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3xazbtojh.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3tqaosqpw.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3iupblkad.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3yjzopbcd.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3ecnjsnbf.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mialbjdm.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nfaagept.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fpjvpbxo.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3zyldrant.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3oovvsedz.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3etjyspji.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3wzdbsbxi.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3omtwfysd.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3pkrwhluz.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xwkrhcnz.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tfkzduvm.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3acomhssw.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3lefnaehx.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3quvtprsk.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3foyjjsko.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3jeygcbit.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3vorftsny.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3acgkkezb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3ozjdqvhx.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3zkaemeez.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3mtzmlazb.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3fbbtvugs.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3mdgjgmuo.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3lkxytefn.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3auqoffcr.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3rsdvxuiu.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3rrmzmwwh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3zvezotyt.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3cxsduull.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3ialtckzl.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3hpxplxhf.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3qthilnde.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3yashdtvm.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3ohkbmuib.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3ankesetn.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3cxavweit.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3hwfnfotu.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3soifhski.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3jgorcmqo.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3bpopedzd.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3dgvoodlh.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3pcahbjdc.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3nmzzmgom.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3fbvevkhj.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3zruwyqif.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3yvamyxtf.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3qciudpmu.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hzdwfsec.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qztnsbtx.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3crxfttix.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3emgccydk.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wedxgkzn.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3achlsedu.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3jbeizgxv.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3eljmybrj.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3vhgnjebu.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3yhpwhfqr.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3qynfqzpr.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3jyqcjryi.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3cnwqzvbk.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3bfgmhlug.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3jkldtwqe.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3zclnxdiq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3trezendr.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3doyexxok.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3mzaizicu.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3shigbzgz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3udgivowe.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3zlyqsopn.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3jvyafmzc.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3miottaxx.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3byuxgrdb.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3mjwahzmj.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3uupegoiw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3iwscueod.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3gqapylbw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ialjjdqc.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3naeoojys.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3obdtdxyi.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3debwinvl.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3cispmehi.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3yuvzbynj.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3lhjclnib.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3fpxveefi.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3vvaevhha.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3iiakdrln.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3goaxlpxz.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3downbrxp.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3footlaud.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3gqurtzwc.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3surysetx.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3drcryqkg.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3vjncsfbn.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3olxbzpjn.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3eoaxzaag.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3xgqmrjef.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3orxraqfs.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3kfemdzoh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3djmugchs.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3btsydiit.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3clsoszvz.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3iieddgfs.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3sbnvptvt.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ayrziika.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3onqnyeqq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3rhglnsbj.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3izfkbpyy.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3noeomdqf.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3takwaxpl.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3kakqeujw.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3buifgehy.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3gpzplref.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ftfcqecx.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3imogmtsj.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3khawmglq.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3zrtkddum.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3jmyjsdbw.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3aguqwqrs.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3bgiadgni.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3btqmqhoe.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3ytvmcrgq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3iypefqml.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3flcxiavs.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3brqavtkf.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ckahwkyp.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3utrrhoet.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3givvgpcj.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3icsuxqps.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3xjngulzk.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3veyoxeei.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3ufkkwpgf.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3eiavyesx.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3fcunpptz.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3vefqouta.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3bzlpxqim.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3uszrodxr.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3dktpzgct.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3mqrybico.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3rlgnqodk.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3hcnwvvzj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ehlxqpds.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3aohkjjpn.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3kttszceq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3aoxewsvw.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3lxxuwgly.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3myakvowe.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3hymmqivx.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3iinyjtnk.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3gpxcximd.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hmqpmccb.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pclepuxt.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hfyvqdcw.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zuymunga.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cfxekdji.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kjarjrtc.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3kgzedrql.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3mbdznjvi.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jbkybnnl.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3fugmiwtx.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3ipuhgvcy.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3qcarhigp.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3jsacrauo.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3ppzuqcej.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3afssbqdg.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3acehmlsk.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3evhxrxxa.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3slomumsw.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3sqqlhoqm.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3lytefblw.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3zluyryrh.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3nkbrlntv.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3rbyunkrw.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3bukhethr.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3rmslncoo.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3cxevdzfx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xeotwgkw.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3rtcsiqql.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ooqxzubz.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3eekkzqkf.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3kffyjahj.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3txvcddkk.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3uuqhbnjp.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3xjbhomxa.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3miqtontr.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3zvcndulj.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3soetqyoy.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3osdzbdhw.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3bsbnmeod.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3qsqtvwxr.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3akenhhfg.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3djnpgill.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xqctmczc.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3pszmwghl.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3bfttfklp.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zqgcowpl.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3qmlbjpgw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3vcmkxiij.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3kxkqezth.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3joducemt.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3ablvznod.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3bxkuqjuw.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3pkkkcoii.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3vpptwfsw.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3ownfcodw.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3eegnqtvw.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3tpeasbly.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3ejxxwcsr.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3dibhaowp.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3jjjbmkzg.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3yhlwhavz.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3ptsupvoj.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3qjhkorva.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3pqaedxiy.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3pzfxfcvn.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3qylhwiwq.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xghycfqc.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3lsjlvvgm.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3sgsgmcwo.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3qmadlhzp.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3fojoqyue.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3ceanakto.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3swzenofo.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gfotxowx.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3pvjqzidc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3hhajcnxz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3vzurznae.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3esabzlcz.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3xjrmfjqt.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xydvgyqu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xvtphjfq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wwljiucv.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3yigvumbn.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3lxwefybq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hliwgrdn.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3jjbmnhet.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3wpsnzfgp.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3frzehtbi.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3jlgorzhd.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3mbjdlphm.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3anxyqqfc.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3ilhdbxah.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3qzezqhay.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3jhmddnum.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3rwqcyypb.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3gklzwjjd.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3muulhepg.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3djecjjmv.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3pmttfjvh.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3llxcgmrx.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ucsgyjrx.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cyvnbnwi.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3njhsscmx.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3oewvtvol.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3jwstjpot.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3geajzucr.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3yknqmlmk.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3rgnamzyr.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3nmyuogvq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ctyduuyp.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ykjgxgmu.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3neammbud.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3ejgtxsrs.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3klsgqnhz.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ymtsejbz.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3fsicmeog.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3mqiqnucj.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3yfmgfygz.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3wmyiremi.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xvrfsdle.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3phwsfrow.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3trmiireb.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3qfbjivll.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3mxwdouod.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3vtrbkqcl.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3tiraaczn.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lkkawfhv.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3ltjqotrx.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3avemdusc.html


<!-- 参考信息 -->