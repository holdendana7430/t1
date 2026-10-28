代发 wailian999

[D07] 切片 / 取子数组
来源：http://hz.yonumen.top/gtfrakbkiv.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.guannengcc.top/gticqaseja.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.jianghu66.top/gtduairraj.html

JS:   arr.slice(1, 4);
来源：http://hz.guannengcc.top/gtnvmhcfhb.html

TS:   arr.slice(1, 4);
来源：http://hz.kuanghao11.cn/gtzmjcxlra.html

Java: list.subList(1, 4);
来源：http://hz.yj202588.top/gtdbkjcokb.html

Go:   arr[1:4]
来源：http://hz.ehwqpu.com/gtwocogroq.html

Ruby: arr[1, 3]
来源：http://hz.zhaomingkeji.xyz/gtwukftyjq.html

C#:   list.GetRange(1, 3);
来源：http://hz.yuxming.cn/gtjxxgwdxs.html

[D08] 合并两个数组
来源：http://hz.zhixingplan.top/gtwsaurtdj.html

Py:   a + b;  a.extend(b)
来源：http://hz.hnqzz.top/gtonrjrpos.html

PHP:  array_merge($a, $b);
来源：http://hz.jiagoushi.top/gtkolajfqt.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.jinqigfzy.top/gtkzxhhkae.html

TS:   [...a, ...b];
来源：http://hz.haohaochexian.top/gtjikuvqvo.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.sxryk.cn/gtimndmwrk.html

Go:   append(a, b...)
来源：http://hz.xuetiantiany.cn/gtryoyvgft.html

Ruby: a + b;  a.concat(b)
来源：http://hz.sweek.top/gtrstumten.html

C#:   a.Concat(b).ToList()
来源：http://hz.shuidangran.top/gtotjkfwyl.html

[D09] 排序（升序）
来源：http://hz.bjfxy.top/gtinfihfrk.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zdqjudy.top/gtvkhfkiku.html

PHP:  sort($arr);
来源：http://hz.daria6918.cn/gtpgbogyzx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.sysykeji.top/gtpcpdtrez.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.yangfankeji.com/gtywnemlgq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.jinyuanbaomall.cn/gtwnafqipx.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.yueranfly.top/gtfkkaqbdu.html

Ruby: arr.sort
来源：http://hz.yuanzhike.top/gtlnftqvyr.html

C#:   list.Sort();
来源：http://hz.zhongyouzk.top/gtgxlwcksa.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.pycfn.com/gtymalgvnl.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.yvedp.cn/gtzezskppi.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yueranfly.top/gtoykfrvdp.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zhongyouzk.top/gttaifmaof.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jqgufenzy.top/gtypomwibs.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.xinyue.icu/gtsvnfwyyn.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.hysaishi.cn/gtygdqhdbc.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.jiagoushi.top/gtznejldij.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.zhoulong.xyz/gtsexxesxg.html

[D11] 反转数组
来源：http://hz.yongpay.top/gtstckvuof.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.chenzaomai.com/gtbyssxbsc.html

PHP:  array_reverse($arr);
来源：http://hz.shuidangran.top/gtlimndane.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.ydzc1.top/gtwecpdxpo.html

TS:   [...arr].reverse();
来源：http://hz.yj20258.top/gtrcjtsfvm.html

Java: Collections.reverse(list);
来源：http://hz.svipenyu.cn/gtxxhgzotg.html

Go:   slices.Reverse(arr)
来源：http://hz.shanyushiyangkeji.top/gtltmtzlcd.html

Ruby: arr.reverse
来源：http://hz.chenzaomai.com/gttkwimlth.html

C#:   list.Reverse();
来源：http://hz.zhengqikj.top/gtuadbxvxe.html

[D12] 查找元素下标
来源：http://hz.tianlin.xyz/gtbcygibdp.html

Py:   arr.index(x);  x in arr
来源：http://hz.cashguo.top/gtcsbimfjz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.shanyushiyangkeji.top/gtlukokvlw.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.ybcxt.top/gtpwzglnrx.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.birdmap.top/gtaqbiuqor.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.yongpay.top/gtutwxbnbn.html

Go:   slices.Index(arr, x)
来源：http://hz.svipenyu.cn/gtcgfpmqet.html

Ruby: arr.index(x)
来源：http://hz.yongpay.top/gtlqbwsjci.html

C#:   list.IndexOf(x);
来源：http://hz.hnqzz.top/gtybtgtcxi.html

[D13] 过滤（保留满足条件的）
来源：http://hz.smart0.xyz/gtozenjdra.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.gaohongyu789.top/gtukxpooaw.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.zhiwuduotai.top/gtvwayyreb.html

JS:   arr.filter(x => x > 3)
来源：http://hz.cucudq.cn/gtbcyoajvv.html

TS:   arr.filter(x => x > 3)
来源：http://hz.redwolf501.top/gtvxbpogvg.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.ywan-chungtsiang.top/gthmmqmdot.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.shuidangran.top/gtyymybnei.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.aizwys.cn/gtdznsjwta.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.yonumen.top/gtszvvkrdd.html

[D14] 映射转换（每个元素变形）
来源：http://hz.quarkkingdee.top/gtkajhkzmq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.ehwqpu.com/gtsqdvarsp.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.yueranfly.top/gtcvrjcjay.html

JS:   arr.map(x => x * 2)
来源：http://hz.jinyuanbaomall.cn/gtenwpvnaw.html

TS:   arr.map(x => x * 2)
来源：http://hz.zhongyouzk.top/gtdzaunalq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.sysykeji.top/gtispjicoj.html

Go:   // 手写循环
来源：http://hz.ehwqpu.com/gttcdfqumq.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.zycfv.cn/gtcrdusqzh.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.fzhhl.top/gtjoxmgsaq.html

[D15] 去重
来源：http://hz.yj202588.top/gtbqdnmeac.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.yangfankeji.com/gtmhqjjhfh.html

PHP:  array_unique($arr);
来源：http://hz.bjfxy.top/gtqofjjbfg.html

JS:   [...new Set(arr)]
来源：http://hz.shanyushiyangkeji.top/gttjmfttfz.html

TS:   [...new Set(arr)]
来源：http://hz.sufxvd.cn/gtdyuydrlt.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.nanxuanxn.top/gtqzpdxhff.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.jinqigufen.top/gtubovdzzd.html

Ruby: arr.uniq
来源：http://hz.zhongyouzk.top/gtztqlclha.html

C#:   list.Distinct().ToList()
来源：http://hz.zhongyouzk.top/gtnpxcnixy.html

[D16] 求和与平均值
来源：http://hz.cheryme.top/gtqfplgvyb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.yuanzhike.top/gthcubrzjw.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.smart0.xyz/gtzkvndqfr.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.52xcode.cn/gtbcvcxfuz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.c1oappe.top/gtjghshcae.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.zdqjudy.top/gtwxjvsgmr.html

Go:   // 手写循环累加
来源：http://hz.tianlin.xyz/gtcyrejwva.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.aibaodan.cn/gtdexpqxbe.html

C#:   list.Sum();  list.Average()
来源：http://hz.zhiwuduotai.top/gtbsygdybg.html

[D17] 最大值与最小值
来源：http://hz.tian-w.cn/gtylenzejt.html

Py:   max(arr);  min(arr)
来源：http://hz.shangyingyoupin.top/gtjxmlifpb.html

PHP:  max($arr);  min($arr);
来源：http://hz.bjfxy.top/gtdfayzcbm.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.zhengqikj.top/gtxqzfmyld.html

TS:   Math.max(...arr);
来源：http://hz.shanyushiyangtech.top/gtkaiviyeg.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.yuanzhike.top/gtcctzqjsf.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.yj20258.top/gtxmyfktgk.html

Ruby: arr.max;  arr.min
来源：http://hz.cdnleiting.top/gtstgmwtor.html

C#:   list.Max();  list.Min()
来源：http://hz.andypj.xyz/gthjrdvhru.html

[D18] 扁平化嵌套数组
来源：http://hz.ybcxt.top/gtvfmjspel.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.ywan-chungtsiang.top/gtcqggfmjn.html

PHP:  array_merge(...$nested);
来源：http://hz.0kj1m.cn/gtgqgnlymp.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.dashuyun.cn/gtayykohco.html

TS:   nested.flat();
来源：http://hz.yj20258.top/gtjfaaphwj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.xylfe.cn/gtiyxapmlv.html

Go:   // 手写双层循环
来源：http://hz.pengpengdd.cyou/gtjrxlqurg.html

Ruby: nested.flatten
来源：http://hz.hnxiangtu.top/gttufutyks.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.guowangkeji.top/gtcioinhvt.html

[D19] 按字段分组
来源：http://hz.yangfankeji.com/gtshmmtomm.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.fzhhl.top/gttayfnvru.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.shzxlz.cn/gttgjxzkws.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.chenlongwang.top/gtwaumrhyq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.chenlongwang.top/gtzdgkzgtn.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.zhoulong.xyz/gtsjmemlrm.html

Go:   // 手写 map[string][]T
来源：http://hz.zhaomingkeji.xyz/gtevbtpvvh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.jinqigfzy.top/gtuxivankg.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.guannengcc.top/gtsqmqvndb.html

[D20] 统计每个元素出现次数
来源：http://hz.jqgufenzy.top/gtasoysvns.html

Py:   Counter(arr)
来源：http://hz.nanxinkj.top/gtnvosriks.html

PHP:  array_count_values($arr);
来源：http://hz.hnxiangtu.top/gtzetutzxv.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.pycfn.com/gtwyyddyvw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jqgfzy.top/gtobjvsdab.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.yuxming.cn/gtzlycqwwf.html

Go:   // 手写 map[T]int
来源：http://hz.chenlongwang.top/gtdgdwnell.html

Ruby: arr.tally
来源：http://hz.xuetiantiany.cn/gtbkwlagen.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.c1oappe.top/gtailvveeu.html

[D21] 判断是否包含某元素
来源：http://hz.yj202588.top/gtdsguqnnj.html

Py:   x in arr
来源：http://hz.aizwys.cn/gtmevzsphh.html

PHP:  in_array($x, $arr, true);
来源：http://hz.gzhubu.top/gtqgoiacrq.html

JS:   arr.includes(x)
来源：http://hz.yuanzhike.top/gtdxmkydsd.html

TS:   arr.includes(x)
来源：http://hz.ydjk.org.cn/gtthuynckf.html

Java: list.contains(x)
来源：http://hz.jqgufenzy.top/gtqvgkoenp.html

Go:   slices.Contains(arr, x)
来源：http://hz.pengpengdd.cyou/gtncfgupbo.html

Ruby: arr.include?(x)
来源：http://hz.iojbl.cn/gtaqbbmqlt.html

C#:   list.Contains(x)
来源：http://hz.yanxiufei.cn/gtccazpahv.html

[D22] 复制数组（避免共享引用）
来源：http://hz.daria6918.cn/gtxijhdjit.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.nwbrower.top/gtkdnmmfgh.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.guowangkeji.top/gtdscuuzfu.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.fzhhl.top/gttupwhvxc.html

TS:   [...arr];
来源：http://hz.9152youxi.cn/gtjezclscm.html

Java: new ArrayList<>(list);
来源：http://hz.iojbl.cn/gtzijxntuj.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.havefunace.top/gtkeqyzvpg.html

Ruby: arr.dup;  arr.clone
来源：http://hz.iojbl.cn/gtsphxkzqc.html

C#:   new List<int>(list);
来源：http://hz.jianghu66.top/gtjbtxnyxs.html

[D23] reduce 累积计算
来源：http://hz.haohaochexian.top/gtnuqumrpt.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.jqgufenzy.top/gtlvuufoou.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.hywenlv.cn/gtnxuemlei.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.cheryme.top/gtrpbjqlje.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.sufxvd.cn/gtegmivvmv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.hywenlv.cn/gtuwpdglvi.html

Go:   // 手写循环
来源：http://hz.hysaishi.cn/gtlbiiffma.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.nwbrower.top/gtfmdhcogx.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.ehwqpu.com/gtfrbnwrri.html

[D24] 字典 / Map 基本操作
来源：http://hz.kuanghao11.cn/gttvetrxfe.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.9152youxi.cn/gtpdziawpf.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.52xcode.cn/gtsiivbcvh.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.pengpengdd.cyou/gtiddxfkuh.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.zhoulong.xyz/gtbwumjuip.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.pengpengdd.cyou/gtxecbswhh.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.svipenyu.cn/gtjedjfugb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.gaohongyu789.top/gtejjvctwn.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.sxryk.cn/gtakkhgjou.html

[D25] Set 集合去重与交并差
来源：http://hz.jyoumei.cn/gtdwfprtau.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.wangdashe.top/gtraawmbal.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.yuxming.cn/gtecvpxllt.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.jinqigufen.top/gtxjbqhecs.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.hongshengwenyu.top/gtlnklvqng.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.yueranfly.top/gtkwagafrr.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.kuanghao11.cn/gtvbgzskjb.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.nanxinkj.top/gtiyncqmmc.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.mhx1999.top/gtrfplapph.html

[D26] 数组转字符串
来源：http://hz.haohaochexian.top/gtxyfylvpu.html

Py:   ", ".join(map(str, arr))
来源：http://hz.zhaomingkeji.xyz/gtchgvovfo.html

PHP:  implode(", ", $arr);
来源：http://hz.jinyuanbaomall.cn/gthxcpreby.html

JS:   arr.join(", ")
来源：http://hz.ydzc1.top/gtryupdbaq.html

TS:   arr.join(", ")
来源：http://hz.fengsongda.top/gtzravvsrz.html

Java: String.join(", ", list)
来源：http://hz.wangshuangyany.cn/gtuqimmayg.html

Go:   strings.Join(strs, ", ")
来源：http://hz.aibaodan.cn/gtjpajwuux.html

Ruby: arr.join(", ")
来源：http://hz.yonumen.top/gtfzkychfa.html

C#:   string.Join(", ", list)
来源：http://hz.jiagoushi.top/gtlorblrwr.html

================================================================================
来源：http://hz.kuanghao11.cn/gthdeblxeg.html

E. 字符串处理
来源：http://hz.ydjk.org.cn/gtngleltfm.html

================================================================================
来源：http://hz.vqdsnc.cn/gtdtfdowbx.html

[E01] 拼接字符串
来源：http://hz.yuanzhike.top/gtyghfuwmg.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.pengpengdd.cyou/gtuvdmxbng.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.jiagoushi.top/gtcpgfyvel.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zhengqikj.top/gtvqbydejk.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jqgfzy.top/gtwfxvrgzt.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.tanke756.top/gthjcgmcct.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.cucudq.cn/gtloyvvfoh.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.xuanzx.com/gtgoonvlnp.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.smart0.xyz/gttrkvtfqh.html

[E02] 重复字符串
来源：http://hz.birdmap.top/gtcdkoixqo.html

Py:   "ab" * 3
来源：http://hz.xziqi.cn/gtemkvrxdi.html

PHP:  str_repeat("ab", 3);
来源：http://hz.chenzaomai.com/gtyhujlnrt.html

JS:   "ab".repeat(3)
来源：http://hz.gotoacloud.top/gtvtojhhxw.html

TS:   "ab".repeat(3)
来源：http://hz.snrcjt.cn/gtcljinckh.html

Java: "ab".repeat(3)
来源：http://hz.cdnleiting.top/gtadcgimpw.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.shanyushiyangkeji.top/gttnmthaex.html

Ruby: "ab" * 3
来源：http://hz.aizwys.cn/gtwkqbwnjs.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.jinqigfzy.top/gtlnahckqh.html

[E03] 截取子串
来源：http://hz.redwolf501.top/gtqpnclxvi.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.yangfankeji.com/gtricknzuc.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.bjfxy.top/gtnsvijztm.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.pengpengdd.cyou/gtylncfkic.html

TS:   s.slice(1, 4)
来源：http://hz.shangyingyoupin.top/gtqctxslwj.html

Java: s.substring(1, 4)
来源：http://hz.svipenyu.cn/gtbzgdieuv.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.yangfankeji.com/gtydjiamrm.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.zhoulong.xyz/gtoicjchxf.html

C#:   s.Substring(1, 3)
来源：http://hz.tanke756.top/gtnjtngfyp.html

[E04] 查找子串位置
来源：http://hz.yj202588.top/gtpsntttnb.html

Py:   s.find("x");  s.index("x")
来源：http://hz.sweek.top/gtuxopoxpk.html

PHP:  strpos($s, "x");
来源：http://hz.cdnleiting.top/gtnmzsyrou.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.shzxlz.cn/gtrpehjgal.html

TS:   s.indexOf("x")
来源：http://hz.jinyuanbaomall.cn/gtsynwhssr.html

Java: s.indexOf("x")
来源：http://hz.hywenlv.cn/gtfjkcfcnh.html

Go:   strings.Index(s, "x")
来源：http://hz.nanxinkj.top/gtonwjrqpo.html

Ruby: s.index("x")
来源：http://hz.xuetiantiany.cn/gtoneqnjfh.html

C#:   s.IndexOf("x")
来源：http://hz.ydjk.org.cn/gthezmgmsq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.c1oappe.top/gtdbvebrat.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.daria6918.cn/gtfifwjhaf.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.guannengcc.top/gtfiqhcnkc.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yuanzhike.top/gtynuspcsl.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.guowangkeji.top/gtxpdwlryn.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.hysaishi.cn/gthznpyxrt.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.yangfankeji.com/gtzbjuiift.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.jinqigufen.top/gtxuvodrfr.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.cheryme.top/gtgujcartx.html

[E06] 替换子串
来源：http://hz.ywan-chungtsiang.top/gtvorigxmb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.9152youxi.cn/gterlspcsh.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.316326.xyz/gtnrcbqmrn.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.hnqzz.top/gtucfjazrx.html

TS:   s.replaceAll("a", "b")
来源：http://hz.cucudq.cn/gtpxwlwiyt.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yangfankeji.com/gtyehcdgue.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.ywan-chungtsiang.top/gtxpqabgpj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.gogol.net.cn/gtyerlvfey.html

C#:   s.Replace("a", "b")
来源：http://hz.gogol.net.cn/gtqoqpsxmf.html

[E07] 按分隔符拆分
来源：http://hz.snrcjt.cn/gtqntowudv.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.shanyushiyangtech.top/gtrodkvxft.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.jinqigfzy.top/gtecxorcgq.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.9152youxi.cn/gtiupeekzb.html

TS:   s.split(",")
来源：http://hz.sysykeji.top/gtfseonokp.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.daxiang520.top/gthlatmdmv.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.yvedp.cn/gtymtnklrv.html

Ruby: s.split(",");  s.split
来源：http://hz.xuetiantiany.cn/gtgbetcfmj.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.jinyuanbaomall.cn/gtjtbabeph.html

[E08] 数组按分隔符合并
来源：http://hz.yonumen.top/gtmmvsojus.html

Py:   ",".join(items)
来源：http://hz.gotoacloud.top/gtycfioupy.html

PHP:  implode(",", $items);
来源：http://hz.ehwqpu.com/gttsbpoanl.html

JS:   items.join(",")
来源：http://hz.sweek.top/gtnjbzzjyj.html

TS:   items.join(",")
来源：http://hz.nanxinkj.top/gtahxqosts.html

Java: String.join(",", items)
来源：http://hz.meibo888.top/gthvqreisg.html

Go:   strings.Join(items, ",")
来源：http://hz.ydjk.org.cn/gtiewzgbvd.html

Ruby: items.join(",")
来源：http://hz.tanke756.top/gtuqndxysn.html

C#:   string.Join(",", items)
来源：http://hz.jianghu66.top/gttvtuzeyh.html

[E09] 去除所有空白字符
来源：http://hz.xylfe.cn/gtuxalawnh.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.cucudq.cn/gtrwtvzdkv.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.tianlin.xyz/gtabvcbejx.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.hongshengwenyu.top/gtncgzlttc.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.yueranfly.top/gtxgwkuuke.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.shanyushiyangtech.top/gtkrkjblhe.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.52xcode.cn/gtkwghidkj.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.ydzc1.top/gtizdzcaea.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.c1oappe.top/gtjfwwajnz.html

[E10] 左侧补零 / 定长填充
来源：http://hz.kuanghao11.cn/gteznqyrfg.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.chenjidiqi.icu/gtyiuapylv.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.daxiang520.top/gtpxmmhcpt.html

JS:   "7".padStart(3, "0")
来源：http://hz.yj20258888.top/gtwpkdchfd.html

TS:   "7".padStart(3, "0")
来源：http://hz.gzhubu.top/gtshaoymoh.html

Java: String.format("%03d", 7)
来源：http://hz.xuetiantiany.cn/gtntokuvox.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.zhaomingkeji.xyz/gthrlbqxdf.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.guowangkeji.top/gttobkpcly.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.xuetiantiany.cn/gtcgxoezqe.html

[E11] 反转字符串
来源：http://hz.zhixingplan.top/gtgorbatqo.html

Py:   s[::-1]
来源：http://hz.hnqzz.top/gtywltqqph.html

PHP:  strrev($s);
来源：http://hz.sxryk.cn/gtwreunhjs.html

JS:   [...s].reverse().join("")
来源：http://hz.mhx1999.top/gtmpzuhxvi.html

TS:   [...s].reverse().join("")
来源：http://hz.yonumen.top/gtdyizztvh.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.c1oappe.top/gtrrigrpsm.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.aibaodan.cn/gtznbnjqpt.html

Ruby: s.reverse
来源：http://hz.gzhubu.top/gtwlhrmpxs.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.tanke756.top/gtyolvodvl.html

[E12] 统计某字符出现次数
来源：http://hz.yonumen.top/gtxaufoabs.html

Py:   s.count("a")
来源：http://hz.smart0.xyz/gtetlbxruk.html

PHP:  substr_count($s, "a");
来源：http://hz.c1oappe.top/gtejlhihwt.html

JS:   s.split("a").length - 1
来源：http://hz.ehwqpu.com/gtuvdqgypo.html

TS:   s.split("a").length - 1
来源：http://hz.tanke756.top/gtirilxfmw.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.gogol.net.cn/gtkfsxxqey.html

Go:   strings.Count(s, "a")
来源：http://hz.yangfankeji.com/gtckzjhydd.html

Ruby: s.count("a")
来源：http://hz.xziqi.cn/gtoapoangd.html

C#:   s.Count(c => c == 'a')
来源：http://hz.quarkkingdee.top/gtasaeyzvd.html

[E13] 逐字符遍历
来源：http://hz.zhiwuduotai.top/gtvpcqwlwb.html

Py:   for ch in s: print(ch)
来源：http://hz.hammf.cn/gtrbgzngse.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.zycfv.cn/gtrkbapksf.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.wangdashe.top/gtfaufbthe.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.0kj1m.cn/gtolqxkgns.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.hnqzz.top/gtknicyolo.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.jianghu66.top/gtzecsrlwb.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.sysykeji.top/gtrdfakdqa.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.aibaodan.cn/gtbbfnvcrr.html


<!-- 参考信息 -->