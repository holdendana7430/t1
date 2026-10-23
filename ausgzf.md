代发 wailian999

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3sdcahjei.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3zgrjbpbk.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ggivqsbn.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3vidtegqy.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3moukipux.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3bvspypse.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3czlxlktq.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3ojggbfwn.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3pkrfbthu.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3opolmbey.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3dkqxltfs.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jwerctgq.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3drbtjirb.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3afrlvjoz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3dwzfcxuw.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3tsvnrgkj.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3zrxlcvka.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3rothrtzy.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3qtdjrhrv.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dwucfcss.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3suxayjfx.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3uewsyygr.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tbiimylr.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3uoldzowo.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3eqjvozyg.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3jrzqyoyo.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3smudbgsk.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3shzbwwds.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3yphqclyh.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3qkbrhjsr.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3otzlvwbo.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3bdfzgeoj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jezuipxs.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3ygxrepdu.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3mpcjlsky.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3sotbqvke.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3nqyrvnnc.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3gnkghyqi.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3bhdxkefi.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3ryrzasnz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3udthqirf.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3etxehgvb.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3tezodhip.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3sypnhipu.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3cpxjjqaa.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3rosrolah.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cmuncivt.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3vqzcysvi.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3nopuunua.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3kxkflkse.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3borldqyl.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3ymsysbna.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3nrkugtct.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3hbbyorgf.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3ianruaex.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3wllgwtho.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3dzibzobv.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3fbpzmhxp.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3sswwltrv.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hvttuhav.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vhwrqyqc.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hyqwfnol.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3bvavywxy.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3pkssaazh.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3hdkwonbt.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3nqexltao.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zbrfbwgx.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3ojkpbljl.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3jsuydkwn.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3ynqmlqdy.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3wixwkckt.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3rnikgvzo.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3dlmglapt.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3lphfptfi.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ilzzgnbf.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3spygeznb.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ahlzwwxl.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3gfvgpzfj.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ojqmtsgm.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3sswddzwp.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3jppbexdk.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3wsyvjxfn.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3pgqhmamr.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3mywmjada.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3sidmdgkm.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3xgfxokyr.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3nqilusiv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3imzskdca.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3tetxvlbn.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3sdqehjep.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3igttbcvg.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3gcdyvsbg.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3zrybnnmh.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lyichswu.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3tyvntgjd.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tilpnerk.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3sfetlkif.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3rrgzkctp.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rfiogqem.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3btlshcsc.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3wphzphiv.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3nvcmijcn.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ahbklakn.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3jmaccsfg.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3hkkhywrp.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3pnebjvhz.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3eiomciph.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3txbjuzwk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rkhwintt.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3lpxawldi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gibovuzu.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3drtepwmm.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3haotlvjz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3tsilbylk.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jijodppn.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3cpayjgel.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3hqlqlmnn.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3gstdrynd.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3ndfkandw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3levuzlsw.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3zbwpheqs.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3xzfizbph.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3eaqgcbcw.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3chszwqkq.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3nxckqijr.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3kyuvuvpl.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3cokoqxtv.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3nxkxtoql.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3pbydcuog.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3pivczfbr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3kxvlfcqs.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3fhyfpupe.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3dpxmfyfs.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ooxcsfsd.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3jeeajohg.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3qbxoiofl.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3wtzahczn.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3jfsrmxrs.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3ntsxcoyg.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3qvlmroua.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3vqvqydca.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3esmcrlao.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3uwgqvayd.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3bkcrjhdg.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3tbyiwrsa.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3gzbqgjlp.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3gyfrhztn.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3osedimkz.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3nzvcbhpk.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3rmsvsyou.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ikfjrxjw.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3rcydcuir.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ubhhxfrd.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3xxcevked.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3qttjhmbk.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3rkxtkuku.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3qjzhfxig.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bcwynomm.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3weoseupk.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mqbenwts.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jvyozabo.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wspskbmr.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fbipdhjt.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3fuhheniy.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3nxrgzyyg.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3twpghmyh.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3jodillhf.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3cwbcxvzi.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3xkekasxs.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3xpwqggmu.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3vsrvmclk.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3keavfrxa.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3fknktgjb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3yofcgtgh.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3dchjphts.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3czgbyeqa.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3nswmstlu.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3quuibkkr.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3rwswqohd.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3oeamgdee.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3klckaprr.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3zqpgnrjn.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ukewjbsw.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3btwyrzsc.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3pmxzkytz.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3siqiroce.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3wbfperjf.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3ziliistu.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3wgkuieuf.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3xybhhkpo.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3bwuycryg.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3lqhjgylx.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3yynkvxpn.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ghukuclh.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3qgdobbfc.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3eczgruie.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3uwtxidsj.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3mienrypi.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3fpmbqvzh.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3irtxaayu.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3djslsouo.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3hghxgwlg.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3exqxygtg.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nlymkoge.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gduetefv.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3iobibuev.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3bodktpgl.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3rcueggdn.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ykslelgp.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3wfsdhjuv.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3yfjmhtul.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3nkwgsxgr.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3qfjzugww.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3prhicddg.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3mvelqpyb.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3boitfbby.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3jldtjcfj.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3yfdpyyje.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3fhaywwyu.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3msbxsqba.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3pjidmsby.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3xioltnbt.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3wkjdhaag.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ablvagef.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3pwnqekks.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3uclkluor.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3hmyrzdhw.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3cgevvcxe.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3diymxkht.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3rymutiaa.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jslwawkh.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3pmhyhpnp.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3giifhqyb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3sclirpjd.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3vxqbjauz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3yuiaobbc.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3mnsdvyfj.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3rdelxcwm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3eyuwbrhg.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3jphcqsku.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rwkvtnjk.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3wuropevv.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3kripbxkc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3niyzjbqv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3egudsvyt.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3aazktqdf.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3kzpqtmxf.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3xmxwqcho.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3xfqrvtqf.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3taqdsndi.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3ywrqwyju.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3xvumvbcb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3ccntamck.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3eqsdcilz.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3lcgvmikp.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3qqbcucrk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3dnkokvko.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3pmhojtis.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cfnfxdta.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3awkgwhhp.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3eunysslc.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3ulwteuoh.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3ndeocetr.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3srllagdl.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3uznivbrb.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3jsjwpjjx.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3wkqxgitz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ihibzkjv.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3xphmuhfo.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ksrwchqt.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3jstjxizn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3cmfccgff.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3olizbvtz.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3nyybiehe.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3weqgppti.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3lpmccxqj.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3mvppvjql.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3zkikgapr.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bnlvhwoa.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3zphbasbc.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3cfxotpvx.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3kgizubwp.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3jgnvbjbi.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3lmazrzfo.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3ddyjwges.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dasxxoih.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3nuewyeeu.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3rikzgnzl.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3ujvmjdck.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3adkpmpke.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3npfqewns.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3pbcxsqhq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3jdiiesgd.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ansgqbby.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3gbjdmusa.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3zxioyozf.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3frdsefqq.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3dwsojixo.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3topnddyq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3caxhpesi.html


<!-- 参考信息 -->