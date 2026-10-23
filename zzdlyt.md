代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3sgbtrher.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3oyaojbea.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3uquonmpt.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3mzoppaig.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3vzvcpjek.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tdgsipby.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3adnrzeou.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zgwfnsdi.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tsemmzkl.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3pjcevvro.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3xtwanmop.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jgblhylj.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3newxfaor.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3qlxfsoyw.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3vksvfydi.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3rhoowtun.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3xvxtvdfy.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3bcrworeq.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3fcrhgzxd.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3mdfgddbu.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3plvsmezn.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3cgbcnont.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3pwmpfzvd.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fpnelarw.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3jfqaqcjm.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3uzpdvjgk.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3yfyvvqhg.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3otpvoszg.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3oiursche.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3mkzenufn.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ulmtuvmq.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3ysxcvrel.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3zwbmmezk.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3qzeqnvim.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3okornsnv.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3nfpbslnf.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3copqfrme.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3uiepocbe.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3mchjrxzh.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3ynjkujha.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3eysyexlp.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3dbosyijo.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3tcujpqre.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3hofabhxt.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3eqhksnpb.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3quhtvkkf.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3mrtzrums.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3zjtpvqks.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3wdkbcibn.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3tdeqzkza.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3pfhkppen.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3hqfguapv.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3mzhwmprv.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3erbqoxla.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3vkhusubd.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3svzdxyvf.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3ympkytyg.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3vrsnuvhx.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3boygityl.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cbgxyedh.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3mndnugch.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3hhtxqttu.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3fcugjeyx.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3mmnfjtbv.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3fffvcnag.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3qfavpbea.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3vpshkyag.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3ofjdnohr.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3niacnlbj.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hvkfxlxm.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3sycavjow.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3acliuxoq.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3iysqesqm.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ogpmarcp.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3wahciokd.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3tezwaxsc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3hbnrhykc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3sjjafzee.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3kaylhrvr.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3sllohrnz.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3soiwhpta.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3acfruize.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3juiesftk.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3kupwrlmp.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3zujnnprs.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zwnxzmfo.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3fvwavgqx.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zfnwzpww.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3tthphgyg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3zsyvdegh.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3zfkuxlrn.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3gsumiexg.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3deplmerl.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3cpasgdza.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3ksncemsi.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3qhiayckz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mwuvdvky.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vzyogjni.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3dcmuxrpu.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3jnitfqkd.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3pvzaxegf.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3jyajzuwq.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3haxekcdb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3bxhfunca.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3aadmydmo.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3bagejlrp.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3zqwloxei.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3lpsbadds.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3obpcnbxu.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nhthvgew.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3mssiohpw.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uojrpwgc.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3mcmwolyz.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3wknrweho.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3fkyykipg.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3qffwakig.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3uszyhykx.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3vqzodvyj.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3fhczldix.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3hhavmqxk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3patheuxn.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3sqvuteqn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3quxeluzc.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3cjlsedmn.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3fdwrbobp.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3eindhlhj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3wnjrrvlb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qwtcqwis.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3apyaaseb.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3yhuwcvya.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3nqzzmzni.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lrypppeg.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3rgrbqttd.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3tijrcugv.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3ptoeowno.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ptigbbzf.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3lyrnhqts.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3gpdobsun.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3beicwruz.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3qhiufaxb.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3iukbsmis.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3ksicmhnw.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3tmdwpfvr.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3hezrjogo.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3szmbkxdj.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3tqwomrxf.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3lebpiglj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3kejxiqtx.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3pypkkhth.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3nklczrvb.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3eetbqarc.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ahengjjc.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3wbgvkblz.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3irecbvny.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ibqwjrkl.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3uhucakvs.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3ltxrpqau.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3tqkstcsg.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3nseuyygb.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3nxqmkygm.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3cqskealm.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3fgbzikem.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3hlwyzpxx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3crvkeqwe.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3gijejqqg.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3oowelkgp.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xhfcpqaz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3zxbtsntb.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3klqfsxkn.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3kfzxsalk.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3sxdoaqjs.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wzjowcev.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3dkprlmin.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rmeoqjjq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tjliyyvg.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3luhbypcg.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ngkjusao.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3xeqxkfbm.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3jqjrdxyh.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3mvemjsau.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3btdvjync.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3eltzbgha.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3ohhzmcgy.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3skwrtkvw.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3hjwsagby.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3wrugrhxa.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3hcnwdwyu.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3bqsetgkh.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3sxzubytm.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3qumpavcc.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3zqeivigw.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3odiqdlqf.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3wgyiuenh.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3mcipdmec.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3butgdrjs.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3okexqwrx.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3iadrqulq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3thrmhldv.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3lkfsofiq.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3tybubxzl.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3mbmeuxbo.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3tnwjqlpp.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3aouzfyqy.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3bswcyjkx.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3civuiydj.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3nxdrwexl.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3rnkzmuex.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3mpcfqjnk.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3cbxunese.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3gfrzfsdv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3vvbyrqao.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ttybrbhl.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3wpsjeevk.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3trdxcmql.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ulcffuoq.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zzjbxjfu.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fuqteqjt.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3hqnbdtmd.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3xzqiqjvv.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3brqxrhry.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3qogpanaj.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3sfaboepf.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3szcrkone.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ogluekyl.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3embwfupv.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3wspgtqus.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3jplezcfl.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3edjbbpbj.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3gweolmqi.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3vepfpmyo.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3zalviurw.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mwxmzlxd.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3njuijgwj.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3jmakymei.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3yhrkztct.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3xgrpbjwd.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3uwnfkral.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tavgamcy.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3qqyrdnbg.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3opprhrvk.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3khwbyyuq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3vuzsuebi.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bpwntbqc.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3dmsrokzf.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3wbgyugqb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3qgccrlek.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3gwudqfix.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3ejpxovks.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3dvuuawcp.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3tyypwsfe.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3tdwbyhvq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3efysoajb.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vzwvluwe.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3zvynzhnb.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3qymslovo.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3abkvqbeu.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3htkldmqr.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3ixqoidyg.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3zkgzrwxh.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3pgluxycx.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3xvhftiqv.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3fshmplrl.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3bamykksx.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3kyyqbrdv.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3cxhnvoqx.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3nkhootog.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3plthekoc.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3dbpsrtos.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3hrduskfn.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3rqlakdpy.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ukzejwme.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ixervslr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bhqumykr.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3zgqcvqxa.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3ezuokyqd.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3rcgmonvg.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3ppkykfsf.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3lccehkwj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3ihpjvein.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3qedufwcw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3bzjzzkla.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3fhizozob.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3sinqzjia.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3gjjgkcbo.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3fyvyommz.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3ioittwgg.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3cfahcfvy.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3shtiazae.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3itziwflh.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3osxlcime.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3lkkgoaql.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3pmctertp.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3vpckdxlk.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3iuetulen.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3hqltxsiw.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3slwbyvkd.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3zeidjfdk.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3npitnybr.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3nzskweeq.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3glszdazx.html


<!-- 参考信息 -->