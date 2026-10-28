代发 wailian999

[D07] 切片 / 取子数组
来源：http://hz.chenzaomai.com/gtzunbyryx.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.haohaochexian.top/gtcsyodbwp.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.cdnleiting.top/gtvhaysdnb.html

JS:   arr.slice(1, 4);
来源：http://hz.sufxvd.cn/gtzeskxcyv.html

TS:   arr.slice(1, 4);
来源：http://hz.zhongyouzk.top/gtnebysxsj.html

Java: list.subList(1, 4);
来源：http://hz.shanyushiyangkeji.top/gthmxhlndn.html

Go:   arr[1:4]
来源：http://hz.chenjidiqi.icu/gtwxnikcsb.html

Ruby: arr[1, 3]
来源：http://hz.jyoumei.cn/gtccgidhnu.html

C#:   list.GetRange(1, 3);
来源：http://hz.shangyingyoupin.top/gtaxysiysz.html

[D08] 合并两个数组
来源：http://hz.yj202588.top/gtobtaysfp.html

Py:   a + b;  a.extend(b)
来源：http://hz.cdnleiting.top/gtxvgnbuzs.html

PHP:  array_merge($a, $b);
来源：http://hz.snrcjt.cn/gtdjwtdtfm.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.redwolf501.top/gtcmhwfqnu.html

TS:   [...a, ...b];
来源：http://hz.yuanzhike.top/gtgfflegtc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.xuetiantiany.cn/gtuwpgxrcx.html

Go:   append(a, b...)
来源：http://hz.jlsjyb.cn/gtypcwbxty.html

Ruby: a + b;  a.concat(b)
来源：http://hz.ybcxt.top/gtbccoinxc.html

C#:   a.Concat(b).ToList()
来源：http://hz.hnxiangtu.top/gtzetwbqvn.html

[D09] 排序（升序）
来源：http://hz.shanyushiyangkeji.top/gtjdwvtqyf.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.shanyushiyangtech.top/gteoegdake.html

PHP:  sort($arr);
来源：http://hz.jinqigfzy.top/gtqzgjhlgi.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.dashuyun.cn/gtmxfphifn.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.jinyuanbaomall.cn/gtwkkpixwr.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.xuetiantiany.cn/gtleaflitd.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.cqqwz.cn/gtlpaitfwd.html

Ruby: arr.sort
来源：http://hz.chenjidiqi.icu/gtvcmjwcim.html

C#:   list.Sort();
来源：http://hz.cheryme.top/gtuffhkwue.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.wangshuangyany.cn/gtstahhdka.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.aibaodan.cn/gtsvinmhrz.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.shanyushiyangtech.top/gtjuvltuhj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jyoumei.cn/gtlloaktxr.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.cucudq.cn/gtncxedqzv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.jlsjyb.cn/gtewxfvtwb.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.daxiang520.top/gtizsfltyl.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.ehwqpu.com/gtjlbiizas.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.gotoacloud.top/gtqqpzyznb.html

[D11] 反转数组
来源：http://hz.guannengcc.top/gtjvkuunai.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.xinyue.icu/gtdcjyfhwm.html

PHP:  array_reverse($arr);
来源：http://hz.shangyingyoupin.top/gtgghopmay.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.jyoumei.cn/gtheoxhpkv.html

TS:   [...arr].reverse();
来源：http://hz.jyoumei.cn/gtbpunotyq.html

Java: Collections.reverse(list);
来源：http://hz.sxryk.cn/gthualetcb.html

Go:   slices.Reverse(arr)
来源：http://hz.fzhhl.top/gtmjfmgrlr.html

Ruby: arr.reverse
来源：http://hz.cashguo.top/gtiiullrvw.html

C#:   list.Reverse();
来源：http://hz.feifeiyinyue.top/gtjtrncrli.html

[D12] 查找元素下标
来源：http://hz.yuanzhike.top/gtedfepuyr.html

Py:   arr.index(x);  x in arr
来源：http://hz.ywan-chungtsiang.top/gtrctofxpn.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.birdmap.top/gtxchtdkdv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.svipenyu.cn/gtrnsdxjac.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zhijiandao.cn/gtqrvfcduf.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.9152youxi.cn/gttxytmukd.html

Go:   slices.Index(arr, x)
来源：http://hz.cheryme.top/gtizfrakxl.html

Ruby: arr.index(x)
来源：http://hz.feifeiyinyue.top/gtutdxvuve.html

C#:   list.IndexOf(x);
来源：http://hz.ywan-chungtsiang.top/gtcsolqeew.html

[D13] 过滤（保留满足条件的）
来源：http://hz.ehwqpu.com/gtxheoxima.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.bjfxy.top/gtzbzljbmd.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.yueranfly.top/gtfddqsqnd.html

JS:   arr.filter(x => x > 3)
来源：http://hz.tianlin.xyz/gtbnbftpwj.html

TS:   arr.filter(x => x > 3)
来源：http://hz.jiagoushi.top/gttzdhbfwu.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.shuidangran.top/gtvhvkhiae.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.zdqjudy.top/gttyarlnzd.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.meibo888.top/gtoncfpzwo.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.tianlin.xyz/gtsrnspxlk.html

[D14] 映射转换（每个元素变形）
来源：http://hz.sweek.top/gtodfzpkoh.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.daria6918.cn/gtzzunvbjb.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.ydjk.org.cn/gtziordsnm.html

JS:   arr.map(x => x * 2)
来源：http://hz.havefunace.top/gtfyeomoin.html

TS:   arr.map(x => x * 2)
来源：http://hz.zycfv.cn/gtqcqpszfh.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.cashguo.top/gtcoxhylfl.html

Go:   // 手写循环
来源：http://hz.yvedp.cn/gthjnbzvft.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.mhx1999.top/gttdjzqmgu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.xuanzx.com/gtftxmlxbf.html

[D15] 去重
来源：http://hz.ydzc1.top/gtmoelckxj.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.jyoumei.cn/gtblmeoryv.html

PHP:  array_unique($arr);
来源：http://hz.fzhhl.top/gtpqdorrad.html

JS:   [...new Set(arr)]
来源：http://hz.meibo888.top/gtqojfsthg.html

TS:   [...new Set(arr)]
来源：http://hz.hongshengwenyu.top/gtjipjfwta.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.316326.xyz/gtpjfhuahj.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.hfpthk.cn/gtbkqnpgwq.html

Ruby: arr.uniq
来源：http://hz.nanxinkj.top/gtyzzllpge.html

C#:   list.Distinct().ToList()
来源：http://hz.gogol.net.cn/gturjklhmi.html

[D16] 求和与平均值
来源：http://hz.aizwys.cn/gtewyjreuk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.hnxiangtu.top/gtptrtkwwz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.quarkkingdee.top/gtbavvkswm.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hammf.cn/gttixmsbms.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zhiwuduotai.top/gtzbuvwxpb.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.gaohongyu789.top/gtesbvafye.html

Go:   // 手写循环累加
来源：http://hz.ybcxt.top/gtgsrrvcxi.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.iojbl.cn/gtpyacnbws.html

C#:   list.Sum();  list.Average()
来源：http://hz.xuetiantiany.cn/gtbqfkpyxl.html

[D17] 最大值与最小值
来源：http://hz.zhaomingkeji.xyz/gtfyocvatf.html

Py:   max(arr);  min(arr)
来源：http://hz.c1oappe.top/gtokyawdce.html

PHP:  max($arr);  min($arr);
来源：http://hz.yanxiufei.cn/gtoyjappmx.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.tian-w.cn/gtwtufywrk.html

TS:   Math.max(...arr);
来源：http://hz.cucudq.cn/gtlsjvxsjl.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.andypj.xyz/gthuvrsxbp.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.dianchejie.cn/gtmjlaxdnh.html

Ruby: arr.max;  arr.min
来源：http://hz.shangyingyoupin.top/gtaqtudjkp.html

C#:   list.Max();  list.Min()
来源：http://hz.zhiwuduotai.top/gttjlpjypg.html

[D18] 扁平化嵌套数组
来源：http://hz.aibaodan.cn/gtqgsoznra.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.kuanghao11.cn/gtdhjgxemm.html

PHP:  array_merge(...$nested);
来源：http://hz.cdnleiting.top/gtxfkoidwk.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.ehwqpu.com/gtcnxryttn.html

TS:   nested.flat();
来源：http://hz.gotoacloud.top/gtjzskwaeb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.fzhhl.top/gtrnddttzt.html

Go:   // 手写双层循环
来源：http://hz.yj202588.top/gtobzguris.html

Ruby: nested.flatten
来源：http://hz.gogol.net.cn/gtbxzacbdj.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.jianghu66.top/gtixnkjxhb.html

[D19] 按字段分组
来源：http://hz.redwolf501.top/gtbuqguodh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.feifeiyinyue.top/gtjzdoqfha.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.316326.xyz/gtdueodfem.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.hnqzz.top/gtwvafnyiu.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.sufxvd.cn/gtwhvfngab.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.hywenlv.cn/gtleytkooj.html

Go:   // 手写 map[string][]T
来源：http://hz.yonumen.top/gtsztqrifa.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.nanxuanxn.top/gtjkrpufup.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.shanyushiyangkeji.top/gtjuubxwgv.html

[D20] 统计每个元素出现次数
来源：http://hz.xylfe.cn/gtqdswofve.html

Py:   Counter(arr)
来源：http://hz.dianchejie.cn/gtqjcealzt.html

PHP:  array_count_values($arr);
来源：http://hz.hnqzz.top/gtetwjoetc.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yueranfly.top/gtsmnpokbd.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.snrcjt.cn/gttjjuqmsl.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.chenzaomai.com/gtiskjumht.html

Go:   // 手写 map[T]int
来源：http://hz.redwolf501.top/gtryiiuqtz.html

Ruby: arr.tally
来源：http://hz.ybcxt.top/gtlqidblvz.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.yonumen.top/gtdhxeogef.html

[D21] 判断是否包含某元素
来源：http://hz.aibaodan.cn/gtiqbkfrul.html

Py:   x in arr
来源：http://hz.xinyue.icu/gtykbjgllt.html

PHP:  in_array($x, $arr, true);
来源：http://hz.tanke756.top/gtocouaxwu.html

JS:   arr.includes(x)
来源：http://hz.gzhubu.top/gtfhkrxeco.html

TS:   arr.includes(x)
来源：http://hz.guowangkeji.top/gtnghrijzk.html

Java: list.contains(x)
来源：http://hz.daxiang520.top/gtxiyypqmv.html

Go:   slices.Contains(arr, x)
来源：http://hz.ivvv.top/gtjjynfuqq.html

Ruby: arr.include?(x)
来源：http://hz.nwbrower.top/gtnmjshyfg.html

C#:   list.Contains(x)
来源：http://hz.tanke756.top/gtywfiypss.html

[D22] 复制数组（避免共享引用）
来源：http://hz.redwolf501.top/gthprejtrq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.wangshuangyany.cn/gtflznpjkd.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.yanxiufei.cn/gtugwjpstd.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.chenlongwang.top/gtpmubxemu.html

TS:   [...arr];
来源：http://hz.shuidangran.top/gtkjqzrfnp.html

Java: new ArrayList<>(list);
来源：http://hz.jyoumei.cn/gtxlfpkyub.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.jqgfzy.top/gtnqdmqvhc.html

Ruby: arr.dup;  arr.clone
来源：http://hz.dianchejie.cn/gttaqqaidy.html

C#:   new List<int>(list);
来源：http://hz.daxiang520.top/gtzcnmprry.html

[D23] reduce 累积计算
来源：http://hz.gotoacloud.top/gtrqmivxwn.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.gzhubu.top/gtbedieeto.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.quarkkingdee.top/gtzkfjqgdr.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.cheryme.top/gttjjgyrgj.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.quarkkingdee.top/gtnerwcfck.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.jqgufenzy.top/gtmcelfulj.html

Go:   // 手写循环
来源：http://hz.sufxvd.cn/gtxoxlkwoj.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.shanyushiyangkeji.top/gthlgbgszp.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.hammf.cn/gtavfipaeq.html

[D24] 字典 / Map 基本操作
来源：http://hz.jlsjyb.cn/gtcneqjuia.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.zhiwuduotai.top/gtcwwznndz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.hammf.cn/gtcvdbbspj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.hfpthk.cn/gtjbwzzkpk.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.hnxiangtu.top/gtvkoemlye.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.gzhubu.top/gtxzrhxgqv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.sweek.top/gtlytspgpk.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.316326.xyz/gttypllqzi.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.cashguo.top/gtpnqcqacc.html

[D25] Set 集合去重与交并差
来源：http://hz.snrcjt.cn/gtjqtljskb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.bjfxy.top/gtdwqyiqgy.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.nanxinkj.top/gtovrjabja.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.zhongyouzk.top/gtfxymodvr.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.pycfn.com/gtpohersbj.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.sweek.top/gthiwzryai.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.birdmap.top/gtcfmgfxca.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.xylfe.cn/gtnvporzfp.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.hongshengwenyu.top/gtbncgtdrs.html

[D26] 数组转字符串
来源：http://hz.wangshuangyany.cn/gtgkbtmlzn.html

Py:   ", ".join(map(str, arr))
来源：http://hz.ehwqpu.com/gtcmopdims.html

PHP:  implode(", ", $arr);
来源：http://hz.52xcode.cn/gtzkfyhmnz.html

JS:   arr.join(", ")
来源：http://hz.aibaodan.cn/gtrfqdpeil.html

TS:   arr.join(", ")
来源：http://hz.zhongyouzk.top/gtmcsnqgjk.html

Java: String.join(", ", list)
来源：http://hz.cheryme.top/gtlihnlrcn.html

Go:   strings.Join(strs, ", ")
来源：http://hz.guowangkeji.top/gtrkesvknl.html

Ruby: arr.join(", ")
来源：http://hz.andypj.xyz/gtlagrufqh.html

C#:   string.Join(", ", list)
来源：http://hz.sysykeji.top/gtygcsnygz.html

================================================================================
来源：http://hz.shzxlz.cn/gthqruofdm.html

E. 字符串处理
来源：http://hz.pengpengdd.cyou/gttslgleqs.html

================================================================================
来源：http://hz.shzxlz.cn/gtrzthiglr.html

[E01] 拼接字符串
来源：http://hz.shangyingyoupin.top/gtfazrokfw.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.ppjwa.cn/gtfazzrvlk.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.jqgfzy.top/gtpntpaljz.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.havefunace.top/gtnruwkrur.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.wangshuangyany.cn/gtsqqynquy.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.jqgfzy.top/gtnaowykax.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.snrcjt.cn/gtzoqirrbu.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.jinghuilouyu.cn/gtgjoyqsfc.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.zycfv.cn/gtstyrodcu.html

[E02] 重复字符串
来源：http://hz.316326.xyz/gtmrjsohge.html

Py:   "ab" * 3
来源：http://hz.zhoulong.xyz/gttgmuvxkm.html

PHP:  str_repeat("ab", 3);
来源：http://hz.aibaodan.cn/gtpssyyrsd.html

JS:   "ab".repeat(3)
来源：http://hz.nanxinkj.top/gtjamefjoo.html

TS:   "ab".repeat(3)
来源：http://hz.ivvv.top/gtxnfgdvvl.html

Java: "ab".repeat(3)
来源：http://hz.ydzc1.top/gtkcmzabkw.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.xingfuxueyuan.xyz/gtreypxcwd.html

Ruby: "ab" * 3
来源：http://hz.yueranfly.top/gtnvwbmesf.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.kuanghao11.cn/gtdnrnkunj.html

[E03] 截取子串
来源：http://hz.gzhubu.top/gtbycjsssw.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.cdnleiting.top/gtzehkawdj.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.zdqjudy.top/gtlazeyxqr.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.quarkkingdee.top/gtgyqpbdwh.html

TS:   s.slice(1, 4)
来源：http://hz.9152youxi.cn/gtltxvzssc.html

Java: s.substring(1, 4)
来源：http://hz.kuanghao11.cn/gtqkgxrrzn.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.gogol.net.cn/gtnjagmvvn.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.yongpay.top/gtmijtzxvz.html

C#:   s.Substring(1, 3)
来源：http://hz.cucudq.cn/gtdewiowkb.html

[E04] 查找子串位置
来源：http://hz.yj20258888.top/gtygtuxlky.html

Py:   s.find("x");  s.index("x")
来源：http://hz.wangdashe.top/gtczgfpbkk.html

PHP:  strpos($s, "x");
来源：http://hz.zhongyouzk.top/gtwhveroqx.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.jqgfzy.top/gtvbwduptj.html

TS:   s.indexOf("x")
来源：http://hz.yongpay.top/gtynjgfywe.html

Java: s.indexOf("x")
来源：http://hz.hnqzz.top/gtbgkhjzha.html

Go:   strings.Index(s, "x")
来源：http://hz.aizwys.cn/gtqrnjldvu.html

Ruby: s.index("x")
来源：http://hz.nwbrower.top/gtisxzhtub.html

C#:   s.IndexOf("x")
来源：http://hz.jinqigfzy.top/gtddqhjnkd.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.yongpay.top/gtsczyfhwj.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.fengsongda.top/gttzczqrmd.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.yvedp.cn/gthkjnckmf.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.shanyushiyangkeji.top/gtgzrgrpmg.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.hysaishi.cn/gtmyldgprl.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.cucudq.cn/gtgjplzqpa.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.havefunace.top/gtbgolvveo.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.ybcxt.top/gtbbssxnny.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.dianchejie.cn/gtprkamrvh.html

[E06] 替换子串
来源：http://hz.jiagoushi.top/gththsfeph.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.yuanzhike.top/gtbgsjkyul.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.shzxlz.cn/gtqdrzaxvg.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jyoumei.cn/gtxsounwwf.html

TS:   s.replaceAll("a", "b")
来源：http://hz.zhoulong.xyz/gtgfaorcem.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.tanke756.top/gtksbruuwo.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.ywan-chungtsiang.top/gtxltkyaka.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.sxryk.cn/gtricaztfn.html

C#:   s.Replace("a", "b")
来源：http://hz.guannengcc.top/gtmymxvrpf.html

[E07] 按分隔符拆分
来源：http://hz.jinghuilouyu.cn/gtcyegtnat.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.tanke756.top/gtjwzteqbx.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.ydzc1.top/gtsiafjrfn.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.cdnleiting.top/gtcnhvukkf.html

TS:   s.split(",")
来源：http://hz.nanxuanxn.top/gtfundnvos.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.daria6918.cn/gtltygyxmj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.sweek.top/gtujaudeje.html

Ruby: s.split(",");  s.split
来源：http://hz.haohaochexian.top/gtknjcsamj.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.meibo888.top/gtruxwjjud.html

[E08] 数组按分隔符合并
来源：http://hz.iojbl.cn/gtghjskrbf.html

Py:   ",".join(items)
来源：http://hz.smart0.xyz/gtixuqxcen.html

PHP:  implode(",", $items);
来源：http://hz.zhixingplan.top/gtwpfobeqw.html

JS:   items.join(",")
来源：http://hz.jinqigufen.top/gtchajsbyu.html

TS:   items.join(",")
来源：http://hz.xziqi.cn/gtastwrfdr.html

Java: String.join(",", items)
来源：http://hz.hongshengwenyu.top/gtfomochhv.html

Go:   strings.Join(items, ",")
来源：http://hz.yonumen.top/gthxjkyjmo.html

Ruby: items.join(",")
来源：http://hz.ehwqpu.com/gtrmbmigxw.html

C#:   string.Join(",", items)
来源：http://hz.gaohongyu789.top/gtykdclyuy.html

[E09] 去除所有空白字符
来源：http://hz.zhixingplan.top/gthitrcxel.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.haohaochexian.top/gtirddypva.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.yvedp.cn/gttllvsoig.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.nanxinkj.top/gtevwcmnky.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.hysaishi.cn/gtqtulvntw.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.shanyushiyangkeji.top/gtoyvjkpan.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.chenjidiqi.icu/gtnyymybqn.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.fengsongda.top/gtftdkohzj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.kuanghao11.cn/gtzcpkdyfy.html

[E10] 左侧补零 / 定长填充
来源：http://hz.iojbl.cn/gtjsnjmdzn.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.shuidangran.top/gtwsigaxmh.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.yuanzhike.top/gtzavgqrpw.html

JS:   "7".padStart(3, "0")
来源：http://hz.zhengqikj.top/gttjxcldse.html

TS:   "7".padStart(3, "0")
来源：http://hz.chenzaomai.com/gteaeghagu.html

Java: String.format("%03d", 7)
来源：http://hz.jlsjyb.cn/gtvhnyiqoo.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.cucudq.cn/gtrxxuwmob.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.52xcode.cn/gtbovkqiaz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.guannengcc.top/gtvyiggukl.html

[E11] 反转字符串
来源：http://hz.bjfxy.top/gtxwwcelgo.html

Py:   s[::-1]
来源：http://hz.shanyushiyangtech.top/gtqaibbpaz.html

PHP:  strrev($s);
来源：http://hz.ybcxt.top/gtpoesdmqv.html

JS:   [...s].reverse().join("")
来源：http://hz.yueranfly.top/gtxouohwlj.html

TS:   [...s].reverse().join("")
来源：http://hz.gogol.net.cn/gtqkynwplq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.ehwqpu.com/gtezvtjhre.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.shuidangran.top/gtpuxlcgah.html

Ruby: s.reverse
来源：http://hz.zhaomingkeji.xyz/gtzfbqodut.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.yj202588.top/gtvritcfpf.html

[E12] 统计某字符出现次数
来源：http://hz.xuetiantiany.cn/gtxvjqcmxz.html

Py:   s.count("a")
来源：http://hz.jianghu66.top/gttvqsnwwp.html

PHP:  substr_count($s, "a");
来源：http://hz.kuanghao11.cn/gtyavgogrp.html

JS:   s.split("a").length - 1
来源：http://hz.smart0.xyz/gtsregkkuf.html

TS:   s.split("a").length - 1
来源：http://hz.birdmap.top/gtvllnasdl.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.mhx1999.top/gtwiqrcuao.html

Go:   strings.Count(s, "a")
来源：http://hz.meibo888.top/gtqaoizhkc.html

Ruby: s.count("a")
来源：http://hz.jiagoushi.top/gtanornnbr.html

C#:   s.Count(c => c == 'a')
来源：http://hz.ywan-chungtsiang.top/gtfjvnngpv.html

[E13] 逐字符遍历
来源：http://hz.zhengqikj.top/gtibizegom.html

Py:   for ch in s: print(ch)
来源：http://hz.tanke756.top/gtymqccrnm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.zhiwuduotai.top/gtqonzyavr.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zdqjudy.top/gtdbhoqokd.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yangfankeji.com/gtoxpyaeml.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.jinqigufen.top/gtsqwyrgfx.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.aibaodan.cn/gtppncgchh.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.nanxinkj.top/gtuiucdjud.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.hammf.cn/gtuoamranm.html


<!-- 参考信息 -->