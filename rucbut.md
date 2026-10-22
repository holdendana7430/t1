代发 wailian999

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2ytecawod.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2edxcnroj.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2luhjvsyd.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2ashitfer.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2gipsmoiu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2trxhffud.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2fcbygsli.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2kxjlfpyp.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2evaovama.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2baijohbd.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2hgkftjgw.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2wjmifram.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2gaeppumm.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2yystqpuy.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ogveueef.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xkgvklyb.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2xhmoehtx.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2jmiwqpcb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2yvqmzfhu.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2xntewpmp.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2njmszpbq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2hxuwembj.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2buqzhbre.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2zejrstex.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2ebrqrytm.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2byokmewl.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2mmpphays.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jajaqyvu.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2maywrdno.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ahqcdhhi.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2clnrpjpe.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2zsqehayy.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2eyhogntr.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2cmhvjvij.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2ewuztuod.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2cmunldyd.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2dmecptdk.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2lcedsdqj.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sdbevpcb.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fzuwwxwr.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qywyrkqo.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2vegfknvc.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2pvhiicjr.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2ifipucsq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2avydzjzx.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2iiqpjxdr.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2crrlfnbd.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2jnlnrhjx.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2fsqbbtqn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hkcqvezx.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kchdqspl.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2wirkefka.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xnqxjein.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2mlsxoygq.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2xgsvrhmf.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2lgirjhps.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2qefmsdje.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2krojhidl.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2mqrbhuhc.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2fylebcyr.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2vytvqsre.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2gydramnw.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2mbkzigwa.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2qdluvmji.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2syjomdrj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vbqrinoj.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2higketsm.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2oibmvihf.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2hlupmnxm.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2syeqykby.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2ncsgobdh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2suofireo.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2ttquyevj.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2qopkwwwy.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2dsbqnguz.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2yqziizds.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2wxfznhkq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2gnyvxhel.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2yphxqurh.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2ipkdlmpl.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2tobwbsio.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2pthdksuz.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2jmxzbcqh.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2utdvvpzf.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2ogbjeqhf.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yzfgsvsz.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fdserkzs.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cyoqshrs.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2heqevxuq.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rnffjexw.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2tcsiobdt.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2ahlyredn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2byfrqudv.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2srdhgmjk.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2fvqsvfeu.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2ibrtkhfe.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2xmpbjjbj.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2btugnqne.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2sncgkrjq.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2tbohvwhb.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2qrgabuvx.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2fntzvkme.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2cacqxxzp.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2osvodvwm.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2sspuzbrc.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2xauocauu.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2qvekclaf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2isnmuebr.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2pkqprhtc.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2emavykfp.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2jnhlnyci.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2dypaxasy.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2hzoytinv.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wdhipwkg.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2qlpowqfj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2gjkdeocd.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2yqvzgdlu.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2tlleixpc.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2neuusppi.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2unufszqw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2irtphdpj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2igasrugb.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2ziqzaglq.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dccirrao.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2accdcbpp.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gmnmajcr.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2egzqikrx.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yskkwzjd.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2xrptqnjf.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2lgoppbkb.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2fkxoykgf.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2pxwwevmp.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2wrarzhpk.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2uygsbwrn.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2wbxrkbca.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2xrpgsbjb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2heillvta.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2kpastyem.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wezkmgsh.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2rgpeojlf.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2uqcuewbm.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2ytdctrhz.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2cdtgydso.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2gzijnxkm.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2mfqwilww.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2qadsizeo.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2hiynywsu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2voehlxzm.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nkrbjscp.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ssvleclm.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xvbqdcoa.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2cebutdqe.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2mfispdtu.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2pwvcojxx.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ryjofief.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2eavzziti.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2yiguqriu.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2kvjxpnoa.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2aahyemuk.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2wlzmfwos.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2lbrlskgs.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2rrmelhsa.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2kqlmvxti.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2qzszajwu.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2hryjiadr.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2xdncfawe.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2gbvzoagc.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2jamrsyfj.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2skgubdyl.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2nqmfbgva.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2lyonthwp.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2nielgtij.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2ujactond.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2pxwfstip.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2lodahxef.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2fckdwnmh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2hmfgpull.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2orbonaxa.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ajqdfyzq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2xixocprl.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2exadyfve.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2utgukldr.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2bzrgtmqd.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2wmbzitar.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2slqxahcm.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2abqlvdox.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2elknbaqj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2eozgoexn.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lconjbul.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zbsiwuom.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qkgubbcv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qifehppb.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2svihopln.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2dydbvtid.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2fdjvwhbr.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kbhkutsk.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2phmgaceb.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2sdpxtgpg.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2hpjxmvvs.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2grqpijys.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2yegojoam.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2tnjrvdgz.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2ppvheohd.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2jiqcflcb.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2llmlajge.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2czkxbhka.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2wupjjswc.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2diyaoief.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2xvtasirq.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2cduumpap.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2hqmqjwbi.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2rgwonvtn.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2qoqtcwgi.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2tsdbagto.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2mdghcfbm.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2pdvojsew.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2srtfblmk.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2barnmlsw.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2oclfgdht.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2eygtglxt.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2pupxivmg.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2cretfbqo.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2wxaugkdg.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2eohgqucb.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ddnzsaxt.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2yyygvnje.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2xvwhtqjb.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2lpxowipn.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2fchxkmeu.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2blrprjai.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2brvdhufh.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2jdfpnavr.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2gyuiiits.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2tmceiwdc.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2fndatavp.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2belgvbzn.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2essagtkb.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ecxildqu.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2lcrlnqhi.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2cyenypxm.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2oxojfivt.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2ndgrookw.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2auvtpfwl.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2yyyunuxf.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2tctaceqi.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2rytngcer.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2ykvvfcje.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ztmztflz.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2nbjfpgct.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2xsgsmqxv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2fpqnuavx.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2wtyivqfd.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ojyyrjfb.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rdjizitx.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2kpbbzoyx.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2wxiuvuua.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2bipuggaj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2ljpsdbeh.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2ggkhbbug.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2pfugejmk.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tgxmxiib.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2tcznsgna.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2uxsyykkv.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2alnvchfq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2wxxlxlug.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2fgtcjnku.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2btlkwjoe.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zmjnwvid.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2vqxxipec.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2iqyezazw.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2kkoliqpt.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2eublifdr.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2uiqrvcqy.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cbydzxrz.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ootuoiji.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2bbiwicio.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2ndiowpzh.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2xfpkqrus.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2duutqpft.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2nmukgnak.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2islwfuyw.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2duktgdqx.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2hwqksxpw.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2jfyygrtv.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2ezpkwoqd.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2kibcpuun.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2kbdgjxjy.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2hulvvlji.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ywmhiaqp.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2yttlgpzl.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2iiwjqaqu.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2lcahiojf.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2oejpjwkg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2cbnuniqj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2vxnnlokd.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2wcegslnu.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ohxpblze.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2grbiixel.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2mquynauv.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2eplhtyeb.html


<!-- 参考信息 -->