代发 wailian999

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2wvxdrkha.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2lpivzlir.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2eitgiemv.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2csatqluj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rykzlbea.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ljadsakz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2gfkpellk.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2nfclkmkb.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qvsbhejy.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2ipjxpfnb.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2uhmvalun.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2awevngux.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2yhozgoqa.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rjwxdxhc.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ucuyxytv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lpeecmpi.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2sfufoopn.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2royhcbab.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2nevjfoyd.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2rvldsrao.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2jimjhwoy.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2scgsasju.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2eaoqbfpc.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kqvmtnfo.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2plcvhbpx.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2sibhknji.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2qlqxgjhl.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ilyjevev.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2rhrlpvjv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2umdwrvco.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qyfftqvr.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2vwebmlcn.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2rjaumlkj.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2iosckcms.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2guqfgfjw.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2mjhstpkg.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jxuzzhrg.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2ockfnhdc.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2iufyifhi.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cvsxnbrx.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2jpubroql.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2bjvfohzs.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2hhwnnwke.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2rpxkynbt.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2uhwenlcx.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2mnbyniou.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2mqklwccm.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2beyzilvn.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pibsnedz.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2vnymkbwd.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lmvegdrm.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2qolwjzzi.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2imrpmzvl.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2ojdggkbl.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2jzupehlo.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2mmhszoks.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2zlgiemcz.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2vqpvfxrj.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2ukzvriro.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2bgsrswtn.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bytniheq.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2iwhgivfp.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2bcqbouve.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zmjkbpwr.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2szftguyo.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2xjbpxrao.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2hknteikg.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2qughvmrg.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2hiqgsfqf.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2xcdadqkg.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2jcnlxiqx.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2patqnhrv.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2lnggrxwb.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2bfmvhpyt.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2mhsccjrt.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nxjdlwcs.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2ctbqbton.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2sozjshdy.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2aasbwyat.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2rchgpkza.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2clnqqnih.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2wrrkwukv.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2bibtoppx.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2zcqgvacw.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ahzqaajh.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ybnrrwom.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2oeeevykv.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ymdvyenu.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wfgxethy.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hkuptcno.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2fposvpli.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2amekevye.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2aushgsnc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2wykwevmz.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2evknjxbo.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2whssznbi.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2turinisq.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2fwxqpjbi.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2bydmqjog.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2lihvbisn.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2brzmhlwr.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2wrofdvlz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2sqxegrlv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fvoqapcn.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xqxsazmb.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2caujbitc.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2nsrwcmjt.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2uqcxmeyi.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2dkbgslwc.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2xhwjjcro.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2smsruvwe.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2gjaedpsg.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2yjulmwnq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2vggecpem.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2hadnzvnn.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2pxlqlrux.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2uwacurnx.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2hctqlgta.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2fkldrwjl.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2zkvlbnqp.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2dpwvwtay.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hpnfucpv.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2gqzwxpuy.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2dwjaxsea.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2jfxieouh.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2wkpgeqme.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2xyqhjoqv.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2kokwzocb.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2zjkvrilm.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dvnmmivj.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2fhrhnhhc.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2lychtksl.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2fsvqjxke.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ckavhmsn.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2esxlcjqm.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2qpskbuxe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2asuqvech.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2pknbshbq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jrjshazg.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2znhhcyif.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2skbcagdr.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2anyrkcen.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pyemzgct.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2cwepawpg.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2qofdopab.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2qmxudmrb.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2aqfjmhto.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xxkbxnvq.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2bjxsjnay.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2pccnztlc.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cstjegcv.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fvzxpuhf.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2wpbsruma.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2zyqxhmoi.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2jhsrzhxd.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2qjuupesa.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2fchyrupq.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2msgxvzbd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2dmvhuthc.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2vfgphebc.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2lxjxeovc.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2zqmlzgfk.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2largmjst.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2zpnxaucv.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2pplpmhlf.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2gnxshpmq.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2iwhldurj.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xrcavizv.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2cejuykay.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2darewggo.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2qzfkeyfd.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2heayfpys.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2cmfewzbm.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2utsspwal.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2dcuadqcm.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2jrfjjoui.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2byjbjmtj.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2udcnsppq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2gpxbehla.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2zeqjtdtn.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2vjhwvrkz.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2hazayfte.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2obfqhdgb.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2nzmhwawu.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2ujdemzxx.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ggjwuqps.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2amklppja.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2plyvllqw.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2udftlxgs.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zljzswkb.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2eefecwfq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ipaqlhtg.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jherxwrl.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2csdwalzp.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2ifxdxnzs.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2dbtzufwz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2lydgfuow.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2vthnibfe.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2jvlkgfpu.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2imjobmea.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2ywbgrlhs.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2bvhgtgoi.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2gqipqogn.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2hkoizihx.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2ujxyhlhd.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2xztvqtun.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2vmtvdrbm.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2hzkrijor.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2yvnrsxgo.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2zgkarqog.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2aywouwgh.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2twksjbwa.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2wgjcxaok.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2efujiypx.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2hwqeicgo.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2wtdrxdnh.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2jimvxwrj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2gdafxubl.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2dtugsejl.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2tzmwcymu.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2ipnetgjx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2lwttqzdr.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2bazuanzd.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2otoxacqf.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2pzikgdua.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2eyhorzqw.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2spgntoda.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2sjcxzdkg.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2eodkwkda.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hwnzaqmw.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2mkuvmypt.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ukxtruex.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2yyrvrfmo.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2stawmhqz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2bptyzhak.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2ffzmyqje.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2sgmfewcd.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2aqkywpcg.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2skhrezkj.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2wpjxkpde.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2kmthdivn.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2psvxkaqk.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2ckhzgjyo.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2lfhodnhg.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2cqwkmtaa.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2pskvcobv.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2plyfuvas.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2opvujpyt.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2wqfdgkyu.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2iuzzaljw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2shbcwkyz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2acckgjyp.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2jqgjikcr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2xqrvvvlb.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2sbfkkrbc.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2gnyfhjyh.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2gtwjpyvy.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2oenpssys.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2kdcmxmwy.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2evyapgac.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2lbgclbgs.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2veiqnymr.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2xapquzgl.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2mwxxhuyk.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2fnwjorqn.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2xblwgpuf.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2uoegnpqk.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qmocacwj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tcjdxefz.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2dovyiqtu.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2iiyanbjr.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2sveglwiq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yyyphdlt.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2fhjnmgwx.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2eahjivcd.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2nmmaksmh.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2wcbvthho.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2eimbjjky.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2qzeidzln.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2bbykiggl.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2nscidhvc.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ylcyqnom.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2ulxqqwbn.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2lsiubujw.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2zydusxso.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2plgtupqp.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rtrslthc.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vzgfugkt.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lafrtimc.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2jenhngds.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2pzozggdf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2dhpubmpb.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2cryhtevv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2hxzuwxhv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2hojinfqc.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2qjcgueoz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2vemgwrgq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2jvulfqzy.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2uukuipua.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2yskheqmy.html


<!-- 参考信息 -->