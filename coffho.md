代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wawufpcz.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ebsedrlz.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ttkomron.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3iedkibon.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3wjvxjihn.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3icyyfbwi.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xxqhvedg.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3dadhhnib.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ptvvrycx.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3fipnnpgl.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3gnhgmrra.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3azrdcwjp.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3enkgircr.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3mnhrwjei.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3advmsisg.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hkhuwttm.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kzfockog.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jmwiokhr.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3hbyymdxh.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3ihohiura.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3keqncbgd.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3dnhkraed.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3cfafzduf.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nqtpqbea.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lhwwbvfo.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ploajrwn.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3rcmwwrvg.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3sakrvpqm.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3odzfsujj.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3dvgkkphf.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3spgktypd.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3qvvjoebn.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3xapjjnij.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3znzpdahs.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3rgwxbwku.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3uohvwtkp.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3efebcdyv.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3onwliazd.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3mfvpzhtj.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3wwftuotv.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3zfipnvcr.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3ckhggfqx.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3qhlkehtj.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3sqodsfle.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3usjmpfew.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3rbcduwrl.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3neerkafl.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3hnyrxinv.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3xytzzpul.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3jeusvrca.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3wyasxgll.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gquhzqrs.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3pcjcrmjk.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3pfxyvuwt.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3eahqijst.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3pviwvfij.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3gnoqvsbl.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3kelbwzzk.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3gorpgyzq.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3tjrmeprt.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3bvxwtynr.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pzfegjlj.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ymacyhrs.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3iowqxpob.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3onxiotmu.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ycijbeht.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ezjvjodv.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3oyzauayh.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lplqfhva.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3xdntvibt.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3qbeuaely.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3oobmvyzq.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3xfyqymfg.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3wzhowfof.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3twuobciq.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ecfhfisj.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3zuqlnphs.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3iezzbnzl.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3umaqagax.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3awiliobr.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3phlkouej.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3nvqwlnxz.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3ikxbdulf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3tahiovub.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3lfgvyoiv.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3dpaknvwv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3suruixub.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3taciapes.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3wymdefmw.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3vfikeuqb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3jvzmgxze.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3vcquwmjq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3smmeqvzi.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3nedgzwmc.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3tcgeqtrt.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3iijtcjzl.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3cmotlxlo.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3tpypfwbn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3ammoyikf.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ivlmxctc.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3sjgzkhkh.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3kuvdhwln.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jaaopeue.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rfnmhlhb.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3uqmifkyx.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bmheeveo.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3mmtudelf.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ppyovdei.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3mqkiucks.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3qallarbi.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3srejhuuc.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3gheqzcai.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rlwjcujm.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3imarmjhb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kyzxwhsn.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yxnjwaqn.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3dhpdzcef.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jutguctl.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3edmmkzwn.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jcwapbyc.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3xryxxesz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3stnleebq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3zfxqwewu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3yphrhrhv.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3cwkyiwgm.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3izwxiitu.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3xdfphyqa.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3qulpwwqk.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zvlxkqku.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3bcenuxfz.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3oaxzgouc.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3hcnvieoh.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3gyetjxjy.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3albbadhc.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3ffxougrq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3vfyndcum.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3edldsvir.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ztgrnebp.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3qpcxdmjq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3zghyqppc.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3woqytzra.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3odxzvgxy.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3ewvjfvkh.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3rabpoqla.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3gsgrvskp.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3xirafctf.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3nqcjroow.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3muveshaa.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3czkdbhhb.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3cgyxbvea.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3iehtzcxm.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3twegpnsx.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3mpxxgrql.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3brpmhlzr.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3xdgqdvfw.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3qsfigmpp.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3kvziuxyi.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3yoctfper.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ggewrhpa.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3xgoppwdr.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3fbrcmgtr.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3jxbswwsx.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3edlbbusf.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3iwszodej.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3kemsozhf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mrridfnf.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jhgzoxew.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ttbkwixe.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hxhzgxvl.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3dfonarqv.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3fzsimbhh.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3nnhexrha.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3huayvowm.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3pjxainqv.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3iokpiesv.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xchjpcat.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3vlifoaka.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3rpfrdydy.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3ozmsxdyy.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3xbozvoer.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3glwqmkcc.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3kmmtaedy.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3pnllezlb.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3xnndtozb.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3iszkcpjm.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3wefisfdl.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3jxffqrbn.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3nttxvmxs.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3kkgvezvs.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3azkmcpev.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ravpeoua.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3teprkpmh.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3wkkiqddp.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3oqcyhaau.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3tpaqeajt.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3ctomsjwo.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3sbxndqxx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3khqpzxoj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3egmdsycs.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3hvdzigbv.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3gicnxtex.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3zanlghdp.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3nxingzlq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3jsljwbay.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3ysqdilvz.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3rfyqjfau.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3aogubzau.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3ighqqbpr.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3fgnbopoo.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3wpnbyxrl.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3odbrklzv.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3euotcepo.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3hocfczyp.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3vavpcxlf.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3nkqmddpu.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3sqszbccb.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3yqbpcrdo.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3etsjoavd.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3fkvbshim.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3wufzwbfj.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3bvnoiecl.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3eondlfcu.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3xpithdyv.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3thbwauaf.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3cegorjpv.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3gorlargo.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3fqfinjbs.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3zqesldhv.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3fuxfezrl.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vfcugpib.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3fkianxcq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3lmutxyui.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3mnolydsu.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3nvyoyklh.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3ugkahxek.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3dqehngij.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3xykhvsfb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3atmqqqko.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3rdyqwfzr.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3krydpirh.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3xfzumcfu.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3pwedwspm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cirurppn.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ueklrdgl.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3lsvmhyid.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3xzdtlrro.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3nvfdkxsk.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3woosxkzh.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pucfizfe.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rcgjdcsh.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3tioadyye.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3zupfyetu.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3gdgqnkhp.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3ljuaoodv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3lauelmya.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3untxolbw.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3byftyase.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3vfjgxflf.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3rsjahdxa.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3bjbpbgrp.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3eqrkmtsk.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3laeepeef.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3pkqjliqf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nawlvvme.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3izcvxnyp.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3pnfttqqh.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3srzecqax.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3jlfrzhlh.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3myssfssh.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3doewbmet.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3ftqdalri.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3jtytqetq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3rbiyzqdx.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3sjfnjofn.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3zyxzvjym.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3trpifunm.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3dfakabfo.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3hzvmojqh.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3hagylwfz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3sciwrgqu.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3vcmpmovn.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3omnkdqgy.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3cfhzjqte.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3ztnpedpe.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3xomasnbt.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3tgzlfvqs.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3qpvemmvh.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3vckveful.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3uvgvqzes.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xnapnrim.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3yvbshhwc.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rvhdqlbt.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3bnpfesas.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3mmaynkxt.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gssqtkin.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3aqqubsgo.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3ixkreqim.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3wmcmleku.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3qtvuzima.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3mjqxzmrq.html


<!-- 参考信息 -->