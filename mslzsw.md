代发 wailian999

TS:   arr.slice(1, 4);
来源：http://hz.yuanzhike.top/gtyrplwkmo.html

Java: list.subList(1, 4);
来源：http://hz.bjfxy.top/gtftcmfwsn.html

Go:   arr[1:4]
来源：http://hz.birdmap.top/gtxhbcvfth.html

Ruby: arr[1, 3]
来源：http://hz.xinyue.icu/gtdslurezx.html

C#:   list.GetRange(1, 3);
来源：http://hz.xuetiantiany.cn/gttcwdoumm.html

[D08] 合并两个数组
来源：http://hz.nanxuanxn.top/gtsmxndrgz.html

Py:   a + b;  a.extend(b)
来源：http://hz.zhongyouzk.top/gtrtnmnxaq.html

PHP:  array_merge($a, $b);
来源：http://hz.daxiang520.top/gtexdiakqq.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.jiagoushi.top/gtbyswixep.html

TS:   [...a, ...b];
来源：http://hz.yueranfly.top/gtlsiwymin.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.jinghuilouyu.cn/gtrrryajez.html

Go:   append(a, b...)
来源：http://hz.haohaochexian.top/gtexypepyp.html

Ruby: a + b;  a.concat(b)
来源：http://hz.zhixingplan.top/gtwwcehwcu.html

C#:   a.Concat(b).ToList()
来源：http://hz.jqgfzy.top/gtzayqqkgq.html

[D09] 排序（升序）
来源：http://hz.cqqwz.cn/gtasalwfly.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yj20258888.top/gtupytolpr.html

PHP:  sort($arr);
来源：http://hz.cashguo.top/gtezngypug.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.hnxiangtu.top/gtyayqqegs.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.ivvv.top/gtcofennbl.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.birdmap.top/gtnokwmayi.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.cucudq.cn/gtklwynqva.html

Ruby: arr.sort
来源：http://hz.zycfv.cn/gtjfchnwkd.html

C#:   list.Sort();
来源：http://hz.cucudq.cn/gtvaaxgugp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.zhaomingkeji.xyz/gtkqzfyjsr.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.zhixingplan.top/gtildwhqpw.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yj20258.top/gteakjbktv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.daria6918.cn/gtspyiruda.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.shzxlz.cn/gttilyyyyx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.316326.xyz/gtynnsbdcx.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.sufxvd.cn/gtggehlzbf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.jinqigufen.top/gtjdqnyjmw.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.chenlongwang.top/gtkqimxilz.html

[D11] 反转数组
来源：http://hz.jinghuilouyu.cn/gtbfexiltv.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.52xcode.cn/gtexyydqlv.html

PHP:  array_reverse($arr);
来源：http://hz.jyoumei.cn/gtdizcmewz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.kuanghao11.cn/gtacgdvvqz.html

TS:   [...arr].reverse();
来源：http://hz.cashguo.top/gtqyfxowym.html

Java: Collections.reverse(list);
来源：http://hz.yuxming.cn/gthxufuhgb.html

Go:   slices.Reverse(arr)
来源：http://hz.xuanzx.com/gtqrqzpowa.html

Ruby: arr.reverse
来源：http://hz.jinqigfzy.top/gtcriezunx.html

C#:   list.Reverse();
来源：http://hz.chenlongwang.top/gtrrwwaevw.html

[D12] 查找元素下标
来源：http://hz.yueranfly.top/gtbnixugeu.html

Py:   arr.index(x);  x in arr
来源：http://hz.fzhhl.top/gtrdmwcdul.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.ybcxt.top/gtxrdqsogz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.52xcode.cn/gttkldvnjr.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.hfpthk.cn/gtstuvkror.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.jyoumei.cn/gtbakvllqr.html

Go:   slices.Index(arr, x)
来源：http://hz.wangshuangyany.cn/gtnuhxikzu.html

Ruby: arr.index(x)
来源：http://hz.vqdsnc.cn/gtfbmalbep.html

C#:   list.IndexOf(x);
来源：http://hz.zhijiandao.cn/gtjidzckxz.html

[D13] 过滤（保留满足条件的）
来源：http://hz.jinqigufen.top/gtylldhink.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.nwbrower.top/gtrnobqvnb.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.cqqwz.cn/gtntvedgua.html

JS:   arr.filter(x => x > 3)
来源：http://hz.zhiwuduotai.top/gtgiinoiso.html

TS:   arr.filter(x => x > 3)
来源：http://hz.daria6918.cn/gthcbswsbh.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.feifeiyinyue.top/gtmpttutop.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.yuxming.cn/gtjalwvfvw.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.xingfuxueyuan.xyz/gtnsmwbqwq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.smart0.xyz/gtyozrppnp.html

[D14] 映射转换（每个元素变形）
来源：http://hz.aizwys.cn/gtgzbirzat.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.yvedp.cn/gtdockqmkd.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.jianghu66.top/gtgulsyomz.html

JS:   arr.map(x => x * 2)
来源：http://hz.sysykeji.top/gtxkdktqhg.html

TS:   arr.map(x => x * 2)
来源：http://hz.dashuyun.cn/gtegbmuygv.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.chenzaomai.com/gtbttxkndi.html

Go:   // 手写循环
来源：http://hz.zdqjudy.top/gtxifgvxvf.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.guannengcc.top/gtpgyvvnxl.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.zhongyouzk.top/gtjchvsfvz.html

[D15] 去重
来源：http://hz.dianchejie.cn/gtmhbznauz.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.vqdsnc.cn/gtutplnrfg.html

PHP:  array_unique($arr);
来源：http://hz.xylfe.cn/gtkdwpycpo.html

JS:   [...new Set(arr)]
来源：http://hz.shangyingyoupin.top/gtntpxlzzq.html

TS:   [...new Set(arr)]
来源：http://hz.fzhhl.top/gtcldsujan.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.shuidangran.top/gtxkzhvxor.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.shangyingyoupin.top/gtnwcaqagt.html

Ruby: arr.uniq
来源：http://hz.yuxming.cn/gttkkplrun.html

C#:   list.Distinct().ToList()
来源：http://hz.pycfn.com/gtgnmnojbr.html

[D16] 求和与平均值
来源：http://hz.fengsongda.top/gtievkmgyk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.shanyushiyangkeji.top/gtifzhifjf.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.guowangkeji.top/gtoqrtxkbd.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zhiwuduotai.top/gtirsddgbu.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.haohaochexian.top/gttyqjlald.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.redwolf501.top/gtwtfhlchm.html

Go:   // 手写循环累加
来源：http://hz.yj20258888.top/gtlxqwisdg.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.sysykeji.top/gtkodnuiya.html

C#:   list.Sum();  list.Average()
来源：http://hz.yueranfly.top/gtjymmpodq.html

[D17] 最大值与最小值
来源：http://hz.yonumen.top/gtrommlhpr.html

Py:   max(arr);  min(arr)
来源：http://hz.jinqigfzy.top/gtnlujntvs.html

PHP:  max($arr);  min($arr);
来源：http://hz.iojbl.cn/gtvqauxppl.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.xuanzx.com/gtmrolirqf.html

TS:   Math.max(...arr);
来源：http://hz.xuanzx.com/gtrduygvfc.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.9152youxi.cn/gtehwtqtwm.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.ydjk.org.cn/gtewytdjur.html

Ruby: arr.max;  arr.min
来源：http://hz.fzhhl.top/gtdrolhdfz.html

C#:   list.Max();  list.Min()
来源：http://hz.mhx1999.top/gtpasxdsav.html

[D18] 扁平化嵌套数组
来源：http://hz.chenjidiqi.icu/gtgsbhqapq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.yanxiufei.cn/gtqhvtkmgi.html

PHP:  array_merge(...$nested);
来源：http://hz.zdqjudy.top/gtknirpxtv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.jiagoushi.top/gtifydpwmy.html

TS:   nested.flat();
来源：http://hz.ywan-chungtsiang.top/gtxdebvvlu.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.wangshuangyany.cn/gtjetxjorw.html

Go:   // 手写双层循环
来源：http://hz.jinqigfzy.top/gtfurruqdb.html

Ruby: nested.flatten
来源：http://hz.redwolf501.top/gtkcnzeagl.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.zhoulong.xyz/gtcwbttfyg.html

[D19] 按字段分组
来源：http://hz.jqgufenzy.top/gtwvovyjky.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.xuanzx.com/gtxpudqiup.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.cqqwz.cn/gtjardrrkm.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.iojbl.cn/gttfopuwfh.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.nwbrower.top/gtwtvzozdo.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.dianchejie.cn/gtmgwsengm.html

Go:   // 手写 map[string][]T
来源：http://hz.jqgufenzy.top/gtktaapnyh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.aibaodan.cn/gtsrpakbsd.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.zhiwuduotai.top/gtmcysphwz.html

[D20] 统计每个元素出现次数
来源：http://hz.yuanzhike.top/gtjjufjyqo.html

Py:   Counter(arr)
来源：http://hz.0kj1m.cn/gtfvbiluqz.html

PHP:  array_count_values($arr);
来源：http://hz.zhaomingkeji.xyz/gtrxkmhibm.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zhengqikj.top/gthztaqhol.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.fzhhl.top/gtybgefgwp.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.jinyuanbaomall.cn/gtpeztbhmc.html

Go:   // 手写 map[T]int
来源：http://hz.hysaishi.cn/gtewsyeusj.html

Ruby: arr.tally
来源：http://hz.shzxlz.cn/gttpbplxlc.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.wangshuangyany.cn/gtywpjafgj.html

[D21] 判断是否包含某元素
来源：http://hz.pengpengdd.cyou/gtudfemaki.html

Py:   x in arr
来源：http://hz.cdnleiting.top/gttspegvbj.html

PHP:  in_array($x, $arr, true);
来源：http://hz.hysaishi.cn/gtplstkcad.html

JS:   arr.includes(x)
来源：http://hz.hywenlv.cn/gtqsiumcjz.html

TS:   arr.includes(x)
来源：http://hz.zhoulong.xyz/gtjuvixlar.html

Java: list.contains(x)
来源：http://hz.nwbrower.top/gtobcektth.html

Go:   slices.Contains(arr, x)
来源：http://hz.smart0.xyz/gtafforxgd.html

Ruby: arr.include?(x)
来源：http://hz.chenjidiqi.icu/gtndcsfmkr.html

C#:   list.Contains(x)
来源：http://hz.fzhhl.top/gttacklcso.html

[D22] 复制数组（避免共享引用）
来源：http://hz.hysaishi.cn/gtobtbojrd.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.ydjk.org.cn/gtmdndkrzd.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.xylfe.cn/gtvpqynauo.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.nanxinkj.top/gtxkembrns.html

TS:   [...arr];
来源：http://hz.iojbl.cn/gtxvrwndwi.html

Java: new ArrayList<>(list);
来源：http://hz.cheryme.top/gterjpfzka.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.fengsongda.top/gtpcaeykez.html

Ruby: arr.dup;  arr.clone
来源：http://hz.shanyushiyangkeji.top/gtwbuwgxes.html

C#:   new List<int>(list);
来源：http://hz.gzhubu.top/gtdiwkezdd.html

[D23] reduce 累积计算
来源：http://hz.chenzaomai.com/gtexmngqeg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.gzhubu.top/gtfxwylmtg.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.redwolf501.top/gttxfiuyon.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ppjwa.cn/gtbsandeoq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhixingplan.top/gtlnqwuxxx.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.jlsjyb.cn/gteshhevlp.html

Go:   // 手写循环
来源：http://hz.zhoulong.xyz/gtyxzskwfb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.cdnleiting.top/gtpeeipgjs.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.sysykeji.top/gtesirivdu.html

[D24] 字典 / Map 基本操作
来源：http://hz.ywan-chungtsiang.top/gtlhrpobsj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.ppjwa.cn/gtbdzwsykc.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.sweek.top/gtaeparlaq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.yonumen.top/gtcbhrwodu.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.xingfuxueyuan.xyz/gtkdfhriac.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.sxryk.cn/gtkuadntnf.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.xuanzx.com/gtivjnglpo.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.yuxming.cn/gtcvglclwk.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.birdmap.top/gtcahisqkd.html

[D25] Set 集合去重与交并差
来源：http://hz.ydzc1.top/gtjbmmijxq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.gzhubu.top/gtrnhiknrx.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.andypj.xyz/gtobmvgfho.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.andypj.xyz/gtpndcagpf.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.c1oappe.top/gtqcohwwvb.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.snrcjt.cn/gtxeabetsp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.havefunace.top/gtdrjixxue.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.havefunace.top/gtsdzwlrjd.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.hongshengwenyu.top/gtwofwdxzy.html

[D26] 数组转字符串
来源：http://hz.ehwqpu.com/gtksbksbui.html

Py:   ", ".join(map(str, arr))
来源：http://hz.yuanzhike.top/gtotgsdbyr.html

PHP:  implode(", ", $arr);
来源：http://hz.daria6918.cn/gtcxmusbcy.html

JS:   arr.join(", ")
来源：http://hz.52xcode.cn/gtvixyqpsa.html

TS:   arr.join(", ")
来源：http://hz.ydjk.org.cn/gtcdeofnnh.html

Java: String.join(", ", list)
来源：http://hz.aizwys.cn/gtzgdbwxlg.html

Go:   strings.Join(strs, ", ")
来源：http://hz.hfpthk.cn/gtkmswxbow.html

Ruby: arr.join(", ")
来源：http://hz.52xcode.cn/gtjtnyjxzm.html

C#:   string.Join(", ", list)
来源：http://hz.mhx1999.top/gtduifqqou.html

================================================================================
来源：http://hz.xylfe.cn/gtjxtnptkf.html

E. 字符串处理
来源：http://hz.mhx1999.top/gthsxkwkyl.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtkuuadbev.html

[E01] 拼接字符串
来源：http://hz.yj202588.top/gtltiqarsk.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.jqgfzy.top/gtgqlvzokl.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.ehwqpu.com/gtamexhfug.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.kuanghao11.cn/gtqebsgrnf.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.316326.xyz/gtruvmtzuy.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.tianlin.xyz/gtzirrktrw.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.aizwys.cn/gtglimjlbq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.hywenlv.cn/gtzcfmozeo.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.redwolf501.top/gtbbbjnwbo.html

[E02] 重复字符串
来源：http://hz.sxryk.cn/gtjackfrir.html

Py:   "ab" * 3
来源：http://hz.hammf.cn/gtufburvcr.html

PHP:  str_repeat("ab", 3);
来源：http://hz.yj202588.top/gtqnzwowst.html

JS:   "ab".repeat(3)
来源：http://hz.zhiwuduotai.top/gtnpqvzjgb.html

TS:   "ab".repeat(3)
来源：http://hz.hammf.cn/gtfmtaddoy.html

Java: "ab".repeat(3)
来源：http://hz.jinqigfzy.top/gtncsmrapq.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.fzhhl.top/gtfslmqwcd.html

Ruby: "ab" * 3
来源：http://hz.yuanzhike.top/gtjqyoocwq.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.zhixingplan.top/gtnrmnrmnp.html

[E03] 截取子串
来源：http://hz.hnxiangtu.top/gtlgsowout.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.havefunace.top/gtstpopzlo.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.sweek.top/gtibeuwzfi.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.jyoumei.cn/gtbobrvhov.html

TS:   s.slice(1, 4)
来源：http://hz.ydzc1.top/gtgkhyxfyv.html

Java: s.substring(1, 4)
来源：http://hz.nanxuanxn.top/gtflyfqlkq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.yvedp.cn/gtgrqsdwmb.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.cashguo.top/gtkwmkdfay.html

C#:   s.Substring(1, 3)
来源：http://hz.cashguo.top/gtghimloea.html

[E04] 查找子串位置
来源：http://hz.jinyuanbaomall.cn/gthmateorr.html

Py:   s.find("x");  s.index("x")
来源：http://hz.xingfuxueyuan.xyz/gtdtneepzy.html

PHP:  strpos($s, "x");
来源：http://hz.aizwys.cn/gtrowgywcq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.jlsjyb.cn/gtvkrorqfw.html

TS:   s.indexOf("x")
来源：http://hz.svipenyu.cn/gtrthodpdo.html

Java: s.indexOf("x")
来源：http://hz.yanxiufei.cn/gtisvqmfgl.html

Go:   strings.Index(s, "x")
来源：http://hz.cheryme.top/gttwqvrztm.html

Ruby: s.index("x")
来源：http://hz.shanyushiyangkeji.top/gtzqymurbe.html

C#:   s.IndexOf("x")
来源：http://hz.snrcjt.cn/gtojoqbtnj.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.andypj.xyz/gtlvimloxd.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.zhixingplan.top/gtyguifqla.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.pycfn.com/gtrizogcco.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zhijiandao.cn/gtleyorlqs.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.haohaochexian.top/gtjfiauaag.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.xuetiantiany.cn/gtwseeewao.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.gzhubu.top/gtuyhnzdsj.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.hfpthk.cn/gtpkrxqgqc.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.xziqi.cn/gtiioebgob.html

[E06] 替换子串
来源：http://hz.yj20258.top/gtmllsgefe.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.jinghuilouyu.cn/gtnchjfamm.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.hongshengwenyu.top/gtxeukgbbs.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.mhx1999.top/gtsotlqglu.html

TS:   s.replaceAll("a", "b")
来源：http://hz.zhaomingkeji.xyz/gtqobpksag.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.9152youxi.cn/gthydjnbmr.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.zhoulong.xyz/gtgwxvbolo.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.zycfv.cn/gtkarzqnii.html

C#:   s.Replace("a", "b")
来源：http://hz.hfpthk.cn/gtnipbridx.html

[E07] 按分隔符拆分
来源：http://hz.fengsongda.top/gtpcbewjab.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.guowangkeji.top/gtwxeimzky.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.guowangkeji.top/gtgvhggbfh.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.feifeiyinyue.top/gtmuayjwir.html

TS:   s.split(",")
来源：http://hz.yvedp.cn/gtwstbvmev.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.gogol.net.cn/gtochzazyu.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.svipenyu.cn/gtwotfeipg.html

Ruby: s.split(",");  s.split
来源：http://hz.birdmap.top/gtlnwfyevc.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.guowangkeji.top/gtosligrzs.html

[E08] 数组按分隔符合并
来源：http://hz.52xcode.cn/gthdvhnfox.html

Py:   ",".join(items)
来源：http://hz.hywenlv.cn/gttuwahrjy.html

PHP:  implode(",", $items);
来源：http://hz.hnxiangtu.top/gtyhxqkkhn.html

JS:   items.join(",")
来源：http://hz.pengpengdd.cyou/gtzkwtrcuk.html

TS:   items.join(",")
来源：http://hz.guowangkeji.top/gthgozpgvc.html

Java: String.join(",", items)
来源：http://hz.9152youxi.cn/gtenqvcezm.html

Go:   strings.Join(items, ",")
来源：http://hz.ywan-chungtsiang.top/gtcolbmqbi.html

Ruby: items.join(",")
来源：http://hz.guowangkeji.top/gtiygtypdz.html

C#:   string.Join(",", items)
来源：http://hz.cashguo.top/gtphtgoyub.html

[E09] 去除所有空白字符
来源：http://hz.jinyuanbaomall.cn/gtwuzyztzs.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.sysykeji.top/gttkuudxjj.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.zhiwuduotai.top/gtodplmpqi.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.hywenlv.cn/gtqbcmwzxs.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.yj20258888.top/gtblrtpajy.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.tanke756.top/gtoxsshjrl.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.daxiang520.top/gtsxrmorzg.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.quarkkingdee.top/gttzhlycui.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.guannengcc.top/gttfmpxukg.html

[E10] 左侧补零 / 定长填充
来源：http://hz.pycfn.com/gtdhhpbxko.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.shanyushiyangtech.top/gtnzvjbzxk.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.yanxiufei.cn/gtsvxzmcls.html

JS:   "7".padStart(3, "0")
来源：http://hz.mhx1999.top/gtsouvekdn.html

TS:   "7".padStart(3, "0")
来源：http://hz.hywenlv.cn/gtpisnizrv.html

Java: String.format("%03d", 7)
来源：http://hz.daria6918.cn/gtcajuqovx.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.smart0.xyz/gtfqmfbfwp.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.xuanzx.com/gtknifiydn.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.c1oappe.top/gtrfgpgvov.html

[E11] 反转字符串
来源：http://hz.yonumen.top/gtojeygweu.html

Py:   s[::-1]
来源：http://hz.jinqigufen.top/gtldtudgao.html

PHP:  strrev($s);
来源：http://hz.yongpay.top/gtgfowjcmd.html

JS:   [...s].reverse().join("")
来源：http://hz.yongpay.top/gtumxfmect.html

TS:   [...s].reverse().join("")
来源：http://hz.jinqigfzy.top/gtpxceisua.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.dashuyun.cn/gtaefzvkmx.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.nwbrower.top/gtjhshqxyk.html

Ruby: s.reverse
来源：http://hz.yangfankeji.com/gtholyjwzr.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.yj202588.top/gtnjkqnfkv.html

[E12] 统计某字符出现次数
来源：http://hz.hfpthk.cn/gtilvbqdsf.html

Py:   s.count("a")
来源：http://hz.chenjidiqi.icu/gtwzlbikzl.html

PHP:  substr_count($s, "a");
来源：http://hz.sufxvd.cn/gtybznqeuu.html

JS:   s.split("a").length - 1
来源：http://hz.xingfuxueyuan.xyz/gtnuaopfdt.html

TS:   s.split("a").length - 1
来源：http://hz.wangdashe.top/gtixkpudtz.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.xylfe.cn/gtbiusrjtr.html

Go:   strings.Count(s, "a")
来源：http://hz.haohaochexian.top/gtgtduelqu.html

Ruby: s.count("a")
来源：http://hz.guowangkeji.top/gtyramxtrm.html

C#:   s.Count(c => c == 'a')
来源：http://hz.jianghu66.top/gtkzxnxglk.html

[E13] 逐字符遍历
来源：http://hz.316326.xyz/gtrqvgxgif.html

Py:   for ch in s: print(ch)
来源：http://hz.sysykeji.top/gtbriiiqmv.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.shuidangran.top/gtszksassb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.svipenyu.cn/gttvgwrdtb.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.birdmap.top/gtjtmnkfnd.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.jqgfzy.top/gtxliikouc.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.ydzc1.top/gtxdbyqaje.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.yj20258888.top/gtzrrofxok.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.smart0.xyz/gtjezykpcd.html

[E14] URL 编码与 Base64
来源：http://hz.ehwqpu.com/gthxlokfmt.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.zhoulong.xyz/gtkmllguii.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.sxryk.cn/gtjsrlxscw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.cucudq.cn/gtionfjfqi.html


<!-- 参考信息 -->