代发 wailian999

C#:   list.Insert(0, 0);
来源：http://hz.yangfankeji.com/gtlmiurmur.html

[D04] 删除元素
来源：http://hz.yj20258.top/gtcrexuoau.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.shuidangran.top/gtapqfwves.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.zhixingplan.top/gtnwfpvgkh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.ydzc1.top/gtotsxpfwk.html

TS:   arr.splice(0, 1);
来源：http://hz.jqgufenzy.top/gtsbgddyzc.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.meibo888.top/gtrhypeqnz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.c1oappe.top/gtewjgffpu.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.aizwys.cn/gtdkbqnsed.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.aibaodan.cn/gtlvucvgsj.html

[D05] 访问与修改元素
来源：http://hz.ydzc1.top/gtrnbojpuc.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.smart0.xyz/gtumgvtrdi.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.yangfankeji.com/gthuhxnwso.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.zhiwuduotai.top/gtxerharwt.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.daxiang520.top/gthhzsycyd.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.xingfuxueyuan.xyz/gtilksnbvt.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.zhixingplan.top/gtzegywsyt.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.xylfe.cn/gthjgwgpcb.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.jqgfzy.top/gtlcjpdqjz.html

[D06] 数组长度
来源：http://hz.jqgfzy.top/gtaasjzatf.html

Py:   len(arr)
来源：http://hz.0kj1m.cn/gtxnryyxbw.html

PHP:  count($arr);
来源：http://hz.dashuyun.cn/gtnuqglkca.html

JS:   arr.length
来源：http://hz.jlsjyb.cn/gtikurfxhd.html

TS:   arr.length
来源：http://hz.hongshengwenyu.top/gtxdtxhqrz.html

Java: list.size();
来源：http://hz.snrcjt.cn/gtrzwtfnsq.html

Go:   len(arr)
来源：http://hz.redwolf501.top/gtfurzpnpe.html

Ruby: arr.length; arr.size
来源：http://hz.shzxlz.cn/gtedknndom.html

C#:   list.Count;
来源：http://hz.jinghuilouyu.cn/gtosttzkol.html

[D07] 切片 / 取子数组
来源：http://hz.wangshuangyany.cn/gtctkdlfda.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.sufxvd.cn/gtcxgsoyek.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.zhoulong.xyz/gtfnxzofhl.html

JS:   arr.slice(1, 4);
来源：http://hz.yangfankeji.com/gttynkelka.html

TS:   arr.slice(1, 4);
来源：http://hz.hongshengwenyu.top/gtpeozmrnt.html

Java: list.subList(1, 4);
来源：http://hz.hfpthk.cn/gteudknjdq.html

Go:   arr[1:4]
来源：http://hz.shzxlz.cn/gtcshsctdz.html

Ruby: arr[1, 3]
来源：http://hz.jqgfzy.top/gtvxzcskxu.html

C#:   list.GetRange(1, 3);
来源：http://hz.shanyushiyangkeji.top/gtmxxbnjlr.html

[D08] 合并两个数组
来源：http://hz.zhongyouzk.top/gtlwzlqdla.html

Py:   a + b;  a.extend(b)
来源：http://hz.chenjidiqi.icu/gtaspoisop.html

PHP:  array_merge($a, $b);
来源：http://hz.zdqjudy.top/gtmpsevutw.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.wangdashe.top/gttskecdzw.html

TS:   [...a, ...b];
来源：http://hz.dianchejie.cn/gtrstscgma.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.cheryme.top/gtpboemugv.html

Go:   append(a, b...)
来源：http://hz.shangyingyoupin.top/gtjhmjskop.html

Ruby: a + b;  a.concat(b)
来源：http://hz.zdqjudy.top/gtwwkrkazx.html

C#:   a.Concat(b).ToList()
来源：http://hz.quarkkingdee.top/gtvyaxucwq.html

[D09] 排序（升序）
来源：http://hz.chenlongwang.top/gteqbvqwoc.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.sufxvd.cn/gtqzuoggke.html

PHP:  sort($arr);
来源：http://hz.bjfxy.top/gtfbfplhaf.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.hammf.cn/gtgmyxalqx.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.yuanzhike.top/gtpwdogeuo.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.andypj.xyz/gtfrdhqnpx.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.zhongyouzk.top/gtxwgteetq.html

Ruby: arr.sort
来源：http://hz.quarkkingdee.top/gtcpzaocxc.html

C#:   list.Sort();
来源：http://hz.52xcode.cn/gtdqaignjz.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.jinghuilouyu.cn/gtyeqnykst.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.birdmap.top/gtumrszgrr.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yj20258.top/gtchgamnur.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hongshengwenyu.top/gtmjmzxgqj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hywenlv.cn/gtlfalxzfm.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.sufxvd.cn/gtobhfgoud.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.iojbl.cn/gtbztumdaw.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.chenlongwang.top/gtxgekekyn.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.zhongyouzk.top/gtelnvlmqm.html

[D11] 反转数组
来源：http://hz.hongshengwenyu.top/gtqdoisfwa.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.yangfankeji.com/gtcapvauwi.html

PHP:  array_reverse($arr);
来源：http://hz.shuidangran.top/gturgalzhr.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.yuanzhike.top/gtqalfzqil.html

TS:   [...arr].reverse();
来源：http://hz.sxryk.cn/gtkhplyhha.html

Java: Collections.reverse(list);
来源：http://hz.ppjwa.cn/gtuotzdzss.html

Go:   slices.Reverse(arr)
来源：http://hz.hammf.cn/gtodxeodst.html

Ruby: arr.reverse
来源：http://hz.zhaomingkeji.xyz/gtxtptqjbc.html

C#:   list.Reverse();
来源：http://hz.52xcode.cn/gtipwpvqce.html

[D12] 查找元素下标
来源：http://hz.ppjwa.cn/gtntkcsxpq.html

Py:   arr.index(x);  x in arr
来源：http://hz.jlsjyb.cn/gtorsiongr.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.shzxlz.cn/gteukaybbg.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.xingfuxueyuan.xyz/gtnbweihnj.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.cheryme.top/gtbucmntrc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.yuanzhike.top/gtqvxpataf.html

Go:   slices.Index(arr, x)
来源：http://hz.yuxming.cn/gtveuqjdex.html

Ruby: arr.index(x)
来源：http://hz.yangfankeji.com/gtadpcusbd.html

C#:   list.IndexOf(x);
来源：http://hz.guowangkeji.top/gtkkfjnfae.html

[D13] 过滤（保留满足条件的）
来源：http://hz.fengsongda.top/gttoqmrexj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.xylfe.cn/gtpomrwvva.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.mhx1999.top/gtatufuand.html

JS:   arr.filter(x => x > 3)
来源：http://hz.gotoacloud.top/gtfpkjdzax.html

TS:   arr.filter(x => x > 3)
来源：http://hz.hongshengwenyu.top/gtkcdfemxr.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.cashguo.top/gtqbwaspmk.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.hammf.cn/gtpxfajfyl.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.zhaomingkeji.xyz/gtgzhhszne.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.shzxlz.cn/gtznpktsgg.html

[D14] 映射转换（每个元素变形）
来源：http://hz.cdnleiting.top/gtfvhtajpa.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.hywenlv.cn/gtoctyavql.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.ydzc1.top/gthditudqe.html

JS:   arr.map(x => x * 2)
来源：http://hz.52xcode.cn/gtwslpulzg.html

TS:   arr.map(x => x * 2)
来源：http://hz.meibo888.top/gtthrxbveq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.chenzaomai.com/gtrtnruwsg.html

Go:   // 手写循环
来源：http://hz.xziqi.cn/gtsxzoilpg.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.sysykeji.top/gtmwrentmp.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.zhongyouzk.top/gtdkjdrcdh.html

[D15] 去重
来源：http://hz.shanyushiyangkeji.top/gthvhxjfnj.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.ydjk.org.cn/gtyvexacce.html

PHP:  array_unique($arr);
来源：http://hz.ywan-chungtsiang.top/gtfktpfxfc.html

JS:   [...new Set(arr)]
来源：http://hz.cqqwz.cn/gtkvgefdzh.html

TS:   [...new Set(arr)]
来源：http://hz.xziqi.cn/gtgovqdkcb.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.hywenlv.cn/gtewatatti.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.fzhhl.top/gttzgvatdl.html

Ruby: arr.uniq
来源：http://hz.chenjidiqi.icu/gtxyhiojfi.html

C#:   list.Distinct().ToList()
来源：http://hz.yj20258.top/gtyiihruwv.html

[D16] 求和与平均值
来源：http://hz.sxryk.cn/gtfafveucq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.ehwqpu.com/gttxxosvms.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.yonumen.top/gtbumgsfxw.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zhongyouzk.top/gtmnrtlucq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.daria6918.cn/gtqjebewgi.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.yonumen.top/gtedblpdxf.html

Go:   // 手写循环累加
来源：http://hz.tianlin.xyz/gtquzkpwgx.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.tian-w.cn/gtdpbuadhr.html

C#:   list.Sum();  list.Average()
来源：http://hz.yongpay.top/gtapkhqlec.html

[D17] 最大值与最小值
来源：http://hz.cheryme.top/gtpgfplmvd.html

Py:   max(arr);  min(arr)
来源：http://hz.shanyushiyangtech.top/gtcqximwux.html

PHP:  max($arr);  min($arr);
来源：http://hz.yongpay.top/gtuobewdpc.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.ywan-chungtsiang.top/gtrcevbgcy.html

TS:   Math.max(...arr);
来源：http://hz.jqgfzy.top/gthidcbqgf.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.jinghuilouyu.cn/gttmxsxlfn.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.jinghuilouyu.cn/gtqagbiagc.html

Ruby: arr.max;  arr.min
来源：http://hz.9152youxi.cn/gtaornwoep.html

C#:   list.Max();  list.Min()
来源：http://hz.shuidangran.top/gtdlmoboij.html

[D18] 扁平化嵌套数组
来源：http://hz.pycfn.com/gtsrprpldu.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.haohaochexian.top/gtqxpwfqoh.html

PHP:  array_merge(...$nested);
来源：http://hz.ydzc1.top/gtnzwzrlpe.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.ehwqpu.com/gtjfwgbhlw.html

TS:   nested.flat();
来源：http://hz.yonumen.top/gtoorzqqeq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.sxryk.cn/gtpefjuzfi.html

Go:   // 手写双层循环
来源：http://hz.fengsongda.top/gthxovsdrw.html

Ruby: nested.flatten
来源：http://hz.quarkkingdee.top/gtuxcggfsu.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.hysaishi.cn/gtfuiuqiwq.html

[D19] 按字段分组
来源：http://hz.yueranfly.top/gtshdkwaov.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.shanyushiyangtech.top/gtlqbkffma.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.jiagoushi.top/gtholpbvcx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.zdqjudy.top/gtgkhazmxj.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.svipenyu.cn/gtniybbnvo.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.jinghuilouyu.cn/gtgdrgzgto.html

Go:   // 手写 map[string][]T
来源：http://hz.jiagoushi.top/gtanuyfssp.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.9152youxi.cn/gtujmadeyo.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.hnqzz.top/gtcewbeekh.html

[D20] 统计每个元素出现次数
来源：http://hz.andypj.xyz/gtgntodchz.html

Py:   Counter(arr)
来源：http://hz.yj202588.top/gtiartqpus.html

PHP:  array_count_values($arr);
来源：http://hz.hongshengwenyu.top/gtsvdxloli.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.nanxinkj.top/gtqsfxborj.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.shzxlz.cn/gteuujashj.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.andypj.xyz/gtrcjvnbjo.html

Go:   // 手写 map[T]int
来源：http://hz.sxryk.cn/gtelgkjmhe.html

Ruby: arr.tally
来源：http://hz.gogol.net.cn/gtgvrcxctx.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.gzhubu.top/gtbzpjiytt.html

[D21] 判断是否包含某元素
来源：http://hz.hysaishi.cn/gtdqrcgguw.html

Py:   x in arr
来源：http://hz.yj20258.top/gtiomurwtm.html

PHP:  in_array($x, $arr, true);
来源：http://hz.wangdashe.top/gtyoitqavz.html

JS:   arr.includes(x)
来源：http://hz.jlsjyb.cn/gtqovqsihm.html

TS:   arr.includes(x)
来源：http://hz.ppjwa.cn/gtsxquoemt.html

Java: list.contains(x)
来源：http://hz.zhengqikj.top/gtspbgmyzr.html

Go:   slices.Contains(arr, x)
来源：http://hz.aizwys.cn/gtblayflup.html

Ruby: arr.include?(x)
来源：http://hz.ppjwa.cn/gtqgaelxbq.html

C#:   list.Contains(x)
来源：http://hz.jinqigufen.top/gttawifubv.html

[D22] 复制数组（避免共享引用）
来源：http://hz.mhx1999.top/gttxlsnolc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.shanyushiyangkeji.top/gtzmtrganm.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.316326.xyz/gtwmwhlshj.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.nwbrower.top/gtcxftcovi.html

TS:   [...arr];
来源：http://hz.shanyushiyangkeji.top/gtnevatgsi.html

Java: new ArrayList<>(list);
来源：http://hz.yvedp.cn/gtaeepezzy.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.zhiwuduotai.top/gtjilttncu.html

Ruby: arr.dup;  arr.clone
来源：http://hz.dashuyun.cn/gtfqcrpxvx.html

C#:   new List<int>(list);
来源：http://hz.dianchejie.cn/gtflizbfsr.html

[D23] reduce 累积计算
来源：http://hz.yj202588.top/gtjarqkpiz.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.redwolf501.top/gtrpoojoix.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.fzhhl.top/gtpojtubnt.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yuanzhike.top/gtoojoemqd.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.hfpthk.cn/gtxtjwgkji.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.ywan-chungtsiang.top/gtbqtqlzob.html

Go:   // 手写循环
来源：http://hz.svipenyu.cn/gtisbpbatt.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.shzxlz.cn/gtooflrsaa.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.wangdashe.top/gtedaubrgw.html

[D24] 字典 / Map 基本操作
来源：http://hz.sufxvd.cn/gtjcauepff.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.yangfankeji.com/gtbmsszqqn.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.sweek.top/gtvnpqpowp.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.hysaishi.cn/gtdcgdanux.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.smart0.xyz/gtxiwiorqs.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.cashguo.top/gtymvoltns.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.fengsongda.top/gtzaadkpgc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.0kj1m.cn/gtrhtdbozx.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.cqqwz.cn/gtijapuqbg.html

[D25] Set 集合去重与交并差
来源：http://hz.yuxming.cn/gtrnluyawy.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.hnqzz.top/gthvysrdhn.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.xinyue.icu/gtxtrvqwjf.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.zhiwuduotai.top/gtyvktthpf.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.havefunace.top/gtyfmuscmd.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.zycfv.cn/gtbbyckdii.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.yuanzhike.top/gtzfrkgmer.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.snrcjt.cn/gtunxsppeo.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.quarkkingdee.top/gttkbeizab.html

[D26] 数组转字符串
来源：http://hz.jlsjyb.cn/gtdzwmtxgh.html

Py:   ", ".join(map(str, arr))
来源：http://hz.zycfv.cn/gtnuthkdmv.html

PHP:  implode(", ", $arr);
来源：http://hz.wangshuangyany.cn/gtvkdzpjnk.html

JS:   arr.join(", ")
来源：http://hz.ydjk.org.cn/gtdhwkgjbl.html

TS:   arr.join(", ")
来源：http://hz.zhaomingkeji.xyz/gtdyublpar.html

Java: String.join(", ", list)
来源：http://hz.tianlin.xyz/gtbhlxsuci.html

Go:   strings.Join(strs, ", ")
来源：http://hz.cheryme.top/gtnlhjxcmr.html

Ruby: arr.join(", ")
来源：http://hz.fzhhl.top/gtyfvxxopm.html

C#:   string.Join(", ", list)
来源：http://hz.xuanzx.com/gtsxduoxcm.html

================================================================================
来源：http://hz.daxiang520.top/gtzgcnytjt.html

E. 字符串处理
来源：http://hz.birdmap.top/gthdvurinh.html

================================================================================
来源：http://hz.c1oappe.top/gtoojniyje.html

[E01] 拼接字符串
来源：http://hz.c1oappe.top/gtmuewkrib.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.hnxiangtu.top/gtnvcppiwl.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.birdmap.top/gthkrajlkd.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.52xcode.cn/gtuopjwzyh.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.xuanzx.com/gtxeloxvvv.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.svipenyu.cn/gtmbiqhvpr.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.bjfxy.top/gtrxxgfxrm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.9152youxi.cn/gtpodxvnfi.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.zhongyouzk.top/gtwxmkfrkf.html

[E02] 重复字符串
来源：http://hz.hnqzz.top/gtvbyjidtb.html

Py:   "ab" * 3
来源：http://hz.yvedp.cn/gtveclotun.html

PHP:  str_repeat("ab", 3);
来源：http://hz.meibo888.top/gteziwmynr.html

JS:   "ab".repeat(3)
来源：http://hz.xuanzx.com/gtkronaiqx.html

TS:   "ab".repeat(3)
来源：http://hz.gogol.net.cn/gtwofaybyf.html

Java: "ab".repeat(3)
来源：http://hz.mhx1999.top/gtqhovpxma.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.aibaodan.cn/gtpsnjciks.html

Ruby: "ab" * 3
来源：http://hz.chenjidiqi.icu/gtxypyctrk.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.sufxvd.cn/gttcbdreba.html

[E03] 截取子串
来源：http://hz.cdnleiting.top/gthmjmoxkr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.chenzaomai.com/gtvkmaiwrf.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.haohaochexian.top/gtsukstjoc.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.zhiwuduotai.top/gtmdgjvxpw.html

TS:   s.slice(1, 4)
来源：http://hz.cashguo.top/gtpjrdgwco.html

Java: s.substring(1, 4)
来源：http://hz.shanyushiyangtech.top/gtmwgtieup.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.xuetiantiany.cn/gtvsinrmvj.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.zhijiandao.cn/gtgnnwcggc.html

C#:   s.Substring(1, 3)
来源：http://hz.jyoumei.cn/gtvezubgdx.html

[E04] 查找子串位置
来源：http://hz.chenjidiqi.icu/gtbcczacpm.html

Py:   s.find("x");  s.index("x")
来源：http://hz.gaohongyu789.top/gtmdlpoltb.html

PHP:  strpos($s, "x");
来源：http://hz.iojbl.cn/gtgpucbjxp.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.xylfe.cn/gtomkderpf.html

TS:   s.indexOf("x")
来源：http://hz.ivvv.top/gtlnctyxfn.html

Java: s.indexOf("x")
来源：http://hz.feifeiyinyue.top/gtpdfngdct.html

Go:   strings.Index(s, "x")
来源：http://hz.bjfxy.top/gtulswniae.html

Ruby: s.index("x")
来源：http://hz.gzhubu.top/gtwrttsber.html

C#:   s.IndexOf("x")
来源：http://hz.hongshengwenyu.top/gtkvpqxykv.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.cucudq.cn/gtfygxzmci.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.yuanzhike.top/gtjgjxfgfv.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.gotoacloud.top/gtpgyaohrb.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.wangshuangyany.cn/gtguqnqeqm.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.9152youxi.cn/gtagnrrkag.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.birdmap.top/gtgbcfkuvw.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.0kj1m.cn/gtpswhxjss.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.kuanghao11.cn/gtyertbohz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.sufxvd.cn/gtgvdcijsg.html

[E06] 替换子串
来源：http://hz.wangshuangyany.cn/gtqcnkhfvz.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.yonumen.top/gtxtvxjzdx.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.havefunace.top/gtrfmcxalo.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.redwolf501.top/gtmoiokucr.html

TS:   s.replaceAll("a", "b")
来源：http://hz.cheryme.top/gteabggxgi.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.shuidangran.top/gtsuframvp.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.andypj.xyz/gtyokouhfg.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.hnxiangtu.top/gtddbborma.html

C#:   s.Replace("a", "b")
来源：http://hz.daxiang520.top/gtmrrgwguf.html

[E07] 按分隔符拆分
来源：http://hz.sxryk.cn/gtminuuqrb.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.andypj.xyz/gtorjnwhfu.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.hnxiangtu.top/gtvjynjnmi.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.zhaomingkeji.xyz/gthtxcdmrd.html

TS:   s.split(",")
来源：http://hz.jinghuilouyu.cn/gtuwqaezpc.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.smart0.xyz/gtphctymoa.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.ivvv.top/gtgxrbkrpu.html

Ruby: s.split(",");  s.split
来源：http://hz.xinyue.icu/gtmefalvhf.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.sxryk.cn/gtqmrdxkat.html

[E08] 数组按分隔符合并
来源：http://hz.cucudq.cn/gtxnuldnqn.html

Py:   ",".join(items)
来源：http://hz.cucudq.cn/gtomtkmvqs.html

PHP:  implode(",", $items);
来源：http://hz.aizwys.cn/gtpmzwrunh.html

JS:   items.join(",")
来源：http://hz.yuanzhike.top/gtmdicatlg.html

TS:   items.join(",")
来源：http://hz.jinghuilouyu.cn/gtbrdvwbjr.html

Java: String.join(",", items)
来源：http://hz.shangyingyoupin.top/gtoybpzxqv.html

Go:   strings.Join(items, ",")
来源：http://hz.mhx1999.top/gtlclcghvn.html

Ruby: items.join(",")
来源：http://hz.svipenyu.cn/gtfsyryvls.html

C#:   string.Join(",", items)
来源：http://hz.hongshengwenyu.top/gtwhvbpvsm.html

[E09] 去除所有空白字符
来源：http://hz.jinqigfzy.top/gtmlfaokqe.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.smart0.xyz/gttvctvjic.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.shanyushiyangtech.top/gteplintbi.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.meibo888.top/gtkprjxtzf.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.zhongyouzk.top/gtifwwbech.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.ivvv.top/gtbzzykoet.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.dianchejie.cn/gtatmyuyzz.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.feifeiyinyue.top/gtxypnjaoi.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.cheryme.top/gtcatggafj.html

[E10] 左侧补零 / 定长填充
来源：http://hz.ppjwa.cn/gttykpoewj.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.dashuyun.cn/gthfgnditz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.feifeiyinyue.top/gtfnhhqplh.html

JS:   "7".padStart(3, "0")
来源：http://hz.yj20258888.top/gtopuggmeu.html

TS:   "7".padStart(3, "0")
来源：http://hz.cqqwz.cn/gtsjxzydst.html

Java: String.format("%03d", 7)
来源：http://hz.aizwys.cn/gtdrenwcdk.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.gogol.net.cn/gtgqagkfnz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.zhaomingkeji.xyz/gtifczecnh.html


<!-- 参考信息 -->