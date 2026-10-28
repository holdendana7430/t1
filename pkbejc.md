代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.shuidangran.top/gtdtvitvkv.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.chenzaomai.com/gtagsvltfb.html

[D05] 访问与修改元素
来源：http://hz.zhaomingkeji.xyz/gtgnnuwcih.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.316326.xyz/gtukyyapep.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.yangfankeji.com/gtgdufcazp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.feifeiyinyue.top/gtoycnulif.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.xziqi.cn/gtigdzdshu.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.sxryk.cn/gtfnufsxbc.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.tian-w.cn/gtvwmavbpx.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.sxryk.cn/gtgbodlubd.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.yuanzhike.top/gtjbktjkjy.html

[D06] 数组长度
来源：http://hz.pycfn.com/gtgsuupcvi.html

Py:   len(arr)
来源：http://hz.fengsongda.top/gtegfahsqs.html

PHP:  count($arr);
来源：http://hz.zhijiandao.cn/gtjklrgvil.html

JS:   arr.length
来源：http://hz.hammf.cn/gtmsmfuscv.html

TS:   arr.length
来源：http://hz.pycfn.com/gttvdunygq.html

Java: list.size();
来源：http://hz.shzxlz.cn/gtmjbgjagd.html

Go:   len(arr)
来源：http://hz.yueranfly.top/gtnyjiofnq.html

Ruby: arr.length; arr.size
来源：http://hz.redwolf501.top/gtjzbybbal.html

C#:   list.Count;
来源：http://hz.ywan-chungtsiang.top/gtwqvvinpj.html

[D07] 切片 / 取子数组
来源：http://hz.cashguo.top/gtvuwcihck.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.shangyingyoupin.top/gtecyvjoze.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.jinghuilouyu.cn/gtwadiwrlq.html

JS:   arr.slice(1, 4);
来源：http://hz.havefunace.top/gtvmzemiqh.html

TS:   arr.slice(1, 4);
来源：http://hz.9152youxi.cn/gtvioirqmj.html

Java: list.subList(1, 4);
来源：http://hz.wangshuangyany.cn/gtikuudlcw.html

Go:   arr[1:4]
来源：http://hz.hongshengwenyu.top/gtjudzkrua.html

Ruby: arr[1, 3]
来源：http://hz.xinyue.icu/gtemxbntnm.html

C#:   list.GetRange(1, 3);
来源：http://hz.daxiang520.top/gtzffdpnme.html

[D08] 合并两个数组
来源：http://hz.yueranfly.top/gtykafhcrx.html

Py:   a + b;  a.extend(b)
来源：http://hz.9152youxi.cn/gtjwwuffgw.html

PHP:  array_merge($a, $b);
来源：http://hz.chenjidiqi.icu/gtonpnlvbc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.dianchejie.cn/gtshzvxwys.html

TS:   [...a, ...b];
来源：http://hz.kuanghao11.cn/gtetecpixp.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.jlsjyb.cn/gtbroepxwd.html

Go:   append(a, b...)
来源：http://hz.jqgfzy.top/gtrmtzumqr.html

Ruby: a + b;  a.concat(b)
来源：http://hz.zdqjudy.top/gtxqddunml.html

C#:   a.Concat(b).ToList()
来源：http://hz.yanxiufei.cn/gtfxinkemd.html

[D09] 排序（升序）
来源：http://hz.gogol.net.cn/gtebamsckz.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jinghuilouyu.cn/gtxfvmgpcs.html

PHP:  sort($arr);
来源：http://hz.shangyingyoupin.top/gtewjtwyij.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.zhijiandao.cn/gthzhlbshe.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.haohaochexian.top/gtgvoobttx.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.tanke756.top/gthxxrzvbe.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.ydjk.org.cn/gtllzaebzm.html

Ruby: arr.sort
来源：http://hz.jinqigufen.top/gtlwsyfjzk.html

C#:   list.Sort();
来源：http://hz.gogol.net.cn/gtivlvotnq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.gotoacloud.top/gtntxkaipv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.vqdsnc.cn/gtlrlktxzq.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.daxiang520.top/gtblhdwuur.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xziqi.cn/gthfttkyqd.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.tian-w.cn/gtgpousjuc.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.xuetiantiany.cn/gtcvevfauw.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.ydjk.org.cn/gtpfjsqabu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.ydjk.org.cn/gtiuzprylj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.nanxinkj.top/gtjcggfofx.html

[D11] 反转数组
来源：http://hz.shanyushiyangkeji.top/gtkkqqyvdz.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.yonumen.top/gtrazjzarr.html

PHP:  array_reverse($arr);
来源：http://hz.zhoulong.xyz/gtfbjktons.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.chenjidiqi.icu/gtziojtoxu.html

TS:   [...arr].reverse();
来源：http://hz.xinyue.icu/gtcyheyijg.html

Java: Collections.reverse(list);
来源：http://hz.fengsongda.top/gtjdprasir.html

Go:   slices.Reverse(arr)
来源：http://hz.hfpthk.cn/gtgaigmqjr.html

Ruby: arr.reverse
来源：http://hz.zycfv.cn/gtctgxsqul.html

C#:   list.Reverse();
来源：http://hz.c1oappe.top/gtehoioviw.html

[D12] 查找元素下标
来源：http://hz.gogol.net.cn/gtlswfwzgu.html

Py:   arr.index(x);  x in arr
来源：http://hz.cucudq.cn/gtyslngucv.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.pengpengdd.cyou/gtgdgddroz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yj20258888.top/gtnpzrvzvm.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.sysykeji.top/gtuvddiufa.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.guowangkeji.top/gtrjzdgxxp.html

Go:   slices.Index(arr, x)
来源：http://hz.52xcode.cn/gtiyfuyipm.html

Ruby: arr.index(x)
来源：http://hz.ivvv.top/gtvdjtcora.html

C#:   list.IndexOf(x);
来源：http://hz.haohaochexian.top/gtwntzeqio.html

[D13] 过滤（保留满足条件的）
来源：http://hz.xingfuxueyuan.xyz/gtffwlqqbl.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.sweek.top/gtnvzpvhnj.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.cdnleiting.top/gtgnzpmpuu.html

JS:   arr.filter(x => x > 3)
来源：http://hz.cqqwz.cn/gtigrocyzw.html

TS:   arr.filter(x => x > 3)
来源：http://hz.jqgfzy.top/gtkvxiliap.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.vqdsnc.cn/gtkopmvhik.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.redwolf501.top/gtbijqzwlt.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.shuidangran.top/gtinygwwjw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.jianghu66.top/gtjjjvsntf.html

[D14] 映射转换（每个元素变形）
来源：http://hz.andypj.xyz/gtjkpdmvwm.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.0kj1m.cn/gtzlugfwks.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.ybcxt.top/gtxebcfczd.html

JS:   arr.map(x => x * 2)
来源：http://hz.jqgfzy.top/gtetdjzzio.html

TS:   arr.map(x => x * 2)
来源：http://hz.sxryk.cn/gtnwrzkgji.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.ivvv.top/gtsaqjpcrr.html

Go:   // 手写循环
来源：http://hz.jyoumei.cn/gtkyjkiuzs.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.yanxiufei.cn/gtgbrqhpba.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.ydzc1.top/gtrpsudsic.html

[D15] 去重
来源：http://hz.c1oappe.top/gtztmpriqf.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.zhengqikj.top/gtblmazdqb.html

PHP:  array_unique($arr);
来源：http://hz.nanxuanxn.top/gtpzhxtbix.html

JS:   [...new Set(arr)]
来源：http://hz.jinqigufen.top/gtlyvlbirq.html

TS:   [...new Set(arr)]
来源：http://hz.cucudq.cn/gtwgqgpyrd.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.shanyushiyangkeji.top/gtjfidzpmz.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.ydzc1.top/gtswrtchas.html

Ruby: arr.uniq
来源：http://hz.svipenyu.cn/gtnkawwday.html

C#:   list.Distinct().ToList()
来源：http://hz.xuetiantiany.cn/gtuphjemih.html

[D16] 求和与平均值
来源：http://hz.mhx1999.top/gtmxjicjlf.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.chenjidiqi.icu/gtpigieluh.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.shanyushiyangtech.top/gtcwczdqnw.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.shzxlz.cn/gtyutljozm.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yangfankeji.com/gtfbeslgce.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.gzhubu.top/gtitsitofq.html

Go:   // 手写循环累加
来源：http://hz.havefunace.top/gttopsyggu.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.cashguo.top/gtxzbhotdq.html

C#:   list.Sum();  list.Average()
来源：http://hz.shanyushiyangtech.top/gthwlwdcue.html

[D17] 最大值与最小值
来源：http://hz.ivvv.top/gtocpthbza.html

Py:   max(arr);  min(arr)
来源：http://hz.feifeiyinyue.top/gtxzijokzx.html

PHP:  max($arr);  min($arr);
来源：http://hz.ivvv.top/gtdyxrtlxu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.gzhubu.top/gtjeaciljy.html

TS:   Math.max(...arr);
来源：http://hz.zhongyouzk.top/gtrwutilmi.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.cheryme.top/gtvaahzhjc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.hongshengwenyu.top/gtlkibodoe.html

Ruby: arr.max;  arr.min
来源：http://hz.yueranfly.top/gtbykbzmth.html

C#:   list.Max();  list.Min()
来源：http://hz.sysykeji.top/gtgylosdiw.html

[D18] 扁平化嵌套数组
来源：http://hz.yongpay.top/gteeoszdqy.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.bjfxy.top/gtdqohoedb.html

PHP:  array_merge(...$nested);
来源：http://hz.hywenlv.cn/gtmeccejnv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.zycfv.cn/gtwiuvroju.html

TS:   nested.flat();
来源：http://hz.cqqwz.cn/gtfcgvyyca.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.gotoacloud.top/gtijhweizw.html

Go:   // 手写双层循环
来源：http://hz.nanxinkj.top/gtqhaxvxoc.html

Ruby: nested.flatten
来源：http://hz.snrcjt.cn/gtypmxagnb.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.meibo888.top/gtduneryyy.html

[D19] 按字段分组
来源：http://hz.hfpthk.cn/gthqerssew.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.tian-w.cn/gttoywnbyo.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.cucudq.cn/gtecbconkv.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.meibo888.top/gtyzztlfed.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.dianchejie.cn/gtsmhsfymf.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.jinqigfzy.top/gtvmplmwco.html

Go:   // 手写 map[string][]T
来源：http://hz.wangshuangyany.cn/gttmszcqrs.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.wangdashe.top/gtqvqtzmop.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.ydjk.org.cn/gtfgjbqsti.html

[D20] 统计每个元素出现次数
来源：http://hz.gzhubu.top/gtxvzvkkbx.html

Py:   Counter(arr)
来源：http://hz.quarkkingdee.top/gtxxgcvdpv.html

PHP:  array_count_values($arr);
来源：http://hz.shangyingyoupin.top/gtxubqoblj.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.chenzaomai.com/gtxzmtiltq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.xuetiantiany.cn/gtujeckdmn.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.pycfn.com/gttdnmipxd.html

Go:   // 手写 map[T]int
来源：http://hz.havefunace.top/gtfzebaqik.html

Ruby: arr.tally
来源：http://hz.jqgfzy.top/gtfssgldaq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.quarkkingdee.top/gtzzarqgdu.html

[D21] 判断是否包含某元素
来源：http://hz.hywenlv.cn/gtahoexaox.html

Py:   x in arr
来源：http://hz.zdqjudy.top/gtisgynvap.html

PHP:  in_array($x, $arr, true);
来源：http://hz.daxiang520.top/gtdcbybwcx.html

JS:   arr.includes(x)
来源：http://hz.chenjidiqi.icu/gtteerspoz.html

TS:   arr.includes(x)
来源：http://hz.shuidangran.top/gtvvnwwpsz.html

Java: list.contains(x)
来源：http://hz.kuanghao11.cn/gtdfvfcqjg.html

Go:   slices.Contains(arr, x)
来源：http://hz.hammf.cn/gtlnvyjtcn.html

Ruby: arr.include?(x)
来源：http://hz.ybcxt.top/gtwmupkreu.html

C#:   list.Contains(x)
来源：http://hz.yanxiufei.cn/gtultopyga.html

[D22] 复制数组（避免共享引用）
来源：http://hz.xuetiantiany.cn/gtarezhbkd.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.aizwys.cn/gtmmepynbs.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.daxiang520.top/gtqcizslba.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.hammf.cn/gtzdheivro.html

TS:   [...arr];
来源：http://hz.xziqi.cn/gtvsgtvvet.html

Java: new ArrayList<>(list);
来源：http://hz.yongpay.top/gtzyazwdwf.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.guannengcc.top/gtxkkgvcoi.html

Ruby: arr.dup;  arr.clone
来源：http://hz.jianghu66.top/gtqtsmyyzo.html

C#:   new List<int>(list);
来源：http://hz.tianlin.xyz/gtfslslgkq.html

[D23] reduce 累积计算
来源：http://hz.zhiwuduotai.top/gtdikzquqb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.guannengcc.top/gtkamdgfmt.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.andypj.xyz/gtwfhvjhmp.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.daria6918.cn/gtduewtemj.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.gaohongyu789.top/gtceyuxwbz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.gaohongyu789.top/gtrrepivkm.html

Go:   // 手写循环
来源：http://hz.tian-w.cn/gtmvnxxczg.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.ybcxt.top/gtkcgtdclx.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.yongpay.top/gtmwiykiwp.html

[D24] 字典 / Map 基本操作
来源：http://hz.aizwys.cn/gtjvljkosk.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.havefunace.top/gtwkbyknko.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.snrcjt.cn/gtdflvsaxv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.hfpthk.cn/gtmcoyjaro.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.cqqwz.cn/gtojufwehu.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.yuanzhike.top/gtymaqutyk.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.mhx1999.top/gtwkogewjt.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.dashuyun.cn/gtjyorpvsh.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.yanxiufei.cn/gtkwzbkfgy.html

[D25] Set 集合去重与交并差
来源：http://hz.sweek.top/gtikpitcsm.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.gzhubu.top/gtpxiicppy.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.tian-w.cn/gtnaeuqnso.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.zhoulong.xyz/gtxrmlejin.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.hfpthk.cn/gtjjxmbqwb.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.zhiwuduotai.top/gtuvfrfnbq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.gzhubu.top/gtdcauaqmo.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.yangfankeji.com/gthtxdvoai.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.havefunace.top/gtkkccjwtn.html

[D26] 数组转字符串
来源：http://hz.316326.xyz/gtrpwelewx.html

Py:   ", ".join(map(str, arr))
来源：http://hz.ppjwa.cn/gttuhqkymq.html

PHP:  implode(", ", $arr);
来源：http://hz.andypj.xyz/gtqpzhsmeu.html

JS:   arr.join(", ")
来源：http://hz.yangfankeji.com/gtwmoyfcyv.html

TS:   arr.join(", ")
来源：http://hz.pycfn.com/gtobbjqcys.html

Java: String.join(", ", list)
来源：http://hz.gogol.net.cn/gtevpzasuh.html

Go:   strings.Join(strs, ", ")
来源：http://hz.aizwys.cn/gtcyymevns.html

Ruby: arr.join(", ")
来源：http://hz.xuetiantiany.cn/gtvwlylxxj.html

C#:   string.Join(", ", list)
来源：http://hz.52xcode.cn/gtmwkhchkt.html

================================================================================
来源：http://hz.ivvv.top/gtrbrdfiem.html

E. 字符串处理
来源：http://hz.hysaishi.cn/gthrfemvol.html

================================================================================
来源：http://hz.xuanzx.com/gtdoabjxcc.html

[E01] 拼接字符串
来源：http://hz.hnxiangtu.top/gtjkkxhkvx.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.sxryk.cn/gtjlzbiofp.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.shanyushiyangtech.top/gtqsiqiftu.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yvedp.cn/gtznllmadt.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yueranfly.top/gtiwzfsxob.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.dashuyun.cn/gtqpjxhyki.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.feifeiyinyue.top/gtoyjaerty.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.svipenyu.cn/gtpjesqkgf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.zhengqikj.top/gtlhxdyalu.html

[E02] 重复字符串
来源：http://hz.cqqwz.cn/gthybanlys.html

Py:   "ab" * 3
来源：http://hz.snrcjt.cn/gteplezxkm.html

PHP:  str_repeat("ab", 3);
来源：http://hz.zhiwuduotai.top/gtgclmwpqt.html

JS:   "ab".repeat(3)
来源：http://hz.guannengcc.top/gtknyfkpwp.html

TS:   "ab".repeat(3)
来源：http://hz.xylfe.cn/gtwsmxezia.html

Java: "ab".repeat(3)
来源：http://hz.vqdsnc.cn/gtzmuocpce.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.gaohongyu789.top/gtozxmqzrv.html

Ruby: "ab" * 3
来源：http://hz.haohaochexian.top/gthyfpgsmk.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.cdnleiting.top/gteafoecfv.html

[E03] 截取子串
来源：http://hz.jqgfzy.top/gtzungslft.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.redwolf501.top/gtynkiwsvu.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.yangfankeji.com/gtnnrgeler.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.xuetiantiany.cn/gtrhogllhz.html

TS:   s.slice(1, 4)
来源：http://hz.sxryk.cn/gtrmxkeojv.html

Java: s.substring(1, 4)
来源：http://hz.sxryk.cn/gtiwsmbvhx.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.chenzaomai.com/gttoydmjfq.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.hammf.cn/gtjciyrfpm.html

C#:   s.Substring(1, 3)
来源：http://hz.guannengcc.top/gtfyniwwmq.html

[E04] 查找子串位置
来源：http://hz.guowangkeji.top/gtnlbsreof.html

Py:   s.find("x");  s.index("x")
来源：http://hz.nanxinkj.top/gtaclmbvvc.html

PHP:  strpos($s, "x");
来源：http://hz.shangyingyoupin.top/gtlawktnla.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.yongpay.top/gtsqakpzcg.html

TS:   s.indexOf("x")
来源：http://hz.jiagoushi.top/gtikidczsz.html

Java: s.indexOf("x")
来源：http://hz.hywenlv.cn/gttkrnadpe.html

Go:   strings.Index(s, "x")
来源：http://hz.hysaishi.cn/gtchfpivdu.html

Ruby: s.index("x")
来源：http://hz.jinghuilouyu.cn/gtdsszvzcf.html

C#:   s.IndexOf("x")
来源：http://hz.haohaochexian.top/gttkzuvdvp.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.wangdashe.top/gtizllcasn.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.cheryme.top/gtmnxeobwn.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.chenlongwang.top/gtbxqvzdku.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.kuanghao11.cn/gtpmcerjgs.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.xylfe.cn/gtrtppaqpb.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jinyuanbaomall.cn/gtkacxrfnj.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.52xcode.cn/gtljurtmxj.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.havefunace.top/gtthbajxnl.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.svipenyu.cn/gtcbxopqit.html

[E06] 替换子串
来源：http://hz.jqgufenzy.top/gtapufatxa.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.dashuyun.cn/gtqffpmsic.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.jiagoushi.top/gtcuryaqay.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.shanyushiyangtech.top/gtoojdfmls.html

TS:   s.replaceAll("a", "b")
来源：http://hz.bjfxy.top/gtdvrqlqpf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.haohaochexian.top/gtctdsnrbh.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.nanxinkj.top/gtdgdczwoi.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.jinqigfzy.top/gtuabviiuq.html

C#:   s.Replace("a", "b")
来源：http://hz.bjfxy.top/gtybcwapwq.html

[E07] 按分隔符拆分
来源：http://hz.kuanghao11.cn/gtcqzjgnui.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.gogol.net.cn/gtgdgiupiy.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.cucudq.cn/gtuvyshxny.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.zhiwuduotai.top/gttnsitbaj.html

TS:   s.split(",")
来源：http://hz.yj20258.top/gtmovmeokt.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.yonumen.top/gtlejmeydc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.zhijiandao.cn/gtpsboyqva.html

Ruby: s.split(",");  s.split
来源：http://hz.yvedp.cn/gtrqijxlxc.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.chenlongwang.top/gtqnqdwqjf.html

[E08] 数组按分隔符合并
来源：http://hz.zhixingplan.top/gttlaygzau.html

Py:   ",".join(items)
来源：http://hz.wangdashe.top/gtvnykjprr.html

PHP:  implode(",", $items);
来源：http://hz.jiagoushi.top/gtoocsfirh.html

JS:   items.join(",")
来源：http://hz.fengsongda.top/gtauicwpec.html

TS:   items.join(",")
来源：http://hz.shangyingyoupin.top/gtpitsqhzx.html

Java: String.join(",", items)
来源：http://hz.zhongyouzk.top/gtdwmprhpo.html

Go:   strings.Join(items, ",")
来源：http://hz.chenlongwang.top/gteorkqkoe.html

Ruby: items.join(",")
来源：http://hz.xuetiantiany.cn/gtjstzaozg.html

C#:   string.Join(",", items)
来源：http://hz.shanyushiyangkeji.top/gtjututxoz.html

[E09] 去除所有空白字符
来源：http://hz.hnxiangtu.top/gtisighugn.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.quarkkingdee.top/gtqiylxvkh.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.ydzc1.top/gtpzcoxukg.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.zhongyouzk.top/gtyjogljtp.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.ybcxt.top/gtnwkvhdiz.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.ppjwa.cn/gthngxkpdt.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.dianchejie.cn/gtgvgkyhxc.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.zhengqikj.top/gttasecire.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.ivvv.top/gtimvsrkih.html

[E10] 左侧补零 / 定长填充
来源：http://hz.guannengcc.top/gtudbscktk.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.andypj.xyz/gtodctjtwp.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.jinghuilouyu.cn/gtluqvjsoi.html

JS:   "7".padStart(3, "0")
来源：http://hz.gotoacloud.top/gtnttdssvy.html

TS:   "7".padStart(3, "0")
来源：http://hz.cdnleiting.top/gtfpqlrqan.html

Java: String.format("%03d", 7)
来源：http://hz.jinqigfzy.top/gtubcpaese.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.yuanzhike.top/gtakrhserz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.jinqigfzy.top/gtjdkktrjt.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.0kj1m.cn/gtzinkevex.html

[E11] 反转字符串
来源：http://hz.jiagoushi.top/gtfbnmwmya.html

Py:   s[::-1]
来源：http://hz.guannengcc.top/gtusgyokyw.html

PHP:  strrev($s);
来源：http://hz.ppjwa.cn/gtbbxyxhvn.html

JS:   [...s].reverse().join("")
来源：http://hz.zhoulong.xyz/gtvajtvrrx.html

TS:   [...s].reverse().join("")
来源：http://hz.hnxiangtu.top/gtljvvmlyw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.yuxming.cn/gtpmoxtynb.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.zhixingplan.top/gtqbphpaob.html


<!-- 参考信息 -->