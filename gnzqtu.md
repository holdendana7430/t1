代发 wailian999

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2vxqrxbhu.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2xqjhxcsf.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2rdgpzcne.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2jqxhajoj.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2nqxhsfme.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2gwqfrdmm.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vroufoyj.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2beeusrrt.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2cmycjbeg.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2dnshmiap.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2yrmxpyxd.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ihvpehlf.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2zdybjfxk.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2dockcihv.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2pdogunbo.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wwwmwjwg.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2qedehcwx.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2nxxcddyg.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2gwffrsvz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jzqygwfd.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mysyqicf.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2smqaewog.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2kixzycln.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2boxzwceu.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2bdketbhp.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2iazaynlq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2uxjyybsp.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2qnjbpuvr.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2alytkxuv.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2kvmvpebp.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xublcfes.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2iqsvudhp.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2pnjjugtl.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2jvarailh.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2jdwdhovs.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xvfpbprs.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2wuqztixg.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2btnqajqw.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vuilbgns.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2peuefnfm.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2yvevksxz.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2loxsuzay.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2fxdkkzpj.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2dkspfapi.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2nbwkljvf.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2tafldxjo.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mnzkeemg.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2mdrxyxbc.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2nqvqrfav.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2fjyemgwd.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2agmihaos.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2bxlctoxe.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2thkmjqsh.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2tziouptf.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2xefvxmzn.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2trlwvebu.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qofyocce.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2melgdwsg.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2pvmfsmyk.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2klbmmhve.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2hjskumjr.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2hmbuhbso.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2oihemegt.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2pugfcgqh.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2dflztsht.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2rfrojpbb.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2hweaivcy.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2tzrmnhyg.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2guwwnavz.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2ejemvclt.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2nzfafagx.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hsemunil.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2onospxyr.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jmychkxs.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2ytekcbpr.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2bnxmjuaw.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2ovprthuc.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2mwabtkui.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2krnvirwe.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2bnjqfybk.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2snodcjnl.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2zblpyvbi.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2arpsvsgx.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2vhrywuhh.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2zfpicole.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2mgesrwpg.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2jhvfjood.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2urpoiquk.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2keqnjiek.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2xtuwzohw.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2yhwjvmmr.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2prsaybqq.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2hbdurypj.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ethwimmg.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2pcmlwzho.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ghtvzjpr.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gdktrbot.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tmwjblbs.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2tujbslyb.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2umbdnwwr.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2ycghgedo.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2rsnqemjz.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2eeubtlse.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2xjxtujpf.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2lfwttpqu.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2bphpxaoa.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2gpawypbt.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2zsmxamgh.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2tnjfkeup.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kbdlicug.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2micjsraa.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2mdouaiac.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2smwufvjy.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2glnvishh.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2nytafcro.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2zkuyktsg.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2lbcgkrpv.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2bemqiglj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2sgkluptv.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2trcadhkx.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gxxaerjb.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ihdvelnv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2atdoziho.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2mrhiywjk.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2tgiafrhh.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2xqfgjwgv.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2sgosmezr.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2xuyzuzmy.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2cprwjkjo.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2oknwatqm.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2bfhivafp.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gdjnfdaq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2lfgskiqj.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2pfyixphv.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2fadkxlhn.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2niujafsl.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2azuiavnn.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jtdweere.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2kesuqhip.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ztuqiovt.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2juatpdrj.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2kzsuqqqe.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ujcffnce.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2uelpzdbp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zvxyysbc.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2gpjnkyoy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ddjxssat.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2dtjirzcb.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2kfbbxmju.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2qinskbyh.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2vdiqqdth.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2othaidco.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2opsyxefo.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2tcqqitss.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2fykstivx.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qbcekcln.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nhsbpxyh.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2sqxairxk.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kahvpzds.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2nzlhcxvc.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ecblfeoh.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ttvjiobj.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2phbwytrl.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2rzvjhwzl.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2lygjemui.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2swqwrwjo.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2dnpnywjp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2meskblhk.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2xgpxgqwr.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2wbqnitap.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2brmtwxbb.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2heaqxojf.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2rfuwgqbe.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2xxpqloxh.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2xqflheuf.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2tyatbils.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2yfctzwoy.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2yrkdchni.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2hsaddzyx.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2gjtquvvy.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2ccepmxho.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2caprivyq.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2mepmjpnt.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2tzvhoqxt.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ecuenuuj.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2zrhwjgfb.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2qzabsudj.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2xriromzd.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2gbxlohue.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2bhgifycn.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2ugnlrfuo.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2chsfpmtx.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2rbqxoidu.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2rxspnout.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2bbbbfxsn.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jvxczlyp.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hzbfsykl.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2geybvjpf.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tyrwrdnj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gmzrnlnj.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zcaiggil.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2wwbswwww.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2kavmcggq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2fmrjguwj.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2lpnvnifl.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2hgrdwiwk.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2pldfkvdp.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2ymqetidf.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2cnhsnkts.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2qmzuzwah.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2kapelres.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2gxmxkdzp.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2cuwfogdz.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2jwajoryg.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2hkglsqgq.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2dhixwziz.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2xwkfogvi.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2pusaftjh.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2iyhppdsm.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2gmbwackn.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2lwtqncsi.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2buqmfbit.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2cheezmlr.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2gybivdcv.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2eaoakalg.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2jjkoqxst.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2fbujildh.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2iheofxbn.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2jnlfhmkd.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2lxjrmmzm.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2ethmbsdy.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2kgcvgdav.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ngcoewrl.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2pestydge.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2arboyswf.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2lgpxjdbx.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2bmwppube.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2iawutsuy.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2mfpiifvy.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2jolfrwvw.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2tclvospq.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2qqomvwne.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2sotaortx.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2drgbyset.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2puhjhqea.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ugvrjjom.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2vziumttl.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2lngeodkz.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2cbiaflaa.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2fhspsgmj.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2znybyvud.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2eepgmwcl.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2kfablktg.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ejgxnyuw.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2qbepdrub.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2ucymuwfy.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2klqtcueg.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2emhvvwea.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2drshvilw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2bqmhpcmj.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2molfaubj.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2gosrqngm.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2bqbhitgl.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2uedwjwdj.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2sjhgirmx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2kvsmjubh.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ytoutvdl.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2swwdyzdo.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2iuiedbuq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2lpbdfnfm.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2agvbfcxy.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2kqbjdvcs.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2shninbdq.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2wtrifwms.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2kafanybb.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2umzcoeqg.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2puyaeotm.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2uwgdegla.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2dcobhrgk.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cnyuidgj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2iamxcaaf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2odzxmkdp.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2rprsjhjk.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2icrcsizs.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2stedxqos.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2lswazgzd.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2owobbzgr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2veudjyby.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2etkhogwg.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2haiddmcn.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2nlnnfknf.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2wytwgipb.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2avtsumyy.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2endgberr.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ybwqlbyk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hizgqkar.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ihbdntex.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2topbokij.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2sghddtcy.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2nwwofbsb.html


<!-- 参考信息 -->