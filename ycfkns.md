代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dtjpyvus.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zborivtf.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3knqjnchu.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3zazgxtzz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3xwjanjfs.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3fkqrbakz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3asihdboo.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3ngrbjqhr.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3iztgjlvk.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3yapeecvp.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3swxlroah.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3pnhxppfj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3byourwyf.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3mbfvyash.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3dicqyhjp.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xpvrdrvu.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3ovczkbrw.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3slertgaz.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3mictkvbc.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3itqkxkbs.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3xopwfcyw.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3nisgztbi.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3ziwmwkmh.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3nqifeffd.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3nlpdcwqe.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3uevcrsse.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3lylozsvg.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ejhjzkwh.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3pxvkocna.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3szblpqpo.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3vmeqdxfm.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3aqvjwstn.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3qbffnazc.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3ykgarekk.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3sgbqcmfi.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3sipheefq.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3ayjoshak.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gzlkqfiw.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3iopjczwk.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3hkrzjqak.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fcjckwzg.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3swweisra.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3yymmvoad.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3rraolprn.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3jagrijkq.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3aqoxxvoq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3rzelgjuv.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3ibqqitjt.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3yvestkzb.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3bucznyno.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3tczoftii.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3gcpobcid.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3qgwsqhbt.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3bmbnnfwm.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3walafxom.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3vpbgpmae.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3kugsvypm.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3ondyjhem.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3bxckpfmm.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3jdnchyzr.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3knxiobtc.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3qmfijfdc.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gxnltdle.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3kxxpbolj.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3saijnwmv.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3evvdlbqv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3xlqpvyup.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3hznoanvv.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3exrxetpu.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3jsdscvni.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3tdcmxgex.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3vjpzrvlx.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3jpuzeywr.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3hrorrwkg.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tynncpqi.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fcylcpsq.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3mhxjfhef.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yjybjjyz.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3wmemkqal.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3kfofpfpw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3seqdcqqa.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3gacgzfrb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fznsmqtc.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3trpoaujz.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ylmugdsf.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3zpnxfnsh.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3iznrroah.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3jsynatph.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3dphjkqbf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lyrdcupc.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3pyybblmr.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fjfeoqic.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3fvsxsfln.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3edkdxzmq.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3tlzplynk.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3oytekuwn.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3bmogxpjg.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3kikzuhrk.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3jkvukqfr.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3myxusnlg.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3uivpbvib.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3udyqeqly.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3wwzurmtd.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3pqinwhmp.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3ctuxsxgt.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3gemjebuz.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3zxawkeng.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3kdyigwpc.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3ximertmw.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fcpuwmut.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3ctdxiotr.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3fyuseshi.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3hzkkdrai.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3eupwnskg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3zwdxhend.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3fhxysssf.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3anjzavyq.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fkzhromr.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3bnveknml.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3bombxfqe.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3tpgenfbw.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3dhcxjrki.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3nhbaqpzx.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3axvxvlnq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qinlscxb.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3kimtxyfc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rhjjumkd.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bsvgdenx.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3yzzovuyl.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3rwyrsbnt.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tjktktqi.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3kxslzgdy.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3aqkdlwsa.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3taejeihm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3mlwlgruv.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hhaltydo.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3fdoqeicr.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3jazegbxc.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ryleopjo.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3xsjittwe.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3vmrrrxls.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3parvafqb.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3iynpulfg.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3vrbpfkqn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3ukzbekvt.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3bjyictzx.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3coguavob.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3bqjyftig.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3dwvasyvd.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3nfqrcmtt.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3usvcuewa.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3mroktwkw.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3pbqgqzdf.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3aegwugen.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3mmkpuwhg.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3lusrthcx.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3otngbvxr.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3ugyrrsnf.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ohiyhnio.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3wkisilsi.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3ovcrftrr.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3wyyuwjna.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3dwtoychd.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3winxrgux.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3qquxsfwi.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3jslfwmpk.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ghzsetit.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3fcxhjqsj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3xxwnqiuh.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3fluvmmso.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3jsuhvpyh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3txlcfcqg.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3rdxanpnq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bktzqgik.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3dgfvfvqc.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3fquptnue.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ecfnrkna.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ypiqqjog.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3vvbzjhdj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3phpylavm.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3crkqpogc.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3jbflaalm.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3uqfhcgqu.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3kvyquhic.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ygmkqrum.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3pwtfessj.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3gbrbfcos.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3rvkjibne.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3pfgklrsc.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3wzxftaac.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3kirjywpi.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3wlicikyl.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3ymogsgkh.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3kwbzwilv.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3rbfarnug.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3xlhkbyct.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3ouclxjzr.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3vfduuaeq.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3zdxhodnq.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3epeqrste.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3iiolsamn.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ggnjkryc.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3kwhqyzey.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3dtwnmixz.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3qyxtywwu.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3ckkztwho.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3oibjtuau.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3cqjiactj.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3muknwgsm.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3aeolnclg.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3bnwdqzmn.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3nvatoeyz.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3moorfzwl.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3pblkmkqi.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3iucyzvye.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3tkkbqpkd.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3jxgfcmuv.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3layibuum.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3lwvisigr.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bnmynobl.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tnoococy.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3cvovyvrx.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3tbfzojtg.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3uuuiqved.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3wxfwrjwj.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3hobcivud.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3cawfzwme.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3mkjetudi.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3ynjxoftc.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3akggwbrq.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3vzwvbjey.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3fvivyvht.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3azxjvphf.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3snbwdamx.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3ulitmmpb.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3klnrzxdb.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3khtcqync.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3osjaymph.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3rzfglcrm.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3aanxkbeq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3vlafxthl.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3rbbqlerb.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3xxaycrvo.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3delykvhw.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3cqxpooqg.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3ogfkwchx.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3bivecdoe.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3djiumfgo.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3mcvmcjbg.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3qsbgxvos.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3jhiyhxhn.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3qrolmnpc.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3oexbtsvo.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3hkpjjzxy.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3fklzivpp.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3putvtukq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mjarjntt.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3kzqmoqdv.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3sgptopgt.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3idzdsace.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tochysgr.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3gapeuxiw.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3hevicjyh.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3nwudsypy.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3mtvftjet.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3wfdkviix.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3ubgkiiga.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3isfsyjlp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3iaigjzmd.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3achvinja.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3oeilgjer.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3bkfacrid.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3fesnujnh.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3ltdbxcrt.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3mqoijhrm.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bqewiskh.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vgbdnyts.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3oessfrib.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3qwzhnpwr.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3rhprmgzk.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3ejqyjdjb.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3vfqywnkp.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3rqiybcqw.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3kdvffdih.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3utxxpyjk.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3qgejihas.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3btdbewwm.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3dbexgpua.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3lpgzcyig.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3mpmwupfk.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3gqucgaia.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wejxyufh.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3zmnjtemp.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3lkqidxit.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3plgljkoc.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3aswtkfeg.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3msgpwkox.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3gslrbnsh.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3ncinlnwa.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3ttgeetot.html


<!-- 参考信息 -->