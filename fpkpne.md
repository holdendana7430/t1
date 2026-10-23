代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3algraqwd.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3fuaeylwq.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3dmjkspqf.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3clziauex.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3ydajroff.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3gcuagcwr.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vrhxvxzc.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3jgmdgcps.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3hziyinff.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3mlvqyacw.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3pfygpavw.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3gxlowoby.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3ztsrwzdw.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3oksytvsd.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3vyryzhsa.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wrayesxl.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3flnkfsuj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mfwdvnto.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3tvikthow.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3zspcbmmw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3kytmejik.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3amwjqemj.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3nxwubhwf.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3mchujgmp.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3kmlpjzil.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3quiieauz.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3rdjtetqk.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3zggfctmd.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3ltjilzln.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3tioxxbhd.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3nbhfiaeo.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3ngofsxlk.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3vaecxffo.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3ddttwebv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3vpboyjii.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3zxnfdmom.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3wfjavgoe.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3jggzwgjl.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3qxvtilct.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3jpupqrkk.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3rlhjldya.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3udptqnqs.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3buvlskbg.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3ebzfikth.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3yvxfffvo.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3fvmicvnf.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3kdoziyib.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3zsypdxdb.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3cghvlver.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3wzvxjihd.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3jjnretco.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3qdxmbeem.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3ditaefay.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3brnzdwmu.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3gftxqpfa.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3qphxvjnl.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3ilwpqqxs.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3vgtkrlgc.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3zsijzabi.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3mkocuxtu.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3gjdzksnc.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3htqlkswl.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3entnxphs.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3trncocrp.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3isftadwz.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nnlzniuz.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bgwjwgwc.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3oznzyewv.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3eojnxpru.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3zpwpjtef.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wblleupj.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3rkrqlcff.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3jkosqloh.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3vkinapmd.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3bdctuewe.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3ljbitpuv.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3qmxyijfm.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ezozdfeg.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3hwhqoutn.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3fekxotbb.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fccwfazv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3sxueszik.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3sbqlryqj.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3gdogtjyo.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3qpudgrti.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3xsaaisyc.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3bjrkqgqw.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3aqwvngbw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3iuortyun.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3todlxkpq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3uwgxbncs.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3fvkbbkmw.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3jezqtfeg.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3kxbhlxfn.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3uqarkaya.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3itrgwqhn.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3pihfnyja.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3ilrrvhju.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3kyvcrfzq.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3rvenoahk.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3ildyityw.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rzbcrqyv.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ojrmxzik.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3jimgmywy.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3tagsapss.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uiceeahl.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3vatohrcw.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3mxouazkg.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3jbmpcvxn.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3kmtmuwik.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3jggxhpzv.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3behrvsmg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ngbwasxs.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3ufxtsxjn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3klgorydm.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3kddpntkk.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3frtvfnkf.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qkfdkyej.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3umabtlcg.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fsojouzd.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3ztehagnx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3icgjdjjp.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3mdrdmbkf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jxzfohph.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nbtaiuyw.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3vgwboscd.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3uauvsxfa.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3lyblhyfi.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3suihlaff.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mbzjzuhn.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3caadbiui.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3mslnelqn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3xjwfwcjs.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3dyyrkqvo.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3rrjprjww.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3aqoyvneu.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3utrhvfyw.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3nvdqbgmo.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3kpguhpfy.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3axwehtmc.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3zqfzvuez.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3tbzehsnq.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3zkvdvlqe.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3juseualm.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3ahzmeljt.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3napjneyt.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3nkqevjfw.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3wbixifof.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3eojujcrq.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3lahaqrmc.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3sedfzbgh.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3ynvrlshe.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3tuenvujt.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3wpiyoako.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3uxdhkvrf.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3icwtverc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3clggnpsc.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3wiaobtpm.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ydraysdx.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3uxywrktl.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3bjfueint.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3kvdeiqnr.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3vxzuryrr.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3pkebdmty.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lrqwyjnn.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3eyuyqioo.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3qixtnvfd.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zfcbjctm.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3orqnrxad.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3dzafrxys.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3qvodrqjx.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wfdcjgwd.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3urzxdkkn.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3vqqheobc.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3ullymsgn.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ybqjqbqf.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3dzwvejei.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3nhmgzvuh.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3vnjkybkk.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3hadnbsxp.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3bhtilzbx.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3vremezjh.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3fqkrcgvr.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3tnthqudr.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3hhibcajg.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3fjobkyvx.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3yygecnud.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3tntnjzig.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3podsupla.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3rsogturd.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3acgfcmdu.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3btejhipi.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3zhrnvtom.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3xagwjxfo.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3dpmhqcce.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3kpcxrdap.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3ivpwwxwc.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3nliqcmyl.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3dnouhfvi.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3jhqumbyu.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3niqbktga.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3jwymaooq.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ubkoqnlh.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3xwjeiand.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3uxcbfhdr.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3euajilch.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3dvoflgla.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3iaapbpzv.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3pxyistyz.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ddfpxbrk.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3flnxtpqd.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3nkamrwmo.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3dvtpbbku.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3uknrhoye.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3gopenbxg.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3hbnqglng.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3dnqylfhi.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3nqdwjxyd.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3nhzmyucg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3jjnchymb.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3wwvwqrta.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3zbjumfyw.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3mevwgpwa.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lghirwhp.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3axfqrjzz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3hqtramhl.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3sxmcaryg.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3nxhoagru.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3sxowpdkl.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3bwfgumdr.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3qykgvbgk.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3oyrioeer.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3awwcthch.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3mxdglzls.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bmarelvh.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3aeiyfvlw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cmiicjcs.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3yjdnnkxi.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3gpoykmbq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3bmmsftdz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3eogfrwrt.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3ffhxukyb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zgyayiji.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3itnasqdk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3tijmpvat.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3yqbmgwoy.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3uoqpfqbd.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ydbmjpeb.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qdpbirhd.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wswrjmeq.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3wbjdusyy.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3dbqmoavc.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3mpbtihey.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3zrvvpklf.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3iiycmiul.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3gbhqrofv.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3nudmpnxq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3hwtdmsek.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3xnhzonvr.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3gxbngmye.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3egckvpqu.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rhgqxdqu.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3jjubwdbv.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ypnoixvk.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pxiivitb.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3mdcgkxup.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3xvratldu.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3dqpwxxlw.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3zlsdsrci.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3vvvuchuj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3zdmsmork.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3llzesyli.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3vafvhwks.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3vfcjmuiw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ldfgctpj.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3rrxifnpi.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3outveaao.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3jucjewuj.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3ijnstety.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3hizwqsre.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3tambulrd.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3lobrjwkz.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3puduwnzt.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3uchqxdri.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3jqjbitjr.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3wmpalxjq.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3gbmogcah.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3xjwusmhk.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3frjuzqqj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3wlqacsna.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3pyplzesf.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ahttycux.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3qgkdfjhe.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3zqvhufhx.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3uyqfxhsk.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3afumiryt.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3jowypwiz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3gjpytvig.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3zfukcrbp.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3uuzcsijl.html


<!-- 参考信息 -->