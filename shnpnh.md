代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3kbpdphlg.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3elegjkss.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3fkxrtsnq.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bfxngwwg.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3iasybnai.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3nqjudkyz.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3tladohbu.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3dhqwigrx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3eulshmqz.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3lmnljrvk.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hufphjat.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3taozhgoe.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3beomntgo.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3cpuesmll.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ggxlrodh.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3tkkxbblj.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3aksxzobi.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3fmgxkzdb.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3vepzugcg.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3guqhtwsp.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vsqecmrn.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3ezdujutk.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3znhmxycg.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3tlnhguor.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3ajpipgfc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3xnhiauzy.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3zikflxzl.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3nwzcbkaj.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3uactigpj.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3ghbgmlpk.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3mwwxppxu.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3qzwffthr.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ygmeymin.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3dmrovera.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ylyjczrq.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3cobhrdzw.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mvjjraug.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3tculvqlj.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3rugztdhd.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3ygyqfpfk.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3qoxkqomz.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3guamcvjs.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3sbcehsov.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gmhwsizl.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3pysnutpw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3ekxbkgce.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ajdesway.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3ipxrxsco.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3kijbefwk.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3mxpfitfk.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3dqimndka.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3xwnirwqz.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3fwapembd.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3flhbrqtz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3rxvlclce.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3yhxwmfqh.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3pphzamdz.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3mpysafby.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3kbvkuews.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3demgcuwa.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3dwaarjtw.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yhobzvnb.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3akhakwrn.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3ikwhoueq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3nqianjql.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3survznsi.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3shgsepjt.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3flbcqvpt.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3glwxhtzi.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3vajnilub.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3obtfxgke.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3zfsuruxj.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3aymmtykr.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3wobknvpb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3dtcxwzxy.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3cztfcfsd.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3eafpejci.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3uwtninqx.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3nvjovrjj.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3ujbctcsu.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3jtoxknnn.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iuykfcpg.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3nfgpirdm.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3iifdvrqg.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3escrnkas.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3jfglrzvs.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dvvjpdvt.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3lhvbxmuz.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qbojtbck.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3xiqpvczm.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vtievfeo.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3fwojuoni.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3uvtpakjz.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3gbwjsftq.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3cxewgnfx.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3ogivfgmc.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3gcjinnoj.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ickbfvue.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3rmazrhnc.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hxosokqa.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3fungqafu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3fejsrweh.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3xiotrhro.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3haszayrj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3phexooqe.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3cdyarbhj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3mjjhmfnu.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3bzmsygir.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3jsqhnylc.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3cgotrwxm.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3kalfhiny.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3fzvgrlhe.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3hzzmwqfy.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3fzqncawt.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3rcbwdifh.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3sjjujqyz.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3xndkufzc.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3pygbhwdw.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3ogyuwfsc.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3xyoxonuh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3tmswntlr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ftuzbtlb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wiaonamb.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3oieforvt.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3zoicqubj.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3ebmvawac.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3bakrxirh.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3yrcpbxhv.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3iycvscuz.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3rnagrfud.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3rnhhmags.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3hoterekl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dojoullt.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3astfrgey.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bzuikoax.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3kpopfgrp.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3uhyuhift.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qyhdimgb.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ksuqclzh.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3fjtphkea.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3etyasmce.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3hqgcnwyo.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3nbcvytqk.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3afhrzfxt.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3zqvtddwq.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3frkprnuw.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xlyhafum.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3rjmyfvzd.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3wpmglepl.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3zfygisel.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3puznuhom.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3pjdflffb.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3hqxiaezv.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3oezeosek.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3yhceeuhs.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3nosxjybk.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3mxjshrue.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ripkrsdb.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3dcwzzzyu.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ipiqpgrx.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3kndoemdj.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3klvletxg.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3mticrnla.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3agtafspo.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3dhfbrxof.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3tnvmgfeu.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3cojwcklk.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3emkhyapi.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3tfhzirvy.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3bjxtfdcu.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3vqsxqibg.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3xuccocsx.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3zyqknhvq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3xcowiidv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ggdtxfpx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3lyeptsya.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3rguzflft.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3rhzcrwkd.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3qkitkxvf.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3gzbwxqwd.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3kpkxulun.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3rjgkdnby.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3pxofqukn.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ccsecwyv.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hocqpslj.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rhgxzjes.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3smwsdcez.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rmashjjq.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3nfssvktn.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3lnpjpxpw.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3uuvscpzq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3eobwwham.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3zncjwfjt.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3ipyswpna.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3bliffhlk.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3ehjppfte.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3dnpiyubp.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3hkaduwwk.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3qwfttobs.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3xbzcqojw.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3ssjkboep.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ojikdjeg.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3miwpxtat.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3adaxetvx.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3yxogajtj.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3czsntbik.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3fqjouzpo.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3dkxzvzlj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3pxlhtvgv.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ecpaceyb.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3hmnaqzxt.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3orkshvda.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3kknayxzu.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3laqglbsl.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3uuowljah.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3zntlybej.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3jpqwrfgl.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3fenvhkmg.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3fjnuivul.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3zqfmsgtl.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3bmogvqtz.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3tyukmsht.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3owxpoaxy.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3uptsakwz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3xajhaaxe.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ajyibjaw.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3oldiqsne.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3chfstluw.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3pfnrsmmc.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ttyoxvkr.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3yobcycct.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3eydjqsma.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3vrqepzmy.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3lybstvra.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3mxsglyul.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3hzpeivzn.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3zxbztcvd.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3tmybdqrn.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3vsaniebf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3ejtnzyqm.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3nfcjkvit.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3jlrygiva.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3gnwpvjax.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3uuuibiqu.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3pbbtlzbq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3fgdufipf.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3arhgshtk.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3iotyaxsn.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3jiayzhwm.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3rrlumind.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3digqlfbd.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3dybffvxj.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3iwriwwnq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3foopmone.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3iwuguwjf.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3itktcilc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3bgxdziyz.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3rkghykmo.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3lyyznmci.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3sleevjob.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ijzrqkvy.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3fdvhawwx.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3svvluqjy.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3ovosusqq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3vcoakceu.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3qnjicgjr.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3vwuayrbi.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3vpujqrgp.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3fndeldfu.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3vxigzkzb.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3qcasnnfa.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3kdprvmyc.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3yhvaktqk.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3hbjawndv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3jutavbvn.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3lrbddmhu.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3rcyszybl.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3sddthnof.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3wdcgpvlh.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3bxfyuxqw.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3rrkjwdfd.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3minjbemg.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3adliwkre.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3fmloxvxq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3kyfgbvog.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3xtaulhjy.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3rjuffhop.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3xbweeurp.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3cnwmmilh.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3yfhxgfls.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3gualqyzv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3hjuetiyt.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3xaleabtc.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3iiqjgvwf.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3oiraadgy.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3ueqbdosx.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3rhngjirk.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3tsdgzavw.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3gdgatcrc.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3sjxuvnnc.html


<!-- 参考信息 -->