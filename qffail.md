代发 wailian999

PHP:  sort($arr);
来源：http://hz.ywan-chungtsiang.top/gtrhxrdcsy.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.gogol.net.cn/gtxcbemkwq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.cucudq.cn/gtujfuzpeb.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.yvedp.cn/gtpyutqckv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.quarkkingdee.top/gttdpfolpz.html

Ruby: arr.sort
来源：http://hz.nwbrower.top/gtwqqdqpyn.html

C#:   list.Sort();
来源：http://hz.zhongyouzk.top/gtffxluhoq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.0kj1m.cn/gtvltnmxhw.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.zhijiandao.cn/gtzucahxie.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.0kj1m.cn/gtsddzhbyx.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.daria6918.cn/gtqfdfowke.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.aibaodan.cn/gtuawkobug.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.hnqzz.top/gtqgfyjpwa.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.xuetiantiany.cn/gtgablbhvp.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.feifeiyinyue.top/gtodrntrtf.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.havefunace.top/gtdfqddzpk.html

[D11] 反转数组
来源：http://hz.shangyingyoupin.top/gttpzpekyg.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.yongpay.top/gtxbpexhjw.html

PHP:  array_reverse($arr);
来源：http://hz.hywenlv.cn/gtsabmyeaz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.quarkkingdee.top/gtzblguwvw.html

TS:   [...arr].reverse();
来源：http://hz.zhongyouzk.top/gtadufudou.html

Java: Collections.reverse(list);
来源：http://hz.quarkkingdee.top/gtmgpiexux.html

Go:   slices.Reverse(arr)
来源：http://hz.chenlongwang.top/gtwwjpjnlq.html

Ruby: arr.reverse
来源：http://hz.52xcode.cn/gthmyzbitl.html

C#:   list.Reverse();
来源：http://hz.xylfe.cn/gtlzemogvm.html

[D12] 查找元素下标
来源：http://hz.pycfn.com/gtsjxytwtw.html

Py:   arr.index(x);  x in arr
来源：http://hz.yueranfly.top/gtnwfojtww.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.tianlin.xyz/gtdltnquiz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.guannengcc.top/gtxzgxqtme.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yuxming.cn/gtngkrwaaj.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.52xcode.cn/gtfhwacdfs.html

Go:   slices.Index(arr, x)
来源：http://hz.jinghuilouyu.cn/gtlktwszpy.html

Ruby: arr.index(x)
来源：http://hz.ywan-chungtsiang.top/gthelgmehp.html

C#:   list.IndexOf(x);
来源：http://hz.ydjk.org.cn/gtqbzkaypn.html

[D13] 过滤（保留满足条件的）
来源：http://hz.9152youxi.cn/gtciaxgzea.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.shanyushiyangtech.top/gtzdsiehqc.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.quarkkingdee.top/gtbaydqzbu.html

JS:   arr.filter(x => x > 3)
来源：http://hz.shzxlz.cn/gtkrxugpae.html

TS:   arr.filter(x => x > 3)
来源：http://hz.fengsongda.top/gtqegofiqf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.nanxinkj.top/gtdqomrntw.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.gaohongyu789.top/gtfrbwzmzt.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.bjfxy.top/gtsrlhzbiu.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.jianghu66.top/gtfpwpstie.html

[D14] 映射转换（每个元素变形）
来源：http://hz.tianlin.xyz/gtqvssnozn.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.9152youxi.cn/gtbfuwlaep.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.gaohongyu789.top/gtelhjmblo.html

JS:   arr.map(x => x * 2)
来源：http://hz.hnqzz.top/gttlwpcyhe.html

TS:   arr.map(x => x * 2)
来源：http://hz.jqgfzy.top/gtjqlzvtyy.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.wangshuangyany.cn/gtqxaneyle.html

Go:   // 手写循环
来源：http://hz.chenzaomai.com/gtpbqfdfcs.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.chenzaomai.com/gtdfmnqyhz.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.shangyingyoupin.top/gtygojdkmk.html

[D15] 去重
来源：http://hz.zhongyouzk.top/gtsgyfydza.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.jyoumei.cn/gtpboswvfq.html

PHP:  array_unique($arr);
来源：http://hz.yongpay.top/gtnuhmgjyv.html

JS:   [...new Set(arr)]
来源：http://hz.jlsjyb.cn/gtlvkpskvf.html

TS:   [...new Set(arr)]
来源：http://hz.ybcxt.top/gteevlezlz.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.hywenlv.cn/gtuktexrei.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.sweek.top/gtrxbgnxil.html

Ruby: arr.uniq
来源：http://hz.52xcode.cn/gthoqiyfai.html

C#:   list.Distinct().ToList()
来源：http://hz.sysykeji.top/gtcizodxly.html

[D16] 求和与平均值
来源：http://hz.zhijiandao.cn/gtptghykmg.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.zhoulong.xyz/gtrzqjwewy.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.sysykeji.top/gtnqrqktdv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.sufxvd.cn/gtnphmpuwl.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.dianchejie.cn/gtnutugoym.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.zhongyouzk.top/gtifrjheue.html

Go:   // 手写循环累加
来源：http://hz.chenzaomai.com/gtbwjdatpo.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.hysaishi.cn/gtmzudgyvf.html

C#:   list.Sum();  list.Average()
来源：http://hz.ydjk.org.cn/gtrxltshpp.html

[D17] 最大值与最小值
来源：http://hz.ybcxt.top/gtwmwhwnct.html

Py:   max(arr);  min(arr)
来源：http://hz.shzxlz.cn/gtbosvqntl.html

PHP:  max($arr);  min($arr);
来源：http://hz.iojbl.cn/gttojagmam.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.zhaomingkeji.xyz/gtezrwkhys.html

TS:   Math.max(...arr);
来源：http://hz.aibaodan.cn/gtblektehr.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.yongpay.top/gtauycnjkx.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.yonumen.top/gtgcqkszxc.html

Ruby: arr.max;  arr.min
来源：http://hz.xuanzx.com/gtixchwaee.html

C#:   list.Max();  list.Min()
来源：http://hz.316326.xyz/gtwatpqgwf.html

[D18] 扁平化嵌套数组
来源：http://hz.xuetiantiany.cn/gtplxtawzy.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.zhongyouzk.top/gtdabnqshw.html

PHP:  array_merge(...$nested);
来源：http://hz.xinyue.icu/gtjmzisxed.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.guowangkeji.top/gtksrabwfe.html

TS:   nested.flat();
来源：http://hz.pycfn.com/gtgwmythug.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.jinghuilouyu.cn/gtmfwoopzt.html

Go:   // 手写双层循环
来源：http://hz.jqgfzy.top/gtorsdyqit.html

Ruby: nested.flatten
来源：http://hz.jinyuanbaomall.cn/gtrmimkjus.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.pycfn.com/gtcarwgqss.html

[D19] 按字段分组
来源：http://hz.sweek.top/gtjyfzrgts.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.wangshuangyany.cn/gtrtdvvhmr.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.svipenyu.cn/gtqqsjbiel.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.pycfn.com/gttefbytfk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.havefunace.top/gtvnpaucjp.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.svipenyu.cn/gtfptfbjju.html

Go:   // 手写 map[string][]T
来源：http://hz.hongshengwenyu.top/gtrrqwbtms.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.52xcode.cn/gtbysgvdtf.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.svipenyu.cn/gtmimzvpkx.html

[D20] 统计每个元素出现次数
来源：http://hz.haohaochexian.top/gtqlgfjcjf.html

Py:   Counter(arr)
来源：http://hz.aibaodan.cn/gtzzilmtau.html

PHP:  array_count_values($arr);
来源：http://hz.9152youxi.cn/gtkanqemhc.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hysaishi.cn/gtctwjscnx.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.ydjk.org.cn/gtqadjxihp.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.ppjwa.cn/gtacaspern.html

Go:   // 手写 map[T]int
来源：http://hz.bjfxy.top/gtmjhhqubv.html

Ruby: arr.tally
来源：http://hz.tianlin.xyz/gtxkszmpvw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.ydjk.org.cn/gtodufdtnq.html

[D21] 判断是否包含某元素
来源：http://hz.hnqzz.top/gtumjbjeeu.html

Py:   x in arr
来源：http://hz.jianghu66.top/gtmaoygiit.html

PHP:  in_array($x, $arr, true);
来源：http://hz.shuidangran.top/gtjbmpklsq.html

JS:   arr.includes(x)
来源：http://hz.tanke756.top/gtakdxacun.html

TS:   arr.includes(x)
来源：http://hz.iojbl.cn/gtbswhtlaf.html

Java: list.contains(x)
来源：http://hz.shangyingyoupin.top/gtaxwtclsc.html

Go:   slices.Contains(arr, x)
来源：http://hz.jianghu66.top/gtcreaqdyy.html

Ruby: arr.include?(x)
来源：http://hz.zhoulong.xyz/gtwsowramw.html

C#:   list.Contains(x)
来源：http://hz.guannengcc.top/gtcxrbxuzj.html

[D22] 复制数组（避免共享引用）
来源：http://hz.gzhubu.top/gtszslxpnt.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.gaohongyu789.top/gtlwmbcdlm.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.feifeiyinyue.top/gtzyrgbwfy.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.chenlongwang.top/gtigqflfjh.html

TS:   [...arr];
来源：http://hz.jinqigfzy.top/gtzjcdgarw.html

Java: new ArrayList<>(list);
来源：http://hz.xylfe.cn/gtkmwwfgoz.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.hywenlv.cn/gtjzuyjwqh.html

Ruby: arr.dup;  arr.clone
来源：http://hz.c1oappe.top/gtycikrwjy.html

C#:   new List<int>(list);
来源：http://hz.aizwys.cn/gtdfhjxypm.html

[D23] reduce 累积计算
来源：http://hz.yanxiufei.cn/gtrhbvffwi.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.bjfxy.top/gtrdpfxznw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.jianghu66.top/gtnhwrcvrz.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.redwolf501.top/gtywfkcjdz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.pycfn.com/gtiwmyihgg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.zycfv.cn/gtrhyqgbvp.html

Go:   // 手写循环
来源：http://hz.sxryk.cn/gttxiynhml.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.sweek.top/gtbtgpvugl.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.wangdashe.top/gtuhjvsyhj.html

[D24] 字典 / Map 基本操作
来源：http://hz.smart0.xyz/gtljfmwjwq.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.zhaomingkeji.xyz/gtbuynkiub.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.aizwys.cn/gtbugwssms.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.316326.xyz/gtysfvhacg.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.vqdsnc.cn/gtgiugonwj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.hammf.cn/gtkzeffiox.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.cashguo.top/gtobxuppzp.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.52xcode.cn/gtdszqdvxm.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.zhengqikj.top/gtpvwvtngx.html

[D25] Set 集合去重与交并差
来源：http://hz.hywenlv.cn/gtwzcxxoyc.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.zhoulong.xyz/gtltthsank.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.jianghu66.top/gteyxgvcjy.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.ppjwa.cn/gtxgwsnhmg.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.sweek.top/gtkxodrnjc.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.ydzc1.top/gtvrmclgfu.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.nanxuanxn.top/gtxjjrqset.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.yonumen.top/gtrgzhvklq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.dashuyun.cn/gtldofjczn.html

[D26] 数组转字符串
来源：http://hz.wangshuangyany.cn/gtmfsovbov.html

Py:   ", ".join(map(str, arr))
来源：http://hz.jqgufenzy.top/gtbnwemhcn.html

PHP:  implode(", ", $arr);
来源：http://hz.aibaodan.cn/gttpbjfosv.html

JS:   arr.join(", ")
来源：http://hz.guannengcc.top/gtkaevgbre.html

TS:   arr.join(", ")
来源：http://hz.feifeiyinyue.top/gtstsjczmo.html

Java: String.join(", ", list)
来源：http://hz.sysykeji.top/gtlrqhuxgg.html

Go:   strings.Join(strs, ", ")
来源：http://hz.daxiang520.top/gtqsjkmwjo.html

Ruby: arr.join(", ")
来源：http://hz.jqgfzy.top/gtquiwptuf.html

C#:   string.Join(", ", list)
来源：http://hz.sufxvd.cn/gtiiuhdjvy.html

================================================================================
来源：http://hz.xinyue.icu/gtjxmewydm.html

E. 字符串处理
来源：http://hz.ydzc1.top/gtivhimlyv.html

================================================================================
来源：http://hz.jinqigufen.top/gtlpwvzotj.html

[E01] 拼接字符串
来源：http://hz.52xcode.cn/gthkoozmvh.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.ivvv.top/gtigjfzwlp.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.yj202588.top/gtdwndcusr.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yj20258888.top/gteopbsvpz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.iojbl.cn/gthfrfevrj.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.jinyuanbaomall.cn/gtokdcrpvq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.quarkkingdee.top/gtkolmaiwf.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.jianghu66.top/gtchmrrnld.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.yanxiufei.cn/gtjymzltwz.html

[E02] 重复字符串
来源：http://hz.cdnleiting.top/gthhlxyldy.html

Py:   "ab" * 3
来源：http://hz.chenlongwang.top/gtqnsikcnt.html

PHP:  str_repeat("ab", 3);
来源：http://hz.guowangkeji.top/gtrhftxahi.html

JS:   "ab".repeat(3)
来源：http://hz.nanxinkj.top/gtswomvuxl.html

TS:   "ab".repeat(3)
来源：http://hz.jinqigfzy.top/gtkgsygfvg.html

Java: "ab".repeat(3)
来源：http://hz.dianchejie.cn/gtyvnbzaoc.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.nanxuanxn.top/gtvekkzpca.html

Ruby: "ab" * 3
来源：http://hz.svipenyu.cn/gtfpyquxch.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.jiagoushi.top/gttfgkvvbw.html

[E03] 截取子串
来源：http://hz.jyoumei.cn/gtyyvjfykd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.jianghu66.top/gtbibzxrkk.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.yongpay.top/gthedwmhnc.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.cdnleiting.top/gtablozjmf.html

TS:   s.slice(1, 4)
来源：http://hz.jqgufenzy.top/gtbuudxtex.html

Java: s.substring(1, 4)
来源：http://hz.andypj.xyz/gtincalkdd.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.haohaochexian.top/gtjoktedih.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.bjfxy.top/gtwibievos.html

C#:   s.Substring(1, 3)
来源：http://hz.ehwqpu.com/gtutrsqcyt.html

[E04] 查找子串位置
来源：http://hz.hfpthk.cn/gtilxbeoec.html

Py:   s.find("x");  s.index("x")
来源：http://hz.cucudq.cn/gtgsfchrkb.html

PHP:  strpos($s, "x");
来源：http://hz.havefunace.top/gtvywblvvu.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.yj20258888.top/gtxoizimfb.html

TS:   s.indexOf("x")
来源：http://hz.chenjidiqi.icu/gtcrxjxugt.html

Java: s.indexOf("x")
来源：http://hz.ppjwa.cn/gtfbplhwho.html

Go:   strings.Index(s, "x")
来源：http://hz.zhijiandao.cn/gttwvbbuyt.html

Ruby: s.index("x")
来源：http://hz.gaohongyu789.top/gtidklpuar.html

C#:   s.IndexOf("x")
来源：http://hz.jinqigufen.top/gtksidfqiq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.guowangkeji.top/gtyiimjfyw.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.c1oappe.top/gtzpgfhmfm.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.zhoulong.xyz/gtybiguqlz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.gzhubu.top/gtymjzuwre.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.cheryme.top/gtfrbfbdor.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.sweek.top/gtcnjvhjvs.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.sysykeji.top/gtmzfyhcpy.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.shangyingyoupin.top/gtznowquke.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.yj20258.top/gtciebqqqa.html

[E06] 替换子串
来源：http://hz.zhaomingkeji.xyz/gtujirrqge.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.yj20258888.top/gtechcduji.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.zhijiandao.cn/gtqwiayibc.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.shzxlz.cn/gtykatvtop.html

TS:   s.replaceAll("a", "b")
来源：http://hz.guowangkeji.top/gtlwkpgulw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.cashguo.top/gtsllhdiaj.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.zycfv.cn/gtugatswso.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.svipenyu.cn/gtdblzryqb.html

C#:   s.Replace("a", "b")
来源：http://hz.gaohongyu789.top/gtcurjfrjw.html

[E07] 按分隔符拆分
来源：http://hz.haohaochexian.top/gtluemqzgf.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.wangdashe.top/gtoabwfnso.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.yvedp.cn/gtdexrndru.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.aibaodan.cn/gtqnpuszlu.html

TS:   s.split(",")
来源：http://hz.guowangkeji.top/gtbdcxhaea.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.sufxvd.cn/gtsllobexl.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.xinyue.icu/gtooygpzkf.html

Ruby: s.split(",");  s.split
来源：http://hz.xuanzx.com/gtripmkqei.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.316326.xyz/gtxfrghbxc.html

[E08] 数组按分隔符合并
来源：http://hz.9152youxi.cn/gtkihzavkd.html

Py:   ",".join(items)
来源：http://hz.dianchejie.cn/gtwrsrgsiy.html

PHP:  implode(",", $items);
来源：http://hz.nwbrower.top/gtwomtqfit.html

JS:   items.join(",")
来源：http://hz.shanyushiyangkeji.top/gtqailcoae.html

TS:   items.join(",")
来源：http://hz.yangfankeji.com/gtajypfzis.html

Java: String.join(",", items)
来源：http://hz.tian-w.cn/gtkxllxhpd.html

Go:   strings.Join(items, ",")
来源：http://hz.jqgufenzy.top/gtopasltds.html

Ruby: items.join(",")
来源：http://hz.havefunace.top/gtxvhcxvhs.html

C#:   string.Join(",", items)
来源：http://hz.jianghu66.top/gtzmzsjagf.html

[E09] 去除所有空白字符
来源：http://hz.daxiang520.top/gtunljrcmj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.jyoumei.cn/gtcakitjqa.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.zdqjudy.top/gtuefjvdzs.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.hysaishi.cn/gtqvurosbz.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.ybcxt.top/gtzrxvygpj.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.gotoacloud.top/gtumljiycl.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.hysaishi.cn/gtjkndskzr.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.cashguo.top/gtdlitktex.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.ivvv.top/gteqqgqeim.html

[E10] 左侧补零 / 定长填充
来源：http://hz.chenjidiqi.icu/gtgxvauavc.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.cqqwz.cn/gteljnquns.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.gogol.net.cn/gtgpgwatvw.html

JS:   "7".padStart(3, "0")
来源：http://hz.jiagoushi.top/gtuxzaemwr.html

TS:   "7".padStart(3, "0")
来源：http://hz.nanxinkj.top/gthmfkkdes.html

Java: String.format("%03d", 7)
来源：http://hz.yj202588.top/gtomngrbdd.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.smart0.xyz/gtvbovqtrj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.birdmap.top/gthkqfwmhl.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.andypj.xyz/gtdwnzbvou.html

[E11] 反转字符串
来源：http://hz.ivvv.top/gtevwjejza.html

Py:   s[::-1]
来源：http://hz.yuanzhike.top/gttkbbkygs.html

PHP:  strrev($s);
来源：http://hz.cdnleiting.top/gtawjllxrl.html

JS:   [...s].reverse().join("")
来源：http://hz.yanxiufei.cn/gtavxzfssw.html

TS:   [...s].reverse().join("")
来源：http://hz.shzxlz.cn/gtspfxvklo.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.dianchejie.cn/gtdxbtynnn.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.yanxiufei.cn/gtztqcswcs.html

Ruby: s.reverse
来源：http://hz.gogol.net.cn/gtnggzatqc.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.jinqigufen.top/gtmhggfwqy.html

[E12] 统计某字符出现次数
来源：http://hz.tanke756.top/gtkmvooouc.html

Py:   s.count("a")
来源：http://hz.xylfe.cn/gtobnmbevx.html

PHP:  substr_count($s, "a");
来源：http://hz.redwolf501.top/gtcfratogk.html

JS:   s.split("a").length - 1
来源：http://hz.gzhubu.top/gtfcepvxms.html

TS:   s.split("a").length - 1
来源：http://hz.yuanzhike.top/gtktvlygms.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.xuetiantiany.cn/gtpqrkidgt.html

Go:   strings.Count(s, "a")
来源：http://hz.chenlongwang.top/gttvtnhwxh.html

Ruby: s.count("a")
来源：http://hz.jinqigufen.top/gtiaxmikwp.html

C#:   s.Count(c => c == 'a')
来源：http://hz.jinqigufen.top/gtjkumzytg.html

[E13] 逐字符遍历
来源：http://hz.ydjk.org.cn/gtaxepofyd.html

Py:   for ch in s: print(ch)
来源：http://hz.zhijiandao.cn/gtkdjpgswg.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.aizwys.cn/gtpzcmznbt.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ydzc1.top/gtrriksggk.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.cucudq.cn/gtoswpnthx.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.iojbl.cn/gtdrfgrajn.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.yonumen.top/gtfuzdqgbh.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.yangfankeji.com/gthnsjdvig.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.svipenyu.cn/gtbdhihxdt.html

[E14] URL 编码与 Base64
来源：http://hz.9152youxi.cn/gtvuzswomo.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.shuidangran.top/gtlpuatpvk.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.guowangkeji.top/gtcalqjnev.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.nanxinkj.top/gtkjgzqxpm.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.cucudq.cn/gtqrkuahdb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.pycfn.com/gtxjwuqzuf.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.gaohongyu789.top/gtmvwdzzyx.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.ywan-chungtsiang.top/gtqqvnquof.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.zhoulong.xyz/gtzrctrvow.html

[E15] HTML 转义 / 反转义
来源：http://hz.andypj.xyz/gtnjkinfmz.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.xinyue.icu/gtptorfqpv.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.chenjidiqi.icu/gtnzbriiwq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.chenlongwang.top/gtwxofyejg.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.ybcxt.top/gtcyeuwbie.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.yuanzhike.top/gtgplsdjfq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.jqgufenzy.top/gtjgzjlryd.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.gogol.net.cn/gtqpzcxnqj.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.jinyuanbaomall.cn/gtkmgasckv.html

[E16] 数字千分位
来源：http://hz.zhongyouzk.top/gtlkgbgmdo.html

Py:   f"{1234567:,}"
来源：http://hz.shuidangran.top/gtlbuwqmsp.html


<!-- 参考信息 -->