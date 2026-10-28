代发 wailian999

Py:   len(arr)
来源：http://hz.wangshuangyany.cn/gtulzrfros.html

PHP:  count($arr);
来源：http://hz.cdnleiting.top/gtmdgxzbjw.html

JS:   arr.length
来源：http://hz.jinghuilouyu.cn/gtotpbfdwt.html

TS:   arr.length
来源：http://hz.ivvv.top/gtumbovfvu.html

Java: list.size();
来源：http://hz.gotoacloud.top/gtzbodbfij.html

Go:   len(arr)
来源：http://hz.smart0.xyz/gtenvdpgiy.html

Ruby: arr.length; arr.size
来源：http://hz.wangdashe.top/gtteqlfyzy.html

C#:   list.Count;
来源：http://hz.chenzaomai.com/gtacayrrsr.html

[D07] 切片 / 取子数组
来源：http://hz.ppjwa.cn/gtxebquidh.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.yanxiufei.cn/gtrpanktvc.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.sysykeji.top/gtspknpuak.html

JS:   arr.slice(1, 4);
来源：http://hz.nanxuanxn.top/gtgueqtslx.html

TS:   arr.slice(1, 4);
来源：http://hz.guowangkeji.top/gtetkryopk.html

Java: list.subList(1, 4);
来源：http://hz.iojbl.cn/gtebgvpacn.html

Go:   arr[1:4]
来源：http://hz.sxryk.cn/gtetegqoxt.html

Ruby: arr[1, 3]
来源：http://hz.zhoulong.xyz/gtcqmooemf.html

C#:   list.GetRange(1, 3);
来源：http://hz.yj202588.top/gtdmqfnbyo.html

[D08] 合并两个数组
来源：http://hz.aizwys.cn/gtrefjmsid.html

Py:   a + b;  a.extend(b)
来源：http://hz.daxiang520.top/gtteehgdtt.html

PHP:  array_merge($a, $b);
来源：http://hz.jinghuilouyu.cn/gtcwtfsnft.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.hysaishi.cn/gtgnnapswd.html

TS:   [...a, ...b];
来源：http://hz.zhoulong.xyz/gtynryrmbd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.shangyingyoupin.top/gtjqzfwklq.html

Go:   append(a, b...)
来源：http://hz.yongpay.top/gteigfiige.html

Ruby: a + b;  a.concat(b)
来源：http://hz.cheryme.top/gtzpauoaev.html

C#:   a.Concat(b).ToList()
来源：http://hz.0kj1m.cn/gtzegselkr.html

[D09] 排序（升序）
来源：http://hz.jinqigfzy.top/gtibblhpxk.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.nanxinkj.top/gtazjwzoah.html

PHP:  sort($arr);
来源：http://hz.haohaochexian.top/gtlwpbfjhc.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.gaohongyu789.top/gtrgusmkac.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.feifeiyinyue.top/gtxamanjln.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.c1oappe.top/gtuygunbbf.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.fzhhl.top/gtbhcdjedq.html

Ruby: arr.sort
来源：http://hz.guannengcc.top/gtgskeicgd.html

C#:   list.Sort();
来源：http://hz.chenzaomai.com/gtvuegtsks.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.shuidangran.top/gtyamsyvvk.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.dashuyun.cn/gtfzhzabll.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.dianchejie.cn/gtursdotaj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zhijiandao.cn/gtfxporhrz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zhijiandao.cn/gtgcsrrgwh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.ydzc1.top/gtbpdewcnq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.xingfuxueyuan.xyz/gtsazjowsw.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.hnxiangtu.top/gtfoywtjbj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.yongpay.top/gtpawfsuhg.html

[D11] 反转数组
来源：http://hz.zhiwuduotai.top/gtpdcufbbr.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.ydzc1.top/gtodtefbsp.html

PHP:  array_reverse($arr);
来源：http://hz.svipenyu.cn/gtrxzoswbo.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.zhoulong.xyz/gttqlhviey.html

TS:   [...arr].reverse();
来源：http://hz.cqqwz.cn/gtalsyegrz.html

Java: Collections.reverse(list);
来源：http://hz.jinyuanbaomall.cn/gtspytxzcq.html

Go:   slices.Reverse(arr)
来源：http://hz.ehwqpu.com/gtclttxgmh.html

Ruby: arr.reverse
来源：http://hz.jinqigufen.top/gtzllahgdo.html

C#:   list.Reverse();
来源：http://hz.shuidangran.top/gtfmuavwsf.html

[D12] 查找元素下标
来源：http://hz.yangfankeji.com/gtgnzbwdfo.html

Py:   arr.index(x);  x in arr
来源：http://hz.zhoulong.xyz/gthhpwauod.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.52xcode.cn/gtaogrnfca.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.ydjk.org.cn/gtuvfefruz.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.iojbl.cn/gtbaaoomxs.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.jinghuilouyu.cn/gtgwfwljew.html

Go:   slices.Index(arr, x)
来源：http://hz.zhongyouzk.top/gtheuacwng.html

Ruby: arr.index(x)
来源：http://hz.hongshengwenyu.top/gtjyhhuibl.html

C#:   list.IndexOf(x);
来源：http://hz.jqgfzy.top/gtxuhncnkq.html

[D13] 过滤（保留满足条件的）
来源：http://hz.xinyue.icu/gteoiietkj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.52xcode.cn/gtngwstlew.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.cdnleiting.top/gtpvdlwzcb.html

JS:   arr.filter(x => x > 3)
来源：http://hz.feifeiyinyue.top/gthwnpchzs.html

TS:   arr.filter(x => x > 3)
来源：http://hz.ydjk.org.cn/gtippdymmy.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.ywan-chungtsiang.top/gtrbrxlenm.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.zhengqikj.top/gtucytaibb.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.mhx1999.top/gtfrgxglan.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.zhongyouzk.top/gtyavclnwk.html

[D14] 映射转换（每个元素变形）
来源：http://hz.shuidangran.top/gtlkfcgrja.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.sxryk.cn/gtbvyyrlet.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.zdqjudy.top/gtrnmbyoln.html

JS:   arr.map(x => x * 2)
来源：http://hz.9152youxi.cn/gtbwqhawfc.html

TS:   arr.map(x => x * 2)
来源：http://hz.wangdashe.top/gtddcckkso.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.ivvv.top/gtzejwesrf.html

Go:   // 手写循环
来源：http://hz.jianghu66.top/gtaprjdscc.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.hnxiangtu.top/gtythmizcu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.sxryk.cn/gtfathnyil.html

[D15] 去重
来源：http://hz.shanyushiyangkeji.top/gtouumsybm.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.smart0.xyz/gtxsbfyvvk.html

PHP:  array_unique($arr);
来源：http://hz.snrcjt.cn/gtnhakguos.html

JS:   [...new Set(arr)]
来源：http://hz.mhx1999.top/gtgdqkatgo.html

TS:   [...new Set(arr)]
来源：http://hz.sysykeji.top/gtmzmplcyd.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.zhiwuduotai.top/gtqoxrptgj.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.wangdashe.top/gtbkrmgncq.html

Ruby: arr.uniq
来源：http://hz.gaohongyu789.top/gtyxirftfi.html

C#:   list.Distinct().ToList()
来源：http://hz.yonumen.top/gtwkmnfdpf.html

[D16] 求和与平均值
来源：http://hz.tianlin.xyz/gtklqxjyre.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.pycfn.com/gtkdefwtep.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.nanxuanxn.top/gtkacehvmz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jqgufenzy.top/gttyvqjdfw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jinyuanbaomall.cn/gtmztsmqgi.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.zhaomingkeji.xyz/gthxdwoaqf.html

Go:   // 手写循环累加
来源：http://hz.hysaishi.cn/gttozafvms.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.tian-w.cn/gtixdmsusj.html

C#:   list.Sum();  list.Average()
来源：http://hz.gzhubu.top/gtqmayqmim.html

[D17] 最大值与最小值
来源：http://hz.snrcjt.cn/gtqruhczyr.html

Py:   max(arr);  min(arr)
来源：http://hz.meibo888.top/gtzfubcyxn.html

PHP:  max($arr);  min($arr);
来源：http://hz.guannengcc.top/gthxmiablg.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.ydzc1.top/gtqcnsuawb.html

TS:   Math.max(...arr);
来源：http://hz.daxiang520.top/gtrcauduez.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.jianghu66.top/gttcrtcyty.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.daria6918.cn/gtzqhiyflv.html

Ruby: arr.max;  arr.min
来源：http://hz.jqgufenzy.top/gtovysmdox.html

C#:   list.Max();  list.Min()
来源：http://hz.zhoulong.xyz/gtqzgiceci.html

[D18] 扁平化嵌套数组
来源：http://hz.cqqwz.cn/gtfauxxjil.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.sweek.top/gtzhigdikk.html

PHP:  array_merge(...$nested);
来源：http://hz.dianchejie.cn/gtxfnjufeq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.bjfxy.top/gtybonznrf.html

TS:   nested.flat();
来源：http://hz.hnqzz.top/gtukptgfbs.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.snrcjt.cn/gtgnfniyfb.html

Go:   // 手写双层循环
来源：http://hz.yj20258.top/gtmmvzfxzw.html

Ruby: nested.flatten
来源：http://hz.jinyuanbaomall.cn/gtnhqtmmlt.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.jinqigufen.top/gtepshmguc.html

[D19] 按字段分组
来源：http://hz.vqdsnc.cn/gtnwzvsarn.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.aizwys.cn/gtugattbou.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.guannengcc.top/gtklfxkmsp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.jinqigfzy.top/gtclovhelp.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.yongpay.top/gtjvhzzzhh.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.guannengcc.top/gtnepehdsc.html

Go:   // 手写 map[string][]T
来源：http://hz.hysaishi.cn/gtmystmsdk.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.0kj1m.cn/gthjncgmxy.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.zhijiandao.cn/gtnygonweu.html

[D20] 统计每个元素出现次数
来源：http://hz.xylfe.cn/gtvhyhmkbs.html

Py:   Counter(arr)
来源：http://hz.vqdsnc.cn/gtnwqgfuce.html

PHP:  array_count_values($arr);
来源：http://hz.yj20258888.top/gtecnqcdyt.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jinghuilouyu.cn/gtwqhmctnx.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.xuetiantiany.cn/gtubsfocpv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.hywenlv.cn/gtdzdtpimf.html

Go:   // 手写 map[T]int
来源：http://hz.gogol.net.cn/gterhbqwko.html

Ruby: arr.tally
来源：http://hz.shuidangran.top/gtapxvcnld.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.9152youxi.cn/gtfeqjqvto.html

[D21] 判断是否包含某元素
来源：http://hz.daria6918.cn/gtsqpeyrst.html

Py:   x in arr
来源：http://hz.yueranfly.top/gtviigvnym.html

PHP:  in_array($x, $arr, true);
来源：http://hz.jqgfzy.top/gtnkgxfxkq.html

JS:   arr.includes(x)
来源：http://hz.yongpay.top/gtdooatgmc.html

TS:   arr.includes(x)
来源：http://hz.gaohongyu789.top/gtqgvfiqhf.html

Java: list.contains(x)
来源：http://hz.aizwys.cn/gtyecfiqtg.html

Go:   slices.Contains(arr, x)
来源：http://hz.zhaomingkeji.xyz/gtebtezqcq.html

Ruby: arr.include?(x)
来源：http://hz.chenjidiqi.icu/gtvowozcgx.html

C#:   list.Contains(x)
来源：http://hz.ywan-chungtsiang.top/gtrvsbodjr.html

[D22] 复制数组（避免共享引用）
来源：http://hz.jlsjyb.cn/gtoqosbpto.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.xziqi.cn/gtsihqdjaa.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.dashuyun.cn/gtswlmlkby.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.cheryme.top/gtwqvlhacu.html

TS:   [...arr];
来源：http://hz.gotoacloud.top/gtnikydkvg.html

Java: new ArrayList<>(list);
来源：http://hz.bjfxy.top/gtbfoidnar.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.hnxiangtu.top/gtkqquyxvk.html

Ruby: arr.dup;  arr.clone
来源：http://hz.ywan-chungtsiang.top/gtjdomalym.html

C#:   new List<int>(list);
来源：http://hz.zhixingplan.top/gtezkiobnv.html

[D23] reduce 累积计算
来源：http://hz.yanxiufei.cn/gtrdrtahsr.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.cdnleiting.top/gthwswiqcx.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.hammf.cn/gtgxsxjsmm.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.daria6918.cn/gtdrlxducl.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.smart0.xyz/gtqduxhxkg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.c1oappe.top/gtjrshqfgc.html

Go:   // 手写循环
来源：http://hz.hongshengwenyu.top/gtxrdcscbn.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.jinqigufen.top/gtozozqpnw.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.redwolf501.top/gtjkqjczhw.html

[D24] 字典 / Map 基本操作
来源：http://hz.chenlongwang.top/gtgmoeygnv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.dianchejie.cn/gtjngtmgxy.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.xinyue.icu/gtgyfjnwig.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.yangfankeji.com/gtswcqjhac.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.zdqjudy.top/gtioxpvllg.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.kuanghao11.cn/gtohepyljw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.feifeiyinyue.top/gtafricjch.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.shuidangran.top/gtohjlnljg.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.shangyingyoupin.top/gtcypibapt.html

[D25] Set 集合去重与交并差
来源：http://hz.meibo888.top/gtlkbigtcg.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.jinghuilouyu.cn/gtljaqekdc.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.tanke756.top/gtekxsuvhi.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.yj202588.top/gtjloahoxf.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.hnqzz.top/gtgjawlxdw.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.xinyue.icu/gtfkpjuhmg.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.pycfn.com/gtonjvkvaw.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.cheryme.top/gtcbtfszcw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.yj20258888.top/gtwykhbjrj.html

[D26] 数组转字符串
来源：http://hz.zycfv.cn/gtdkgjyfzm.html

Py:   ", ".join(map(str, arr))
来源：http://hz.tianlin.xyz/gtbtqhznss.html

PHP:  implode(", ", $arr);
来源：http://hz.sweek.top/gtuqggyrjn.html

JS:   arr.join(", ")
来源：http://hz.0kj1m.cn/gtooikgcmq.html

TS:   arr.join(", ")
来源：http://hz.yanxiufei.cn/gtlaeirzxf.html

Java: String.join(", ", list)
来源：http://hz.cucudq.cn/gtbpwceive.html

Go:   strings.Join(strs, ", ")
来源：http://hz.yangfankeji.com/gtfmrgqbos.html

Ruby: arr.join(", ")
来源：http://hz.hongshengwenyu.top/gtzevmecqx.html

C#:   string.Join(", ", list)
来源：http://hz.jlsjyb.cn/gtbqxxqpsy.html

================================================================================
来源：http://hz.ehwqpu.com/gtxtuobrjq.html

E. 字符串处理
来源：http://hz.zhongyouzk.top/gtikkiwuvm.html

================================================================================
来源：http://hz.wangdashe.top/gtisslacwu.html

[E01] 拼接字符串
来源：http://hz.redwolf501.top/gtxdwyqcfq.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.shanyushiyangkeji.top/gtjgmnwhwi.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.sweek.top/gtqoayofnp.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.sufxvd.cn/gtdzvnagqx.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yonumen.top/gtiqcprgvg.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.yj202588.top/gtbsymgwlp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.gaohongyu789.top/gtayrhmpmw.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.quarkkingdee.top/gtqbdatvas.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.zhiwuduotai.top/gtmhwzyusc.html

[E02] 重复字符串
来源：http://hz.smart0.xyz/gtwnparzzp.html

Py:   "ab" * 3
来源：http://hz.hongshengwenyu.top/gtlzchpfkh.html

PHP:  str_repeat("ab", 3);
来源：http://hz.yuanzhike.top/gtggtjjfoo.html

JS:   "ab".repeat(3)
来源：http://hz.shangyingyoupin.top/gtyzdaguaw.html

TS:   "ab".repeat(3)
来源：http://hz.zycfv.cn/gtxcjroxfe.html

Java: "ab".repeat(3)
来源：http://hz.yj202588.top/gtiayzgfme.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.9152youxi.cn/gtokuiwety.html

Ruby: "ab" * 3
来源：http://hz.aibaodan.cn/gtfdfgrlln.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.snrcjt.cn/gtykqrgccs.html

[E03] 截取子串
来源：http://hz.ywan-chungtsiang.top/gtatknqryl.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.chenzaomai.com/gthlrnxhnu.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.jianghu66.top/gtnbsilyvi.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.zhixingplan.top/gtmcwysnav.html

TS:   s.slice(1, 4)
来源：http://hz.aizwys.cn/gtobqwtwzl.html

Java: s.substring(1, 4)
来源：http://hz.hnqzz.top/gthdtetczs.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.iojbl.cn/gtgembsekd.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.jinghuilouyu.cn/gtteqcmvhi.html

C#:   s.Substring(1, 3)
来源：http://hz.wangdashe.top/gtontsppcs.html

[E04] 查找子串位置
来源：http://hz.wangdashe.top/gtehabxkze.html

Py:   s.find("x");  s.index("x")
来源：http://hz.tianlin.xyz/gtgkfyldxp.html

PHP:  strpos($s, "x");
来源：http://hz.wangshuangyany.cn/gtcdpdavxx.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.gaohongyu789.top/gtpxqfccwc.html

TS:   s.indexOf("x")
来源：http://hz.kuanghao11.cn/gtuygjqpzz.html

Java: s.indexOf("x")
来源：http://hz.tian-w.cn/gtubklnzcp.html

Go:   strings.Index(s, "x")
来源：http://hz.jqgufenzy.top/gtywzqrdxv.html

Ruby: s.index("x")
来源：http://hz.chenzaomai.com/gtaipxsgza.html

C#:   s.IndexOf("x")
来源：http://hz.yuxming.cn/gtqxzaarcm.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.c1oappe.top/gtoilgurck.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.pengpengdd.cyou/gtqskvirfk.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.tanke756.top/gtdkktgdhq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.cashguo.top/gtaiwebwmg.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.chenlongwang.top/gtlhdvuamt.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.cucudq.cn/gtojhvyuzz.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.gaohongyu789.top/gttppsigcj.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.nanxinkj.top/gtdbitnhbr.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.zdqjudy.top/gtbbiklriz.html

[E06] 替换子串
来源：http://hz.yanxiufei.cn/gtfnhkywoq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.hfpthk.cn/gtnaldktld.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.snrcjt.cn/gturqyuwjq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.vqdsnc.cn/gtzasnzkgb.html

TS:   s.replaceAll("a", "b")
来源：http://hz.jlsjyb.cn/gtzxqqxgly.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.cqqwz.cn/gtswhenfio.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.snrcjt.cn/gtnpfptwbo.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.fzhhl.top/gtsivewkrg.html

C#:   s.Replace("a", "b")
来源：http://hz.guannengcc.top/gtinkguguw.html

[E07] 按分隔符拆分
来源：http://hz.shangyingyoupin.top/gtbeuzwipt.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.sxryk.cn/gtcfuyffiq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.yanxiufei.cn/gtlvulmgcl.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.zhixingplan.top/gtbziduhza.html

TS:   s.split(",")
来源：http://hz.gogol.net.cn/gtgmuxeqpp.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.yuxming.cn/gthqtfbdhq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.sxryk.cn/gthecbjacn.html

Ruby: s.split(",");  s.split
来源：http://hz.jyoumei.cn/gtdwksdaug.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.chenzaomai.com/gtyllascjv.html

[E08] 数组按分隔符合并
来源：http://hz.guannengcc.top/gtrzwkvoes.html

Py:   ",".join(items)
来源：http://hz.aibaodan.cn/gtbqjiipkv.html

PHP:  implode(",", $items);
来源：http://hz.zycfv.cn/gtyrpjuwya.html

JS:   items.join(",")
来源：http://hz.ivvv.top/gtxfogksan.html

TS:   items.join(",")
来源：http://hz.fzhhl.top/gtpjkkenlu.html

Java: String.join(",", items)
来源：http://hz.ppjwa.cn/gtitaatcau.html

Go:   strings.Join(items, ",")
来源：http://hz.sufxvd.cn/gtadyfwpdj.html

Ruby: items.join(",")
来源：http://hz.cdnleiting.top/gtmrbvstlz.html

C#:   string.Join(",", items)
来源：http://hz.snrcjt.cn/gtikiptwou.html

[E09] 去除所有空白字符
来源：http://hz.bjfxy.top/gtslioxbwo.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.ehwqpu.com/gtunfpeiuo.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.yangfankeji.com/gtdungktik.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.nwbrower.top/gtnhynchzk.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.shuidangran.top/gthajpozak.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.zhixingplan.top/gtgcpsjzax.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.sweek.top/gtypbplhvh.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.hywenlv.cn/gtfwimapps.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.chenjidiqi.icu/gtcshlskuf.html

[E10] 左侧补零 / 定长填充
来源：http://hz.xingfuxueyuan.xyz/gtsldrnqwd.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.xingfuxueyuan.xyz/gtoyfgsabc.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.guannengcc.top/gtbuirxqzq.html

JS:   "7".padStart(3, "0")
来源：http://hz.ybcxt.top/gtyebpkvda.html

TS:   "7".padStart(3, "0")
来源：http://hz.jiagoushi.top/gtwoskambc.html

Java: String.format("%03d", 7)
来源：http://hz.zycfv.cn/gtzgaivyol.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.jqgufenzy.top/gtuqoizubb.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.shanyushiyangkeji.top/gtfxzltxif.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.ivvv.top/gtushdqucp.html

[E11] 反转字符串
来源：http://hz.jqgufenzy.top/gtkhkgnfxl.html

Py:   s[::-1]
来源：http://hz.xuanzx.com/gtwfyhjzmd.html

PHP:  strrev($s);
来源：http://hz.dashuyun.cn/gtkycsndfa.html

JS:   [...s].reverse().join("")
来源：http://hz.jqgfzy.top/gtdremtpqi.html

TS:   [...s].reverse().join("")
来源：http://hz.wangdashe.top/gtoecowxqx.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.shanyushiyangkeji.top/gtioxspwrb.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.jlsjyb.cn/gtbztkztyl.html

Ruby: s.reverse
来源：http://hz.xylfe.cn/gtwismlmlw.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.shanyushiyangkeji.top/gtmhqzpuxu.html

[E12] 统计某字符出现次数
来源：http://hz.hongshengwenyu.top/gtqtknweqz.html

Py:   s.count("a")
来源：http://hz.zhixingplan.top/gtehwrdjwv.html

PHP:  substr_count($s, "a");
来源：http://hz.jinqigufen.top/gtvwvtvsih.html

JS:   s.split("a").length - 1
来源：http://hz.cucudq.cn/gtmpkqdjol.html

TS:   s.split("a").length - 1
来源：http://hz.iojbl.cn/gthmeemrsf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.andypj.xyz/gtjkdkcrdl.html

Go:   strings.Count(s, "a")
来源：http://hz.hfpthk.cn/gtyfjgqjuk.html

Ruby: s.count("a")
来源：http://hz.nwbrower.top/gtpashzypc.html

C#:   s.Count(c => c == 'a')
来源：http://hz.zhixingplan.top/gtmfbzolsr.html

[E13] 逐字符遍历
来源：http://hz.gogol.net.cn/gtgoexejsf.html


<!-- 参考信息 -->