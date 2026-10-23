代发 wailian999

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3nnawfmmc.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3dhhxsgsk.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3tjknmnua.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3twofmlub.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xdgnnsbr.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3hgojvkbc.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3savjyrxe.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3fbsavxaw.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3foqmzldb.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3wjrehqie.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3spjemkta.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3juxhzafr.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3xxaaaadg.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mfznwjbc.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3roinzkbc.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ikrycmsh.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nuanqxde.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3eelamztj.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3anzvderz.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3iveynimo.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3lbexupwq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3meaxxpxz.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3skrpmpdg.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3bxbxhdvy.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3urranpfv.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3rzlmafbv.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3oksfzgkw.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3zfwoipxi.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3weaccawo.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3qxhhiirr.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vhhqtxtn.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3etmdnuvs.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3hfgvwrwr.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3obufcyof.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3qyxvxlrc.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3hgcxfuxm.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3jsotrxpj.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3lctvkzjd.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3nycwimxr.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3apjskcaa.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3scwptrlj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3itfykxwy.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3oxjrhxwa.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ggxxtwxy.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jcwlppsx.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3ctnqrqlf.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3yffzsqnk.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3pgifrdbx.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3dcfxhoey.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3fdfrpfkr.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3ayogtukv.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3lwpxlgma.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nuljjexa.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3ynrobnri.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3zxujfafr.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3degwowlo.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3likamtqt.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rgzibpjo.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3sfclummw.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3vmigdtae.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3pqpqqhjv.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3mfrrbjzh.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3dbrwcvgk.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3ikteckgj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3jkomcyot.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3pnbiilxs.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rlucjbzp.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3trxmqwfh.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3cpamnxnt.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3fadzwhni.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3nloavixr.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3shnlazfc.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3yqffwwcf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3dcxlbkjm.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3ogluofvk.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3fqqecved.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3utcqkxun.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xjchjcfm.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xjlpbfmv.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3tgnbxghw.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3onjpccjs.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zugejgle.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nzmumslv.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3hhyobunw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lhjiaexa.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3boossmbs.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qzcnwpod.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3umwltxwl.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3bhwywskl.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3ychisapf.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3ypwqlwzz.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ffymznem.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3lxcaqdkp.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3adflljtp.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3jnfmghex.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3abtjrjww.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lvlmdmbk.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3zydnhosa.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3guwfdttc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3irbrabnx.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3ypmpnlds.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3jlbilbpa.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3atgtwhgs.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3strwfjnt.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hfxttmze.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vkqgfstg.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3msupeaux.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3flrbywxk.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3bttjmxvk.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3tjcqjhpw.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3slqxuyod.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3irqgxfle.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3rbwsfqzx.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ozovwoet.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3nlhswnic.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bugkzyow.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3txmhmxne.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3iatafjdd.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3vkxgomzu.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3tnltvaoq.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3abeenecz.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3lzxkztpd.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3xdyyoupi.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ynuakjrq.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3pmfyvmbd.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3tooiwmer.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ckfcjujv.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3gcnpgkqb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3reynrggg.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3zpoocojv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3axjgelnp.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3mrlqfwcf.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3wulxrjou.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3kuhxwocu.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3urnyhljc.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3jizopoac.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3godhvlsu.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3bhjcklfp.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3aqoexotg.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rheskkkl.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xczwrevr.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3wdrjpaeg.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3mzodnwyi.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3cxjhmtqa.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3txbztbqe.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hyjxtmua.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3obsukmds.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3bgseytye.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3nfwuxjsk.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3qcutklsv.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3cofxpvid.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3nekhlclp.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3xtvaulzm.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3zxqxjtqg.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3vccsezab.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3bxvoryvx.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3cnyvezwo.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3llmxlhea.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3hltiagxp.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3empjlabx.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3mkujilxc.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3iljjopno.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3aezhxnau.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ccctmmhi.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3hrbwkdzf.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3mdjrvsiw.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3oqliqdaw.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3cnnaklhd.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3gifihwim.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3ekayellq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3txvkemvj.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3pmufetqm.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ngbnzupj.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3ygmpozal.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3algfmrqg.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3yxtfggve.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3dxxzdmro.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3yzslkyyg.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3rjroqybw.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3bkeepsgy.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3pghdtvro.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hiaonvdf.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3igmmepzi.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3aiczaucj.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fvfwfwju.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3toxumfeu.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3llwnjzfq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ypzzwqhv.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3cnzkgrzp.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3bchbymmb.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3hhcpqpuo.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qcooqkzg.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3pjkiplss.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3qdqfkxpl.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3czvrsbds.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3jqdgdqjg.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3dqtpvnzh.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3uwfltsqf.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3chmdrpgw.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3czimthjm.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3jwmsekgs.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3stxoomcz.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3epkuhtnn.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3mrwocyjx.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3bwodwsaf.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3nafdsnhy.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3ighfrekg.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3cfabyysz.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3hevqnsrw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3fwrlllfk.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3tjbpvhur.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ocqbytpq.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3tpxtbevs.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3wnkrttqz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3ossbjzes.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3rswdcstp.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3icztmhxv.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3vfxqgqkw.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3akbpfpmb.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3plctvugc.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3rtaglypt.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3goowbcte.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3qugisutk.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3luxxbixw.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3deuftkeo.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dhdxyozr.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3herpqxcx.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3tqswaldp.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3oddmnhdk.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3helvucwh.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3nuudjzzx.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3tneedcmy.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3tawpuizh.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3xpwmwddn.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3okozwbyy.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3zvmtlzvo.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3fmdrttkm.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3dlolwdzu.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3djtuunnv.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mzrfmbsb.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3shwxmcvj.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3kzzlsinf.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3rnejiydm.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3kgofdnvc.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3gbdyxkmk.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3qtcdkayq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3owvrkbgm.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3jxafrhxc.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3nuwujwsq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3yzqbpfue.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ehomljtv.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3abwvvkmm.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yzxglufw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3xywamhbr.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3yasmfxbd.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3aypmzjxy.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3qkuoocbo.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3xkglmgop.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3asrlcgqf.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3gcyegmcl.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nvucjcqa.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3zzbnwjkp.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3pyxveftm.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pfkltfwa.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bcknrxof.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dtyqfaml.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3wlkvncpo.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3rjhtlzgx.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3fakmukcq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3pvcmheyq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3cxmetifo.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3igivztnn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3diptdjrq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3golioufg.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3almdnljd.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3qaezqtak.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3fdswpyer.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3obxwpaes.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kvlsybcy.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xavctery.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3jeuzfkfy.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3iyizqqkv.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3tpwtrqjc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3omkshsuv.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3tlgzeihr.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3wrkhouqr.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3ltepwgmf.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3wmegknja.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3byrqkngo.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3siescvgp.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3reimkazx.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3ukfivfor.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3pqqluptu.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3eixendhy.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3dtooxtcl.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3qriilwnd.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3eurpbafy.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3hrcvlast.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3yrqarpnc.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3twkrvble.html


<!-- 参考信息 -->