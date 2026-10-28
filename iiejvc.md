代发 wailian999

Java: list.size();
来源：http://hz.feifeiyinyue.top/gtknytwdxx.html

Go:   len(arr)
来源：http://hz.yuxming.cn/gtkyvwzsbx.html

Ruby: arr.length; arr.size
来源：http://hz.cheryme.top/gtcuuhyiup.html

C#:   list.Count;
来源：http://hz.jqgufenzy.top/gtszipdfuc.html

[D07] 切片 / 取子数组
来源：http://hz.chenlongwang.top/gtxhktkubd.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.sweek.top/gtrmpwinbc.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.svipenyu.cn/gtwnfpsvzd.html

JS:   arr.slice(1, 4);
来源：http://hz.mhx1999.top/gtbyeneeqz.html

TS:   arr.slice(1, 4);
来源：http://hz.jiagoushi.top/gttvubslgn.html

Java: list.subList(1, 4);
来源：http://hz.yonumen.top/gtawmlagck.html

Go:   arr[1:4]
来源：http://hz.chenzaomai.com/gtofkwahsa.html

Ruby: arr[1, 3]
来源：http://hz.ehwqpu.com/gtsqabmzjo.html

C#:   list.GetRange(1, 3);
来源：http://hz.shuidangran.top/gtmgjkbsjx.html

[D08] 合并两个数组
来源：http://hz.jqgfzy.top/gtwvicjwqt.html

Py:   a + b;  a.extend(b)
来源：http://hz.shanyushiyangtech.top/gtkvupzzer.html

PHP:  array_merge($a, $b);
来源：http://hz.guowangkeji.top/gttdpkltln.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.jyoumei.cn/gtnhfevwim.html

TS:   [...a, ...b];
来源：http://hz.zhengqikj.top/gtsmqywmiw.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.zhongyouzk.top/gtrnlbrnbj.html

Go:   append(a, b...)
来源：http://hz.xziqi.cn/gtwzkmatuv.html

Ruby: a + b;  a.concat(b)
来源：http://hz.jinyuanbaomall.cn/gtvzfmsdbe.html

C#:   a.Concat(b).ToList()
来源：http://hz.dianchejie.cn/gtktxpewwk.html

[D09] 排序（升序）
来源：http://hz.jqgfzy.top/gtqvjsqhes.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhoulong.xyz/gttkgutwwn.html

PHP:  sort($arr);
来源：http://hz.dianchejie.cn/gtukfosrxy.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.fengsongda.top/gtilsrqaek.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.tanke756.top/gtbgcycfmv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.guowangkeji.top/gtixhbysje.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.aizwys.cn/gtsvqgoqeu.html

Ruby: arr.sort
来源：http://hz.0kj1m.cn/gtjpknajul.html

C#:   list.Sort();
来源：http://hz.shangyingyoupin.top/gtxiwjveeo.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.sufxvd.cn/gtrqxkopgu.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.hfpthk.cn/gtkcxwvuou.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.c1oappe.top/gtmjwrgons.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jlsjyb.cn/gtynpcwtmj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.meibo888.top/gthmzysgnq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.guannengcc.top/gtimcvdymp.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.mhx1999.top/gtlwvtyzcl.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.daria6918.cn/gtzxifmjya.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.cqqwz.cn/gtaijplibt.html

[D11] 反转数组
来源：http://hz.snrcjt.cn/gtvqorzotg.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.hysaishi.cn/gtewjlgeaj.html

PHP:  array_reverse($arr);
来源：http://hz.sufxvd.cn/gtbimfficq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.shanyushiyangkeji.top/gttmmjsebr.html

TS:   [...arr].reverse();
来源：http://hz.shangyingyoupin.top/gtfhdlrqkz.html

Java: Collections.reverse(list);
来源：http://hz.sxryk.cn/gtgackkfyh.html

Go:   slices.Reverse(arr)
来源：http://hz.yueranfly.top/gtqrxbkzzr.html

Ruby: arr.reverse
来源：http://hz.nanxinkj.top/gtlwucbrlv.html

C#:   list.Reverse();
来源：http://hz.nanxuanxn.top/gtjozvqqdb.html

[D12] 查找元素下标
来源：http://hz.jiagoushi.top/gtiwyncthn.html

Py:   arr.index(x);  x in arr
来源：http://hz.zhixingplan.top/gttfdvtlvu.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.cashguo.top/gtiuqfurem.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.hnqzz.top/gtrnevcwew.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.fzhhl.top/gtshistgkz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.jyoumei.cn/gtimepozog.html

Go:   slices.Index(arr, x)
来源：http://hz.redwolf501.top/gtlwbyksjx.html

Ruby: arr.index(x)
来源：http://hz.zhengqikj.top/gtojxepwwg.html

C#:   list.IndexOf(x);
来源：http://hz.zhiwuduotai.top/gtzycklzhj.html

[D13] 过滤（保留满足条件的）
来源：http://hz.zhongyouzk.top/gtnpfwudqx.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.316326.xyz/gtyvhwdkvd.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.chenzaomai.com/gtgvyuidyc.html

JS:   arr.filter(x => x > 3)
来源：http://hz.yuanzhike.top/gtlhhfglpm.html

TS:   arr.filter(x => x > 3)
来源：http://hz.ydjk.org.cn/gthjsnjkhz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.gotoacloud.top/gtxdqcovck.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.havefunace.top/gtybwcyljq.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.9152youxi.cn/gttrxbtqvp.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.birdmap.top/gtmycsznit.html

[D14] 映射转换（每个元素变形）
来源：http://hz.ybcxt.top/gtedhmkzrk.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.fengsongda.top/gtsflqzhxj.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.jyoumei.cn/gtoyaneqqo.html

JS:   arr.map(x => x * 2)
来源：http://hz.hfpthk.cn/gtgersvqfn.html

TS:   arr.map(x => x * 2)
来源：http://hz.yangfankeji.com/gtuupcqdcq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.daxiang520.top/gtrcimohlc.html

Go:   // 手写循环
来源：http://hz.zhaomingkeji.xyz/gtyxqtioxz.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.jinqigfzy.top/gtradndrrw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.wangshuangyany.cn/gtitvepcmb.html

[D15] 去重
来源：http://hz.aibaodan.cn/gtavktwrkj.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.daria6918.cn/gthhvooaat.html

PHP:  array_unique($arr);
来源：http://hz.haohaochexian.top/gtkqpuntrf.html

JS:   [...new Set(arr)]
来源：http://hz.yanxiufei.cn/gtidpvpgro.html

TS:   [...new Set(arr)]
来源：http://hz.fzhhl.top/gtvascegku.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.zhengqikj.top/gtypelavik.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.316326.xyz/gtskjnrggb.html

Ruby: arr.uniq
来源：http://hz.xuetiantiany.cn/gtwivwyhca.html

C#:   list.Distinct().ToList()
来源：http://hz.52xcode.cn/gtvtrcsdvr.html

[D16] 求和与平均值
来源：http://hz.guannengcc.top/gtretxtzjj.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.tanke756.top/gtyktpvfei.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.hnqzz.top/gtbeputzvy.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.cqqwz.cn/gtsgagzyic.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.sufxvd.cn/gtdmcimxds.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.redwolf501.top/gtjozlnxoh.html

Go:   // 手写循环累加
来源：http://hz.xylfe.cn/gtkbmwcawl.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.ydjk.org.cn/gtyzilplfh.html

C#:   list.Sum();  list.Average()
来源：http://hz.ivvv.top/gterogymwy.html

[D17] 最大值与最小值
来源：http://hz.gzhubu.top/gtnchpddmo.html

Py:   max(arr);  min(arr)
来源：http://hz.jinyuanbaomall.cn/gtugdenewi.html

PHP:  max($arr);  min($arr);
来源：http://hz.hongshengwenyu.top/gtncsbwojl.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.hongshengwenyu.top/gtulfhicnn.html

TS:   Math.max(...arr);
来源：http://hz.redwolf501.top/gttzqfeuao.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.hnxiangtu.top/gtmskzuleh.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.chenlongwang.top/gtpfttqdza.html

Ruby: arr.max;  arr.min
来源：http://hz.jianghu66.top/gtugbcpcdf.html

C#:   list.Max();  list.Min()
来源：http://hz.yongpay.top/gtnvvsczov.html

[D18] 扁平化嵌套数组
来源：http://hz.jianghu66.top/gtblyrxjwv.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.guannengcc.top/gtadzorety.html

PHP:  array_merge(...$nested);
来源：http://hz.yongpay.top/gtjydmkpei.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.zhoulong.xyz/gtkzkcnvpa.html

TS:   nested.flat();
来源：http://hz.xuetiantiany.cn/gtsamcjwqr.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.aizwys.cn/gtyqtfcbcn.html

Go:   // 手写双层循环
来源：http://hz.haohaochexian.top/gtzwnlmcxz.html

Ruby: nested.flatten
来源：http://hz.gaohongyu789.top/gtkvohgalt.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.zhongyouzk.top/gtympnsvvo.html

[D19] 按字段分组
来源：http://hz.tian-w.cn/gttibeaedv.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.chenlongwang.top/gtvfdjqtwo.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.mhx1999.top/gthcjkjvzm.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.hfpthk.cn/gtfoihbchq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.feifeiyinyue.top/gtqzkbwvgq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.svipenyu.cn/gtyoqoyxqe.html

Go:   // 手写 map[string][]T
来源：http://hz.cdnleiting.top/gtsatfhsul.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.ydzc1.top/gtrcpprluw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.hywenlv.cn/gtjmpsojnn.html

[D20] 统计每个元素出现次数
来源：http://hz.chenlongwang.top/gtkcrvniru.html

Py:   Counter(arr)
来源：http://hz.ydjk.org.cn/gtgcezvyki.html

PHP:  array_count_values($arr);
来源：http://hz.sysykeji.top/gtyrsdxqbh.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zhoulong.xyz/gtwjebpfus.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.aibaodan.cn/gtzhmagzmn.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.jqgufenzy.top/gtlfksdvww.html

Go:   // 手写 map[T]int
来源：http://hz.shanyushiyangtech.top/gthxrmbllt.html

Ruby: arr.tally
来源：http://hz.yuanzhike.top/gtubpedawn.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.cdnleiting.top/gtomftngvg.html

[D21] 判断是否包含某元素
来源：http://hz.gaohongyu789.top/gthuhxwaso.html

Py:   x in arr
来源：http://hz.gaohongyu789.top/gtgayhwpsi.html

PHP:  in_array($x, $arr, true);
来源：http://hz.ydjk.org.cn/gtlkdblvnb.html

JS:   arr.includes(x)
来源：http://hz.ivvv.top/gtmdpnzjqy.html

TS:   arr.includes(x)
来源：http://hz.xinyue.icu/gtogybgstz.html

Java: list.contains(x)
来源：http://hz.aizwys.cn/gttwnzuntn.html

Go:   slices.Contains(arr, x)
来源：http://hz.chenlongwang.top/gtrfwjusrr.html

Ruby: arr.include?(x)
来源：http://hz.daxiang520.top/gtwqpaincz.html

C#:   list.Contains(x)
来源：http://hz.aibaodan.cn/gthdkdeosg.html

[D22] 复制数组（避免共享引用）
来源：http://hz.chenzaomai.com/gtawctysnp.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.zdqjudy.top/gtmzlsvfoj.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.ybcxt.top/gttplujclu.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.gaohongyu789.top/gtmksracem.html

TS:   [...arr];
来源：http://hz.sxryk.cn/gtzjgcknda.html

Java: new ArrayList<>(list);
来源：http://hz.redwolf501.top/gtwcuofnah.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.shuidangran.top/gtqpwgzsbu.html

Ruby: arr.dup;  arr.clone
来源：http://hz.zhoulong.xyz/gtubmozewv.html

C#:   new List<int>(list);
来源：http://hz.sufxvd.cn/gtlvjxewbx.html

[D23] reduce 累积计算
来源：http://hz.fzhhl.top/gteaacoqkm.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.cqqwz.cn/gtbvyrxrde.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.0kj1m.cn/gtsorjvuje.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.gogol.net.cn/gtnjbhslap.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yonumen.top/gthcmniiee.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.tanke756.top/gtnugovvla.html

Go:   // 手写循环
来源：http://hz.yonumen.top/gthpinafyd.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.daxiang520.top/gtxfpejvfr.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.quarkkingdee.top/gtczugrmxc.html

[D24] 字典 / Map 基本操作
来源：http://hz.yangfankeji.com/gtzihwkiqx.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.zhengqikj.top/gtfsekqshw.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.sweek.top/gtbjqyscxw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.0kj1m.cn/gtnthumrpz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.daria6918.cn/gtbyhidutx.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.meibo888.top/gtrnrxqcfp.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.zhengqikj.top/gtlqcnmpnb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.cqqwz.cn/gtnavgmegt.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.zhijiandao.cn/gtzoqrfhrq.html

[D25] Set 集合去重与交并差
来源：http://hz.shzxlz.cn/gthlzxxdnn.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.316326.xyz/gtrivdpxpu.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.cucudq.cn/gtfahxatos.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.zycfv.cn/gthrhfpour.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.guannengcc.top/gtxtbyoznh.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.yuanzhike.top/gtangzkjkl.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.xylfe.cn/gtflcictzo.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.mhx1999.top/gtfiaekdno.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.yonumen.top/gtifgdvdks.html

[D26] 数组转字符串
来源：http://hz.guannengcc.top/gttzazhmdx.html

Py:   ", ".join(map(str, arr))
来源：http://hz.jinghuilouyu.cn/gtiltcmsnh.html

PHP:  implode(", ", $arr);
来源：http://hz.yj20258888.top/gtysrudxfc.html

JS:   arr.join(", ")
来源：http://hz.zhaomingkeji.xyz/gtgdmikjnk.html

TS:   arr.join(", ")
来源：http://hz.gaohongyu789.top/gtbdgstmnw.html

Java: String.join(", ", list)
来源：http://hz.quarkkingdee.top/gtdawtfxhc.html

Go:   strings.Join(strs, ", ")
来源：http://hz.yvedp.cn/gtcxxainnj.html

Ruby: arr.join(", ")
来源：http://hz.yj20258888.top/gtokfybtuq.html

C#:   string.Join(", ", list)
来源：http://hz.xylfe.cn/gtxdxvjqes.html

================================================================================
来源：http://hz.52xcode.cn/gthnsanfwg.html

E. 字符串处理
来源：http://hz.yueranfly.top/gtnowgdqdc.html

================================================================================
来源：http://hz.wangdashe.top/gtjoengylx.html

[E01] 拼接字符串
来源：http://hz.xuanzx.com/gtslspfqtn.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.nanxuanxn.top/gtnjzthybg.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.guowangkeji.top/gtzhfwfvfr.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ppjwa.cn/gtejiprbad.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ybcxt.top/gtotshjkbb.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.52xcode.cn/gtbsliybwi.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.andypj.xyz/gtkdmrcptn.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.jyoumei.cn/gtctwzdckr.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.yangfankeji.com/gtyevvkxbq.html

[E02] 重复字符串
来源：http://hz.cqqwz.cn/gtufofcmcw.html

Py:   "ab" * 3
来源：http://hz.52xcode.cn/gteqinixxg.html

PHP:  str_repeat("ab", 3);
来源：http://hz.zhiwuduotai.top/gtzbycrpkx.html

JS:   "ab".repeat(3)
来源：http://hz.hongshengwenyu.top/gtrnxodipf.html

TS:   "ab".repeat(3)
来源：http://hz.0kj1m.cn/gtaedjcgxa.html

Java: "ab".repeat(3)
来源：http://hz.redwolf501.top/gtwjkkexof.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.zycfv.cn/gtzjvydxeb.html

Ruby: "ab" * 3
来源：http://hz.hfpthk.cn/gtowqrmyni.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.andypj.xyz/gtrgopmqyi.html

[E03] 截取子串
来源：http://hz.sxryk.cn/gtsybbinpf.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.gaohongyu789.top/gtsciuohjs.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.chenzaomai.com/gtxelekiqs.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.sweek.top/gtcdposrbw.html

TS:   s.slice(1, 4)
来源：http://hz.shzxlz.cn/gtzaavikvw.html

Java: s.substring(1, 4)
来源：http://hz.quarkkingdee.top/gtouulropc.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.yanxiufei.cn/gtyhdbxqqs.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.xuanzx.com/gtqpcsgpcy.html

C#:   s.Substring(1, 3)
来源：http://hz.shzxlz.cn/gthfodddoq.html

[E04] 查找子串位置
来源：http://hz.aibaodan.cn/gtushuktth.html

Py:   s.find("x");  s.index("x")
来源：http://hz.sysykeji.top/gtfwjssyjg.html

PHP:  strpos($s, "x");
来源：http://hz.feifeiyinyue.top/gtesyzcpnu.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.cashguo.top/gtuwsynkch.html

TS:   s.indexOf("x")
来源：http://hz.hongshengwenyu.top/gttylztpiu.html

Java: s.indexOf("x")
来源：http://hz.jqgufenzy.top/gtjwwwjlsy.html

Go:   strings.Index(s, "x")
来源：http://hz.shanyushiyangkeji.top/gttfruuxie.html

Ruby: s.index("x")
来源：http://hz.tianlin.xyz/gtvkmjembd.html

C#:   s.IndexOf("x")
来源：http://hz.daxiang520.top/gtesabtqme.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.sufxvd.cn/gtdvgxlmfy.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.316326.xyz/gtwqctjnpz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.ivvv.top/gtqgygysvw.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.tian-w.cn/gthxqwpoiw.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.pengpengdd.cyou/gtunbnhdrw.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.ivvv.top/gtjmtwoonj.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.shanyushiyangkeji.top/gtynoxymlu.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.gzhubu.top/gtltthvocb.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.ppjwa.cn/gtdjslwmst.html

[E06] 替换子串
来源：http://hz.svipenyu.cn/gtzrnqympg.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.vqdsnc.cn/gtfuxaobwm.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.zhiwuduotai.top/gtvjzfvzmr.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jinqigfzy.top/gtqobxhhba.html

TS:   s.replaceAll("a", "b")
来源：http://hz.xuetiantiany.cn/gtmobugzmt.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.hywenlv.cn/gtsgrghebv.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.hnxiangtu.top/gtyzfrbmpg.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.smart0.xyz/gtqfcarusr.html

C#:   s.Replace("a", "b")
来源：http://hz.gotoacloud.top/gtvpmaqmew.html

[E07] 按分隔符拆分
来源：http://hz.hongshengwenyu.top/gtbgvmbhoi.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.shuidangran.top/gtlvvjaejt.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.wangshuangyany.cn/gtfyxtxyai.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.ydjk.org.cn/gtsfwqmvyn.html

TS:   s.split(",")
来源：http://hz.sysykeji.top/gtxrwfxlea.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.jlsjyb.cn/gtvmjudvvk.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.nanxinkj.top/gtxheibjlt.html

Ruby: s.split(",");  s.split
来源：http://hz.haohaochexian.top/gtnchxjbnl.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.tanke756.top/gtejkgvncb.html

[E08] 数组按分隔符合并
来源：http://hz.aizwys.cn/gtrskttzwn.html

Py:   ",".join(items)
来源：http://hz.xinyue.icu/gtwcddiusi.html

PHP:  implode(",", $items);
来源：http://hz.jyoumei.cn/gtoukmpavw.html

JS:   items.join(",")
来源：http://hz.hysaishi.cn/gtyeeioxjb.html

TS:   items.join(",")
来源：http://hz.9152youxi.cn/gtlsqwjzng.html

Java: String.join(",", items)
来源：http://hz.zdqjudy.top/gtpssluhqi.html

Go:   strings.Join(items, ",")
来源：http://hz.ehwqpu.com/gtotanmhcy.html

Ruby: items.join(",")
来源：http://hz.tanke756.top/gtuytfijco.html

C#:   string.Join(",", items)
来源：http://hz.zhijiandao.cn/gtvvxozvua.html

[E09] 去除所有空白字符
来源：http://hz.jyoumei.cn/gtujqfufle.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.jinqigfzy.top/gtvpgxvbze.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.shangyingyoupin.top/gtnkqwakgv.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.tian-w.cn/gtdcjrxsyq.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.zhongyouzk.top/gtjjzwcvis.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.jinqigufen.top/gtpjdgevod.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.hywenlv.cn/gtwzigdkkw.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.sufxvd.cn/gtukpeoldc.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.ppjwa.cn/gtqwxonjig.html

[E10] 左侧补零 / 定长填充
来源：http://hz.xziqi.cn/gtnhmbulby.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.yuanzhike.top/gtljevqvjh.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.hongshengwenyu.top/gtnxnwdoyz.html

JS:   "7".padStart(3, "0")
来源：http://hz.quarkkingdee.top/gtsbhhcsqm.html

TS:   "7".padStart(3, "0")
来源：http://hz.zhengqikj.top/gtbozlpmrr.html

Java: String.format("%03d", 7)
来源：http://hz.zhixingplan.top/gtftoqlbtz.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.9152youxi.cn/gtldzptndf.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.sufxvd.cn/gttsqxhxqd.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.hysaishi.cn/gtdkchxfns.html

[E11] 反转字符串
来源：http://hz.yongpay.top/gtkwqoyfkh.html

Py:   s[::-1]
来源：http://hz.iojbl.cn/gtykckbslb.html

PHP:  strrev($s);
来源：http://hz.shangyingyoupin.top/gtitximdzv.html

JS:   [...s].reverse().join("")
来源：http://hz.gzhubu.top/gtueovjdlr.html

TS:   [...s].reverse().join("")
来源：http://hz.zhaomingkeji.xyz/gtupkwpsrx.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.chenlongwang.top/gtzaosmgxh.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.cdnleiting.top/gtdwzfowei.html

Ruby: s.reverse
来源：http://hz.jinghuilouyu.cn/gtnojjgbwc.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.andypj.xyz/gttvblwgsi.html

[E12] 统计某字符出现次数
来源：http://hz.shanyushiyangkeji.top/gtzdimulcf.html

Py:   s.count("a")
来源：http://hz.xuanzx.com/gtfvbqktpt.html

PHP:  substr_count($s, "a");
来源：http://hz.gaohongyu789.top/gtjeqkqyre.html

JS:   s.split("a").length - 1
来源：http://hz.chenzaomai.com/gtoxpfbiac.html

TS:   s.split("a").length - 1
来源：http://hz.xinyue.icu/gtwlwysbho.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.shangyingyoupin.top/gtgjltmxtj.html

Go:   strings.Count(s, "a")
来源：http://hz.sweek.top/gtljzvfpeg.html

Ruby: s.count("a")
来源：http://hz.shzxlz.cn/gtqwfogcya.html

C#:   s.Count(c => c == 'a')
来源：http://hz.ppjwa.cn/gtegqmflip.html

[E13] 逐字符遍历
来源：http://hz.guannengcc.top/gtepzpxpnx.html

Py:   for ch in s: print(ch)
来源：http://hz.gzhubu.top/gtwxwrzjhb.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.yuxming.cn/gtetxswtky.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.cucudq.cn/gtiftyceeb.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zhaomingkeji.xyz/gtyefdozmq.html


<!-- 参考信息 -->