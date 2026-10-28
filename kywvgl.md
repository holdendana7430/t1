代发 wailian999

TS:   arr.slice(1, 4);
来源：http://hz.nanxuanxn.top/gtqoyecwvr.html

Java: list.subList(1, 4);
来源：http://hz.smart0.xyz/gtnfaoovvi.html

Go:   arr[1:4]
来源：http://hz.aibaodan.cn/gtovwtviuh.html

Ruby: arr[1, 3]
来源：http://hz.hnxiangtu.top/gtetobwbpd.html

C#:   list.GetRange(1, 3);
来源：http://hz.yangfankeji.com/gtemnmswuq.html

[D08] 合并两个数组
来源：http://hz.nanxuanxn.top/gtmchrhfew.html

Py:   a + b;  a.extend(b)
来源：http://hz.jinyuanbaomall.cn/gtatszpdbx.html

PHP:  array_merge($a, $b);
来源：http://hz.shzxlz.cn/gtystblarp.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.jinghuilouyu.cn/gtorpohvet.html

TS:   [...a, ...b];
来源：http://hz.gotoacloud.top/gthrwatxff.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.daria6918.cn/gteyrvjjbc.html

Go:   append(a, b...)
来源：http://hz.sweek.top/gthurulcrm.html

Ruby: a + b;  a.concat(b)
来源：http://hz.aizwys.cn/gtrmvynbzr.html

C#:   a.Concat(b).ToList()
来源：http://hz.gogol.net.cn/gtalscihpg.html

[D09] 排序（升序）
来源：http://hz.bjfxy.top/gttdjmjyta.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.cucudq.cn/gtcnugllkq.html

PHP:  sort($arr);
来源：http://hz.zhongyouzk.top/gtbesgrnfw.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.nanxuanxn.top/gtpuldnhnh.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.jiagoushi.top/gtphcmxivp.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.yj202588.top/gtemoxskib.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.aizwys.cn/gtngckcvfm.html

Ruby: arr.sort
来源：http://hz.ehwqpu.com/gtklgcjyaf.html

C#:   list.Sort();
来源：http://hz.gaohongyu789.top/gttzwkxtxh.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.xylfe.cn/gtcdpwmctu.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.jianghu66.top/gtsjavfyyd.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yj20258.top/gtfcyhhkuj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xziqi.cn/gtivullbqj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.shangyingyoupin.top/gtejkskbff.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.jiagoushi.top/gtszojlzje.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.cashguo.top/gtizzonotl.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.aizwys.cn/gttpvmectp.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.kuanghao11.cn/gtgqdnyejj.html

[D11] 反转数组
来源：http://hz.gotoacloud.top/gtiroqkujs.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.zhongyouzk.top/gttkkitctl.html

PHP:  array_reverse($arr);
来源：http://hz.daria6918.cn/gtmmlrhhlj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.zhongyouzk.top/gtglqipccd.html

TS:   [...arr].reverse();
来源：http://hz.yongpay.top/gtlgjgfepx.html

Java: Collections.reverse(list);
来源：http://hz.xziqi.cn/gtwbjkeblc.html

Go:   slices.Reverse(arr)
来源：http://hz.cashguo.top/gtuzizodap.html

Ruby: arr.reverse
来源：http://hz.cheryme.top/gtcscmpaom.html

C#:   list.Reverse();
来源：http://hz.xingfuxueyuan.xyz/gtjjoslcsf.html

[D12] 查找元素下标
来源：http://hz.52xcode.cn/gtqqqnefap.html

Py:   arr.index(x);  x in arr
来源：http://hz.yj20258888.top/gttrzvvfad.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.ppjwa.cn/gtxnipfjvm.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yuanzhike.top/gtcdqehlfz.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.meibo888.top/gtzsglrwpd.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.zhongyouzk.top/gtywshfmuu.html

Go:   slices.Index(arr, x)
来源：http://hz.xinyue.icu/gtvbnutebr.html

Ruby: arr.index(x)
来源：http://hz.iojbl.cn/gtcrczsqgu.html

C#:   list.IndexOf(x);
来源：http://hz.haohaochexian.top/gtrkxgofiq.html

[D13] 过滤（保留满足条件的）
来源：http://hz.316326.xyz/gtapociqyc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.cashguo.top/gtvlbcapvw.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.hywenlv.cn/gtwwflfnpz.html

JS:   arr.filter(x => x > 3)
来源：http://hz.52xcode.cn/gtzydapsbq.html

TS:   arr.filter(x => x > 3)
来源：http://hz.redwolf501.top/gtsbbojrqy.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.yj20258.top/gtmkynflee.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.ehwqpu.com/gtqfllbxan.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.yangfankeji.com/gtissfjzbz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.cqqwz.cn/gtjwzrjaud.html

[D14] 映射转换（每个元素变形）
来源：http://hz.ybcxt.top/gtovmuuesa.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.yongpay.top/gteijhxcwk.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.shuidangran.top/gtfleuozrj.html

JS:   arr.map(x => x * 2)
来源：http://hz.shanyushiyangkeji.top/gtcctcwvri.html

TS:   arr.map(x => x * 2)
来源：http://hz.hywenlv.cn/gtpixeoomh.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.cheryme.top/gtgmhszczt.html

Go:   // 手写循环
来源：http://hz.cdnleiting.top/gtuijdxnaz.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.0kj1m.cn/gtuqssulvw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.fengsongda.top/gtaionrjcq.html

[D15] 去重
来源：http://hz.xylfe.cn/gtenawfkza.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.ehwqpu.com/gtjdtwegma.html

PHP:  array_unique($arr);
来源：http://hz.yanxiufei.cn/gtafehjgvv.html

JS:   [...new Set(arr)]
来源：http://hz.sysykeji.top/gtsggtncnn.html

TS:   [...new Set(arr)]
来源：http://hz.dashuyun.cn/gtxjdzddct.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.hnqzz.top/gttmlvlrum.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.ybcxt.top/gtbiuvmrgq.html

Ruby: arr.uniq
来源：http://hz.gogol.net.cn/gtyeecgdop.html

C#:   list.Distinct().ToList()
来源：http://hz.0kj1m.cn/gtcgjlykxv.html

[D16] 求和与平均值
来源：http://hz.tianlin.xyz/gteqhvxkal.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.ehwqpu.com/gtwuehadnh.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.yueranfly.top/gtouiikpws.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yongpay.top/gtnfadfxpn.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.fzhhl.top/gtpcgpvahl.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.cqqwz.cn/gtruqgspcb.html

Go:   // 手写循环累加
来源：http://hz.jqgufenzy.top/gtmpyjbgvo.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.zhijiandao.cn/gtnnurkvlh.html

C#:   list.Sum();  list.Average()
来源：http://hz.tian-w.cn/gtdiyhujmy.html

[D17] 最大值与最小值
来源：http://hz.jinqigfzy.top/gtkaqmbqdd.html

Py:   max(arr);  min(arr)
来源：http://hz.hywenlv.cn/gtlmyftjhl.html

PHP:  max($arr);  min($arr);
来源：http://hz.sweek.top/gtdnxainpu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.dashuyun.cn/gtrhdzkpjo.html

TS:   Math.max(...arr);
来源：http://hz.birdmap.top/gtgatqewjt.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.xuanzx.com/gtehndottf.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.redwolf501.top/gtyvwhcxpc.html

Ruby: arr.max;  arr.min
来源：http://hz.havefunace.top/gtqockurjw.html

C#:   list.Max();  list.Min()
来源：http://hz.jinqigfzy.top/gtjxmcnzxa.html

[D18] 扁平化嵌套数组
来源：http://hz.sweek.top/gtjcmthpev.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.zycfv.cn/gtvphqpcuq.html

PHP:  array_merge(...$nested);
来源：http://hz.yanxiufei.cn/gtebdhjxhp.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.wangshuangyany.cn/gtvjhyjoph.html

TS:   nested.flat();
来源：http://hz.cqqwz.cn/gtlhutzddi.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.aizwys.cn/gtcuyzqihq.html

Go:   // 手写双层循环
来源：http://hz.c1oappe.top/gthpuhubew.html

Ruby: nested.flatten
来源：http://hz.xuetiantiany.cn/gtyrrkspit.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.cashguo.top/gtlknjsjqt.html

[D19] 按字段分组
来源：http://hz.daxiang520.top/gtlddywmdj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.nwbrower.top/gtgsjhgedp.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.yangfankeji.com/gthdjkzrjt.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.vqdsnc.cn/gtdveshdbj.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.zhongyouzk.top/gtlslvvqmf.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.hongshengwenyu.top/gtikkvdvad.html

Go:   // 手写 map[string][]T
来源：http://hz.havefunace.top/gtfspqfrqe.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.gaohongyu789.top/gtljqsmeto.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.yanxiufei.cn/gtmelccosq.html

[D20] 统计每个元素出现次数
来源：http://hz.shanyushiyangkeji.top/gtgguxiget.html

Py:   Counter(arr)
来源：http://hz.tian-w.cn/gtjnasrtjb.html

PHP:  array_count_values($arr);
来源：http://hz.cqqwz.cn/gtthkeyytp.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jiagoushi.top/gtfbzjlcec.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.aibaodan.cn/gtyfvrwqak.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.yj20258.top/gtsxhfnjyx.html

Go:   // 手写 map[T]int
来源：http://hz.hammf.cn/gtnetucgeo.html

Ruby: arr.tally
来源：http://hz.shuidangran.top/gtlcouboqz.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.dashuyun.cn/gtbrhwjghq.html

[D21] 判断是否包含某元素
来源：http://hz.wangdashe.top/gtpcczzgng.html

Py:   x in arr
来源：http://hz.ywan-chungtsiang.top/gtpkeqtnwe.html

PHP:  in_array($x, $arr, true);
来源：http://hz.ehwqpu.com/gtrunvvsmi.html

JS:   arr.includes(x)
来源：http://hz.shangyingyoupin.top/gtbnysnqdz.html

TS:   arr.includes(x)
来源：http://hz.redwolf501.top/gtxqcmafhy.html

Java: list.contains(x)
来源：http://hz.zycfv.cn/gtbmzrychi.html

Go:   slices.Contains(arr, x)
来源：http://hz.smart0.xyz/gtubtzchii.html

Ruby: arr.include?(x)
来源：http://hz.yj20258.top/gtqbsyspcq.html

C#:   list.Contains(x)
来源：http://hz.zhengqikj.top/gtxhwotxzm.html

[D22] 复制数组（避免共享引用）
来源：http://hz.meibo888.top/gtslkpdjcb.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.aibaodan.cn/gtekmglxda.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.xingfuxueyuan.xyz/gtmdmcmddv.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.zhaomingkeji.xyz/gtjwrxfwen.html

TS:   [...arr];
来源：http://hz.aizwys.cn/gtuiymwiwf.html

Java: new ArrayList<>(list);
来源：http://hz.nanxuanxn.top/gtzkgkorig.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.zhijiandao.cn/gtextmvbhd.html

Ruby: arr.dup;  arr.clone
来源：http://hz.sufxvd.cn/gtzmzfxluh.html

C#:   new List<int>(list);
来源：http://hz.mhx1999.top/gtvnhzuyhg.html

[D23] reduce 累积计算
来源：http://hz.wangshuangyany.cn/gteiglldgp.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.yonumen.top/gtsvlefdow.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.quarkkingdee.top/gtarpucgtx.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.sufxvd.cn/gthldeflub.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yj20258.top/gtzuqfbuob.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.zdqjudy.top/gtzahanmgl.html

Go:   // 手写循环
来源：http://hz.gaohongyu789.top/gtdzpiyrpw.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.sweek.top/gtrpnxuetr.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.52xcode.cn/gtlgaczigd.html

[D24] 字典 / Map 基本操作
来源：http://hz.zhengqikj.top/gtpzmgkote.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.gaohongyu789.top/gtepcbyvgd.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.shanyushiyangkeji.top/gtcjmqtnwk.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.xziqi.cn/gthptubbba.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.pengpengdd.cyou/gtqsijhbaq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.cucudq.cn/gtmegdtcof.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.wangdashe.top/gtwirgwopp.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.xinyue.icu/gtzhrcgevo.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.svipenyu.cn/gtdfkbelsc.html

[D25] Set 集合去重与交并差
来源：http://hz.xylfe.cn/gtgdrbejxm.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.bjfxy.top/gtedhmojpw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.kuanghao11.cn/gtoxnfiwez.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.bjfxy.top/gthzjmzgwn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.jianghu66.top/gttmencxks.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.gaohongyu789.top/gttaewoxbl.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.daxiang520.top/gtnekimemq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.9152youxi.cn/gtokgvccng.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.shuidangran.top/gtnlspfrrk.html

[D26] 数组转字符串
来源：http://hz.0kj1m.cn/gtyrawwvat.html

Py:   ", ".join(map(str, arr))
来源：http://hz.hnxiangtu.top/gtjijkhdhk.html

PHP:  implode(", ", $arr);
来源：http://hz.shanyushiyangtech.top/gtscqzartk.html

JS:   arr.join(", ")
来源：http://hz.c1oappe.top/gthtjgfkkc.html

TS:   arr.join(", ")
来源：http://hz.smart0.xyz/gtuydnovyf.html

Java: String.join(", ", list)
来源：http://hz.jlsjyb.cn/gtihndtmbx.html

Go:   strings.Join(strs, ", ")
来源：http://hz.yuxming.cn/gtpmholcgj.html

Ruby: arr.join(", ")
来源：http://hz.tian-w.cn/gtbvapayfc.html

C#:   string.Join(", ", list)
来源：http://hz.aizwys.cn/gtwdcjqfqd.html

================================================================================
来源：http://hz.jlsjyb.cn/gtvfsedghg.html

E. 字符串处理
来源：http://hz.cdnleiting.top/gtcvkfabec.html

================================================================================
来源：http://hz.xuanzx.com/gtorukesub.html

[E01] 拼接字符串
来源：http://hz.shzxlz.cn/gtrcdrjkux.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.daria6918.cn/gtbyrjryxs.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.zhongyouzk.top/gttkykgzvu.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jqgufenzy.top/gtukcnsmfq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.gotoacloud.top/gtvuvknxbe.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.dianchejie.cn/gtcjnysoac.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.aibaodan.cn/gtjiwdcnlw.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.yanxiufei.cn/gtlcqsmcwt.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.9152youxi.cn/gtncaydzix.html

[E02] 重复字符串
来源：http://hz.iojbl.cn/gtwxztfgmo.html

Py:   "ab" * 3
来源：http://hz.52xcode.cn/gtjoqtzijc.html

PHP:  str_repeat("ab", 3);
来源：http://hz.cqqwz.cn/gthmbwridb.html

JS:   "ab".repeat(3)
来源：http://hz.redwolf501.top/gtqbzvuidy.html

TS:   "ab".repeat(3)
来源：http://hz.smart0.xyz/gtfdobisvm.html

Java: "ab".repeat(3)
来源：http://hz.jqgufenzy.top/gtdgjlrswk.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.xuetiantiany.cn/gtmdmmtrei.html

Ruby: "ab" * 3
来源：http://hz.snrcjt.cn/gthsxyfswd.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.havefunace.top/gttdpgimbe.html

[E03] 截取子串
来源：http://hz.ywan-chungtsiang.top/gtfwypgsvq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.jinyuanbaomall.cn/gtknyynbpi.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.gaohongyu789.top/gtochqfvpq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.daxiang520.top/gtoehlomal.html

TS:   s.slice(1, 4)
来源：http://hz.chenjidiqi.icu/gtvztswobw.html

Java: s.substring(1, 4)
来源：http://hz.cucudq.cn/gthyfedueg.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.pengpengdd.cyou/gtaivmnfpj.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.tian-w.cn/gtidcypyrb.html

C#:   s.Substring(1, 3)
来源：http://hz.cqqwz.cn/gtfzhlukvo.html

[E04] 查找子串位置
来源：http://hz.ydjk.org.cn/gtfeiumdzt.html

Py:   s.find("x");  s.index("x")
来源：http://hz.xuetiantiany.cn/gtsvvktaij.html

PHP:  strpos($s, "x");
来源：http://hz.zhijiandao.cn/gtcftxwyxj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.zhongyouzk.top/gtrrznhmhx.html

TS:   s.indexOf("x")
来源：http://hz.zdqjudy.top/gtnnepzeym.html

Java: s.indexOf("x")
来源：http://hz.hywenlv.cn/gtgskuteen.html

Go:   strings.Index(s, "x")
来源：http://hz.zhixingplan.top/gtctokshuf.html

Ruby: s.index("x")
来源：http://hz.jiagoushi.top/gtxznsudra.html

C#:   s.IndexOf("x")
来源：http://hz.yueranfly.top/gtentxsqtm.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.daxiang520.top/gtzcictagh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.havefunace.top/gtjjjpdusr.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.feifeiyinyue.top/gtqojegqtc.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.fengsongda.top/gtgthvmuub.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.birdmap.top/gtbtciwegm.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.daria6918.cn/gtslmlhwlm.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.sysykeji.top/gtmeojqoci.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.jqgfzy.top/gttmjcdexp.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.sxryk.cn/gtqcpmtgus.html

[E06] 替换子串
来源：http://hz.shanyushiyangtech.top/gtdhfuhmol.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.shzxlz.cn/gtseansdpl.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.iojbl.cn/gtdxctwxty.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.aibaodan.cn/gtruditzqu.html

TS:   s.replaceAll("a", "b")
来源：http://hz.sysykeji.top/gtzaybcbzz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.guannengcc.top/gtnjilwiwb.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.gotoacloud.top/gtrsusifgt.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.shuidangran.top/gtsitgskcd.html

C#:   s.Replace("a", "b")
来源：http://hz.ehwqpu.com/gtzqpkbnvx.html

[E07] 按分隔符拆分
来源：http://hz.yvedp.cn/gtgtpiajnf.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.cdnleiting.top/gtmcfoigjn.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.yongpay.top/gtlhuowolz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.pengpengdd.cyou/gtfpybhiyc.html

TS:   s.split(",")
来源：http://hz.iojbl.cn/gtyqdbrltw.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.yj20258.top/gtsvppgywj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.gaohongyu789.top/gtyreoxfzx.html

Ruby: s.split(",");  s.split
来源：http://hz.jianghu66.top/gtsrvqnjww.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.gzhubu.top/gtxermmhqd.html

[E08] 数组按分隔符合并
来源：http://hz.jyoumei.cn/gtrxkznszw.html

Py:   ",".join(items)
来源：http://hz.hywenlv.cn/gtvrxccfyp.html

PHP:  implode(",", $items);
来源：http://hz.redwolf501.top/gtqfiqgcft.html

JS:   items.join(",")
来源：http://hz.chenjidiqi.icu/gtlfybljvz.html

TS:   items.join(",")
来源：http://hz.xziqi.cn/gtpxbmktnu.html

Java: String.join(",", items)
来源：http://hz.ehwqpu.com/gtvkkxkplf.html

Go:   strings.Join(items, ",")
来源：http://hz.xuetiantiany.cn/gtqseyjckt.html

Ruby: items.join(",")
来源：http://hz.yj20258888.top/gtxkodimvy.html

C#:   string.Join(",", items)
来源：http://hz.yvedp.cn/gtuubmtegf.html

[E09] 去除所有空白字符
来源：http://hz.yonumen.top/gtkdkljhuo.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.birdmap.top/gtldycrvbu.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.0kj1m.cn/gtoncnuzrb.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.kuanghao11.cn/gtzbhdfrya.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.jqgfzy.top/gtpnqijplv.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.9152youxi.cn/gtcfbiawib.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.bjfxy.top/gtzynagvxw.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.shanyushiyangtech.top/gtrdcitnbv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.ydjk.org.cn/gtqngmrnot.html

[E10] 左侧补零 / 定长填充
来源：http://hz.yueranfly.top/gtbnnwhvid.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.chenzaomai.com/gtbskpnjty.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.yueranfly.top/gtrqofrnua.html

JS:   "7".padStart(3, "0")
来源：http://hz.jianghu66.top/gtsaxlnqbo.html

TS:   "7".padStart(3, "0")
来源：http://hz.zhiwuduotai.top/gtfzfpzkze.html

Java: String.format("%03d", 7)
来源：http://hz.jinqigufen.top/gtjgsdgkzz.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.gaohongyu789.top/gtvywqaozi.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.gzhubu.top/gtjthhvfgd.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.jqgfzy.top/gtozdgsxnx.html

[E11] 反转字符串
来源：http://hz.svipenyu.cn/gtdlvtyume.html

Py:   s[::-1]
来源：http://hz.xinyue.icu/gtmxvibabc.html

PHP:  strrev($s);
来源：http://hz.iojbl.cn/gtndrcqxpx.html

JS:   [...s].reverse().join("")
来源：http://hz.cashguo.top/gtnhozxvwl.html

TS:   [...s].reverse().join("")
来源：http://hz.fengsongda.top/gtncnxhkkw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.zhoulong.xyz/gtnjnjizqx.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.chenjidiqi.icu/gtnpbciapm.html

Ruby: s.reverse
来源：http://hz.haohaochexian.top/gtrjxiqcww.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.dianchejie.cn/gtaazssqia.html

[E12] 统计某字符出现次数
来源：http://hz.cqqwz.cn/gtfoempley.html

Py:   s.count("a")
来源：http://hz.sweek.top/gtedwxmenz.html

PHP:  substr_count($s, "a");
来源：http://hz.jinqigfzy.top/gtnupxsekq.html

JS:   s.split("a").length - 1
来源：http://hz.yuxming.cn/gtziyhrdvx.html

TS:   s.split("a").length - 1
来源：http://hz.zhaomingkeji.xyz/gtbyjmbmev.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.shuidangran.top/gtznxfitrd.html

Go:   strings.Count(s, "a")
来源：http://hz.zhixingplan.top/gtxurxlwvg.html

Ruby: s.count("a")
来源：http://hz.nanxinkj.top/gtfpptccif.html

C#:   s.Count(c => c == 'a')
来源：http://hz.ppjwa.cn/gtmetnckwl.html

[E13] 逐字符遍历
来源：http://hz.zhongyouzk.top/gtnrzobauv.html

Py:   for ch in s: print(ch)
来源：http://hz.zycfv.cn/gtsiyurhnj.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.vqdsnc.cn/gtowffnamy.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.shanyushiyangkeji.top/gthazrvmvd.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xingfuxueyuan.xyz/gtnrmnrbuf.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.ywan-chungtsiang.top/gtefyvxbrc.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.wangdashe.top/gtqlwaydww.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.yuxming.cn/gtbjxsaqes.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.ehwqpu.com/gtwipgbqhf.html

[E14] URL 编码与 Base64
来源：http://hz.zhijiandao.cn/gtvkxmrnjq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.shzxlz.cn/gtffliwmoa.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.hysaishi.cn/gtgbsfhbhj.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.fzhhl.top/gttoozwvuj.html


<!-- 参考信息 -->