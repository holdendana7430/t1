代发 wailian999

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2sylgcbnd.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2vcwqoyzh.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2pmnwqtdm.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2hfwhhupa.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2kebcaotb.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2zuibrcsi.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2anlsnolq.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2projmlud.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bmmytzmy.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2plcfynih.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2edftratc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2kxiafhrj.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hxzeimmt.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2izjttakk.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2wjrqdaro.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2asanwbca.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2mbuywnbr.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2pcnfondk.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2wrtkuuub.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2xvjoynbr.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2nfwhokwx.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lmrxryru.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2zywcaiyg.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tueujwlu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2cwhifsmc.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2boascyww.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2dlgfsnwp.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2pvaekshr.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2icyuyivl.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2hqgtjshg.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2eqqrcyit.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ibuqhezt.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2xfgkkrws.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2eubjfusm.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2aqzblepy.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2wnlxyjwa.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2mvcqgiwp.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2edtgykly.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2grrtwzcb.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qcvghrhv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2unjqtoss.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ocoiajfs.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2ajlgzoul.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2gotdmicf.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2vvvropjp.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2nysxppam.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2gwbdabey.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2whxibsql.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mgmuccsd.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2qmbiasjp.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bofwvftm.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2toznrquu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2khzfocqf.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2xcalxjfu.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2gxcatyhn.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2nyyuloxr.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2ytqjewjn.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2prdxwtkq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2hkjzyflh.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2vrnpdjso.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2krofsnxq.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2xnfuopkx.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2wbvymrix.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2wnbiewkn.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2qacpwlsj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ifsymfzf.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2xglhfoje.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2lyxvjgxr.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2awacbuyq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2hnidznrx.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2qaywyxis.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2nvzooohm.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2nbnbgzfz.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2jwdnekif.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2xdsmxcrh.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2hwbtnoij.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2bgupblil.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2biixjoui.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2dxprybvv.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2ibxwojgv.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2agwlrytz.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2wcvpzlfv.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2dztuvzmo.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2dxnrlhja.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2flwvwemb.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lviubpqs.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2fcomhytu.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2oqdsqpxt.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2okubekec.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mrcxepgu.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nkkndzkt.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2qhsgkxlv.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2mtpzlhnt.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2ktbovhln.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bniivyxm.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2krhixpwv.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2trfqdmke.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2rltrvsog.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2cxkjqhdq.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2pzuoggzj.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2vfiizlpe.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2yuquaddm.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2yepnrykl.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ecebfzhr.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2envelmkx.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2kuihjtzj.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2azmqlcum.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2bsblceyi.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2xhfnrwsj.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2iwqtrghc.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2wbjraoxe.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2gypuoixz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qbfjrlha.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2oxbdigoa.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ysszizvz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2rhavukwx.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2itqkffdr.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2clqumqyw.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2yymmldir.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2jykiexib.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2vlytylls.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pizglfae.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2cwsssjtp.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2odqzkaxw.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2anzmbbjq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2klnbskcy.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2sxunawtc.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nvltvuxo.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2llcaxdsr.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2xestrdoj.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2gqoypjog.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2qbjaikhs.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2lbhadlvn.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2yqoctzux.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2gkpunqde.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2rzxpsiws.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dfmtconx.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2tglrkhba.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sktfhfke.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2juvyefsn.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2uknfuamd.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2oihjykkx.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hoqlxmzm.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ebzcqdtz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2gmyfiwcp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2xnncafnh.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2ohbcrfgp.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zmijrscw.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2khyiigiq.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ccwendcu.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lgnfspwx.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2qkqjpneg.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2grxpkycv.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2obnlpywo.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2odshdklp.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2shwmyagl.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2aofcjqbg.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2sdkexmqr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2egumfxab.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2caxdhrnf.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2sehtyfyw.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2rfedoqrp.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2uldsrxgt.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2olrzyblj.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2qqxhtjcl.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2hxzpmtvm.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2cmwtogur.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2iqckdbpg.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2dsrvzwrp.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2nuiubuvh.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2bivofbka.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2bsvtceyl.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2ptcooezs.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2eeuwvyzd.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2woephphv.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2tzsqeiwy.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2kfnvogqf.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2ogsfniab.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2epthcboo.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2etprelkf.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2dkigfvdr.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2cwisaedf.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2dgjortkf.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2yrtyrefz.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2veqlmonc.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2pcelrzac.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2knsduypn.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zmylgoio.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2tgmktehv.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2smagovlm.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2yjivubpy.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vzwlibcd.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ssyiutvs.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2axakkvjd.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2cxctkuys.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zqskkqse.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2jvqgitnj.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2hlxyxysn.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2asrskoyg.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dnndprax.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2ljgdqwxm.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2soifwosd.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2dvqmcjyd.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2kketedsh.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2oujxltvd.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2kexqbaxt.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2hyskhdqp.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2huggtmeo.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2zernijep.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2pfmrraci.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2wtmxwogf.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2soccgzos.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ccfjuxhb.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2btywdgar.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2bueasrhi.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2gwwvcbmc.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2mmtpstnk.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2mrbkykjs.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ljdvhbqh.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2emycemff.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2hmuvpaqt.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2xyrxijcm.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2puxvadql.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2jotsfcgz.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2swsbucvg.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2hiomchvk.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2dylllkgq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2qolossvd.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2eymcdemi.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bsmykcsf.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2jyqeuymo.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2btxvurcv.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kuffyoxl.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2awftmpek.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2mdjvjkdk.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2sdggwdpv.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ivmcvelx.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2aqangxbi.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2ocwnmooo.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2fmrdxkrp.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2yjvwrjqq.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2oiufslgc.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2kfhfdhxg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2uljgosxa.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2qxlrtwvw.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2fdzpibun.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2qiwoflyg.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tdkntilp.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2sgxfpecy.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2tlckhkdf.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ngwficnk.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2bwoberdm.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2utmxjxaa.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2lpawfoap.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2ljgyeoju.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2lblbkjko.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2salayisg.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2sdshotyu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2kikzhgfq.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2alejvqgk.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qycduwpc.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2pivmcndr.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2uqbtvlqu.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2ndejggxb.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2wskhgkxp.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2niwyytln.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2ransyvhw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2kwzqxyol.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2vlcszhgf.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2hxpnuguk.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2iubrbpln.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2qznufkop.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lhmuisui.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2upwpiebd.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2vczjvsfb.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2aedsxiao.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2livmzbgr.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2gtfwgwbm.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2vxjojrwo.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2nckrdnxr.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2jbvgdsuu.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2qcipspsy.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2seevqhnc.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2qdoaqqta.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2qwnndlnr.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2uappbtpm.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2tdghafmz.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dqxwwavr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ghikqxln.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2qhbymcvo.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2vfrcpong.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2mbvuihvo.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2wjwdmtfl.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2ocfwyota.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2belynzfj.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2vtjzecuk.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2jktpblnw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ncelujwi.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2iqjtujds.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2ptzughnl.html


<!-- 参考信息 -->