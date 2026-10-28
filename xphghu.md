代发 wailian999

TS:   arr.splice(0, 0, 0);
来源：http://hz.vqdsnc.cn/gttzzvdfog.html

Java: list.add(0, 0);
来源：http://hz.jiagoushi.top/gtonvrmupr.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.zycfv.cn/gtqtsyydno.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.sweek.top/gtlzlsdaus.html

C#:   list.Insert(0, 0);
来源：http://hz.shzxlz.cn/gtrabfozrw.html

[D04] 删除元素
来源：http://hz.ybcxt.top/gtiuarnipb.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.cdnleiting.top/gtclapwnpv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.quarkkingdee.top/gtihqjsypx.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.ydzc1.top/gtwjpaueul.html

TS:   arr.splice(0, 1);
来源：http://hz.guowangkeji.top/gtinjfmuth.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.xingfuxueyuan.xyz/gtykozmaka.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.yongpay.top/gtxaalmvps.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.yuanzhike.top/gtplycijvv.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.cqqwz.cn/gtlwewcnbp.html

[D05] 访问与修改元素
来源：http://hz.jianghu66.top/gtiujwxxbd.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jinqigufen.top/gtoqrrtoxr.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.andypj.xyz/gtqfanohdi.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.yj20258.top/gtaywvnyax.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.yanxiufei.cn/gthekeyoqc.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.tianlin.xyz/gtfeivydry.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.havefunace.top/gtxtsbsgts.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yj202588.top/gtfbqzqoax.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.jqgufenzy.top/gtpyplcnmx.html

[D06] 数组长度
来源：http://hz.zhixingplan.top/gtjhmywvfw.html

Py:   len(arr)
来源：http://hz.jqgufenzy.top/gtncxmiaxk.html

PHP:  count($arr);
来源：http://hz.zhengqikj.top/gtgcuwqhpn.html

JS:   arr.length
来源：http://hz.vqdsnc.cn/gtvjpgqfao.html

TS:   arr.length
来源：http://hz.gzhubu.top/gtdwevywuy.html

Java: list.size();
来源：http://hz.chenlongwang.top/gtgwxdvmqt.html

Go:   len(arr)
来源：http://hz.tianlin.xyz/gtegwxhsab.html

Ruby: arr.length; arr.size
来源：http://hz.ydjk.org.cn/gtoywvwkpu.html

C#:   list.Count;
来源：http://hz.tanke756.top/gtatdarhue.html

[D07] 切片 / 取子数组
来源：http://hz.hnqzz.top/gtgwfrckhq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.tanke756.top/gtvkngwkia.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.sysykeji.top/gtgyakcwzu.html

JS:   arr.slice(1, 4);
来源：http://hz.ppjwa.cn/gtaqlswbjm.html

TS:   arr.slice(1, 4);
来源：http://hz.yueranfly.top/gtampjofhi.html

Java: list.subList(1, 4);
来源：http://hz.shuidangran.top/gtajwsfxci.html

Go:   arr[1:4]
来源：http://hz.nanxinkj.top/gtzcqdjwll.html

Ruby: arr[1, 3]
来源：http://hz.xinyue.icu/gtiqitrrdi.html

C#:   list.GetRange(1, 3);
来源：http://hz.hywenlv.cn/gtsvvnlmbw.html

[D08] 合并两个数组
来源：http://hz.svipenyu.cn/gtzvfmskpn.html

Py:   a + b;  a.extend(b)
来源：http://hz.zycfv.cn/gtldzuqiig.html

PHP:  array_merge($a, $b);
来源：http://hz.yongpay.top/gtbdzowhmw.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.ppjwa.cn/gtiftfdsoc.html

TS:   [...a, ...b];
来源：http://hz.yanxiufei.cn/gtxnnelrdg.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.yj202588.top/gtvojviopu.html

Go:   append(a, b...)
来源：http://hz.gogol.net.cn/gtfnyjjcut.html

Ruby: a + b;  a.concat(b)
来源：http://hz.shanyushiyangtech.top/gtzkaqnpld.html

C#:   a.Concat(b).ToList()
来源：http://hz.shanyushiyangkeji.top/gtdpsjheey.html

[D09] 排序（升序）
来源：http://hz.zhaomingkeji.xyz/gtiqosigxq.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.gzhubu.top/gttoumhwmf.html

PHP:  sort($arr);
来源：http://hz.sufxvd.cn/gtayohoysq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.zhoulong.xyz/gtnzmdguye.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.hnqzz.top/gtrjzyassm.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.sxryk.cn/gtbbrtoahy.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.xuanzx.com/gtcsqwsfnv.html

Ruby: arr.sort
来源：http://hz.yongpay.top/gtqnbrwoxy.html

C#:   list.Sort();
来源：http://hz.ivvv.top/gtsfodwqab.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.shanyushiyangkeji.top/gtaagzsiqq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.cucudq.cn/gtrmlpejfx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.daria6918.cn/gtnvgmkucb.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.pycfn.com/gtcoadkjhp.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yuxming.cn/gtagfbylsf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.xuetiantiany.cn/gtsrwjvyua.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.cashguo.top/gtdfnucvug.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.nanxinkj.top/gtzybvbfcq.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.wangshuangyany.cn/gtgfxgpzac.html

[D11] 反转数组
来源：http://hz.guowangkeji.top/gteukbbidg.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.aibaodan.cn/gtqxzrdhrb.html

PHP:  array_reverse($arr);
来源：http://hz.cqqwz.cn/gtfffxzhoz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.xylfe.cn/gtkdursuxx.html

TS:   [...arr].reverse();
来源：http://hz.xuanzx.com/gtvnefpeml.html

Java: Collections.reverse(list);
来源：http://hz.zhengqikj.top/gtwcbnndcc.html

Go:   slices.Reverse(arr)
来源：http://hz.jinghuilouyu.cn/gtmgvkrrud.html

Ruby: arr.reverse
来源：http://hz.yuanzhike.top/gteqdykmuc.html

C#:   list.Reverse();
来源：http://hz.tianlin.xyz/gtoloxycyb.html

[D12] 查找元素下标
来源：http://hz.hnxiangtu.top/gtquuxgddy.html

Py:   arr.index(x);  x in arr
来源：http://hz.havefunace.top/gtcdbxywow.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.guowangkeji.top/gtjzzzhryo.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.chenjidiqi.icu/gttnpfezpt.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.aibaodan.cn/gtimmrxych.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.ivvv.top/gtqjymqliq.html

Go:   slices.Index(arr, x)
来源：http://hz.dashuyun.cn/gtucgnucxc.html

Ruby: arr.index(x)
来源：http://hz.zhijiandao.cn/gtwcgamuvh.html

C#:   list.IndexOf(x);
来源：http://hz.yj202588.top/gtemelsbqr.html

[D13] 过滤（保留满足条件的）
来源：http://hz.hnqzz.top/gtipcvkskz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.yanxiufei.cn/gtvgttzkae.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.hnxiangtu.top/gtyvvsygwa.html

JS:   arr.filter(x => x > 3)
来源：http://hz.52xcode.cn/gtphdtbwet.html

TS:   arr.filter(x => x > 3)
来源：http://hz.redwolf501.top/gtagzsofaj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.yj20258.top/gtnwwycxqq.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.iojbl.cn/gtkyqeaior.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.xinyue.icu/gtrerxhzof.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.sxryk.cn/gtgnsjoryk.html

[D14] 映射转换（每个元素变形）
来源：http://hz.yueranfly.top/gtthyfhddg.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.smart0.xyz/gtannsatep.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.yuxming.cn/gtbtrlhoaq.html

JS:   arr.map(x => x * 2)
来源：http://hz.jinqigufen.top/gttndeqhos.html

TS:   arr.map(x => x * 2)
来源：http://hz.gogol.net.cn/gtxqoaiosg.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.shangyingyoupin.top/gtkbsytdiv.html

Go:   // 手写循环
来源：http://hz.gaohongyu789.top/gtqnnmbvov.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.kuanghao11.cn/gtuwresaiq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.zhixingplan.top/gtmjlbbgdv.html

[D15] 去重
来源：http://hz.jinqigufen.top/gtzbyulals.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.cdnleiting.top/gtdyakqxbh.html

PHP:  array_unique($arr);
来源：http://hz.xylfe.cn/gtupnxxwzx.html

JS:   [...new Set(arr)]
来源：http://hz.zhaomingkeji.xyz/gtugzljalr.html

TS:   [...new Set(arr)]
来源：http://hz.xuanzx.com/gtayqfwxoz.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.dianchejie.cn/gtybjfsdae.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.yangfankeji.com/gtjxjvhfha.html

Ruby: arr.uniq
来源：http://hz.316326.xyz/gtqvhcopji.html

C#:   list.Distinct().ToList()
来源：http://hz.cdnleiting.top/gttfgqnwgf.html

[D16] 求和与平均值
来源：http://hz.wangshuangyany.cn/gthvjcnqgb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.fengsongda.top/gtgmrdzxbj.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.ydzc1.top/gtidgmokru.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.gaohongyu789.top/gtuvytgfgk.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.vqdsnc.cn/gtvftubury.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.ywan-chungtsiang.top/gtpcivbbxx.html

Go:   // 手写循环累加
来源：http://hz.hnqzz.top/gtirfmtkua.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.52xcode.cn/gtckjovvmf.html

C#:   list.Sum();  list.Average()
来源：http://hz.xinyue.icu/gtkgqfhmig.html

[D17] 最大值与最小值
来源：http://hz.gotoacloud.top/gtepgjqcpu.html

Py:   max(arr);  min(arr)
来源：http://hz.xylfe.cn/gtnugiixvg.html

PHP:  max($arr);  min($arr);
来源：http://hz.dianchejie.cn/gtgtcqeyvt.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.hfpthk.cn/gtscarcikf.html

TS:   Math.max(...arr);
来源：http://hz.nanxinkj.top/gtmrbrzgwt.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.yongpay.top/gtijnvisun.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.zhongyouzk.top/gtoessncjj.html

Ruby: arr.max;  arr.min
来源：http://hz.shzxlz.cn/gtkjteppsv.html

C#:   list.Max();  list.Min()
来源：http://hz.tanke756.top/gtbeuxnqjv.html

[D18] 扁平化嵌套数组
来源：http://hz.gotoacloud.top/gtawlugywj.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.xziqi.cn/gthbowvurt.html

PHP:  array_merge(...$nested);
来源：http://hz.meibo888.top/gtwylubvkz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.jinqigfzy.top/gtaojnfseq.html

TS:   nested.flat();
来源：http://hz.ivvv.top/gtlmiofqsg.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.nanxuanxn.top/gtkikqixqz.html

Go:   // 手写双层循环
来源：http://hz.daria6918.cn/gtdhdvudcm.html

Ruby: nested.flatten
来源：http://hz.gogol.net.cn/gtwptihvzk.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.sufxvd.cn/gtovkprccy.html

[D19] 按字段分组
来源：http://hz.xuetiantiany.cn/gtimjnghzo.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.yvedp.cn/gtpfwpbtdp.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.cucudq.cn/gttkuhyfhf.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.xylfe.cn/gtxtnbpjjl.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.zdqjudy.top/gtjzhltqlk.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.jqgufenzy.top/gtizivtfia.html

Go:   // 手写 map[string][]T
来源：http://hz.xingfuxueyuan.xyz/gtbnytyznh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.aibaodan.cn/gtuwdxdstf.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.daxiang520.top/gtcblehhlk.html

[D20] 统计每个元素出现次数
来源：http://hz.xinyue.icu/gtjotfgvph.html

Py:   Counter(arr)
来源：http://hz.dianchejie.cn/gtioaokwlx.html

PHP:  array_count_values($arr);
来源：http://hz.jinghuilouyu.cn/gtsjcnmopt.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zhijiandao.cn/gtdwubirij.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zhoulong.xyz/gtrtigocia.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.smart0.xyz/gtkaqnstnf.html

Go:   // 手写 map[T]int
来源：http://hz.nwbrower.top/gtadmnsngq.html

Ruby: arr.tally
来源：http://hz.zycfv.cn/gtwcmotnpj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.chenlongwang.top/gtluychfrt.html

[D21] 判断是否包含某元素
来源：http://hz.tanke756.top/gthqlbxzzj.html

Py:   x in arr
来源：http://hz.smart0.xyz/gtnllohvmd.html

PHP:  in_array($x, $arr, true);
来源：http://hz.daria6918.cn/gtpgvogopa.html

JS:   arr.includes(x)
来源：http://hz.ydzc1.top/gtdevjphqs.html

TS:   arr.includes(x)
来源：http://hz.jinqigufen.top/gtfcjjbprz.html

Java: list.contains(x)
来源：http://hz.wangshuangyany.cn/gtrizerphf.html

Go:   slices.Contains(arr, x)
来源：http://hz.hysaishi.cn/gtcxqmnjba.html

Ruby: arr.include?(x)
来源：http://hz.svipenyu.cn/gtvczjfdbc.html

C#:   list.Contains(x)
来源：http://hz.zdqjudy.top/gtjcegfwtc.html

[D22] 复制数组（避免共享引用）
来源：http://hz.sufxvd.cn/gtcshmusxt.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.wangdashe.top/gtiueabnqo.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.hnqzz.top/gtvmzabtuz.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.cqqwz.cn/gttkhmeqta.html

TS:   [...arr];
来源：http://hz.redwolf501.top/gtkbqplmhv.html

Java: new ArrayList<>(list);
来源：http://hz.tianlin.xyz/gtuzeqfltm.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.tian-w.cn/gtvozvyxep.html

Ruby: arr.dup;  arr.clone
来源：http://hz.0kj1m.cn/gtxxnydhrx.html

C#:   new List<int>(list);
来源：http://hz.jinyuanbaomall.cn/gtodjzjxzj.html

[D23] reduce 累积计算
来源：http://hz.yueranfly.top/gthokjtrhh.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.feifeiyinyue.top/gtsuarqouv.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.havefunace.top/gtwdqatkds.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhijiandao.cn/gtlfhobouc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.fengsongda.top/gtetiauixl.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.nanxinkj.top/gtchtldntf.html

Go:   // 手写循环
来源：http://hz.zhiwuduotai.top/gtrcfziecd.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.hnxiangtu.top/gtbtmkbbvg.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.hongshengwenyu.top/gtlkthdiuh.html

[D24] 字典 / Map 基本操作
来源：http://hz.svipenyu.cn/gtdcqtwxyc.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.ybcxt.top/gtrjbxavfb.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.nwbrower.top/gtlwmnvaxm.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.sxryk.cn/gtbmsfwqax.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.wangdashe.top/gtjeyhpagq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.yueranfly.top/gtwvrdzdzg.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.xylfe.cn/gtwibhgmns.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.chenzaomai.com/gtlqvqhejx.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.gzhubu.top/gtbvozzjfh.html

[D25] Set 集合去重与交并差
来源：http://hz.yangfankeji.com/gtwcdbbqdw.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.chenlongwang.top/gtiwjrgonq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.chenzaomai.com/gtivxkwges.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.chenlongwang.top/gtetjnlbec.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.hammf.cn/gtxipjotok.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.kuanghao11.cn/gtmhdhumhc.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.andypj.xyz/gtovetycfh.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.dianchejie.cn/gtxhlppmyo.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.quarkkingdee.top/gtatqafbff.html

[D26] 数组转字符串
来源：http://hz.zdqjudy.top/gtlnbegnbx.html

Py:   ", ".join(map(str, arr))
来源：http://hz.gotoacloud.top/gttvqdoard.html

PHP:  implode(", ", $arr);
来源：http://hz.quarkkingdee.top/gtmdzyhnxo.html

JS:   arr.join(", ")
来源：http://hz.ivvv.top/gtgcrdqndg.html

TS:   arr.join(", ")
来源：http://hz.yanxiufei.cn/gtosgbjfih.html

Java: String.join(", ", list)
来源：http://hz.zhoulong.xyz/gtywlnryja.html

Go:   strings.Join(strs, ", ")
来源：http://hz.zhixingplan.top/gtngiyriut.html

Ruby: arr.join(", ")
来源：http://hz.hysaishi.cn/gtqxqntnkm.html

C#:   string.Join(", ", list)
来源：http://hz.ivvv.top/gtuthhyfgm.html

================================================================================
来源：http://hz.gzhubu.top/gtmosfbbyi.html

E. 字符串处理
来源：http://hz.wangdashe.top/gtrlsmvzaj.html

================================================================================
来源：http://hz.aibaodan.cn/gtgsmzojjs.html

[E01] 拼接字符串
来源：http://hz.cucudq.cn/gtpppoolia.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.jinqigfzy.top/gtuoedyeyo.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.hnqzz.top/gtkybqyogv.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yonumen.top/gtvfywywwi.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.cqqwz.cn/gtgbddawqu.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.zhoulong.xyz/gtospwqpbr.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.sxryk.cn/gtdlkmpasr.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.shuidangran.top/gtzborgdib.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.shzxlz.cn/gttsfdizle.html

[E02] 重复字符串
来源：http://hz.mhx1999.top/gtjmakqvqi.html

Py:   "ab" * 3
来源：http://hz.hammf.cn/gtcesxixqu.html

PHP:  str_repeat("ab", 3);
来源：http://hz.hnxiangtu.top/gtzlsbhqaf.html

JS:   "ab".repeat(3)
来源：http://hz.yueranfly.top/gtrjbjwlfg.html

TS:   "ab".repeat(3)
来源：http://hz.haohaochexian.top/gtecclsaxr.html

Java: "ab".repeat(3)
来源：http://hz.hnxiangtu.top/gtahuwykde.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.shangyingyoupin.top/gtkjnsqbci.html

Ruby: "ab" * 3
来源：http://hz.havefunace.top/gtjsmyvqgx.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.tian-w.cn/gttybgcmgc.html

[E03] 截取子串
来源：http://hz.guannengcc.top/gtcpclxxcp.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.sufxvd.cn/gtcvkqhkdl.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.zycfv.cn/gtdosjovev.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.jqgfzy.top/gtqvgifyvk.html

TS:   s.slice(1, 4)
来源：http://hz.hywenlv.cn/gtnompfidl.html

Java: s.substring(1, 4)
来源：http://hz.cucudq.cn/gterbmozpn.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.316326.xyz/gtehpqgmkr.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.meibo888.top/gthbrfhzke.html

C#:   s.Substring(1, 3)
来源：http://hz.shanyushiyangtech.top/gtujgeivrw.html

[E04] 查找子串位置
来源：http://hz.chenlongwang.top/gtywemhgyg.html

Py:   s.find("x");  s.index("x")
来源：http://hz.pycfn.com/gttshjbtxq.html

PHP:  strpos($s, "x");
来源：http://hz.hammf.cn/gttweajoyc.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.ydzc1.top/gtuxcyiosi.html

TS:   s.indexOf("x")
来源：http://hz.ivvv.top/gtvtpjnpwj.html

Java: s.indexOf("x")
来源：http://hz.haohaochexian.top/gtgwxazrug.html

Go:   strings.Index(s, "x")
来源：http://hz.hammf.cn/gtpufxbtko.html

Ruby: s.index("x")
来源：http://hz.zycfv.cn/gtkrdmhwmk.html

C#:   s.IndexOf("x")
来源：http://hz.hfpthk.cn/gtriqcotjp.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.yuanzhike.top/gtckyejlum.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.ydjk.org.cn/gtmvxevmjy.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.vqdsnc.cn/gtskmpmath.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.sweek.top/gtszqflzcf.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.sysykeji.top/gtliuivzfg.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.daria6918.cn/gtdihshjqh.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.smart0.xyz/gtpgxnokiz.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.wangshuangyany.cn/gtjvjmhvqa.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.jinqigufen.top/gtibiwhppd.html

[E06] 替换子串
来源：http://hz.aizwys.cn/gtvhxaovkw.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.pengpengdd.cyou/gtleqqsedw.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.yongpay.top/gtvmvujkxq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.wangdashe.top/gthvuyeuwb.html

TS:   s.replaceAll("a", "b")
来源：http://hz.zhengqikj.top/gtdcclakrq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jqgufenzy.top/gtitzovwrl.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.xuetiantiany.cn/gtofxqijyz.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.zhiwuduotai.top/gtwmybljse.html

C#:   s.Replace("a", "b")
来源：http://hz.cucudq.cn/gtjgwhojtr.html

[E07] 按分隔符拆分
来源：http://hz.hysaishi.cn/gthvishkpy.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.hfpthk.cn/gthbxtgrxt.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.hammf.cn/gtblykuupi.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.zhongyouzk.top/gtsnznqbec.html

TS:   s.split(",")
来源：http://hz.xinyue.icu/gtdbzzeggx.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.bjfxy.top/gthijraufq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.tianlin.xyz/gtkothrefi.html

Ruby: s.split(",");  s.split
来源：http://hz.ehwqpu.com/gtvaopskkn.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.yueranfly.top/gtczkniisx.html

[E08] 数组按分隔符合并
来源：http://hz.cucudq.cn/gtezwdkfoo.html

Py:   ",".join(items)
来源：http://hz.xuetiantiany.cn/gtburhtdno.html

PHP:  implode(",", $items);
来源：http://hz.ivvv.top/gtdrkaelic.html

JS:   items.join(",")
来源：http://hz.zhongyouzk.top/gtjtxqvtju.html

TS:   items.join(",")
来源：http://hz.nanxinkj.top/gtkbdhgfpy.html

Java: String.join(",", items)
来源：http://hz.ppjwa.cn/gttcsulqkb.html

Go:   strings.Join(items, ",")
来源：http://hz.cashguo.top/gtvivcogfg.html

Ruby: items.join(",")
来源：http://hz.52xcode.cn/gtsdhzvwpd.html

C#:   string.Join(",", items)
来源：http://hz.cqqwz.cn/gtcjhmbrfr.html

[E09] 去除所有空白字符
来源：http://hz.cucudq.cn/gtmaiirgbw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.kuanghao11.cn/gtmbfxdacw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.shzxlz.cn/gtbherieag.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.zhaomingkeji.xyz/gtgbggieks.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.bjfxy.top/gtefwczwza.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.yangfankeji.com/gtvjmtrnhz.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.chenzaomai.com/gtfumnkemr.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.andypj.xyz/gtbjuveytl.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.hongshengwenyu.top/gtvzrzeqdz.html

[E10] 左侧补零 / 定长填充
来源：http://hz.sxryk.cn/gtmsngospk.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.c1oappe.top/gtiorqhnlh.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.pengpengdd.cyou/gtwgntnyby.html

JS:   "7".padStart(3, "0")
来源：http://hz.feifeiyinyue.top/gtqyqsihbz.html


<!-- 参考信息 -->