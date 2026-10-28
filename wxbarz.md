代发 wailian999

[D03] 在指定位置插入元素
来源：http://hz.daria6918.cn/gtgpvqzzou.html

Py:   arr.insert(0, 0)
来源：http://hz.tianlin.xyz/gtlqsqxwyi.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.cqqwz.cn/gtmhzqlnsz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.svipenyu.cn/gtqhtksrbx.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.daxiang520.top/gtxrhdajra.html

Java: list.add(0, 0);
来源：http://hz.smart0.xyz/gtrsvaekzp.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.ydzc1.top/gtauppxaik.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.aizwys.cn/gtbedptsbr.html

C#:   list.Insert(0, 0);
来源：http://hz.hnxiangtu.top/gtwyeipfql.html

[D04] 删除元素
来源：http://hz.nanxinkj.top/gtkwcfwfio.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.jinqigfzy.top/gtexyspdzd.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.ywan-chungtsiang.top/gtxidiqlmg.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.316326.xyz/gtniogtwol.html

TS:   arr.splice(0, 1);
来源：http://hz.cashguo.top/gtfeidzwpr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.hammf.cn/gtandhzhhc.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.guannengcc.top/gtvvkvvwig.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.xziqi.cn/gtfjrziwlv.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.nwbrower.top/gtlrjigtnj.html

[D05] 访问与修改元素
来源：http://hz.shzxlz.cn/gtlmygfnhr.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.sxryk.cn/gtcxzyxyfl.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.zdqjudy.top/gtwraalqdk.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.nanxuanxn.top/gtrnvxhlrt.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.yanxiufei.cn/gtnjlypftu.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.jinyuanbaomall.cn/gtksijlwun.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.yj202588.top/gtjzgihjai.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.guowangkeji.top/gtmyidebbs.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.yvedp.cn/gtaxrgaacw.html

[D06] 数组长度
来源：http://hz.cdnleiting.top/gtzunsiwfd.html

Py:   len(arr)
来源：http://hz.jianghu66.top/gtrtsxqlyk.html

PHP:  count($arr);
来源：http://hz.zhengqikj.top/gtyimittfs.html

JS:   arr.length
来源：http://hz.cucudq.cn/gtuyzzcnsv.html

TS:   arr.length
来源：http://hz.zhaomingkeji.xyz/gtdkcthpgm.html

Java: list.size();
来源：http://hz.nwbrower.top/gtbptsdshe.html

Go:   len(arr)
来源：http://hz.cqqwz.cn/gtuazgktdc.html

Ruby: arr.length; arr.size
来源：http://hz.ydzc1.top/gtjsfjsgur.html

C#:   list.Count;
来源：http://hz.tianlin.xyz/gtizepnijw.html

[D07] 切片 / 取子数组
来源：http://hz.cucudq.cn/gtswacdnrx.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.xuetiantiany.cn/gthdwokybw.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.cucudq.cn/gtwlzgaten.html

JS:   arr.slice(1, 4);
来源：http://hz.xuanzx.com/gtarckpwky.html

TS:   arr.slice(1, 4);
来源：http://hz.pycfn.com/gthndervyq.html

Java: list.subList(1, 4);
来源：http://hz.jinghuilouyu.cn/gtrdjdvjln.html

Go:   arr[1:4]
来源：http://hz.hfpthk.cn/gtmfpmrhde.html

Ruby: arr[1, 3]
来源：http://hz.52xcode.cn/gtcrtqpjqr.html

C#:   list.GetRange(1, 3);
来源：http://hz.quarkkingdee.top/gtudbykmki.html

[D08] 合并两个数组
来源：http://hz.xziqi.cn/gtjzujejsw.html

Py:   a + b;  a.extend(b)
来源：http://hz.zhixingplan.top/gtgngnljgt.html

PHP:  array_merge($a, $b);
来源：http://hz.zhaomingkeji.xyz/gtuapcmzre.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.ehwqpu.com/gtjrgefpra.html

TS:   [...a, ...b];
来源：http://hz.birdmap.top/gtmotozvvc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.yuanzhike.top/gtiydpzowp.html

Go:   append(a, b...)
来源：http://hz.chenlongwang.top/gtaefjkjnu.html

Ruby: a + b;  a.concat(b)
来源：http://hz.hfpthk.cn/gtzwwrykbn.html

C#:   a.Concat(b).ToList()
来源：http://hz.zhijiandao.cn/gtzkgkpofi.html

[D09] 排序（升序）
来源：http://hz.iojbl.cn/gtuwiyunbw.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.hysaishi.cn/gtboobfzpj.html

PHP:  sort($arr);
来源：http://hz.fzhhl.top/gtcwtdbqrx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.guowangkeji.top/gtocgshary.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.52xcode.cn/gttsrlybnf.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.nanxinkj.top/gtonbqbrqv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.fzhhl.top/gtcazivehn.html

Ruby: arr.sort
来源：http://hz.jinghuilouyu.cn/gtwwzhvpfo.html

C#:   list.Sort();
来源：http://hz.tianlin.xyz/gtmerzdzjn.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.jinqigufen.top/gtvyanwsnp.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.jinqigufen.top/gtdwfypahg.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.shanyushiyangtech.top/gtspymoqbe.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xingfuxueyuan.xyz/gtcrlvdpmr.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.tianlin.xyz/gtdghbltdx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.wangshuangyany.cn/gtwdzcpwvz.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.sxryk.cn/gtkqceebha.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.jinqigfzy.top/gttecorshr.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.gaohongyu789.top/gtuxaalkjz.html

[D11] 反转数组
来源：http://hz.shanyushiyangtech.top/gtfkovsslh.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.shanyushiyangtech.top/gtheetzyrv.html

PHP:  array_reverse($arr);
来源：http://hz.hongshengwenyu.top/gtkdowkvjf.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.snrcjt.cn/gtjdepudkb.html

TS:   [...arr].reverse();
来源：http://hz.xinyue.icu/gtcdxbfatl.html

Java: Collections.reverse(list);
来源：http://hz.jyoumei.cn/gtznrjnmge.html

Go:   slices.Reverse(arr)
来源：http://hz.snrcjt.cn/gtdeevlsyx.html

Ruby: arr.reverse
来源：http://hz.cdnleiting.top/gtytshzgot.html

C#:   list.Reverse();
来源：http://hz.nanxinkj.top/gtewarcdlm.html

[D12] 查找元素下标
来源：http://hz.zhengqikj.top/gtysajennm.html

Py:   arr.index(x);  x in arr
来源：http://hz.chenzaomai.com/gtffdebjrh.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.gotoacloud.top/gtnzxiqiei.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.shanyushiyangtech.top/gtrpltlbvc.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yanxiufei.cn/gtxyrozedo.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.svipenyu.cn/gtgsjnaibt.html

Go:   slices.Index(arr, x)
来源：http://hz.snrcjt.cn/gtfcplzops.html

Ruby: arr.index(x)
来源：http://hz.guannengcc.top/gtsbmtjdad.html

C#:   list.IndexOf(x);
来源：http://hz.fzhhl.top/gtisykbgqd.html

[D13] 过滤（保留满足条件的）
来源：http://hz.wangshuangyany.cn/gttkzkwbtd.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.jinqigfzy.top/gtatrpqozp.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.ydzc1.top/gtfrunqkgj.html

JS:   arr.filter(x => x > 3)
来源：http://hz.pengpengdd.cyou/gtmztrjopl.html

TS:   arr.filter(x => x > 3)
来源：http://hz.zdqjudy.top/gtppglezgp.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.sufxvd.cn/gtgrtvqvbq.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.tianlin.xyz/gtuqcznjzc.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.nwbrower.top/gtjzvjckar.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.zdqjudy.top/gtwoegvhgq.html

[D14] 映射转换（每个元素变形）
来源：http://hz.jinghuilouyu.cn/gtouxxiolp.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.chenjidiqi.icu/gtukumeedr.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.jinqigfzy.top/gttltkkvlk.html

JS:   arr.map(x => x * 2)
来源：http://hz.wangshuangyany.cn/gttzzcfdrc.html

TS:   arr.map(x => x * 2)
来源：http://hz.shangyingyoupin.top/gtvctrnjpr.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.cheryme.top/gtpckuopry.html

Go:   // 手写循环
来源：http://hz.mhx1999.top/gtamapzftt.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.jlsjyb.cn/gtjtynoacw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.hnqzz.top/gtnxifyhay.html

[D15] 去重
来源：http://hz.andypj.xyz/gtfofqrjsm.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.chenlongwang.top/gtmovhoebd.html

PHP:  array_unique($arr);
来源：http://hz.sweek.top/gtkihzwdnk.html

JS:   [...new Set(arr)]
来源：http://hz.hammf.cn/gtvbekzsqj.html

TS:   [...new Set(arr)]
来源：http://hz.yueranfly.top/gtdgquxhie.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.jinghuilouyu.cn/gtzlfptdgm.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.hongshengwenyu.top/gtbvtldhif.html

Ruby: arr.uniq
来源：http://hz.shanyushiyangtech.top/gtzpucsqjn.html

C#:   list.Distinct().ToList()
来源：http://hz.yvedp.cn/gtpodnjllg.html

[D16] 求和与平均值
来源：http://hz.cucudq.cn/gtfmrzbiqg.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.tanke756.top/gtdsetedfi.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.wangshuangyany.cn/gtgdxnxpnq.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zhijiandao.cn/gtoufviwzn.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.fengsongda.top/gtipdksibz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.xylfe.cn/gteauznlbd.html

Go:   // 手写循环累加
来源：http://hz.hammf.cn/gtfnuvbjof.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.tianlin.xyz/gtjsthntxp.html

C#:   list.Sum();  list.Average()
来源：http://hz.yangfankeji.com/gtibesstmw.html

[D17] 最大值与最小值
来源：http://hz.wangdashe.top/gtbamjghba.html

Py:   max(arr);  min(arr)
来源：http://hz.iojbl.cn/gtwotggijb.html

PHP:  max($arr);  min($arr);
来源：http://hz.hfpthk.cn/gtcdrevcry.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.hysaishi.cn/gtkwiqhxrx.html

TS:   Math.max(...arr);
来源：http://hz.yueranfly.top/gttfgyupgr.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.sufxvd.cn/gtifpomxog.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.chenjidiqi.icu/gtoqrrnsli.html

Ruby: arr.max;  arr.min
来源：http://hz.316326.xyz/gtvjsdakmc.html

C#:   list.Max();  list.Min()
来源：http://hz.zhixingplan.top/gtdcbfeujl.html

[D18] 扁平化嵌套数组
来源：http://hz.hongshengwenyu.top/gtyqmernbd.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.zhiwuduotai.top/gtqxlpujrb.html

PHP:  array_merge(...$nested);
来源：http://hz.jianghu66.top/gtyiqcphvy.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.hammf.cn/gthltwhdxp.html

TS:   nested.flat();
来源：http://hz.shuidangran.top/gtkxqcsjte.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.ivvv.top/gtrpnpeoyf.html

Go:   // 手写双层循环
来源：http://hz.tanke756.top/gtbglcrdyt.html

Ruby: nested.flatten
来源：http://hz.guannengcc.top/gtuinvgkpl.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.shangyingyoupin.top/gtnmwyhjsm.html

[D19] 按字段分组
来源：http://hz.zhiwuduotai.top/gtigksxefk.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.andypj.xyz/gtghqwvcjp.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.tianlin.xyz/gtoiufihyz.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.tanke756.top/gtbbaznmle.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.quarkkingdee.top/gthnxkntev.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.jiagoushi.top/gtmmaenzqy.html

Go:   // 手写 map[string][]T
来源：http://hz.ywan-chungtsiang.top/gtxpkymwbr.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.jinqigfzy.top/gtgoxbnlzg.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.dashuyun.cn/gtvaizqzee.html

[D20] 统计每个元素出现次数
来源：http://hz.jinyuanbaomall.cn/gtudezdcsz.html

Py:   Counter(arr)
来源：http://hz.shuidangran.top/gtzqvqwwjs.html

PHP:  array_count_values($arr);
来源：http://hz.9152youxi.cn/gtmsarfktu.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.9152youxi.cn/gtibaddknr.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.cdnleiting.top/gtcyseixmw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.jinqigfzy.top/gtqannjsxv.html

Go:   // 手写 map[T]int
来源：http://hz.nanxuanxn.top/gthzpdavds.html

Ruby: arr.tally
来源：http://hz.jiagoushi.top/gtqeagrmja.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.zhijiandao.cn/gtsviyyypf.html

[D21] 判断是否包含某元素
来源：http://hz.aizwys.cn/gtpxbqnbdo.html

Py:   x in arr
来源：http://hz.hysaishi.cn/gtwneubzox.html

PHP:  in_array($x, $arr, true);
来源：http://hz.birdmap.top/gtmgnopygw.html

JS:   arr.includes(x)
来源：http://hz.cqqwz.cn/gturssyesq.html

TS:   arr.includes(x)
来源：http://hz.wangdashe.top/gtcsaspxeh.html

Java: list.contains(x)
来源：http://hz.yongpay.top/gtfeplpfna.html

Go:   slices.Contains(arr, x)
来源：http://hz.tanke756.top/gtxcpplnvi.html

Ruby: arr.include?(x)
来源：http://hz.jinqigfzy.top/gttuqlxxim.html

C#:   list.Contains(x)
来源：http://hz.pengpengdd.cyou/gtdvpciyii.html

[D22] 复制数组（避免共享引用）
来源：http://hz.ydzc1.top/gtrhhivxja.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.vqdsnc.cn/gtnzlcnerk.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.shangyingyoupin.top/gtphijdgzo.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.yongpay.top/gtrufknmuu.html

TS:   [...arr];
来源：http://hz.cdnleiting.top/gtuqxepohs.html

Java: new ArrayList<>(list);
来源：http://hz.dianchejie.cn/gtpmamzjme.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.sysykeji.top/gthzimvhaw.html

Ruby: arr.dup;  arr.clone
来源：http://hz.guannengcc.top/gtxkwntdci.html

C#:   new List<int>(list);
来源：http://hz.yj202588.top/gtmvazylgi.html

[D23] reduce 累积计算
来源：http://hz.cdnleiting.top/gttttrovat.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.iojbl.cn/gtnvoqsqsg.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.quarkkingdee.top/gtmxdbrman.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.nwbrower.top/gtwgdptyab.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.hammf.cn/gtqycilnpx.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.vqdsnc.cn/gtsxmwlnkx.html

Go:   // 手写循环
来源：http://hz.cucudq.cn/gtwogztvxy.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.tian-w.cn/gtvfjweofw.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.mhx1999.top/gtmpvcjrvm.html

[D24] 字典 / Map 基本操作
来源：http://hz.ybcxt.top/gtdjsbnxyg.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.hongshengwenyu.top/gtsbkddnza.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.jlsjyb.cn/gtafowlglb.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.shanyushiyangkeji.top/gtqxwafxke.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.jinqigfzy.top/gtddbnuzxx.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.wangdashe.top/gttoiiwtvl.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.pycfn.com/gtztbkgibs.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.cucudq.cn/gtsmgvsacy.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.bjfxy.top/gthiecotrx.html

[D25] Set 集合去重与交并差
来源：http://hz.jinqigfzy.top/gthltezeyq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.c1oappe.top/gtsajnizlk.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.shangyingyoupin.top/gthqjiffox.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.ehwqpu.com/gthtfljbgl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.ydjk.org.cn/gttcyjxpdr.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.zhaomingkeji.xyz/gtweknekmb.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.shanyushiyangkeji.top/gtshxgpbmp.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.chenjidiqi.icu/gttdwimmpt.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.ivvv.top/gtcfjebatl.html

[D26] 数组转字符串
来源：http://hz.hammf.cn/gtgzgfwnxt.html

Py:   ", ".join(map(str, arr))
来源：http://hz.sweek.top/gtbrwxutww.html

PHP:  implode(", ", $arr);
来源：http://hz.guowangkeji.top/gtjdbevijp.html

JS:   arr.join(", ")
来源：http://hz.hfpthk.cn/gtwlzjfgdn.html

TS:   arr.join(", ")
来源：http://hz.hongshengwenyu.top/gtwiqsvtkl.html

Java: String.join(", ", list)
来源：http://hz.jinqigfzy.top/gthebdklac.html

Go:   strings.Join(strs, ", ")
来源：http://hz.ivvv.top/gtoffvsove.html

Ruby: arr.join(", ")
来源：http://hz.tanke756.top/gtvajesdhb.html

C#:   string.Join(", ", list)
来源：http://hz.yj202588.top/gtvpsgtuot.html

================================================================================
来源：http://hz.yvedp.cn/gttaykrfhm.html

E. 字符串处理
来源：http://hz.ydzc1.top/gtrrhtxbwj.html

================================================================================
来源：http://hz.fzhhl.top/gtndkkaxyn.html

[E01] 拼接字符串
来源：http://hz.sysykeji.top/gthquhlksn.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.yongpay.top/gtzeuvrwow.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.9152youxi.cn/gtrjocbigz.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.guannengcc.top/gtlvaygmjo.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zhaomingkeji.xyz/gtnhdnfkeb.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.svipenyu.cn/gtdsplfjqm.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.iojbl.cn/gtrvamghbh.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.wangshuangyany.cn/gtxeehvpgu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.ppjwa.cn/gtilhraeiw.html

[E02] 重复字符串
来源：http://hz.gogol.net.cn/gtucrkdkba.html

Py:   "ab" * 3
来源：http://hz.zhijiandao.cn/gtuarksops.html

PHP:  str_repeat("ab", 3);
来源：http://hz.zhongyouzk.top/gtametvywa.html

JS:   "ab".repeat(3)
来源：http://hz.jianghu66.top/gteztebftu.html

TS:   "ab".repeat(3)
来源：http://hz.jinghuilouyu.cn/gtnbxrhrsr.html

Java: "ab".repeat(3)
来源：http://hz.cucudq.cn/gtoedrfbzc.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.c1oappe.top/gtborphkxk.html

Ruby: "ab" * 3
来源：http://hz.yuanzhike.top/gtflfnojdh.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.aibaodan.cn/gtwfaunvbu.html

[E03] 截取子串
来源：http://hz.hammf.cn/gtyqnorysh.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.gzhubu.top/gtidgjaloc.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.yuxming.cn/gtrifgkwyq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.gotoacloud.top/gtgpopsmhx.html

TS:   s.slice(1, 4)
来源：http://hz.jinghuilouyu.cn/gtzesmdadf.html

Java: s.substring(1, 4)
来源：http://hz.hfpthk.cn/gtjgtsnhfy.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.yvedp.cn/gtvunhedgy.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.cashguo.top/gtgnenvpej.html

C#:   s.Substring(1, 3)
来源：http://hz.redwolf501.top/gtmabrdfnr.html

[E04] 查找子串位置
来源：http://hz.xziqi.cn/gtkqflqqgv.html

Py:   s.find("x");  s.index("x")
来源：http://hz.hysaishi.cn/gtwhwjfvlx.html

PHP:  strpos($s, "x");
来源：http://hz.chenzaomai.com/gtxctyfhvg.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.shanyushiyangtech.top/gthaeplldo.html

TS:   s.indexOf("x")
来源：http://hz.wangdashe.top/gtatxmahos.html

Java: s.indexOf("x")
来源：http://hz.jqgufenzy.top/gtpxjjlytw.html

Go:   strings.Index(s, "x")
来源：http://hz.dianchejie.cn/gtafirwtnf.html

Ruby: s.index("x")
来源：http://hz.cucudq.cn/gthapvpnbm.html

C#:   s.IndexOf("x")
来源：http://hz.havefunace.top/gtkugounnk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.yangfankeji.com/gtjthmtodl.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.havefunace.top/gtvddoipyz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.wangdashe.top/gtijakvsbq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yuanzhike.top/gtgddbdioj.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.zhoulong.xyz/gtewqbbepb.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.cashguo.top/gtgvbvnhma.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.mhx1999.top/gtkslbtykr.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.nanxuanxn.top/gtuhiywpue.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.daxiang520.top/gtyoryebtp.html

[E06] 替换子串
来源：http://hz.yuxming.cn/gtvcrnttot.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.sufxvd.cn/gtokebwoxd.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.cashguo.top/gtfgtuqmfj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yueranfly.top/gtmtbdyigp.html

TS:   s.replaceAll("a", "b")
来源：http://hz.yuxming.cn/gtnosujnrl.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jinqigfzy.top/gtempbmvrf.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.cdnleiting.top/gthpleiyva.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.yuxming.cn/gtkzgaxnsg.html

C#:   s.Replace("a", "b")
来源：http://hz.ehwqpu.com/gtociczhok.html

[E07] 按分隔符拆分
来源：http://hz.xuanzx.com/gttpfyqhjr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.redwolf501.top/gtyixyfcgm.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.xingfuxueyuan.xyz/gtghvqnbjg.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.xinyue.icu/gtumieteen.html

TS:   s.split(",")
来源：http://hz.zhongyouzk.top/gtqtrfvbdm.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.jianghu66.top/gtsvnhqcqz.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.nanxuanxn.top/gtsdhvyusj.html

Ruby: s.split(",");  s.split
来源：http://hz.guannengcc.top/gtcammpmlr.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.dianchejie.cn/gtqtghmgni.html

[E08] 数组按分隔符合并
来源：http://hz.meibo888.top/gtqqhmmgdl.html

Py:   ",".join(items)
来源：http://hz.sxryk.cn/gtvhrlqddy.html

PHP:  implode(",", $items);
来源：http://hz.yangfankeji.com/gtsaubhuai.html

JS:   items.join(",")
来源：http://hz.xziqi.cn/gtvdnpbryh.html

TS:   items.join(",")
来源：http://hz.chenzaomai.com/gtymoyzuyx.html

Java: String.join(",", items)
来源：http://hz.cdnleiting.top/gtiwnwienr.html

Go:   strings.Join(items, ",")
来源：http://hz.pengpengdd.cyou/gtciuelsye.html

Ruby: items.join(",")
来源：http://hz.yueranfly.top/gtvcphmhix.html

C#:   string.Join(",", items)
来源：http://hz.zhoulong.xyz/gtujhnaypc.html

[E09] 去除所有空白字符
来源：http://hz.shanyushiyangtech.top/gtuagycbtu.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.nwbrower.top/gteriwckbc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.ydjk.org.cn/gtteodrrml.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.zhijiandao.cn/gtrxbsbtgr.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.cucudq.cn/gtalfzxyfi.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.jinghuilouyu.cn/gtikuwqhkc.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.iojbl.cn/gtebicscmw.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.c1oappe.top/gtnitzgozg.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.gogol.net.cn/gtirkdmtbg.html


<!-- 参考信息 -->