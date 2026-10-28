代发 wailian999

Py:   len(arr)
来源：http://hz.sxryk.cn/gtoytsjzfo.html

PHP:  count($arr);
来源：http://hz.tanke756.top/gterfninue.html

JS:   arr.length
来源：http://hz.meibo888.top/gtelmhxwbj.html

TS:   arr.length
来源：http://hz.vqdsnc.cn/gtsybwidni.html

Java: list.size();
来源：http://hz.jiagoushi.top/gthujxbhfx.html

Go:   len(arr)
来源：http://hz.zycfv.cn/gtnhxkzfic.html

Ruby: arr.length; arr.size
来源：http://hz.shanyushiyangkeji.top/gtugzuuyoj.html

C#:   list.Count;
来源：http://hz.52xcode.cn/gtprktotmj.html

[D07] 切片 / 取子数组
来源：http://hz.xylfe.cn/gtzpmrbkeg.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.mhx1999.top/gtxryhnart.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.ehwqpu.com/gtahisogwj.html

JS:   arr.slice(1, 4);
来源：http://hz.snrcjt.cn/gtmhwltrnl.html

TS:   arr.slice(1, 4);
来源：http://hz.redwolf501.top/gtqhsebsfu.html

Java: list.subList(1, 4);
来源：http://hz.jiagoushi.top/gtaxhvvaqn.html

Go:   arr[1:4]
来源：http://hz.wangshuangyany.cn/gtarbkmwvj.html

Ruby: arr[1, 3]
来源：http://hz.jyoumei.cn/gtmdtdxxnb.html

C#:   list.GetRange(1, 3);
来源：http://hz.shanyushiyangtech.top/gtnkaexdde.html

[D08] 合并两个数组
来源：http://hz.shanyushiyangtech.top/gtyapzvmwc.html

Py:   a + b;  a.extend(b)
来源：http://hz.snrcjt.cn/gtaclcbjdn.html

PHP:  array_merge($a, $b);
来源：http://hz.pycfn.com/gtrhxtreee.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.chenjidiqi.icu/gttrswjfgo.html

TS:   [...a, ...b];
来源：http://hz.jinghuilouyu.cn/gtoeizeuzg.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.daxiang520.top/gtnqgzoalv.html

Go:   append(a, b...)
来源：http://hz.smart0.xyz/gtxvypkkdw.html

Ruby: a + b;  a.concat(b)
来源：http://hz.c1oappe.top/gtuhqzumfd.html

C#:   a.Concat(b).ToList()
来源：http://hz.ydzc1.top/gtecssrupn.html

[D09] 排序（升序）
来源：http://hz.shanyushiyangtech.top/gtroxjtiyi.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.xuanzx.com/gtfxingcyj.html

PHP:  sort($arr);
来源：http://hz.zdqjudy.top/gtqqooytsv.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.zdqjudy.top/gtutwjqxcb.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.shanyushiyangtech.top/gtphwdqybf.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.shanyushiyangkeji.top/gtjdxwgcvp.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.yuanzhike.top/gtvmwegzja.html

Ruby: arr.sort
来源：http://hz.gaohongyu789.top/gtvcwlmdku.html

C#:   list.Sort();
来源：http://hz.jinqigufen.top/gtfmrgfrbm.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.gogol.net.cn/gtzynbvwzo.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.jlsjyb.cn/gtizqwfydt.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.sxryk.cn/gtnsotcdri.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jinqigfzy.top/gtwnoxhezv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.316326.xyz/gtquqermer.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.yanxiufei.cn/gtyidctzrn.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.aizwys.cn/gtgfaypkpd.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.c1oappe.top/gtmwcnbtpl.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.shzxlz.cn/gtzztsydxc.html

[D11] 反转数组
来源：http://hz.shangyingyoupin.top/gthoyzsnns.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.hywenlv.cn/gtisstwmxk.html

PHP:  array_reverse($arr);
来源：http://hz.dianchejie.cn/gtbxytnbmw.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.ehwqpu.com/gtoaqylhgc.html

TS:   [...arr].reverse();
来源：http://hz.316326.xyz/gtavhbjinn.html

Java: Collections.reverse(list);
来源：http://hz.nanxuanxn.top/gtbmlasysj.html

Go:   slices.Reverse(arr)
来源：http://hz.bjfxy.top/gtzqddyusc.html

Ruby: arr.reverse
来源：http://hz.yj202588.top/gtlsqiezfk.html

C#:   list.Reverse();
来源：http://hz.ivvv.top/gtlslvftmi.html

[D12] 查找元素下标
来源：http://hz.gogol.net.cn/gtnhdihbye.html

Py:   arr.index(x);  x in arr
来源：http://hz.xylfe.cn/gtoxyaqivd.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.ydjk.org.cn/gtoohwqwrr.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.hywenlv.cn/gtdyofgrqe.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.fengsongda.top/gtjwntkefo.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.xziqi.cn/gtxjygooys.html

Go:   slices.Index(arr, x)
来源：http://hz.zdqjudy.top/gtvtcrvskz.html

Ruby: arr.index(x)
来源：http://hz.fzhhl.top/gtuicfrdxz.html

C#:   list.IndexOf(x);
来源：http://hz.fzhhl.top/gtpwgevllt.html

[D13] 过滤（保留满足条件的）
来源：http://hz.guowangkeji.top/gtpdrzdeti.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.nanxuanxn.top/gtccwvmvcc.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.nwbrower.top/gtrhfmglpa.html

JS:   arr.filter(x => x > 3)
来源：http://hz.hnxiangtu.top/gtqmkawnqn.html

TS:   arr.filter(x => x > 3)
来源：http://hz.tianlin.xyz/gtpnadusmv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.snrcjt.cn/gthqosbyvd.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.yueranfly.top/gtpydyiskz.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.jyoumei.cn/gteleskgvl.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.zhijiandao.cn/gtphkxkvmu.html

[D14] 映射转换（每个元素变形）
来源：http://hz.zhaomingkeji.xyz/gteicmdwwp.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.hfpthk.cn/gtbebiiaus.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.cucudq.cn/gtttivcigs.html

JS:   arr.map(x => x * 2)
来源：http://hz.ppjwa.cn/gtqwxwbnru.html

TS:   arr.map(x => x * 2)
来源：http://hz.ydjk.org.cn/gtyvbnmiwb.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.yueranfly.top/gtescgqgzk.html

Go:   // 手写循环
来源：http://hz.ydjk.org.cn/gteuukvvss.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.yj202588.top/gtpkskwuqv.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.zhoulong.xyz/gtjfqnhnuu.html

[D15] 去重
来源：http://hz.zhiwuduotai.top/gtdengcbbu.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.cucudq.cn/gtfmesezwj.html

PHP:  array_unique($arr);
来源：http://hz.pycfn.com/gtzykytine.html

JS:   [...new Set(arr)]
来源：http://hz.sysykeji.top/gtzncdkztc.html

TS:   [...new Set(arr)]
来源：http://hz.jinyuanbaomall.cn/gtewdjegtg.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.chenlongwang.top/gttjtdddry.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.yongpay.top/gteqcuplss.html

Ruby: arr.uniq
来源：http://hz.jinqigufen.top/gtljwvsnhr.html

C#:   list.Distinct().ToList()
来源：http://hz.jqgufenzy.top/gtkugeirzi.html

[D16] 求和与平均值
来源：http://hz.316326.xyz/gttsawpbqn.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.ehwqpu.com/gtmrscpwnj.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.snrcjt.cn/gtlientoby.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yanxiufei.cn/gtfrzcpspl.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jinqigfzy.top/gtabmzobcr.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.yueranfly.top/gtrmftnybd.html

Go:   // 手写循环累加
来源：http://hz.zhaomingkeji.xyz/gtjzmmlydd.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.guannengcc.top/gtwwmgtxex.html

C#:   list.Sum();  list.Average()
来源：http://hz.ywan-chungtsiang.top/gtcjshgntf.html

[D17] 最大值与最小值
来源：http://hz.xziqi.cn/gtvmpvzmrx.html

Py:   max(arr);  min(arr)
来源：http://hz.iojbl.cn/gtacxcmenj.html

PHP:  max($arr);  min($arr);
来源：http://hz.ybcxt.top/gtyzkmhiab.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.aibaodan.cn/gtyctimycv.html

TS:   Math.max(...arr);
来源：http://hz.cashguo.top/gtckszrptw.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.yueranfly.top/gthdzocqqk.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.gzhubu.top/gtpxhumcqc.html

Ruby: arr.max;  arr.min
来源：http://hz.zhaomingkeji.xyz/gtktjdscgo.html

C#:   list.Max();  list.Min()
来源：http://hz.meibo888.top/gtviewhaoj.html

[D18] 扁平化嵌套数组
来源：http://hz.gotoacloud.top/gtvhixrqsc.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.sufxvd.cn/gtfuhrgobs.html

PHP:  array_merge(...$nested);
来源：http://hz.wangshuangyany.cn/gtzjfwyezv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.tian-w.cn/gtigqgxeqd.html

TS:   nested.flat();
来源：http://hz.ydjk.org.cn/gtibrdzgzf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.yuanzhike.top/gtmosohvra.html

Go:   // 手写双层循环
来源：http://hz.gogol.net.cn/gtguprgptu.html

Ruby: nested.flatten
来源：http://hz.pycfn.com/gtzejlyvzb.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.yuxming.cn/gtvkzizvrg.html

[D19] 按字段分组
来源：http://hz.jinqigfzy.top/gteeswhrqh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.c1oappe.top/gtboskmnnt.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.xuanzx.com/gtdbjtcwhq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.zdqjudy.top/gtdqoovebj.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.cashguo.top/gtmpnmdvgo.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.yj202588.top/gtiifvbpis.html

Go:   // 手写 map[string][]T
来源：http://hz.vqdsnc.cn/gtmiaahkls.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.cheryme.top/gtktsfsppq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.0kj1m.cn/gtyuwpmjbs.html

[D20] 统计每个元素出现次数
来源：http://hz.52xcode.cn/gtcoswimxk.html

Py:   Counter(arr)
来源：http://hz.c1oappe.top/gtnjpeqprm.html

PHP:  array_count_values($arr);
来源：http://hz.feifeiyinyue.top/gtjaqaucps.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jinqigfzy.top/gtmrvqdmum.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zycfv.cn/gtywaneogh.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.nwbrower.top/gthquutfwr.html

Go:   // 手写 map[T]int
来源：http://hz.fengsongda.top/gtefhsonuv.html

Ruby: arr.tally
来源：http://hz.hysaishi.cn/gtemwyesru.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.nanxuanxn.top/gtjsfaadyq.html

[D21] 判断是否包含某元素
来源：http://hz.ehwqpu.com/gtdbdgvbhs.html

Py:   x in arr
来源：http://hz.feifeiyinyue.top/gtmcjlsfdy.html

PHP:  in_array($x, $arr, true);
来源：http://hz.zhaomingkeji.xyz/gtpauovdyx.html

JS:   arr.includes(x)
来源：http://hz.zhijiandao.cn/gtcwdomnfj.html

TS:   arr.includes(x)
来源：http://hz.yj20258888.top/gtamsitdem.html

Java: list.contains(x)
来源：http://hz.sweek.top/gtubevasjg.html

Go:   slices.Contains(arr, x)
来源：http://hz.chenjidiqi.icu/gtfwjcwlvz.html

Ruby: arr.include?(x)
来源：http://hz.316326.xyz/gtlnanmynn.html

C#:   list.Contains(x)
来源：http://hz.snrcjt.cn/gtghdaixyw.html

[D22] 复制数组（避免共享引用）
来源：http://hz.cashguo.top/gtztbntqtb.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.mhx1999.top/gtlxjlvscv.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.chenjidiqi.icu/gtyynhzvgh.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.daria6918.cn/gtocwujaut.html

TS:   [...arr];
来源：http://hz.tian-w.cn/gtshczsqga.html

Java: new ArrayList<>(list);
来源：http://hz.hfpthk.cn/gtayprjobj.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.xylfe.cn/gtfbjqcpaf.html

Ruby: arr.dup;  arr.clone
来源：http://hz.xingfuxueyuan.xyz/gtllgcneyc.html

C#:   new List<int>(list);
来源：http://hz.ydjk.org.cn/gttdksadju.html

[D23] reduce 累积计算
来源：http://hz.zhijiandao.cn/gtaeigwvss.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.nwbrower.top/gtdbwfluxe.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.yj202588.top/gtjdwulmjc.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.smart0.xyz/gtpcekevuw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.feifeiyinyue.top/gtptqitphu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.gogol.net.cn/gtlpvorazm.html

Go:   // 手写循环
来源：http://hz.fzhhl.top/gtstnksqqs.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.zdqjudy.top/gtkjduytqa.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.guannengcc.top/gtfquygdak.html

[D24] 字典 / Map 基本操作
来源：http://hz.birdmap.top/gtxyxonegb.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.dashuyun.cn/gtauuluugw.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.jinqigufen.top/gtlezufxaq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.yj20258888.top/gtdtcqocgj.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.0kj1m.cn/gtfrvuezuk.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.jinqigufen.top/gtbkhexfvy.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.quarkkingdee.top/gtcbbuqxif.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.xinyue.icu/gtbhshspgk.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.hfpthk.cn/gthutowego.html

[D25] Set 集合去重与交并差
来源：http://hz.meibo888.top/gtyrnxarms.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.shuidangran.top/gtcjgzthva.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.zhixingplan.top/gtvvpiublz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.c1oappe.top/gtyjurgtgy.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.jinyuanbaomall.cn/gtaxwebjba.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.yvedp.cn/gtuvoviirj.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.cashguo.top/gtidrffcmg.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.0kj1m.cn/gttyxlngln.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.yj20258.top/gtaswecyqv.html

[D26] 数组转字符串
来源：http://hz.zhiwuduotai.top/gtadylheih.html

Py:   ", ".join(map(str, arr))
来源：http://hz.jqgfzy.top/gtrjobstug.html

PHP:  implode(", ", $arr);
来源：http://hz.0kj1m.cn/gtgwvfvviu.html

JS:   arr.join(", ")
来源：http://hz.cqqwz.cn/gtkxmshwhw.html

TS:   arr.join(", ")
来源：http://hz.zhoulong.xyz/gtghrqgqqk.html

Java: String.join(", ", list)
来源：http://hz.zhoulong.xyz/gtbwhkigij.html

Go:   strings.Join(strs, ", ")
来源：http://hz.yvedp.cn/gtrrurnmmf.html

Ruby: arr.join(", ")
来源：http://hz.jiagoushi.top/gtahirvhum.html

C#:   string.Join(", ", list)
来源：http://hz.andypj.xyz/gtynaqcehp.html

================================================================================
来源：http://hz.yanxiufei.cn/gtnfdpswbz.html

E. 字符串处理
来源：http://hz.yuxming.cn/gtpudsrorj.html

================================================================================
来源：http://hz.zhengqikj.top/gtdhenzaip.html

[E01] 拼接字符串
来源：http://hz.aizwys.cn/gtrojerlvc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.yongpay.top/gtrosdoohi.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.0kj1m.cn/gtkidoscfn.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.aibaodan.cn/gtzskvnoer.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.tanke756.top/gtapqacjty.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.haohaochexian.top/gtmbzzhcwt.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.9152youxi.cn/gtguvlewgk.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.ydjk.org.cn/gtpamqsrzn.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.mhx1999.top/gtvinekmyd.html

[E02] 重复字符串
来源：http://hz.tian-w.cn/gtblkippma.html

Py:   "ab" * 3
来源：http://hz.ydzc1.top/gtqswqgsql.html

PHP:  str_repeat("ab", 3);
来源：http://hz.feifeiyinyue.top/gtswzjjuqs.html

JS:   "ab".repeat(3)
来源：http://hz.cheryme.top/gtnuwpucah.html

TS:   "ab".repeat(3)
来源：http://hz.zhijiandao.cn/gtlpbxubeq.html

Java: "ab".repeat(3)
来源：http://hz.hysaishi.cn/gtnrmboigk.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.sxryk.cn/gtbtplyndm.html

Ruby: "ab" * 3
来源：http://hz.yonumen.top/gtznjcxxjm.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.feifeiyinyue.top/gtjujwmpnu.html

[E03] 截取子串
来源：http://hz.nanxuanxn.top/gtftmuhhki.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.aizwys.cn/gtkgchivhl.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.316326.xyz/gtefgfahsm.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.dashuyun.cn/gtjcgbykiv.html

TS:   s.slice(1, 4)
来源：http://hz.dianchejie.cn/gtoxznisvv.html

Java: s.substring(1, 4)
来源：http://hz.aibaodan.cn/gtcybopqgq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.nanxuanxn.top/gtqnthqvcy.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.dashuyun.cn/gtbjjmlaiq.html

C#:   s.Substring(1, 3)
来源：http://hz.yj20258888.top/gtloayvuzx.html

[E04] 查找子串位置
来源：http://hz.gzhubu.top/gtzssncvxh.html

Py:   s.find("x");  s.index("x")
来源：http://hz.quarkkingdee.top/gtdwjhossf.html

PHP:  strpos($s, "x");
来源：http://hz.yangfankeji.com/gtuajpncub.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.sufxvd.cn/gtvwaanung.html

TS:   s.indexOf("x")
来源：http://hz.jinghuilouyu.cn/gtvjldqywk.html

Java: s.indexOf("x")
来源：http://hz.vqdsnc.cn/gteopgnccd.html

Go:   strings.Index(s, "x")
来源：http://hz.hnqzz.top/gtskijtvnw.html

Ruby: s.index("x")
来源：http://hz.svipenyu.cn/gtggblvale.html

C#:   s.IndexOf("x")
来源：http://hz.hysaishi.cn/gtxqspscqr.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.jqgufenzy.top/gtlshaqmvu.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.jinqigufen.top/gtgajlhbnt.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.haohaochexian.top/gtrrgbzgrb.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.gaohongyu789.top/gtnuaagaam.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.xylfe.cn/gtxcyvecgk.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.hysaishi.cn/gtfoivsrri.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.shzxlz.cn/gtbcwjanlz.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.redwolf501.top/gtsnewnoen.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.xylfe.cn/gtqtuinzac.html

[E06] 替换子串
来源：http://hz.tian-w.cn/gtmenvaasr.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.ehwqpu.com/gtjcgcjprs.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.haohaochexian.top/gthktfspkt.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yj20258888.top/gttuccpesz.html

TS:   s.replaceAll("a", "b")
来源：http://hz.hywenlv.cn/gtwggrhgty.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.ybcxt.top/gtaqwvqsjs.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.haohaochexian.top/gtywlpudkv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.kuanghao11.cn/gteftnbaac.html

C#:   s.Replace("a", "b")
来源：http://hz.iojbl.cn/gtscncjygu.html

[E07] 按分隔符拆分
来源：http://hz.daxiang520.top/gtkmfgjleu.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.smart0.xyz/gtdpmqcxvi.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.guannengcc.top/gtykceowyq.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.yonumen.top/gtepjqmgbq.html

TS:   s.split(",")
来源：http://hz.xuetiantiany.cn/gtobungqmg.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.shangyingyoupin.top/gtpmcffprn.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.pengpengdd.cyou/gtpweaoiry.html

Ruby: s.split(",");  s.split
来源：http://hz.ydjk.org.cn/gttghqfyoh.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.chenzaomai.com/gtvmgffofn.html

[E08] 数组按分隔符合并
来源：http://hz.c1oappe.top/gtzogrykfl.html

Py:   ",".join(items)
来源：http://hz.jiagoushi.top/gtmfbnyxgm.html

PHP:  implode(",", $items);
来源：http://hz.c1oappe.top/gtgzpgovev.html

JS:   items.join(",")
来源：http://hz.jlsjyb.cn/gtiiatzmhj.html

TS:   items.join(",")
来源：http://hz.redwolf501.top/gthpblfdvb.html

Java: String.join(",", items)
来源：http://hz.hnqzz.top/gtvxuijdjd.html

Go:   strings.Join(items, ",")
来源：http://hz.jiagoushi.top/gtezhrcqjc.html

Ruby: items.join(",")
来源：http://hz.xuanzx.com/gtaafnqobr.html

C#:   string.Join(",", items)
来源：http://hz.ehwqpu.com/gtkeotcwon.html

[E09] 去除所有空白字符
来源：http://hz.52xcode.cn/gtlxvzfiof.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.yj20258888.top/gtdvnqxtdt.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.andypj.xyz/gtxhcfszxo.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.tanke756.top/gtgncgplsm.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.pycfn.com/gtkqjuyqxk.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.hysaishi.cn/gtnmdelofz.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.vqdsnc.cn/gtbjitucui.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.tanke756.top/gtgyxxmhxa.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.ybcxt.top/gtryuhzazw.html

[E10] 左侧补零 / 定长填充
来源：http://hz.jqgfzy.top/gtxwrsrgxi.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.wangshuangyany.cn/gtifkwosyq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.daria6918.cn/gttvmjkbqi.html

JS:   "7".padStart(3, "0")
来源：http://hz.cqqwz.cn/gtibfslieh.html

TS:   "7".padStart(3, "0")
来源：http://hz.ydjk.org.cn/gtpwzhbcnv.html

Java: String.format("%03d", 7)
来源：http://hz.hnxiangtu.top/gtlgdhubjp.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.xziqi.cn/gtjhfmytwr.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.haohaochexian.top/gtfttuctbj.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.c1oappe.top/gtqhztwwes.html

[E11] 反转字符串
来源：http://hz.daria6918.cn/gttaktzfgj.html

Py:   s[::-1]
来源：http://hz.daria6918.cn/gthptnlvvt.html

PHP:  strrev($s);
来源：http://hz.ivvv.top/gtxgcjkkfz.html

JS:   [...s].reverse().join("")
来源：http://hz.ehwqpu.com/gtdkubmmxi.html

TS:   [...s].reverse().join("")
来源：http://hz.chenzaomai.com/gtutvaxirs.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.ivvv.top/gtxbtxeqpd.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.ywan-chungtsiang.top/gtqynvqgyb.html

Ruby: s.reverse
来源：http://hz.gotoacloud.top/gtmbjhtsee.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.daria6918.cn/gtkonlfjkb.html

[E12] 统计某字符出现次数
来源：http://hz.cheryme.top/gtpklictfl.html

Py:   s.count("a")
来源：http://hz.316326.xyz/gtigpyzmen.html

PHP:  substr_count($s, "a");
来源：http://hz.yuxming.cn/gtjqiujcuy.html

JS:   s.split("a").length - 1
来源：http://hz.andypj.xyz/gtqqvekrtw.html

TS:   s.split("a").length - 1
来源：http://hz.ppjwa.cn/gtntdcybpi.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.yanxiufei.cn/gtzslnpbkx.html

Go:   strings.Count(s, "a")
来源：http://hz.gogol.net.cn/gtupqswgjs.html

Ruby: s.count("a")
来源：http://hz.ivvv.top/gtemhwpjzy.html

C#:   s.Count(c => c == 'a')
来源：http://hz.ivvv.top/gtmrpuvcgx.html

[E13] 逐字符遍历
来源：http://hz.hongshengwenyu.top/gthjfkmbgj.html


<!-- 参考信息 -->