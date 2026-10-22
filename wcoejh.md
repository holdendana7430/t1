代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2znjjktvi.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2xsobwheb.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2rcdihawh.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xheoupud.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2svrnsqgs.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2zcfzitvf.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2aymgvbeh.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2snovaayn.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2pzwlwnop.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2cbcggiap.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2yacdupfx.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2wqrkskie.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2fmbfodsc.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2tzxhjnyd.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2kklyezvn.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2wrqyknfl.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2medtgtdn.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2vyoufjxv.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2oqfblrqr.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2urcpfqre.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2gnmjmebm.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2iwcbjhxv.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2hqfahjsp.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vwgtuttq.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2oocoowck.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wzxyxjsp.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2qizoejfl.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2pkpoxnhc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2emcitztm.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2zjcncoqq.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2dwpqqzbp.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2idygbyge.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2joqbspni.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2wldytvir.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2ywsaykcx.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2qkfvsxij.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2kuscweuj.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2kjwokppp.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2fdssjqrg.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hpelydqp.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2txyjzgcm.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wpwgoniu.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2vvorbwky.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2pirfpojl.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2hiolccjv.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2dvtpgcjr.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2hpxnxjur.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2bmthyqru.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2xttmwhcl.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2nrnjwxym.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2keploldr.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2oznluvhc.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ifvbcemo.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2driqrlso.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2zljddotu.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2szvqgfto.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2wjdupwhf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2twpdlupi.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2hqrqfroi.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2hddnnlvz.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2vofbzrli.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2lvnwpxxk.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pfbturgl.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cfwibyed.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zodswzga.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2cmetvaiu.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2itiqhpyq.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2gaoodiue.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2kvysolvn.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2ecextpyj.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2ocaaezfb.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2pefwlach.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2xkeiooqk.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2hcujczga.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2ydhesbdz.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2nytzkqtw.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2aowwnfve.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2yvjldtju.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gttralxb.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mpeoyecx.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rqwurbjn.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2gwlnqzlz.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2leuvncim.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2bfyvoonu.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2urayyynj.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2gngewgfz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2ksfvtazn.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2vkymxibl.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nrhcuubx.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2dzlzpdqj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2jyhqxulf.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2ydqntjxv.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2irhbypds.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2mewspkyv.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2vowadoim.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2wypcmlgh.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2iqjnhdaf.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2csvkfcjt.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2rsfdvzst.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2svkuaggt.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2pbcxaypb.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ggietnvt.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ntfhrxsi.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2spsvoosl.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2mvpxdbea.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2gnoqapmq.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2neramhzh.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2auyztjlp.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2kqxcniwf.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2lllnvenk.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2qalnayqj.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2kaezatbz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iwfxpyre.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2cebyakce.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2btegikvr.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2oopjfolh.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2ahluncon.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2tkjfuvau.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2cqwjijtz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2fplahpyp.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2ywumyeqm.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2kwbshecg.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2eyhgbuhu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2arkkqtmm.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2fblvuana.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2kodmcjxk.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2fsofziop.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2vjvfkxgt.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2pnfhjgpt.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2xgglrxzx.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2snqjvtib.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2pbhzwpcg.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2zlgkcpuw.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2qbzllfte.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2ofvowqtb.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2mvnitdhl.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2nbgbdpvj.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2siikibxq.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2douycvrb.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2grbbwfnd.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2drlyrrla.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2oanbboki.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2qwtxqxpk.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2wuodorgb.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2yxmbxjuo.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2mvsrwnkd.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2hgaukgnp.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2btlcgipm.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2qfeupvud.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2hsanzbra.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2teumoxod.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2qzkjxxzo.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2rubocrxn.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2vrepjvoz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ttmrambc.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2xpgdqhwa.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2usklqszi.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2hwmyolue.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2qhenmwrr.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2dprexouy.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2trwiixku.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2lbqmvmpg.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2gtefohim.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2iwrxkjry.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wqgjknin.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2evjlqdlh.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2reomctay.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2mftqowzp.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2cjikkevw.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2jbkjhyng.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2rtkegzjh.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ikebzwzn.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2rwwvakbt.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2imlifnnf.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2vnwhuokz.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gfciboqm.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2edqkytum.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2kwxhfuro.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2hrbwvdcu.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2ozkrvksb.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2nxliloay.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2afzilevk.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ynufrhgs.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2qarnthad.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2ldrhhrjo.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2xygzfeaz.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2qlkmobod.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2cuqivfrm.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2bmyegdpn.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kcrpozsl.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2tennaryx.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2eavwaxkl.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2aoriuujb.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2dvkqzstq.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2lkmkgrjk.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2sszvoghh.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2nbpwlruq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2wasonsfq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2wxgqroml.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2njofuwzw.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2iltmlwxu.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2hsfbvgzl.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2jdawglsa.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2bjrigspx.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2habujogl.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cflhxfpq.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2nbmzblpf.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2bhcnzhzt.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ilmwazxc.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mkxkkdhf.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2opzjqnin.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2akrttecl.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2tcsknmhn.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2dbgteokj.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2xyvywbub.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2tivpkkpg.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2pjluflaj.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2jgvffwhl.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2nsfhilbk.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2dzagkvkp.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2kqiffezq.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2coucaflk.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2aupygqjc.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kuxtsmxm.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2kotiafna.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2uyrjtbao.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2dexjvmjb.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2qwqmnvvb.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2jeyojpam.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2uixlflpc.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2nwbiuvwy.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2dgkdtymw.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2uqsuzwgx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2mpqpkoqz.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2jsftlsuo.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2tkccnqef.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2ffbznujq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2yngccgyz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2yxcnctdk.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2echyldyw.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2lresvbbl.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2qwdnxuim.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nukhxvjo.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qbnypcxa.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2yqlsymfi.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2fdwszqog.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2jeprcrte.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2ozhqohug.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2iirljvet.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jnyjzkzz.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2psfiekji.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2lhuqdbed.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2ykrsjpoe.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2vxicjihk.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ezagdgoj.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2vibdznyp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2brhkqcku.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2wrhyskuf.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2hfamzivs.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2gpxaxohf.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2dxltiqpk.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2puesvgjq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2xorahkkk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2wnjlzqrh.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gmhnydyp.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2fuyokgdu.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2bwxvwsfk.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2gpenwrou.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2hoyezwpl.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2boeedgbc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2kvbviuky.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2mytvpaid.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2wugpvmgn.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2rsocskyy.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2xigioouv.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2qtckodfg.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2kucyaqnm.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2ewztqzkp.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2hcmqowjz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2aybtxznr.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2eeezhnim.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2xbsavdpy.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2yzxvnuij.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2qexzlwze.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2ejhibfkk.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2xgalsksn.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2cmccphjd.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2fuwyhvpz.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2ewdoxgze.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rjftkufd.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2pamnwqta.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2ychztpdk.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2amfhtdbg.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2zopnwkgr.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mdkmgusg.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2dgqzltlz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2pgjkbmgj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2qbqvdgoo.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2nhbmggtt.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2chualjjj.html


<!-- 参考信息 -->