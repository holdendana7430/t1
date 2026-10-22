代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2cwzzqgli.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fviqoqem.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vvarefow.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2hhsuvoba.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2sfxcyyxy.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2xfhfmpcr.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2falozlgg.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2xtoplvgx.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2xyqfmyfp.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2lqacbblk.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2bmmvbuau.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2mtnfmlbo.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2fulmnppc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2ppilleah.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2wutgofjr.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2kxmxxnnp.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2boenzdis.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2wzbrjfrq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jhinvett.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2fcpphrib.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2croiryxm.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2cyufwvmd.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2sjbayngr.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2lsmoqusr.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2rjpsrixn.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2mesxmska.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2msytqycb.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2jikjufqk.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xheiwlqj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2ulflgarc.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2iedgrlzs.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2vveafmzm.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xzyehbvv.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2mishbxxk.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2akfclrpo.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2vagqfmzy.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2hoacpmcf.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2gmqoveww.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2qsgsmudn.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2dtqceage.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2elhejsxg.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2rhamyqsy.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2bamzblqd.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2nbvxuvni.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2qeaxtqvi.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2jshtfbtp.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2hpkacqjo.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2sshgpsgw.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2hizuyfew.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2shufyusn.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2nyncklnw.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2tnupxpvb.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2mpfosrdu.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2atuuzrjo.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2dsxbucsr.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2azqjxfiv.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2ykveyvus.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2gmjyxkcs.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2zjqkfetn.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2wgdblfxx.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2jwbxlili.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2ocrwgflt.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2dbureqwg.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2cyotrimu.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2lkzpacai.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2azydbxch.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uloqgava.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zumcrrdi.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2foiitvrs.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2almwbule.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2awmkbutw.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2evceaxay.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2bgybqryr.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2igxkxkuc.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lqpuebyh.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2llesdulg.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2vzhsiimb.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2jgpuenas.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2gomugsyk.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2etjpigmh.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2uynbynpg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hnjgllqp.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2synxncxq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2xhwvjutx.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2lnvgpvtm.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2akjeespr.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2yfzxeerh.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2ddelzkzs.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2adbwlayc.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2adpvsure.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2jhrnghrt.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2sakxrvrh.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2abazvoob.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wlipfobj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2hjyibkya.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2xjojwtdz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2mlszvngj.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2hhhivlzr.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2pcwyonoh.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2vfrfqwbv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2dgyahibi.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2azfjbmiw.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2melrosyp.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2uflhfvmj.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2anjdqwme.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wgidnbjk.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ihbajlya.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bzsxdaag.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2xziabvtf.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2faamhtqo.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2xygmqmxv.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2zqynopbk.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2cxkemksc.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2rqppayfd.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2tqiotsgb.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2amjfzbkd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qejvpysw.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2dqknyavi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eclwuohw.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rhdosupd.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2unwfovpt.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jviicqkp.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2cgjibmmd.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rwdpepez.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2qdbqhypl.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2nsixglcg.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2zmvldhjd.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2twfwndgz.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2iayzpjyk.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2tbzmuqrh.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2bjtyhwqb.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2erhcnhhl.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2euwdebnm.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ofwvhqgu.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2cnygcghs.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ccosyinn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2vhmqokhv.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2bbwrtsfx.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2lzpjfxmr.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ubifrbsh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2uwsgyzkx.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2okqsqkkz.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2xpfoptfw.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2ekfjnijr.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2eksmkmci.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2dhqblvrl.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2mdjjhqkb.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2etzrvwly.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2zyusirox.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2fiiqqysk.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2uiwlcapk.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2qqwgscib.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2syjkeqzo.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2dfgvrrxc.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2qbedrwup.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2ofqksqvb.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2bxvknppf.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2fnnfyppa.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2qiojcicz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2yuaaslzr.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2mlawlgmq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2huoulopq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2nzdocles.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2pwutcyfo.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2oixvgpub.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2znnvlgmq.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2usiftums.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2yitbcnep.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2wsywerlp.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2abvcttzu.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2szlenkhe.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2nipmuuzn.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2pdnatigp.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2cmgjdihu.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2vnehujah.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2cjregepi.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2mxojsmtk.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2kcdbrlsw.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2ymebhphp.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2jnlixncy.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2brqhzdab.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2lqrclnzp.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2zpbdzdya.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2hwgengwh.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2bfmeinzf.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2tfouqlai.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2vuqqnhij.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2zpybqohg.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2ihvqufhh.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2beoktyvn.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2obtsolov.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2oqrefive.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2dtlwtrsm.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mpqakrwz.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2xaeoyvbz.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2urygnflz.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2oarishvn.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2ejfdygit.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2juqsqkug.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2xwysnefq.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2cnbeomlk.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2yaxzdzmn.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2zowxmmfw.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2rxtisrzw.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2hoxnurjo.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2lxgjffcq.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ktdxukjp.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2iebmuzwn.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2qwbzfbmr.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2foodwxvm.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2hcznrvry.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2bqudjzdq.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2uzdqvfkn.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2idiowmim.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2pelvwdxs.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2hwdrktds.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ctiaodul.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2cxadjqpp.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2wvuntvxz.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2hhkgxbjr.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2ygimkdux.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2fgqxbszi.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2pbxorhno.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2krlpczky.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2hhwebrbt.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2tbtzeqsc.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2mjzpwrbp.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wgmequzb.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2cpfroslo.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2jpeuvquy.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2sqebgirk.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2lozvypkc.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2xomxqlsc.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dxzaqpbr.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2ebycmmci.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2jinnwbno.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2zhrpjhmt.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2mfyldyvl.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2ukfetpqf.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2keiozyct.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xzjncjzk.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2mjoankmk.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2jfwuefiy.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2fslfjulf.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2thinsddc.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2jerybjdc.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2bsfuuako.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2rjfcixhk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2juphesbe.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2oszyazbk.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2nqqhjocw.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2xagezquk.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vcwnkblp.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zxwefxuf.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2qmbggfcq.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ztszvvuy.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2zxuuowub.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2snohrzbd.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2ugkmjxho.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2pogdmhyq.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2nkuykbjj.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2bdwssclx.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2iccswsfy.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2rifebjvb.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2pyfqihya.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2mdiqywab.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bnftfyzu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2sguskpxr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pgffsdmi.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2fagweftp.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2eghmhieb.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2foriyghb.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2kiazvljr.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2yuxjuugg.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2tleotwxq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2yjmsfldr.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ylxgvtxs.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2rgsmgpqd.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2uwohkkur.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2tqrhmkbb.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2faaqxllp.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2ojfkmkwm.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2bhvmcomg.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2zdecwuiz.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2vkaqjada.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2doyrdvfn.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ahthqrqg.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2sahsjibc.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2nkqobdxc.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2vugyfywh.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2lzglizkz.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2xxvowiwz.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2frvwdnsh.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hfjojypg.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2xmeyfhwa.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2zfawxohi.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2jbmnlouu.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2cwottltk.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zwaojipl.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2kpstopxv.html


<!-- 参考信息 -->