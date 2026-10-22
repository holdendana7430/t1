代发 wailian999

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2qvodhpjc.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2cfhdscdu.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2mbkzkysk.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2zzdqqefo.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2mmiqjnvu.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2dahtyjjq.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2uwodmusj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mtqaumwq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2ywjbyicu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2ncfyabyv.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2egkbxvoc.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2eojhoqio.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2skrbmkqv.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2dzcywntg.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2ntlccedf.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2zhufelsj.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2odlxodiu.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ilegjzwl.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2tylhpbnd.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tuowqwiy.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2dlkysgnw.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2vuqckoad.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2rqyydhna.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2fihzucsj.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2dmyazgjf.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2mxdbsirc.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lzoachuy.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2wisnyrwg.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2uzbxwcrs.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2rzribsyg.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2tthegewt.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2cdpmvzux.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2gkesymwa.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2zzfcqjdr.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kxyavonl.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2mgoxcbwg.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2vntlhysl.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2nwhomjow.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2fgkxhxfn.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2psjzfljt.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2lhqpdjai.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2pzhcgoqe.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mnpgymea.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2hcozsalu.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2edbysvnz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2hwbsqyrp.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2yvqvhmnv.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2vmvppujn.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ixdsurrb.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2aojuufja.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2gogihwge.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ifkuvkuz.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yjrqgcla.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pvdsobop.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2sepabrvn.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2xawdlpzm.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ddpsmqqb.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2igsngdwo.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2axmzxuhf.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2fzobeopu.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2wolvbhej.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2ilgjunmw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2gpljzjtu.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2dgpomcgo.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hskcmtuw.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2zxfubilx.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2ijbuwgrz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2kozxwici.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2famqjilq.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xcavzuzp.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2wesgwdjl.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2hcpkynwp.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2uqnbmrlf.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2upnptxno.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2exizajte.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2yowjvklo.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2csjthpao.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2xtonpdhd.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2btswccue.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2idprlxjs.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2bpzhewzo.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2zrpzlrlx.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2yxcoccwr.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2jzhirfsh.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2vrvjqylg.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2eujpzxyy.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2oknojisr.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2dkbobigh.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2iydwbunl.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2onkohcll.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ankjzmsf.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2hgqybiea.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bremdfgv.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2roytghmx.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2fhecliro.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2tgkjiiuc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cvzjbrss.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2pobuuymi.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2ypdnprmo.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2pkfhblif.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2himdqycr.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2frauytto.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2ruqscrpk.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2rzbkdssu.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2vrcncnnf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hfkdlvcb.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2pfufijyt.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bsmaulfb.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nbadricv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2wgrnrhsd.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2fbbfaukk.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2fpwsompz.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2jyfetyhb.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2iksmclvn.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ojbdscfs.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2rucposph.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2oukhiixe.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2cundaqup.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2ddnawcki.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2zubcswgv.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2stosqcnv.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2meyujxtp.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2ljlmkwsd.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2yjuiudvw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2kueoeayh.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pawafssj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2kaqamdwq.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2dguqbvxm.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2mtgqezmo.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2qdmqjueb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hbbkistz.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2oioafsml.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ahvuytmd.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qvrkrjsm.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2mrcutgbv.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2cqjgehrd.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2lrdoimed.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2zawepeop.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2xenfwhzp.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2wtshoxlq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lrkepasp.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2tthtoxxd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hvzlduuy.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ebblzetj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2lsjvpiqf.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2qhdqyowj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ytypnkrw.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2jhsvmmzf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2ftedbdrv.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2syxlnirn.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2hkbtpxzs.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ymznefka.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wdfiqubx.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2fsjbxwaa.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ixuzevsj.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2dvqjypub.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2zdutkgjk.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2xuiibipn.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ktxjvdjm.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2pucbmrxp.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2jwzyjkun.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2vuvpblfu.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2jytiyitn.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2wiepcomx.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2omcezrnc.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2xafymihc.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2tobrmqir.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2dmccijks.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2pzrffbjq.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ihnjdgwd.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2mwxjzsgs.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2lyotqfje.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2naunygzc.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2vkmfyrtc.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2njhbxxkz.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xkkvafhw.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2fjychijb.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2gsyzyvxe.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2aqxxysip.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2cyqoyfvy.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2umahexxz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2tkrdobgf.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2dmwcfwai.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2wrcrvbtv.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2bpqfhqph.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2ptszsijl.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2gcrsoxwh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2wydyipso.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2gpsytfry.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2uyodsyxz.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2qpjoggls.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2sbebvmis.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2eriqqliw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2kqeubwyn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2gzxcjcyo.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2waldcque.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2czciuyrz.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2axsgupys.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2nsguiqnj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2hobldnre.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2mfkrvarj.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2mujezhxy.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2ekwzlolj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nmfxoqdc.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2qlckzrqc.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2yrhakuty.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2hcitzlxp.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2hbcoczut.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2vqocwtbk.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2iqkelzro.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2agzkvdbn.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2mbktsbqn.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2hcjsseeg.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2euonlrad.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2oridapql.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2toyldtmw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ihnxvhtj.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mchpmawc.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2fujxzkkv.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2bqhadabi.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2vsaudzop.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2ikxsytcp.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2szqafbve.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2tzfwyvzn.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2nkeieypn.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2pawbqqpl.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2pmkdkjej.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2wppyjmya.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2lhtobyyg.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ybvblrsd.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ydkwekag.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2lwsulevh.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2fnsebeih.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2oortkfeg.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2ydsgbvim.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2zssvtnaz.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2icvcwvbx.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dxeorxov.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2tfhadopf.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2oqjbwcbr.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2kvqlahbw.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2phohlbqa.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2mexepoiy.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2oelookks.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2epsjyhvr.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2rlcavnmh.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2vqrmzgbd.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2jvaerdih.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2aaikbgev.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2imgcofxz.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2kruzxmde.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2ptvavkob.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2aantokoq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2yboxdlux.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2oakfvbex.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2lsczvoli.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ptunikri.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2pqiqzkdz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2mbeosxfl.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2hgnmjfvt.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2wtfmjfnj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2retqwgve.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2mvrinfsv.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2cgjfapvc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2nrkdcmpv.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2rhiiyqbc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2mjgktspi.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2gwdoidns.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2drfpvzph.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2ojmdqliu.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uhihybfn.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jtfbcmms.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2lefxxwau.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2icdohizb.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2krbscqmz.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2lsblceex.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cohvgiyv.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ykxxdwob.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ldgxqqor.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2vaegfuwj.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2mhdclgde.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2hwhrrsri.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2fcvheyon.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2xvleilbp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2tttkcoei.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2obynzczy.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2modvewrv.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2wpuwvzlz.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2kekbogrx.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jmazefsh.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ixewfcct.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2dkunqnmu.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2gwlurafo.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2pslzessp.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2crfktptc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2jczsckmm.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2lsmbcuxg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2gvwbhkpr.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2xziuzfyv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2tvdllney.html


<!-- 参考信息 -->