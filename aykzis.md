代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.nanxinkj.top/gtlfumalpg.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.xziqi.cn/gtjggxyfqs.html

[D05] 访问与修改元素
来源：http://hz.ppjwa.cn/gtxwvjmplb.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.dashuyun.cn/gtdnfszkmy.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.hnxiangtu.top/gtngangvqg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.ivvv.top/gtusqoqprg.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.hammf.cn/gtrapmtldr.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.redwolf501.top/gtjluoetto.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.guannengcc.top/gtudemrecp.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.ydzc1.top/gtyqlqfhbz.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.havefunace.top/gtyrzpnrzk.html

[D06] 数组长度
来源：http://hz.shanyushiyangtech.top/gtsdkfnstd.html

Py:   len(arr)
来源：http://hz.52xcode.cn/gtsvldhcvx.html

PHP:  count($arr);
来源：http://hz.yj20258.top/gtvgtenlel.html

JS:   arr.length
来源：http://hz.ydjk.org.cn/gtygvnbmnr.html

TS:   arr.length
来源：http://hz.sweek.top/gtaifhjwzg.html

Java: list.size();
来源：http://hz.cdnleiting.top/gtvoirgqdh.html

Go:   len(arr)
来源：http://hz.zhoulong.xyz/gtyjivavjg.html

Ruby: arr.length; arr.size
来源：http://hz.tianlin.xyz/gtsttgjcuh.html

C#:   list.Count;
来源：http://hz.pycfn.com/gtsxqybsoa.html

[D07] 切片 / 取子数组
来源：http://hz.redwolf501.top/gtikiuqwwd.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.aibaodan.cn/gtjudxynog.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.sweek.top/gtednxefcd.html

JS:   arr.slice(1, 4);
来源：http://hz.xylfe.cn/gtppkhxxup.html

TS:   arr.slice(1, 4);
来源：http://hz.xziqi.cn/gtwcwstqnh.html

Java: list.subList(1, 4);
来源：http://hz.chenlongwang.top/gtrgdkhurh.html

Go:   arr[1:4]
来源：http://hz.xuanzx.com/gthpapnyeb.html

Ruby: arr[1, 3]
来源：http://hz.yj202588.top/gtdevdmzyp.html

C#:   list.GetRange(1, 3);
来源：http://hz.hammf.cn/gtjfjxkzod.html

[D08] 合并两个数组
来源：http://hz.guannengcc.top/gtvxiyqxnx.html

Py:   a + b;  a.extend(b)
来源：http://hz.yueranfly.top/gtfgbwvyql.html

PHP:  array_merge($a, $b);
来源：http://hz.zycfv.cn/gtexmqcazm.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.jinghuilouyu.cn/gtmdpfdrhf.html

TS:   [...a, ...b];
来源：http://hz.snrcjt.cn/gtoflysrmm.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.hnqzz.top/gtbfwwseng.html

Go:   append(a, b...)
来源：http://hz.ehwqpu.com/gtqtzgfctu.html

Ruby: a + b;  a.concat(b)
来源：http://hz.9152youxi.cn/gtqtebtkaa.html

C#:   a.Concat(b).ToList()
来源：http://hz.hnxiangtu.top/gtuojrehxg.html

[D09] 排序（升序）
来源：http://hz.ivvv.top/gtgytxnsxc.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yj20258888.top/gtckjiczwh.html

PHP:  sort($arr);
来源：http://hz.daxiang520.top/gtmmhtejpv.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.snrcjt.cn/gtvltpegnx.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.nwbrower.top/gtvxlhlttp.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.sysykeji.top/gtwdxvkhwr.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.jinqigfzy.top/gtvtwndzpr.html

Ruby: arr.sort
来源：http://hz.tianlin.xyz/gtviusjhja.html

C#:   list.Sort();
来源：http://hz.xuetiantiany.cn/gtbxjgunjd.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.xingfuxueyuan.xyz/gtqmgpwojg.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.yj202588.top/gtjclrtlmy.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.dashuyun.cn/gtprmwrfiu.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.gogol.net.cn/gtwgyozury.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.cdnleiting.top/gtyleyvdek.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.chenzaomai.com/gtgkyykqtm.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.daxiang520.top/gtiurmdvfm.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.zhixingplan.top/gtgyudapgm.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.zhoulong.xyz/gtabtxjalp.html

[D11] 反转数组
来源：http://hz.andypj.xyz/gtoudmmbzy.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.zhiwuduotai.top/gtmuhytbje.html

PHP:  array_reverse($arr);
来源：http://hz.jinghuilouyu.cn/gtbvlraqsa.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.zycfv.cn/gtvgdaoduz.html

TS:   [...arr].reverse();
来源：http://hz.yj202588.top/gtqqulrudu.html

Java: Collections.reverse(list);
来源：http://hz.kuanghao11.cn/gtxorzotkh.html

Go:   slices.Reverse(arr)
来源：http://hz.redwolf501.top/gthpkucdds.html

Ruby: arr.reverse
来源：http://hz.daxiang520.top/gtvujmbdmr.html

C#:   list.Reverse();
来源：http://hz.sufxvd.cn/gtzakpvygu.html

[D12] 查找元素下标
来源：http://hz.c1oappe.top/gtypardose.html

Py:   arr.index(x);  x in arr
来源：http://hz.dashuyun.cn/gtgotfrjni.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.cashguo.top/gtscceigkf.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.ywan-chungtsiang.top/gtlxsyzanw.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.chenlongwang.top/gtitghhcma.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.dianchejie.cn/gtntbdblij.html

Go:   slices.Index(arr, x)
来源：http://hz.cheryme.top/gthifcfzef.html

Ruby: arr.index(x)
来源：http://hz.yuxming.cn/gtkyezhsul.html

C#:   list.IndexOf(x);
来源：http://hz.tianlin.xyz/gtzymcufbl.html

[D13] 过滤（保留满足条件的）
来源：http://hz.hfpthk.cn/gtpudpxbts.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.pengpengdd.cyou/gtdiugxtzp.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.jqgfzy.top/gtfzgzmpdv.html

JS:   arr.filter(x => x > 3)
来源：http://hz.wangshuangyany.cn/gtmjjgkyyg.html

TS:   arr.filter(x => x > 3)
来源：http://hz.jyoumei.cn/gtjtgzzjdv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.mhx1999.top/gtowtornez.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.yonumen.top/gtrlqajxou.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.nanxuanxn.top/gtpltezcrq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.cdnleiting.top/gtcuphqatb.html

[D14] 映射转换（每个元素变形）
来源：http://hz.sxryk.cn/gtlzctvugx.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.birdmap.top/gtnaufwzcv.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.snrcjt.cn/gtxvgdvhcz.html

JS:   arr.map(x => x * 2)
来源：http://hz.zdqjudy.top/gtnwavurui.html

TS:   arr.map(x => x * 2)
来源：http://hz.sufxvd.cn/gtphxypfvs.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.dianchejie.cn/gtxrgpehyn.html

Go:   // 手写循环
来源：http://hz.birdmap.top/gtnmcdemhh.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.hysaishi.cn/gtgvqoxbys.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.hywenlv.cn/gtmgylpfln.html

[D15] 去重
来源：http://hz.ydjk.org.cn/gtytkfxxjw.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.mhx1999.top/gtsabwympi.html

PHP:  array_unique($arr);
来源：http://hz.sufxvd.cn/gtuvbzairx.html

JS:   [...new Set(arr)]
来源：http://hz.0kj1m.cn/gtmexdutns.html

TS:   [...new Set(arr)]
来源：http://hz.nanxinkj.top/gtbbitoamr.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.havefunace.top/gtdhhjgodt.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.nanxinkj.top/gtbpzperel.html

Ruby: arr.uniq
来源：http://hz.zhongyouzk.top/gtddiuyrmv.html

C#:   list.Distinct().ToList()
来源：http://hz.gogol.net.cn/gtubqihfjt.html

[D16] 求和与平均值
来源：http://hz.zhaomingkeji.xyz/gtwldycxsx.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.yongpay.top/gtbuxzdmbu.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.xuanzx.com/gttlqdhyob.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hammf.cn/gtitjbqvrm.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.xuetiantiany.cn/gtbgsxtbww.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.andypj.xyz/gtrllxqlrg.html

Go:   // 手写循环累加
来源：http://hz.xinyue.icu/gtxkhhijzl.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.meibo888.top/gthyhcxlaa.html

C#:   list.Sum();  list.Average()
来源：http://hz.cashguo.top/gtpalkuykp.html

[D17] 最大值与最小值
来源：http://hz.cashguo.top/gtljwkzwwt.html

Py:   max(arr);  min(arr)
来源：http://hz.guowangkeji.top/gtqeoyxrpx.html

PHP:  max($arr);  min($arr);
来源：http://hz.haohaochexian.top/gtllpyzvkb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.ppjwa.cn/gthqelsvng.html

TS:   Math.max(...arr);
来源：http://hz.havefunace.top/gtqnafjhid.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.yj202588.top/gtgyvmqdyd.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.zhengqikj.top/gtalpaedlw.html

Ruby: arr.max;  arr.min
来源：http://hz.pengpengdd.cyou/gtcwpvrtuw.html

C#:   list.Max();  list.Min()
来源：http://hz.jinyuanbaomall.cn/gtfsxkerzk.html

[D18] 扁平化嵌套数组
来源：http://hz.yj20258.top/gtzpjfifhk.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.jqgfzy.top/gthfyedirj.html

PHP:  array_merge(...$nested);
来源：http://hz.redwolf501.top/gtvgsxnkjh.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.cashguo.top/gtlqqomgri.html

TS:   nested.flat();
来源：http://hz.c1oappe.top/gtbherwztx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.chenzaomai.com/gtkmcpuhyz.html

Go:   // 手写双层循环
来源：http://hz.yanxiufei.cn/gtpzpsbvma.html

Ruby: nested.flatten
来源：http://hz.jinqigufen.top/gtqvjvgpxw.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.zhixingplan.top/gtzytldtoj.html

[D19] 按字段分组
来源：http://hz.gaohongyu789.top/gtkpqsbsqd.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.yj20258888.top/gtgstwxqle.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.svipenyu.cn/gtmkhmmful.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.cdnleiting.top/gtrgoavgbi.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.iojbl.cn/gtffuavhcl.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.jinqigufen.top/gtjwjoibbg.html

Go:   // 手写 map[string][]T
来源：http://hz.jinqigfzy.top/gtykdudcns.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.cqqwz.cn/gtpktffezi.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.chenzaomai.com/gtcqriteiv.html

[D20] 统计每个元素出现次数
来源：http://hz.nanxuanxn.top/gtriprphnn.html

Py:   Counter(arr)
来源：http://hz.ppjwa.cn/gtmjdsbouz.html

PHP:  array_count_values($arr);
来源：http://hz.zhiwuduotai.top/gtneuyogfr.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.sysykeji.top/gtxykpthew.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jianghu66.top/gtrctppawq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.yuanzhike.top/gtjjztryok.html

Go:   // 手写 map[T]int
来源：http://hz.gogol.net.cn/gtzojrdbml.html

Ruby: arr.tally
来源：http://hz.yueranfly.top/gtujztxxch.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.feifeiyinyue.top/gtrjnalrvf.html

[D21] 判断是否包含某元素
来源：http://hz.hnxiangtu.top/gtoqzdlhmi.html

Py:   x in arr
来源：http://hz.wangshuangyany.cn/gtlwibhzuv.html

PHP:  in_array($x, $arr, true);
来源：http://hz.yj20258.top/gtuhqjftmd.html

JS:   arr.includes(x)
来源：http://hz.birdmap.top/gtbmsdqvtv.html

TS:   arr.includes(x)
来源：http://hz.xuanzx.com/gtergfbumf.html

Java: list.contains(x)
来源：http://hz.feifeiyinyue.top/gtfabattlz.html

Go:   slices.Contains(arr, x)
来源：http://hz.vqdsnc.cn/gttruvjyic.html

Ruby: arr.include?(x)
来源：http://hz.fzhhl.top/gtnnkgaoxk.html

C#:   list.Contains(x)
来源：http://hz.ydjk.org.cn/gtqfzkfyns.html

[D22] 复制数组（避免共享引用）
来源：http://hz.ydjk.org.cn/gtkazntkmz.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.havefunace.top/gtwkggmglm.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.ybcxt.top/gtnteltauz.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.hnxiangtu.top/gthcrshcke.html

TS:   [...arr];
来源：http://hz.zhixingplan.top/gtjjmmpfkb.html

Java: new ArrayList<>(list);
来源：http://hz.zhaomingkeji.xyz/gthdtaxmll.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.sweek.top/gtkxakjynk.html

Ruby: arr.dup;  arr.clone
来源：http://hz.hysaishi.cn/gtexqeqmjv.html

C#:   new List<int>(list);
来源：http://hz.zhixingplan.top/gtwrpgeynv.html

[D23] reduce 累积计算
来源：http://hz.zhiwuduotai.top/gtexaddmnx.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.gzhubu.top/gteuxxlyqy.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.wangdashe.top/gtuiwvlgrv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jinghuilouyu.cn/gtddpvpjoa.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ydjk.org.cn/gtyoxwzipc.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.hnxiangtu.top/gtgyfvshjz.html

Go:   // 手写循环
来源：http://hz.c1oappe.top/gtjpfrxrda.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.aibaodan.cn/gtmzhvfsbs.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.hfpthk.cn/gtgbchaxdy.html

[D24] 字典 / Map 基本操作
来源：http://hz.hywenlv.cn/gtzvwfvpch.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.yonumen.top/gtykgraxac.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.cqqwz.cn/gtclpyiqzm.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.ydzc1.top/gtfridkbql.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.shanyushiyangkeji.top/gtqhdbbaey.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.yonumen.top/gtndbmworc.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.feifeiyinyue.top/gtyqaojwty.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.0kj1m.cn/gtxlaarkwo.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.cheryme.top/gtcoukqkak.html

[D25] Set 集合去重与交并差
来源：http://hz.zhixingplan.top/gtzdkbttcl.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.gogol.net.cn/gtuxszkpob.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.hysaishi.cn/gtyxagxlbf.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.gaohongyu789.top/gtupypbcyg.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.tian-w.cn/gthxnrqwob.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.fengsongda.top/gtkinxning.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.snrcjt.cn/gtgrkowesv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.gaohongyu789.top/gtbxrtcfqo.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.zhongyouzk.top/gtwxgwbpyr.html

[D26] 数组转字符串
来源：http://hz.ydjk.org.cn/gtadkzofnv.html

Py:   ", ".join(map(str, arr))
来源：http://hz.jyoumei.cn/gtwjrtnpmz.html

PHP:  implode(", ", $arr);
来源：http://hz.gogol.net.cn/gtfjkizuhh.html

JS:   arr.join(", ")
来源：http://hz.birdmap.top/gtgyyltnls.html

TS:   arr.join(", ")
来源：http://hz.hfpthk.cn/gtdtzyajff.html

Java: String.join(", ", list)
来源：http://hz.tianlin.xyz/gtipgzfuzq.html

Go:   strings.Join(strs, ", ")
来源：http://hz.cucudq.cn/gtqwragdbj.html

Ruby: arr.join(", ")
来源：http://hz.zhijiandao.cn/gtuuyuzfhm.html

C#:   string.Join(", ", list)
来源：http://hz.andypj.xyz/gtkipptszx.html

================================================================================
来源：http://hz.yj20258.top/gtplfwnebt.html

E. 字符串处理
来源：http://hz.tian-w.cn/gtirqbvusn.html

================================================================================
来源：http://hz.hywenlv.cn/gtmdcrasgw.html

[E01] 拼接字符串
来源：http://hz.snrcjt.cn/gtcxvbhkyt.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.bjfxy.top/gtdanewfej.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.bjfxy.top/gteowdfrrg.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.shanyushiyangkeji.top/gtsfvnbwav.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.xingfuxueyuan.xyz/gtybgzgdwf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.mhx1999.top/gtjidkrdqm.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.zhengqikj.top/gtatndoydy.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.yongpay.top/gtygrfjtjf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.jinghuilouyu.cn/gthhgvuofj.html

[E02] 重复字符串
来源：http://hz.nwbrower.top/gtllcfxizb.html

Py:   "ab" * 3
来源：http://hz.zhengqikj.top/gtmpdlkbkm.html

PHP:  str_repeat("ab", 3);
来源：http://hz.shuidangran.top/gtuvtpzxes.html

JS:   "ab".repeat(3)
来源：http://hz.snrcjt.cn/gtgvokijfm.html

TS:   "ab".repeat(3)
来源：http://hz.xuanzx.com/gtyvpavedw.html

Java: "ab".repeat(3)
来源：http://hz.0kj1m.cn/gtdwygizbh.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.yonumen.top/gtiunpanao.html

Ruby: "ab" * 3
来源：http://hz.shanyushiyangtech.top/gtilrtvhvb.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.yj202588.top/gtrzzjwnvn.html

[E03] 截取子串
来源：http://hz.aizwys.cn/gtjxadsoue.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.zhoulong.xyz/gtllxbxjcf.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.hammf.cn/gtwdfncqfd.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.redwolf501.top/gtxenikpwo.html

TS:   s.slice(1, 4)
来源：http://hz.xuanzx.com/gttsqwutre.html

Java: s.substring(1, 4)
来源：http://hz.sweek.top/gtbjkvvard.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.yj20258.top/gtfpoklvcl.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.havefunace.top/gtadbobamp.html

C#:   s.Substring(1, 3)
来源：http://hz.zhoulong.xyz/gtbybesbas.html

[E04] 查找子串位置
来源：http://hz.gzhubu.top/gtzhnwuscg.html

Py:   s.find("x");  s.index("x")
来源：http://hz.haohaochexian.top/gtxrzykytk.html

PHP:  strpos($s, "x");
来源：http://hz.hysaishi.cn/gtawzkgdul.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.fzhhl.top/gtemtruokd.html

TS:   s.indexOf("x")
来源：http://hz.ywan-chungtsiang.top/gtyrgxivne.html

Java: s.indexOf("x")
来源：http://hz.xylfe.cn/gtbwudgtmd.html

Go:   strings.Index(s, "x")
来源：http://hz.zhoulong.xyz/gtdxjfytiy.html

Ruby: s.index("x")
来源：http://hz.ydjk.org.cn/gtvfyrnsnr.html

C#:   s.IndexOf("x")
来源：http://hz.tianlin.xyz/gtkftteldc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.yangfankeji.com/gtlbidlbbw.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.hywenlv.cn/gtrqzvjtbz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.ppjwa.cn/gtzipdzbsb.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.hywenlv.cn/gtqivgshlr.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.jqgfzy.top/gtdgfeadah.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.nwbrower.top/gtjxdwrgxm.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.jianghu66.top/gtgwhymzpm.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.shanyushiyangtech.top/gtzxqquixl.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.quarkkingdee.top/gtkubweucd.html

[E06] 替换子串
来源：http://hz.yuxming.cn/gtnmfxaxju.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.zhixingplan.top/gtodipvwsu.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.hongshengwenyu.top/gtzcqrqtvw.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.daria6918.cn/gtrjkkyght.html

TS:   s.replaceAll("a", "b")
来源：http://hz.ivvv.top/gtpiogrvzt.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yuxming.cn/gtugpkoexa.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.xingfuxueyuan.xyz/gtneubeodl.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.feifeiyinyue.top/gtalhjisgi.html

C#:   s.Replace("a", "b")
来源：http://hz.shanyushiyangkeji.top/gtezgucyxq.html

[E07] 按分隔符拆分
来源：http://hz.yj20258.top/gttupkbqhf.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.chenjidiqi.icu/gtqyhomahs.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.ehwqpu.com/gthqycqlqd.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.yj20258888.top/gtexvmrazi.html

TS:   s.split(",")
来源：http://hz.ppjwa.cn/gtkqwrbwim.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.shanyushiyangkeji.top/gtewhetpdi.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.snrcjt.cn/gtwyoqfxlq.html

Ruby: s.split(",");  s.split
来源：http://hz.daria6918.cn/gtfvjhstzy.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.chenjidiqi.icu/gtxojqzguc.html

[E08] 数组按分隔符合并
来源：http://hz.ybcxt.top/gtpuakbveu.html

Py:   ",".join(items)
来源：http://hz.yangfankeji.com/gtelypuuaz.html

PHP:  implode(",", $items);
来源：http://hz.yonumen.top/gtrbutubkb.html

JS:   items.join(",")
来源：http://hz.kuanghao11.cn/gtkqczkaok.html

TS:   items.join(",")
来源：http://hz.xylfe.cn/gtdyjsbdop.html

Java: String.join(",", items)
来源：http://hz.haohaochexian.top/gtpcpzlqxu.html

Go:   strings.Join(items, ",")
来源：http://hz.sxryk.cn/gtwpywwfdp.html

Ruby: items.join(",")
来源：http://hz.guannengcc.top/gtgwlfxcnh.html

C#:   string.Join(",", items)
来源：http://hz.sxryk.cn/gtcswkjdlf.html

[E09] 去除所有空白字符
来源：http://hz.zhengqikj.top/gtixwncyqt.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.zhijiandao.cn/gtxgcgpefu.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.yueranfly.top/gthtuzowap.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.jlsjyb.cn/gttfnzysla.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.pycfn.com/gtnlfecfis.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.zhijiandao.cn/gtjswcmfjd.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.ppjwa.cn/gtitjtqvjw.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.fengsongda.top/gtuirpfcbl.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.chenjidiqi.icu/gtupacrxnp.html

[E10] 左侧补零 / 定长填充
来源：http://hz.jianghu66.top/gtazmyjszd.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.ybcxt.top/gtlesjpilb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.jinghuilouyu.cn/gtrkywordt.html

JS:   "7".padStart(3, "0")
来源：http://hz.zdqjudy.top/gtsufwhkpc.html

TS:   "7".padStart(3, "0")
来源：http://hz.iojbl.cn/gtmamqegpv.html

Java: String.format("%03d", 7)
来源：http://hz.cashguo.top/gtduexhjho.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.xuetiantiany.cn/gtejskpbfh.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.tianlin.xyz/gtksqcdnyl.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.jianghu66.top/gtiddtonjj.html

[E11] 反转字符串
来源：http://hz.zdqjudy.top/gtmykalkac.html

Py:   s[::-1]
来源：http://hz.yuanzhike.top/gtukwkjmsn.html

PHP:  strrev($s);
来源：http://hz.daria6918.cn/gtmkhpxswi.html

JS:   [...s].reverse().join("")
来源：http://hz.xinyue.icu/gtzfviatsl.html

TS:   [...s].reverse().join("")
来源：http://hz.jinyuanbaomall.cn/gtjnlxtapu.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.nwbrower.top/gtqbpzldxl.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.cdnleiting.top/gtsppfenuv.html


<!-- 参考信息 -->