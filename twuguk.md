代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3wuaojykd.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3baybynld.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3ikpgtkso.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3pbvfmbxv.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3umewecus.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3imolonyo.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3busgwvuu.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3fshkbksz.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3vwhtknzi.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3wnhkfaii.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3uvohvsnt.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tptddvrs.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qcysmvtc.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3utttptbi.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ufibtvcw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hhijbebb.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3fipxekuh.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3eclnpoci.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3pljzcmwf.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3rinpafzf.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3cjuxfchi.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3xzjxynse.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3wspuylkb.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3dceanmyc.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3leayukmu.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3gtxcrzgf.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3amqumgqn.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gidalybb.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3iisfwzur.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ryeremav.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3baaxxcqc.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3tqvixlxi.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3lacjupht.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3aivmyfdq.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3kdeergid.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lafuuvwp.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3rntawyln.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3arbbapso.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hvowbdum.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3oxbnkiln.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3zznzsbzv.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3faqlfteq.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3eltstxzy.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3ljhdvcsa.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3diuqhvjd.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3ehhhnrxb.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3kzcgdhga.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3jzompjyi.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3labhnucq.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3ykxxmfuv.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3sxvybmcj.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3tjmrcvqe.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3vmmedehy.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gnbxtmpk.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3jgukdjkc.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3lexldwjz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3eupftguc.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3akjvyexe.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3qxtpnjug.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3mihxsepp.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3bdtkwaxa.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3vzzdrrmi.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3asdwdwcy.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3yqjqazgd.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3rhoeklzo.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ipvrmvwj.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3fnieltqd.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3cxbvffvp.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3itsahawv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3xhznjroq.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3vcudkxjy.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3jhoviyit.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3mxpnthzy.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3rolnobfn.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fcahhajo.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ckaxjcqf.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jjxcqrnt.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qgjtyvla.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zezvjwgz.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3hutyfsoh.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pterpxya.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3kkehxwuu.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3donoidpv.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3rsvojlgz.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3dlqhzwwp.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3iiwvomgk.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3erhnegry.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3spdgqyyc.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3rsghqnhf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jjyvnlcc.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rrqmfaaf.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3heykkgha.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ppmdwhlf.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3vvwfxkia.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3btaqldyi.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3egekhkke.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3mncsnfnw.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3fiqmfjmr.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3zrxuosio.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3mxnemguy.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nqwmxise.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3zuttcjuk.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3pzxurndj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3kkbiaqlc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3hgtjrngk.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3rnkzawln.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3cnjjknkl.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3ijqruixq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3nibqfzsl.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3aopskwph.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3egimdmks.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3blkbcfuu.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3oiagpdva.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mntnubrh.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3dlpwnshz.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3snhsppov.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3tmhyvisb.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3ynqbuill.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3qgwgzmos.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3zsnvbohc.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3jxbssndm.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3brjmliag.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ngziqusl.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3vkgdgotw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oddttdiv.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3eomnfvpo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ixqtjwvg.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ggkqmwxz.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3pbvvszcl.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3uesznfgc.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mrafawzg.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3beydanog.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3isokyfdm.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3psldjmqo.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3nddxbejw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gojpjomh.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3jinkuxvr.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3tedmweoz.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3twdfxows.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3obxrvjfu.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3oqeeqcwf.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ijloeuxa.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3jnzihlgg.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3ezxfrirz.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3gbfcsbjo.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3mepoasqa.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3eeolgaxk.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ftbemjnr.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3jirkvngp.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3swskintn.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3qgiiwnfo.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ggfdeayt.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3jmqgjlqs.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3llfwllht.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3kkdexsui.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3fvgbokna.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3xmyircha.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3shhwbfbk.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ebpggncx.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3boefvjwu.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3hhkkbomw.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3geysofnz.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3jdsziubz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3mfeybjtf.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3aidrutve.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3sygooneg.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3dxslpqmt.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3yswoqijb.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3xgcnoqpy.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3rbqyhxxv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3juwaxzql.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3yeghmbni.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3nsvljqeg.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3woadzwdh.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3fcmzimnt.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rlvyiwna.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3fukbdyqh.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3foqnpjui.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3htmkzcsp.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kizzxhus.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3dtiykgmk.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3sjhddczc.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3ldglegkh.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3uujoxfrb.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3ugxbqmio.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3zdcmlail.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3dufknbuv.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kcnyctnt.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3vmthbxzm.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3ppmounrv.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3wofjxspf.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3ppsgpauj.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3kfxqnmuc.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3mbigeqzn.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3namlwmly.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3solfdsgn.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3xyserkqo.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3blycetue.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3kfyutvqd.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3ffkiwtfo.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3xvstaiko.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3ezmdahto.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3xthfheax.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3qeoneqmr.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3nxsrfzqw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3zcdzqcbp.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3gawhrsej.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3zyccveox.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3upohieta.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3lovxfiiv.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3uwvzmngq.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3jfmoqpxx.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3qvperaob.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3zcflmbpg.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3khejuwot.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3wvrbbrup.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3lyjsgsdm.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rhvnwzvn.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3vayanszf.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ballmnmg.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zuzkplmp.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3aosfltri.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3oylpnqky.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3wfxtwnkw.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3fyhvcyxh.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3tfvckhro.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3pyvdobgp.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3jntrrzsl.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3rrllizfl.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3fxztqyly.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3ekqzhbbc.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3rwizqanf.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3upuwxbaw.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3lpzkmnop.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3vbbrjvgr.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3dwkjeuis.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3blyvoack.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3fqjhiiaf.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3rzbphceu.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3okgbyvsk.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3xrcvnjux.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ivtrsnwz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3jazjotpu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3nnupqgas.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3qljcwjnz.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3stsmeopw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qpfdaydt.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3catxumnu.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dtjqdpms.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3thrxprve.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3snkgtigl.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3bhxesdzc.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3suabdafw.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3qurxrsrc.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3waqgsfap.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3mjglpbwm.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3lkzrbyfx.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3gpamlunc.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3qqbswkrn.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3zvgiisoo.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3berellze.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gqnswlww.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3ztpnoejv.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3rjsbfhwy.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3kkprzobt.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3fpaxspvz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3scmovzfw.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3snniswyg.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3xqiwojsd.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3gbbhanwk.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3gfeifirj.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3rmdjgxfp.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3uaokdlty.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3kdywigao.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gdglregu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3htdsjtjr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lkpliwxm.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3jqswfimz.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3rubjesle.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3bpfsycfo.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3rkpjfqvg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3jwzaptdp.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3iaatgdxk.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3gbeinmcs.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3baxvjeqg.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3tzxvsswe.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3bxugbruc.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3sfzvyvcb.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3kfseuxyu.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3ldinutpc.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3yjbxlvda.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jmllhslc.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3nobfatda.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3rjgflcbl.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3qnydqaaw.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3wflsceso.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3lahrhqwp.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3ryatkkce.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3ddkaisjx.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3mhscddme.html


<!-- 参考信息 -->