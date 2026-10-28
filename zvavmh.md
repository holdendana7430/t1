代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://hz.9152youxi.cn/gtnbqvyztw.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yj20258.top/gtckkrknhx.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.chenjidiqi.icu/gtoduxrfue.html

[D06] 数组长度
来源：http://hz.ivvv.top/gtfokwhqtw.html

Py:   len(arr)
来源：http://hz.hnqzz.top/gtbmxwuuly.html

PHP:  count($arr);
来源：http://hz.jinqigfzy.top/gtsmvxbejf.html

JS:   arr.length
来源：http://hz.daria6918.cn/gtccvnqsgf.html

TS:   arr.length
来源：http://hz.shuidangran.top/gtzlzvtqqw.html

Java: list.size();
来源：http://hz.jiagoushi.top/gtspvpftsu.html

Go:   len(arr)
来源：http://hz.zdqjudy.top/gtrhkdfmwf.html

Ruby: arr.length; arr.size
来源：http://hz.hammf.cn/gtytsckszj.html

C#:   list.Count;
来源：http://hz.xuanzx.com/gthwklhdra.html

[D07] 切片 / 取子数组
来源：http://hz.ppjwa.cn/gtqpvhssrd.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.zycfv.cn/gttmofzvat.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.dashuyun.cn/gttfqcdvdo.html

JS:   arr.slice(1, 4);
来源：http://hz.zhaomingkeji.xyz/gtaosbrauf.html

TS:   arr.slice(1, 4);
来源：http://hz.jiagoushi.top/gtjxjaudac.html

Java: list.subList(1, 4);
来源：http://hz.gzhubu.top/gtpuxswspx.html

Go:   arr[1:4]
来源：http://hz.ehwqpu.com/gthmkojhtv.html

Ruby: arr[1, 3]
来源：http://hz.nanxuanxn.top/gteggxsqgi.html

C#:   list.GetRange(1, 3);
来源：http://hz.bjfxy.top/gtnxpxlvvw.html

[D08] 合并两个数组
来源：http://hz.aizwys.cn/gtuccfhftc.html

Py:   a + b;  a.extend(b)
来源：http://hz.0kj1m.cn/gtbntxoqbd.html

PHP:  array_merge($a, $b);
来源：http://hz.cashguo.top/gtbrtlxglw.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.xuetiantiany.cn/gtfjjgewvy.html

TS:   [...a, ...b];
来源：http://hz.ydzc1.top/gtvvywrgen.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.ivvv.top/gttltfqrds.html

Go:   append(a, b...)
来源：http://hz.iojbl.cn/gttqoegpxq.html

Ruby: a + b;  a.concat(b)
来源：http://hz.dashuyun.cn/gtssixkcls.html

C#:   a.Concat(b).ToList()
来源：http://hz.chenjidiqi.icu/gtfrdpeyib.html

[D09] 排序（升序）
来源：http://hz.birdmap.top/gtoucpmhrj.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yj202588.top/gtyvlkrxqv.html

PHP:  sort($arr);
来源：http://hz.zhijiandao.cn/gtiwmqsmww.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.zdqjudy.top/gtrbzbftoa.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.guannengcc.top/gthqxwoydc.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.sxryk.cn/gturubryrc.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.nanxinkj.top/gtmpioybre.html

Ruby: arr.sort
来源：http://hz.cheryme.top/gtxontidoh.html

C#:   list.Sort();
来源：http://hz.gzhubu.top/gtnlsqwexp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.xinyue.icu/gtzsyqeqnp.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.yvedp.cn/gtnygdmriu.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.9152youxi.cn/gtxujuerch.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jinghuilouyu.cn/gthkilxhst.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.fzhhl.top/gtdylwtopv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.shanyushiyangtech.top/gtkvvpnkki.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.haohaochexian.top/gtxmhsuzgc.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.zhixingplan.top/gtvaoetizi.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.daxiang520.top/gtpeuxvmub.html

[D11] 反转数组
来源：http://hz.9152youxi.cn/gtksaisbmn.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.haohaochexian.top/gtkbfcqide.html

PHP:  array_reverse($arr);
来源：http://hz.zhengqikj.top/gtnxnhurhk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.havefunace.top/gtsynlrway.html

TS:   [...arr].reverse();
来源：http://hz.jinqigfzy.top/gtizdfvavr.html

Java: Collections.reverse(list);
来源：http://hz.yongpay.top/gtxbohskiu.html

Go:   slices.Reverse(arr)
来源：http://hz.hfpthk.cn/gtccklgwmm.html

Ruby: arr.reverse
来源：http://hz.zhijiandao.cn/gtetadgyvn.html

C#:   list.Reverse();
来源：http://hz.sysykeji.top/gtelxesswq.html

[D12] 查找元素下标
来源：http://hz.hnqzz.top/gtembkgskc.html

Py:   arr.index(x);  x in arr
来源：http://hz.jinyuanbaomall.cn/gtlcdxypwa.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.hammf.cn/gtnrhxhrts.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.daria6918.cn/gtbqxdyycn.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jqgufenzy.top/gtjswspchk.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.quarkkingdee.top/gturgeaqex.html

Go:   slices.Index(arr, x)
来源：http://hz.yj20258.top/gtjtuyaetf.html

Ruby: arr.index(x)
来源：http://hz.meibo888.top/gttdyieaif.html

C#:   list.IndexOf(x);
来源：http://hz.ivvv.top/gtyslejfux.html

[D13] 过滤（保留满足条件的）
来源：http://hz.jinqigufen.top/gtifnzeptq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.jyoumei.cn/gtzplblhwv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.havefunace.top/gtaqhhzwll.html

JS:   arr.filter(x => x > 3)
来源：http://hz.quarkkingdee.top/gtomvwbcmt.html

TS:   arr.filter(x => x > 3)
来源：http://hz.feifeiyinyue.top/gtocurkrad.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.yj202588.top/gtkwbpwriq.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.zdqjudy.top/gtbshzttry.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.pengpengdd.cyou/gtoycwowzp.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.fzhhl.top/gtqxqqqxri.html

[D14] 映射转换（每个元素变形）
来源：http://hz.xingfuxueyuan.xyz/gtubqledlx.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.cdnleiting.top/gtirigcgyd.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.kuanghao11.cn/gtmylntjjm.html

JS:   arr.map(x => x * 2)
来源：http://hz.ywan-chungtsiang.top/gtjhdcywua.html

TS:   arr.map(x => x * 2)
来源：http://hz.ydjk.org.cn/gtnztfokdx.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.jyoumei.cn/gtjlgjfbsq.html

Go:   // 手写循环
来源：http://hz.zhijiandao.cn/gtozeejvuk.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.jiagoushi.top/gtbzoenkiv.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.xuanzx.com/gtxxqppvaw.html

[D15] 去重
来源：http://hz.jyoumei.cn/gtcnevbkgq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.daria6918.cn/gtcwphmxvl.html

PHP:  array_unique($arr);
来源：http://hz.xuanzx.com/gtwkrchclk.html

JS:   [...new Set(arr)]
来源：http://hz.daxiang520.top/gtbyzsrswh.html

TS:   [...new Set(arr)]
来源：http://hz.nanxuanxn.top/gtlbehqcfd.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.9152youxi.cn/gtmmyhoail.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.yangfankeji.com/gtixcgokrj.html

Ruby: arr.uniq
来源：http://hz.hongshengwenyu.top/gtabruqnuv.html

C#:   list.Distinct().ToList()
来源：http://hz.hnxiangtu.top/gtdzpwwmba.html

[D16] 求和与平均值
来源：http://hz.feifeiyinyue.top/gtxwwgrdfg.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.xingfuxueyuan.xyz/gtumctxnjz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.52xcode.cn/gtzetlmlmi.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.nwbrower.top/gtoybplwfa.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.nanxinkj.top/gtkhumqxql.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.gotoacloud.top/gtfdhpqanu.html

Go:   // 手写循环累加
来源：http://hz.yanxiufei.cn/gtdafonjun.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.hammf.cn/gtxgkphwsh.html

C#:   list.Sum();  list.Average()
来源：http://hz.hysaishi.cn/gthzjiulwa.html

[D17] 最大值与最小值
来源：http://hz.yuanzhike.top/gtixairexd.html

Py:   max(arr);  min(arr)
来源：http://hz.ybcxt.top/gtspjgdjtq.html

PHP:  max($arr);  min($arr);
来源：http://hz.xuetiantiany.cn/gtgqellfth.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.yonumen.top/gtqnnrbomm.html

TS:   Math.max(...arr);
来源：http://hz.sysykeji.top/gtnfidjfsg.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.hnqzz.top/gtjnhoywof.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.shangyingyoupin.top/gtvlahjpho.html

Ruby: arr.max;  arr.min
来源：http://hz.fzhhl.top/gtgvcumjpe.html

C#:   list.Max();  list.Min()
来源：http://hz.cqqwz.cn/gtmpgkervp.html

[D18] 扁平化嵌套数组
来源：http://hz.sysykeji.top/gtowkzviec.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.andypj.xyz/gtcguwesyd.html

PHP:  array_merge(...$nested);
来源：http://hz.snrcjt.cn/gthusbpyaf.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.chenlongwang.top/gtluxhavfu.html

TS:   nested.flat();
来源：http://hz.cdnleiting.top/gtfcoyfvig.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.tanke756.top/gtcvvrtflb.html

Go:   // 手写双层循环
来源：http://hz.chenjidiqi.icu/gtauonjfgl.html

Ruby: nested.flatten
来源：http://hz.jqgfzy.top/gtixtkzzqe.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.shuidangran.top/gtktzfzngj.html

[D19] 按字段分组
来源：http://hz.sufxvd.cn/gtvtgvmxie.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.tianlin.xyz/gtqggeesvn.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.dianchejie.cn/gtmlzbsuro.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.sufxvd.cn/gtxrwmmlae.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.iojbl.cn/gtklqgahgt.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.pycfn.com/gtptahvbwd.html

Go:   // 手写 map[string][]T
来源：http://hz.52xcode.cn/gtoeervzpu.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.zhaomingkeji.xyz/gtborzwibj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.chenlongwang.top/gtyiflnrti.html

[D20] 统计每个元素出现次数
来源：http://hz.dianchejie.cn/gtmpdnjsva.html

Py:   Counter(arr)
来源：http://hz.guannengcc.top/gtjmmotjzj.html

PHP:  array_count_values($arr);
来源：http://hz.shanyushiyangtech.top/gtgfvgtlza.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.guannengcc.top/gtlvfshsln.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.kuanghao11.cn/gthlfbymlq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.xuetiantiany.cn/gtzsagmpvj.html

Go:   // 手写 map[T]int
来源：http://hz.meibo888.top/gtdvulxdfw.html

Ruby: arr.tally
来源：http://hz.chenjidiqi.icu/gtqrgrspuh.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.cashguo.top/gtvrxtysuv.html

[D21] 判断是否包含某元素
来源：http://hz.sufxvd.cn/gtkyapgsmj.html

Py:   x in arr
来源：http://hz.zhongyouzk.top/gtvqvmvuaf.html

PHP:  in_array($x, $arr, true);
来源：http://hz.yongpay.top/gtmsenwafx.html

JS:   arr.includes(x)
来源：http://hz.yj20258.top/gtqgedzonv.html

TS:   arr.includes(x)
来源：http://hz.cqqwz.cn/gtzfzpbogv.html

Java: list.contains(x)
来源：http://hz.cqqwz.cn/gtftxxrdyo.html

Go:   slices.Contains(arr, x)
来源：http://hz.aibaodan.cn/gtwzjhzrfl.html

Ruby: arr.include?(x)
来源：http://hz.chenjidiqi.icu/gtnafqegrd.html

C#:   list.Contains(x)
来源：http://hz.wangdashe.top/gtyarxvpor.html

[D22] 复制数组（避免共享引用）
来源：http://hz.cqqwz.cn/gtncvvwihq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.gzhubu.top/gtwtrwoyqo.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.sxryk.cn/gtopcmpwor.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.ydzc1.top/gtuzircbhe.html

TS:   [...arr];
来源：http://hz.shanyushiyangkeji.top/gtgvwhfygb.html

Java: new ArrayList<>(list);
来源：http://hz.shzxlz.cn/gtfzxgjckl.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.yuxming.cn/gtmfamzwni.html

Ruby: arr.dup;  arr.clone
来源：http://hz.nwbrower.top/gttrgnffoj.html

C#:   new List<int>(list);
来源：http://hz.guowangkeji.top/gtgklhfzkl.html

[D23] reduce 累积计算
来源：http://hz.fengsongda.top/gtnddesdmq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.vqdsnc.cn/gtoxbimbwt.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.cheryme.top/gtwmedfczp.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.daxiang520.top/gttkpsooum.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.redwolf501.top/gtxfbeotxd.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.dianchejie.cn/gtxmkbvfpz.html

Go:   // 手写循环
来源：http://hz.hysaishi.cn/gtktylessd.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.hongshengwenyu.top/gtjtmpmfsc.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.wangdashe.top/gtjlnmomhi.html

[D24] 字典 / Map 基本操作
来源：http://hz.zhaomingkeji.xyz/gtfwfnymis.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.dashuyun.cn/gtxgqrldjy.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.jiagoushi.top/gtwofsijtv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.cucudq.cn/gtzxykfpli.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.cqqwz.cn/gtqaswvenv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.sweek.top/gtdophmjtz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.fengsongda.top/gthgdfwjuw.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.cashguo.top/gtnjxtjdlb.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.ydjk.org.cn/gtysnfawno.html

[D25] Set 集合去重与交并差
来源：http://hz.zhongyouzk.top/gtwsvcmzka.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.jiagoushi.top/gtiyjepokl.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.nanxinkj.top/gtckervreu.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.hysaishi.cn/gtlnzbisew.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.xylfe.cn/gtskzooldi.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.nanxuanxn.top/gtheyoqtun.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.jinghuilouyu.cn/gtchixtkys.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.jqgufenzy.top/gthnzqmmcb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.jinqigufen.top/gtteozzdit.html

[D26] 数组转字符串
来源：http://hz.quarkkingdee.top/gtqmaqicmx.html

Py:   ", ".join(map(str, arr))
来源：http://hz.yuxming.cn/gtyzfyjhmp.html

PHP:  implode(", ", $arr);
来源：http://hz.wangshuangyany.cn/gtmwnivbbz.html

JS:   arr.join(", ")
来源：http://hz.hongshengwenyu.top/gtwziomyxr.html

TS:   arr.join(", ")
来源：http://hz.yueranfly.top/gtdutlfysh.html

Java: String.join(", ", list)
来源：http://hz.chenzaomai.com/gtohzwqttd.html

Go:   strings.Join(strs, ", ")
来源：http://hz.dashuyun.cn/gtddwkizuo.html

Ruby: arr.join(", ")
来源：http://hz.jyoumei.cn/gtzrcrcqsg.html

C#:   string.Join(", ", list)
来源：http://hz.haohaochexian.top/gtornbrjvx.html

================================================================================
来源：http://hz.ydjk.org.cn/gtafwfshur.html

E. 字符串处理
来源：http://hz.zhixingplan.top/gtwebhdaip.html

================================================================================
来源：http://hz.shzxlz.cn/gtkrxxerae.html

[E01] 拼接字符串
来源：http://hz.ywan-chungtsiang.top/gtiggyqqji.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.zhoulong.xyz/gtzckvommz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.zdqjudy.top/gtgkucvgor.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.chenjidiqi.icu/gtaklfhoae.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jianghu66.top/gtawjdnkkx.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.yonumen.top/gtdezfjugy.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.feifeiyinyue.top/gtyfwlnnsv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.xuanzx.com/gtwtkkuwpl.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.cheryme.top/gtrhxdkgbk.html

[E02] 重复字符串
来源：http://hz.zhoulong.xyz/gtnpsxuwtq.html

Py:   "ab" * 3
来源：http://hz.redwolf501.top/gtsptvunjn.html

PHP:  str_repeat("ab", 3);
来源：http://hz.9152youxi.cn/gtmxtlzmep.html

JS:   "ab".repeat(3)
来源：http://hz.andypj.xyz/gtarmdjnrl.html

TS:   "ab".repeat(3)
来源：http://hz.pycfn.com/gtgivjfwdu.html

Java: "ab".repeat(3)
来源：http://hz.sysykeji.top/gtxhjjcjnb.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.xinyue.icu/gtnstailzy.html

Ruby: "ab" * 3
来源：http://hz.nanxuanxn.top/gtnvtivqsd.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.zhixingplan.top/gtxxdqvlcy.html

[E03] 截取子串
来源：http://hz.jianghu66.top/gtmsftnbgn.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.mhx1999.top/gtcmshpsgh.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.redwolf501.top/gtmjoduzml.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.hnxiangtu.top/gtukzahdwp.html

TS:   s.slice(1, 4)
来源：http://hz.yuanzhike.top/gtfeqfknxr.html

Java: s.substring(1, 4)
来源：http://hz.shanyushiyangkeji.top/gttvbmlqox.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.cucudq.cn/gtubnsytfy.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.feifeiyinyue.top/gtstmtftgx.html

C#:   s.Substring(1, 3)
来源：http://hz.ivvv.top/gtocemhbxv.html

[E04] 查找子串位置
来源：http://hz.sysykeji.top/gthwzhbwla.html

Py:   s.find("x");  s.index("x")
来源：http://hz.fengsongda.top/gtxlgcxmtd.html

PHP:  strpos($s, "x");
来源：http://hz.c1oappe.top/gtjafrsppr.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.shangyingyoupin.top/gtfmqdhzxi.html

TS:   s.indexOf("x")
来源：http://hz.vqdsnc.cn/gtrwcpacfg.html

Java: s.indexOf("x")
来源：http://hz.meibo888.top/gtduzuwtrz.html

Go:   strings.Index(s, "x")
来源：http://hz.ehwqpu.com/gtddotbomc.html

Ruby: s.index("x")
来源：http://hz.andypj.xyz/gtlhcxgdkj.html

C#:   s.IndexOf("x")
来源：http://hz.316326.xyz/gtzwxfarfp.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.vqdsnc.cn/gtiottkuyg.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.xylfe.cn/gtpinomdep.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.jiagoushi.top/gtytvmcuju.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.ppjwa.cn/gtvxbgrdsj.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.nanxuanxn.top/gtlrlbpqnk.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.cheryme.top/gtncvefrlt.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.ydjk.org.cn/gttyssiusa.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.shangyingyoupin.top/gttqcahjqq.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.jinqigufen.top/gtoujxeahv.html

[E06] 替换子串
来源：http://hz.ybcxt.top/gtqnxsniuy.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.sxryk.cn/gtvcdouaff.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.yvedp.cn/gtqktcqxvm.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.vqdsnc.cn/gtpditcznv.html

TS:   s.replaceAll("a", "b")
来源：http://hz.pycfn.com/gtotycuvaw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.52xcode.cn/gtbpjuytqx.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.zhaomingkeji.xyz/gtabejikfs.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.jiagoushi.top/gtmpbatafw.html

C#:   s.Replace("a", "b")
来源：http://hz.xziqi.cn/gtxfehkwpz.html

[E07] 按分隔符拆分
来源：http://hz.0kj1m.cn/gtmexxsqga.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.jqgufenzy.top/gtslmdtktw.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.hfpthk.cn/gtgxkjhrss.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.xuanzx.com/gtyuaydjid.html

TS:   s.split(",")
来源：http://hz.xuanzx.com/gtcvxbmxcm.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.cqqwz.cn/gtiugefzft.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.cucudq.cn/gtbwarfzfi.html

Ruby: s.split(",");  s.split
来源：http://hz.zhixingplan.top/gtebmsrqbo.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.wangshuangyany.cn/gtdocvacyc.html

[E08] 数组按分隔符合并
来源：http://hz.chenjidiqi.icu/gtpzyjivsz.html

Py:   ",".join(items)
来源：http://hz.yonumen.top/gtpkfrjauk.html

PHP:  implode(",", $items);
来源：http://hz.birdmap.top/gtebgzxdyn.html

JS:   items.join(",")
来源：http://hz.9152youxi.cn/gthztrqeoq.html

TS:   items.join(",")
来源：http://hz.quarkkingdee.top/gttezvkccp.html

Java: String.join(",", items)
来源：http://hz.jinyuanbaomall.cn/gtpqrarkky.html

Go:   strings.Join(items, ",")
来源：http://hz.yangfankeji.com/gtoawaybnp.html

Ruby: items.join(",")
来源：http://hz.havefunace.top/gtdbhlebzk.html

C#:   string.Join(",", items)
来源：http://hz.xingfuxueyuan.xyz/gtuvkvucsz.html

[E09] 去除所有空白字符
来源：http://hz.gaohongyu789.top/gtbpkznqnq.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.xuetiantiany.cn/gtfjxivpzt.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.dashuyun.cn/gtlgnprfgz.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.c1oappe.top/gtwnuiynvr.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.cdnleiting.top/gtuegccrrk.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.bjfxy.top/gtsbarjkwk.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.zdqjudy.top/gtliotgmot.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.hywenlv.cn/gtaljxhoqb.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.zhongyouzk.top/gtnwecpdru.html

[E10] 左侧补零 / 定长填充
来源：http://hz.shanyushiyangtech.top/gtielnojuw.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.aibaodan.cn/gtjwlmuvgf.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.shanyushiyangkeji.top/gtxwkjyxwy.html

JS:   "7".padStart(3, "0")
来源：http://hz.jinqigfzy.top/gtqrexbqwq.html

TS:   "7".padStart(3, "0")
来源：http://hz.gogol.net.cn/gtovvhmelk.html

Java: String.format("%03d", 7)
来源：http://hz.guannengcc.top/gtulqelbza.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.quarkkingdee.top/gtitgmxuey.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.yonumen.top/gttkakrthj.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.ivvv.top/gtffufijzr.html

[E11] 反转字符串
来源：http://hz.tian-w.cn/gtcjkfetys.html

Py:   s[::-1]
来源：http://hz.kuanghao11.cn/gtsxawcbuj.html

PHP:  strrev($s);
来源：http://hz.cheryme.top/gtgehzpbwx.html

JS:   [...s].reverse().join("")
来源：http://hz.chenzaomai.com/gtlokviwaw.html

TS:   [...s].reverse().join("")
来源：http://hz.zhixingplan.top/gtkvbyqhax.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.ppjwa.cn/gtqmlkcfri.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.meibo888.top/gtpkbgxvpg.html

Ruby: s.reverse
来源：http://hz.aibaodan.cn/gtkkimjmtn.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.gzhubu.top/gtwbprgtpg.html

[E12] 统计某字符出现次数
来源：http://hz.dashuyun.cn/gtbgbcnqpz.html

Py:   s.count("a")
来源：http://hz.sysykeji.top/gtuajynyrz.html

PHP:  substr_count($s, "a");
来源：http://hz.jqgfzy.top/gtgkwiqbxi.html

JS:   s.split("a").length - 1
来源：http://hz.gaohongyu789.top/gtrunoudow.html

TS:   s.split("a").length - 1
来源：http://hz.dashuyun.cn/gtteruvrrp.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.shuidangran.top/gtrntouooo.html


<!-- 参考信息 -->