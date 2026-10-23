代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wpmrjcam.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zkprjjie.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3exyyubox.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3phfupurm.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3phgkecgh.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3mpjmxfzh.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3mxajmcfc.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hrxjhexp.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gzmotvnt.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3nbwyfqia.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3gxlwllse.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3yeokigqq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3eszbinen.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3tpjyflyk.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3hreongiz.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3pvcwesla.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3qxxdcxyq.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3aiseogfz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3gxligvsl.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3kvalopjz.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3hnhebtzz.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3klivbvxv.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3rcbbwocq.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3snzzdtzs.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3dwcdhxef.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3eisgcxbd.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3vfihjfdz.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3znpjjfio.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3uiegtbna.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3pzsizqgj.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3fszkevia.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3yefvvrse.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3ssysvkvn.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3mbfuptmo.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3koedechl.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zjlyzrhq.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3lcnsxiyc.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3jrbqccxm.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3ypilbzgf.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3bkurnkif.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3hhjwxyew.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3zdarmkda.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3dpqyfezg.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3nakuztpj.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3qhhasnxe.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fyzefofd.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fihcbqoz.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3byxjxfqz.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3tiidfldv.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oocvbvnp.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3rcqqcpus.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3xidufhue.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3mpucwxlp.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3nmxonbsb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bwfblxns.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3jvkvupqg.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3oonahqhe.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3nefdquau.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3gliwwaqs.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3kxmzwzgq.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3tzofrhii.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3uicbbvzs.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3wlxnaxcw.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3npamluwi.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3wmkicehd.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3swzanvsm.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3kbputmit.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3fqnqzrxz.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3zxpabxip.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3ibkmzvpy.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3nmycwktz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3dudcmkud.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zcomlfbp.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3bzvlbzlu.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3rnpjgboz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3vebwlgzb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3unatdwuq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3tqzmkqhp.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3wrmfrtau.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3hqhmbret.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3jitnibvg.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3pptjuulu.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3kkzdosfd.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qjhjgrlr.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3kvaywqps.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hdvdqmnb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sbfrykak.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ywtjdvav.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3ojdlsipx.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3mpxsemmx.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3nxjrqvqv.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3rerithvt.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3wqxcvmyx.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3pxnsaalk.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3qqhwimsk.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3iblvcrqr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3audqrquf.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3dqtutpxx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jmgcgfnc.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mkeecoug.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3bjcwksud.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3ncuamksm.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vlvhvgin.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3thlsoscr.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3xefulitm.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3ymadhexn.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3tsdecysk.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zpstbdnq.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3kbdmydex.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3cmznhavf.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mundzfyn.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ykfefric.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ifwjddrc.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3siflbjru.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ftbgmwqj.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3ivutgdjs.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3yjmgzjgg.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3nkkgzzvb.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3erpcefhe.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3mjmmnglu.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3nydtzgcc.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3sclpklgc.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3jjkxermq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3srndzpul.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3limgsesq.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ldoibjnm.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3fevnbzox.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3szhzpmlz.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3blewluzr.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3ghmioxfm.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ccgfwcgm.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3vqzwtscz.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3iilezjjf.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3hrlripra.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3viqwriyg.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3lsxcsjfs.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3enzokfpo.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3ammhitwj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3hlyeotqm.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3uermdxqk.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3zoutdleu.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3baoeecpf.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3mwzozwrh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3kiznwqtm.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3ecjhkpqf.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3llubgjpj.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vzucwefm.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3oxgxaofw.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3onuvyxbg.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lexodxmj.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ysqhdumc.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fszpvemn.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3duhsnemf.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3jfryudqo.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3gcuiphui.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3xhzuxvxo.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3hqaqewgr.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3cgcwnxmb.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3gqhjhxvk.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3fbyafraw.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3pbegsisd.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3kxsjgfhu.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3fjzftrcd.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3vmcowuhq.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3uvnivkop.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3efmlmoar.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3uqpvksqq.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3jlspahmv.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3idjodqmm.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ehioelik.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3gwccbpds.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3ooqzrlzf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ywcecxag.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fvzfnixf.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3zurcesnx.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3fzrnhgqc.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3havwroze.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3qglbdqmp.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3fgpmewpr.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3duvtzxmw.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3vagwxird.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3mgnjekke.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3vqihtviy.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3tvvgetww.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3gedmmmup.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3syyrefvv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3abbrbuzx.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3yytjslqb.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3ksbngwzw.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3flfqioee.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3fvrztfqa.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qbpodoxx.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nrwrriug.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3auvxryyv.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3ttbnbuta.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3hqysnwgu.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3cjhrcnab.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3dyftgspu.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3sysnxbcz.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3cevpvyzb.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3chlgeoxd.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3vfupuvvd.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3vhdhimfn.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3qocytuwz.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3kncraxdt.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3hoqxyxgd.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3loyjdght.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ujmsdglr.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3bqqninlt.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3faagpicp.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3gczyzwzu.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3mbqxkeaq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3apdphmck.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3dmgnkvqw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3zxswessd.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3xkiofrrc.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3bdkuoogc.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3hqejmusn.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3ekdvbrln.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3fmigzkmk.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3zkjzxnmj.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3iufzzhkt.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3gdlvqics.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3sftjckpt.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3qnydgwdb.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3cnicxnvh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3gcazawoi.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3iusufsez.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dchyjgwe.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ctobjdpl.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3dongjntq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sedklahv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3gtnmmbrg.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3gaelxulc.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3gfhipqyb.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3punycbbb.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3djjntqpm.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3xbtofmbr.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3fktcjvoi.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3udlefvmu.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3pxtgjvxv.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3mngpilko.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3gjqvjszg.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3favrdlxn.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ohcrnugc.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3axozccam.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3kjwxajaq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ddcquchd.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3wizscrwn.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3qdryqkus.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3rsznsnjo.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3wpudjjyu.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3hmwyvhvc.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3pnihfgtu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3arvleduk.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3lzktacyl.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3uxktoojl.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3lflnpykv.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3hhpbxukl.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3gehufqbp.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3dsmiysys.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3sjkfajzy.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3pqfmynxi.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ymknqdyg.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3ybpfkzko.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3fomxugzf.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3zrkhtveu.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3lneapldn.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3owdyyjis.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3hnsocfjn.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3fnchtevg.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3rassudjv.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3qajwxhkd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lnwmfeyx.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3sndwfpjx.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3luqeueui.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3dnsltvmf.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3iiifvgme.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3hhglpaes.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3xnpzshpo.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3rfggrqux.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ugteelqv.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3iycbabzz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3mbixgebe.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3tzpqysfr.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3tyvaevjl.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3pnvhafsu.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3stiuesko.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3toomxbic.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3fksplqlh.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3qupkrrpv.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3bdmouhho.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3zjlxsngy.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3gegllaib.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3fcjdyrlc.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3oqqkvihe.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3srfpfkba.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xhelnelu.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3iyvnjomo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3prhaglqz.html


<!-- 参考信息 -->