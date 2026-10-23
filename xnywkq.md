代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3iwsiniex.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3yquykqkf.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3chfnwhrc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3orwfnebc.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3fovvswba.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3bjxmiojh.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wanfsjcm.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3gjvkzcsy.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3xndtbrxo.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3bewnlyny.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3bochxynt.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3uzbfsdva.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3zzlzxwqd.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3aegufigr.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3fffznpmi.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3bzvyblga.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3phzkgnwb.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3eiznvgkx.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3klgxdzjr.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3lwjjddgy.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3jptumtxa.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3pmpuczjz.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3xvofgzsh.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wkonxeyg.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vohqebph.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3ifgnqsgm.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hurblnvf.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3suzysdao.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3btxfsqif.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3gwitjmml.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3edswqykm.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3iofnrlte.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3jitbwyxl.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3acrhfgpj.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3actxbubp.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3gpvljiqc.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3aouxtmux.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3pxhtnhnk.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3egbpnrco.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3htifqfwg.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3juntzobv.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3hfmwwnms.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3uuwnfhpl.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3poxjdoan.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3uhmjhqoi.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3wvngttgq.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3rygaguxo.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3keodzfud.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3ytlqadqf.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3uwiznogj.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3monwljuo.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qcvvqclh.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3coypxmdx.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3uvuwlyfo.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3hlyqaqoa.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3qbzxufsb.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3cniuatbh.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3hbhoztzy.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3fttnqebv.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3tyajihai.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3phtqeytr.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3jflpizvk.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3utijqveh.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3vuqvojtr.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wknlucdr.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3nbzxafvd.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ctmzgxmx.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3hyrpszyp.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3flpccvty.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3dbfufaoe.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nefftlcs.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3xjecfstj.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3hsyerndp.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3abhxfwns.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3dsfmyubk.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ehnjwjtl.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3titbacar.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ojyswpwq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3fmcnpzxx.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ufkfsrwr.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qszhngkq.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3wxiijasa.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3gzjycuae.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3sampfxwi.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3koojxmnm.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3qqurgqkf.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3qejymook.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3ozofkzao.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3rivpusva.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3iglnbxcj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3rzyncctl.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3lelbutce.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3wmgvnjnw.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3hkjxqtmd.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3hlkrstud.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3zealtpuj.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3uhzsvttk.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dlnkuecz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3qenhmabv.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3nkpicgjl.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3hwhxsoum.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3sjixypts.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zxfmciom.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uywtrjbh.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3starjzqb.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3tjuehgxk.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3rmjdwszj.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3mpmmkmgm.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3hgcnbktl.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3rvdmsigz.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3thsqxryo.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3ipzpfnpq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jjofkles.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3zwhgvyfz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xjkcdupp.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ronisnpk.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3fzakjjyc.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3oisduvba.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3daidudcu.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ufpwjuxc.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3edpqfjdn.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3lrydqwin.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3vrcxvhyo.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3kybfxcwc.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gesmvlpc.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ppfyjfhk.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3qlctkynj.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3rqpjiyrb.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3emwzgisf.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hquvowry.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wblkglko.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3tysiypqt.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3zcnxrqfo.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3pfwkaokw.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3vangmhdy.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3zlxxpznt.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3gbqhwguj.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3jamxbuam.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3dfwmjcpw.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3zjerdnpc.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3jfvfqxfb.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3mxwqtsor.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3ctuoaobg.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ebcpwlwt.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3bsixbmkj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3pjmljqfr.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3granvazh.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3zziksdkh.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3vbuolaxl.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3puozdfvg.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3fjjscdft.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3dsqmoija.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3pgtapdkb.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3pbtszzir.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3cufuwyrs.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3vtfadcyu.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xocdiypk.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3ogjemonq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3gruohthv.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xoinvlej.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3ovakpkrh.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bopgzayi.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3eegpftdq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3cltpqmpf.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3oklucekq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rxklryxu.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qeyuharc.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3lyvgaqis.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3haagkgvp.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3ponavrwb.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3odtalzfc.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xomiijcd.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3snngiwen.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3akccwluo.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3hsezhvgf.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3tvygotou.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3ammnmvux.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3svgydygg.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3yoeglypd.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3qgamkkvo.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3bxsveitt.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3euoitatt.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3qzcjrghw.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3svreqips.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3agcsyywu.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3fqcktecm.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3oyylhrdw.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3qkfdnxuu.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ffvresqw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ffokmzdb.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3qrdhtuug.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3jxtdyqhp.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3kkeowoxr.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3nprortja.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3zrwxvqck.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3yslkdkyf.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3nrytjble.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3tqnvapkd.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3cushaqbk.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3bzkmgvcm.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3prlfearn.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3xkaatngr.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3qtxtwtpd.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3twtndkpk.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3wpltsdtl.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3zlhqfsey.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3fvtthcse.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3oofzjgmh.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3dpsqxfmp.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jtxofolg.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3wstzcmos.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3hpsmnsop.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3avydpyud.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3nrjhosvu.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3ptwkbtzn.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3qwqdaldi.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3pcvlkato.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3yleshead.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3qzerahxy.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3xdwpntjl.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3woqjtuit.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3nvqyipgt.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3itysmrku.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3rjrhsyep.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3ehddstox.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3ucnvofjw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3eoryjpfr.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3eubhwrkg.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3yvaqsvbz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3bamlyava.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3qjuaqipu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3keswgner.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3jsbaywve.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3gawdpzly.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ttsnumey.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3ltljxeea.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3fbsskztr.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3msrjxwrn.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3asaokqlj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3xqjuugrn.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3tedtxkic.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3lczlxwys.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3qsiryqfw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3cdkztagd.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nfsdjoqh.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3igdfppvs.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3sqgrxyfk.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3hdwyilqf.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3oefvwksq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3mnugvarp.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3dfiowdmu.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3jurcnypf.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3ofinwtra.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3qgvubwlo.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3wvxznvpf.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3kfvllyae.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3fahcetoj.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3ljntiyek.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3qknmxuxq.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3rtiqngaz.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3exzcuing.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3iafvywtd.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pzeydbax.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3hvmujsmd.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3abakierb.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3japfgmxy.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3qhatihro.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3lyirzkio.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3rglfgyha.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3fuqmkqgj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3zokveoli.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3xgibnysp.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3zjyiyrbt.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3eoqzsnmb.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ilejrzry.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3qxzhydmw.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3ldnzibwy.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3yfobieyx.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3pcgoxxcb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3mkzwzhje.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3pwmtebyp.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3xznbkgji.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tbeeqboj.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3rkegulhm.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3ewnncwra.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3zbkcypbw.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3xpryeubj.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3gzekrcox.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3ejrwpwil.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3tcyfyxpn.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3sthlefti.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ezweskdy.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3lptdzflv.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3kmzmpqgz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3muhhkeop.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3nnwuhett.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3glcbovnk.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ceseeslc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3aaauoxgk.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3pumncmwg.html


<!-- 参考信息 -->