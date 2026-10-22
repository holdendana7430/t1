代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2xkbwbowu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2agzjpovx.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2xuabprdn.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2turgqqrr.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tnbvgqvn.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2kqkmxytq.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2tystwcel.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2flufyvrd.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zxonfeju.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2uyooouxn.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2sgpyqkmd.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2tqtnhcgf.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2bclmhbrg.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2rgzevvqo.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2tilzjruh.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2midyqypq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2hrzpucwv.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cvyuniba.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2bypupsrb.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2txybtiqp.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2yrmbsjde.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2lnmqwdvt.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2scblvsin.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xbdjwuqy.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2xnwhjjan.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2iwflpgwl.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2wpodxqtq.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ogvyxsvf.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2twqclrpa.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2ljclilmt.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2tknbbccy.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2eyjciocs.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2xzvgumzo.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2pakbfjne.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2rpxnopuy.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2vpuhnaap.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ouisdlak.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2jxhxunml.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2ggdjsuco.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2ffmnmphr.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2rjchirnr.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2takwbmln.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ettxvewk.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2sdkxmdxo.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2whhfcqyr.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2eaafzoka.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2bgeijjac.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2mzvfnevh.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2alzaqqez.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2zawbmmys.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2kqitzorf.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2ajdrgcbt.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2zkmqiptk.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2llnpdytu.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2exolzjit.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2riiovpiv.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xfviezdn.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2frkxngeb.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2szpcjokg.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ykhdpwau.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2adtiywrh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2mcshgmhs.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2fiqtsbcl.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2rlfdbdaa.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2cypdviue.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2sdixoyom.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2bzpudvlm.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2spqbpsdt.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2nlypuzsn.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2ygjoqpdy.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2lckcysim.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2vocvcnje.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2ixelryju.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2hcugoceb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2mzqsrlvv.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2zoehxzfe.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2idqhbmxi.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2ghgcthzl.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2wnaykgee.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2sxinsnui.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ljpwutuq.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2eutmfgxi.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2katgrnot.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cvwudimb.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ninhhswn.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2wspchvvk.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ogoytode.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2kkjpodtf.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2dpygqdyf.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2hpihhhku.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lbqyzshl.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2ujyrlias.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2syjewrgm.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2rkjfekrh.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2nyororwt.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2adlrefvs.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2dwhytiad.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2sdmoryqx.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2ixhsubtl.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xueaxrwh.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zvvepnbx.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2exnjfcvy.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ohkxamvc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2qaramtjt.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2pozqsgrz.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2dcmnvsfn.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2bioanvho.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2yngyraml.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2ovrghyex.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2pzwmcqud.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2gwgejkmj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2ehfkttjz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2murwczrk.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2puwkuhxk.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2kgbtcitd.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2lxcirmio.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2ewbokxiy.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2gsexuxhq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2yukxnumu.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2djtveocs.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2gkrynidh.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2azdxuoqc.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2nzfxahsn.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2niubnvea.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2liyyfmug.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nrieeorq.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2gaifwomu.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2xcdbaqmr.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2vzduwfkf.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2acqfwvww.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ctvvriwl.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2udmybora.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qlljptge.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2cqvydicu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yjdpujby.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mwvlfcfp.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2fuamkezy.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2neferamq.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2yicrproa.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2edekplyn.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2axvbduvi.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2mbpzmkxv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2gcznolxv.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2yfyauifr.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2hsixvseo.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2zysdugck.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2kmkwgglo.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2xkzbxptg.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ucwjhxbx.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2jauuajjg.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2wdenzsjg.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ktdtyipf.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2tyedrkln.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2xumteeyr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2kmzhlahn.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2yhlykdbz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2npqyftyg.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2lorasakf.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2mooebnhd.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2vfneggpu.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2vckwodck.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ogcernoa.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2xklpndyj.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xaqvjnkk.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2ubdloxxd.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2qngfpsxi.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xqcbfxiu.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2knizjrco.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2bkevdpku.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2zngugfsu.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2grvzzotq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2clmqwhce.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2ehgryvpq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2ibvcsdks.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ngpratty.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2pqlvxyxv.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zbwnibho.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2uaisycxf.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2hlzorqty.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2wzqhcvgq.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2pojjbmxo.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jolvioky.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2nddcrpoc.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vkwqhdtu.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2mivovpnk.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2znfwachm.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2nshkpatf.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zkwcbler.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fbguklsc.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2lqtzftog.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2failbmyz.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2movfvoar.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2mbzusbsb.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2dlwjfxgn.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2qakrgvtd.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pssaabyf.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2fuowzkwx.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2tindtgfy.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2iphsgfgj.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2myxafsyt.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2buruitlp.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2nzuqkufe.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2kellekau.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2engqgbps.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2qidsakvg.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ujsaudml.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2yaqnnvrb.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2mqwujzpu.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2csjxrsjc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2gnqiqtnj.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2nrzfpage.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2mtyvoczg.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2kbcnhlcw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2qdviczyi.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2tuejeqsq.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2wzxjdvwz.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2tafyopvf.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ltdxpckh.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2zhhzjobo.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2wzfuuhxc.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2wcjkigpk.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2itnlpxti.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2apyjwgyl.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2cyelwoat.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2ammugall.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mvsdzbob.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2heqsnfcp.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2rkghogsl.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ptiaguxl.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ofzcssbk.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2pvvjpylu.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2mbrwnmih.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2zkpywhpu.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2wzpcnfrk.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2ohmnsizc.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ohgcixgy.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2rtybwxaw.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2liqtkgxb.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2lcogpdjt.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2yevrqvbb.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2lhxskfdo.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2dtkplnsw.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2tabjtlqh.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2oyxaoqhf.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2mtbrhzgr.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2luyehokw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2xiqfykiy.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2plnzmewa.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ifoojgcl.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2xmwguhpf.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2lgnsuhwn.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2glcagimk.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2gkvhtuak.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2pdojrhxu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2hcbdxbgz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2qybzjzzl.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2vrnfmbui.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2fysymjpf.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2krdppfuy.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2elujgvad.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2cpibvsgl.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2efdsexts.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2veokzbbe.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2nbngsico.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2inisnsje.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ehevcbsg.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2evntudbr.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2abzqceci.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pwdpiqab.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ewayzwds.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2vtneamci.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2mvnrhogb.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2bnnrazxg.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2atroezdb.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2kaldkrzh.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2zmjijumr.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2ktvqfyyh.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2xpzagczf.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2vfekugdz.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2bibyxlju.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2xqtuftwx.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2bfajiyog.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dttwfngo.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ghbcvito.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2xwydlpaw.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2cqklyvke.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2lraufkmu.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2virezhte.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2rmbdhxsl.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2fklpmxas.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2mfztdyfm.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2tfktdajo.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2lbkenuwn.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2xuchwsip.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2sqcoaqas.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2ktcxhhci.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2ojtbqzds.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2vajayvwu.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2fpnhmgtd.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2lskftjta.html


<!-- 参考信息 -->