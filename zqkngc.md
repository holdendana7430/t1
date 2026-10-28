代发 wailian999

Py:   len(arr)
来源：http://hz.gotoacloud.top/gtkwozromo.html

PHP:  count($arr);
来源：http://hz.yanxiufei.cn/gtpqmutkln.html

JS:   arr.length
来源：http://hz.fzhhl.top/gtqvitjsyx.html

TS:   arr.length
来源：http://hz.sysykeji.top/gtkbdrertq.html

Java: list.size();
来源：http://hz.guannengcc.top/gthstovwmq.html

Go:   len(arr)
来源：http://hz.cheryme.top/gtnxrdyfee.html

Ruby: arr.length; arr.size
来源：http://hz.wangshuangyany.cn/gtbspzcbam.html

C#:   list.Count;
来源：http://hz.sufxvd.cn/gthrhpagyf.html

[D07] 切片 / 取子数组
来源：http://hz.shanyushiyangkeji.top/gtpedqcnuy.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.zhongyouzk.top/gtfdbndnjl.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.sufxvd.cn/gtuazzvbhj.html

JS:   arr.slice(1, 4);
来源：http://hz.wangdashe.top/gtljxpjfip.html

TS:   arr.slice(1, 4);
来源：http://hz.nanxinkj.top/gtplwzkrot.html

Java: list.subList(1, 4);
来源：http://hz.hnqzz.top/gtlrkuwtho.html

Go:   arr[1:4]
来源：http://hz.redwolf501.top/gttmkhbico.html

Ruby: arr[1, 3]
来源：http://hz.jiagoushi.top/gtctsnxqve.html

C#:   list.GetRange(1, 3);
来源：http://hz.fengsongda.top/gtandaorkk.html

[D08] 合并两个数组
来源：http://hz.hywenlv.cn/gtcmsjbjcu.html

Py:   a + b;  a.extend(b)
来源：http://hz.yj20258888.top/gtjxzohgnu.html

PHP:  array_merge($a, $b);
来源：http://hz.ywan-chungtsiang.top/gtfelhpwhh.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.gogol.net.cn/gtmxyourtz.html

TS:   [...a, ...b];
来源：http://hz.shanyushiyangtech.top/gtwjtirfye.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.tanke756.top/gtflkolvay.html

Go:   append(a, b...)
来源：http://hz.zdqjudy.top/gtoctuoncj.html

Ruby: a + b;  a.concat(b)
来源：http://hz.cdnleiting.top/gtfnjvytta.html

C#:   a.Concat(b).ToList()
来源：http://hz.cdnleiting.top/gtrdbxrghi.html

[D09] 排序（升序）
来源：http://hz.jinghuilouyu.cn/gtvhipewgq.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.dianchejie.cn/gttzyqtcok.html

PHP:  sort($arr);
来源：http://hz.svipenyu.cn/gtwmmfhswx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.yuanzhike.top/gtcmncdfnl.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.wangdashe.top/gthznfggyg.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.daxiang520.top/gtzmohevxa.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.guowangkeji.top/gtplyudttm.html

Ruby: arr.sort
来源：http://hz.hfpthk.cn/gtkutevxcx.html

C#:   list.Sort();
来源：http://hz.redwolf501.top/gtcfpwdwvb.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.shuidangran.top/gtdegebvam.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.daxiang520.top/gtbowjixuj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.c1oappe.top/gtzkzmowoc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yangfankeji.com/gtchcerwso.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yj202588.top/gtuesolnov.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.redwolf501.top/gtkfvamhxl.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.yonumen.top/gttvkegzmc.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.yanxiufei.cn/gtjhrgdyez.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.jinqigufen.top/gtkdqchrjf.html

[D11] 反转数组
来源：http://hz.yvedp.cn/gtfcwgvvyp.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.andypj.xyz/gttmpbwpdz.html

PHP:  array_reverse($arr);
来源：http://hz.hnxiangtu.top/gtmwonjzpo.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.hnqzz.top/gtlacdrdde.html

TS:   [...arr].reverse();
来源：http://hz.sysykeji.top/gtrtyjdknz.html

Java: Collections.reverse(list);
来源：http://hz.gogol.net.cn/gtozyeurid.html

Go:   slices.Reverse(arr)
来源：http://hz.nwbrower.top/gtjlpqhhxv.html

Ruby: arr.reverse
来源：http://hz.svipenyu.cn/gtdukjlbql.html

C#:   list.Reverse();
来源：http://hz.sxryk.cn/gtjvwwjbkk.html

[D12] 查找元素下标
来源：http://hz.tanke756.top/gtblnfywrz.html

Py:   arr.index(x);  x in arr
来源：http://hz.dianchejie.cn/gtwqmbmgug.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.chenlongwang.top/gtvebijrgv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.kuanghao11.cn/gtyjwwyqnm.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.hywenlv.cn/gtpfkbtmub.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.hywenlv.cn/gtjhneikof.html

Go:   slices.Index(arr, x)
来源：http://hz.chenzaomai.com/gtqzobrpya.html

Ruby: arr.index(x)
来源：http://hz.yongpay.top/gtrymrczro.html

C#:   list.IndexOf(x);
来源：http://hz.kuanghao11.cn/gtublvtmyu.html

[D13] 过滤（保留满足条件的）
来源：http://hz.mhx1999.top/gtkyelknaw.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.ydzc1.top/gtoxdnlimq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.jlsjyb.cn/gtkjkosjdc.html

JS:   arr.filter(x => x > 3)
来源：http://hz.chenjidiqi.icu/gtzgfvreea.html

TS:   arr.filter(x => x > 3)
来源：http://hz.0kj1m.cn/gtgmmkvbzt.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.chenjidiqi.icu/gtmoyttvru.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.nanxinkj.top/gtqwbwhshc.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.jqgfzy.top/gtalfplhlb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.fzhhl.top/gthzdudrgw.html

[D14] 映射转换（每个元素变形）
来源：http://hz.jinqigfzy.top/gtabfxvgcv.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.shangyingyoupin.top/gtptxcsyhr.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.shanyushiyangtech.top/gtpvyncega.html

JS:   arr.map(x => x * 2)
来源：http://hz.fengsongda.top/gtipvosoah.html

TS:   arr.map(x => x * 2)
来源：http://hz.sweek.top/gtymibyasv.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.kuanghao11.cn/gtsbuqcdju.html

Go:   // 手写循环
来源：http://hz.vqdsnc.cn/gtogtilgwz.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.ppjwa.cn/gtvvnsalec.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.yuanzhike.top/gttgghnhke.html

[D15] 去重
来源：http://hz.aizwys.cn/gtowtyiump.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.jqgfzy.top/gthkgfpgyv.html

PHP:  array_unique($arr);
来源：http://hz.yueranfly.top/gtppdxgvvm.html

JS:   [...new Set(arr)]
来源：http://hz.jinyuanbaomall.cn/gtstzbfmga.html

TS:   [...new Set(arr)]
来源：http://hz.cqqwz.cn/gtyllbnzqn.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.ybcxt.top/gtzrrtzpet.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.jiagoushi.top/gtwbrocwrs.html

Ruby: arr.uniq
来源：http://hz.mhx1999.top/gtbsxkippc.html

C#:   list.Distinct().ToList()
来源：http://hz.nwbrower.top/gtxcpfjlmb.html

[D16] 求和与平均值
来源：http://hz.ivvv.top/gtziylezij.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.jqgufenzy.top/gtuxxoljhk.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.hysaishi.cn/gtltqtovrt.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.daria6918.cn/gtmnovmgyv.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.haohaochexian.top/gtswoekqel.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.c1oappe.top/gtqfzzizgm.html

Go:   // 手写循环累加
来源：http://hz.zhongyouzk.top/gtkgefxxrx.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.shangyingyoupin.top/gtwpxmgngh.html

C#:   list.Sum();  list.Average()
来源：http://hz.jinqigufen.top/gtcgwybbvy.html

[D17] 最大值与最小值
来源：http://hz.chenjidiqi.icu/gtufrwwapi.html

Py:   max(arr);  min(arr)
来源：http://hz.fzhhl.top/gtniuoloez.html

PHP:  max($arr);  min($arr);
来源：http://hz.nanxinkj.top/gtcacnvtsk.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.52xcode.cn/gtlairhhxm.html

TS:   Math.max(...arr);
来源：http://hz.yvedp.cn/gtvrvtczaf.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.jqgfzy.top/gtevcnmdaz.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.aizwys.cn/gtftfciykl.html

Ruby: arr.max;  arr.min
来源：http://hz.hywenlv.cn/gtgxsgdoqr.html

C#:   list.Max();  list.Min()
来源：http://hz.nwbrower.top/gtlyjgzbqd.html

[D18] 扁平化嵌套数组
来源：http://hz.0kj1m.cn/gtndjscxwm.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.ybcxt.top/gtyzymwxwv.html

PHP:  array_merge(...$nested);
来源：http://hz.gzhubu.top/gtyrmbbxbv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.xingfuxueyuan.xyz/gtkcvcssxn.html

TS:   nested.flat();
来源：http://hz.sweek.top/gteboenmec.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.yuxming.cn/gtyvdanexo.html

Go:   // 手写双层循环
来源：http://hz.ehwqpu.com/gtdclrpnjq.html

Ruby: nested.flatten
来源：http://hz.chenjidiqi.icu/gtqirvgbwn.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.jinghuilouyu.cn/gteyeeznwt.html

[D19] 按字段分组
来源：http://hz.aizwys.cn/gtqhelshit.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.meibo888.top/gtoujyhzta.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.jyoumei.cn/gtsnlmikxh.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.fengsongda.top/gtrdbsfznp.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.yuanzhike.top/gtdyhacrgr.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.nanxinkj.top/gtspaejgre.html

Go:   // 手写 map[string][]T
来源：http://hz.zycfv.cn/gtjhbvdkak.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.ybcxt.top/gtfnwfsagw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.shuidangran.top/gtryfruabc.html

[D20] 统计每个元素出现次数
来源：http://hz.cqqwz.cn/gtnarwlewd.html

Py:   Counter(arr)
来源：http://hz.xuetiantiany.cn/gtatjciaqv.html

PHP:  array_count_values($arr);
来源：http://hz.snrcjt.cn/gtjhtgfdmh.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.andypj.xyz/gtictfzbhu.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.chenlongwang.top/gtbpiorxox.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.zhoulong.xyz/gthmzfdijj.html

Go:   // 手写 map[T]int
来源：http://hz.ivvv.top/gttcrsxqts.html

Ruby: arr.tally
来源：http://hz.ybcxt.top/gtaokqzqyx.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.xinyue.icu/gtwbtfojkz.html

[D21] 判断是否包含某元素
来源：http://hz.dianchejie.cn/gttubmznex.html

Py:   x in arr
来源：http://hz.guannengcc.top/gtgucmfpwm.html

PHP:  in_array($x, $arr, true);
来源：http://hz.shzxlz.cn/gtaytagqpi.html

JS:   arr.includes(x)
来源：http://hz.ydjk.org.cn/gtwyfcxtty.html

TS:   arr.includes(x)
来源：http://hz.zhoulong.xyz/gthaauwcqa.html

Java: list.contains(x)
来源：http://hz.0kj1m.cn/gtopynifqs.html

Go:   slices.Contains(arr, x)
来源：http://hz.tianlin.xyz/gtfegxfcpe.html

Ruby: arr.include?(x)
来源：http://hz.cucudq.cn/gtegdzexlz.html

C#:   list.Contains(x)
来源：http://hz.xingfuxueyuan.xyz/gtggfoyoig.html

[D22] 复制数组（避免共享引用）
来源：http://hz.gzhubu.top/gtueanrqcm.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.smart0.xyz/gtkduwhyvv.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.cashguo.top/gthpsiqxly.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.birdmap.top/gtadkvzsjp.html

TS:   [...arr];
来源：http://hz.sysykeji.top/gtnnofqauu.html

Java: new ArrayList<>(list);
来源：http://hz.birdmap.top/gtzzuanqad.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.jinghuilouyu.cn/gtddlaamaw.html

Ruby: arr.dup;  arr.clone
来源：http://hz.fengsongda.top/gtdsahkofx.html

C#:   new List<int>(list);
来源：http://hz.0kj1m.cn/gtbuebywin.html

[D23] reduce 累积计算
来源：http://hz.snrcjt.cn/gtdsyizmpd.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.guowangkeji.top/gtssqawsfz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.dianchejie.cn/gtiixpzmhn.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yvedp.cn/gtafuyboiw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jiagoushi.top/gttewjmoku.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.yj20258.top/gtgmuoorkt.html

Go:   // 手写循环
来源：http://hz.gotoacloud.top/gthcyrfxnb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.xinyue.icu/gtfsvgufiu.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.haohaochexian.top/gthlfwuskg.html

[D24] 字典 / Map 基本操作
来源：http://hz.feifeiyinyue.top/gtckwzrary.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.gogol.net.cn/gttliofkyy.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.9152youxi.cn/gthjyyqlmg.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.nanxinkj.top/gtldpbbloy.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.zdqjudy.top/gtxwehythp.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.ydzc1.top/gthejpesga.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.xingfuxueyuan.xyz/gtmgpdxcdp.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.dashuyun.cn/gtxmkvtcvp.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.yuanzhike.top/gtaenuulnf.html

[D25] Set 集合去重与交并差
来源：http://hz.quarkkingdee.top/gtywkcjtrl.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.haohaochexian.top/gtktlnwrnr.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.haohaochexian.top/gtajbstvnu.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.zhoulong.xyz/gtvwyurhye.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.ppjwa.cn/gtqdnnjxvq.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.ivvv.top/gttvyfxpqw.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.iojbl.cn/gtieopimzm.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.pycfn.com/gtylmrvnms.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.hnqzz.top/gtdzsryvpf.html

[D26] 数组转字符串
来源：http://hz.yanxiufei.cn/gtefqssdxm.html

Py:   ", ".join(map(str, arr))
来源：http://hz.c1oappe.top/gtqicukyta.html

PHP:  implode(", ", $arr);
来源：http://hz.fengsongda.top/gtsfiaifub.html

JS:   arr.join(", ")
来源：http://hz.tian-w.cn/gtgcjyccvy.html

TS:   arr.join(", ")
来源：http://hz.jiagoushi.top/gthvgnsydp.html

Java: String.join(", ", list)
来源：http://hz.shanyushiyangkeji.top/gtzrjvwpsg.html

Go:   strings.Join(strs, ", ")
来源：http://hz.guannengcc.top/gtlppborbx.html

Ruby: arr.join(", ")
来源：http://hz.tanke756.top/gtslorbymi.html

C#:   string.Join(", ", list)
来源：http://hz.shzxlz.cn/gtcccjxsnm.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtmwlzvfpv.html

E. 字符串处理
来源：http://hz.jiagoushi.top/gtlvmgxlxu.html

================================================================================
来源：http://hz.jianghu66.top/gtfbaktlsr.html

[E01] 拼接字符串
来源：http://hz.xinyue.icu/gtwhhqjmac.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.hnxiangtu.top/gtanqhgapd.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.yueranfly.top/gtxabuxepv.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zhoulong.xyz/gtunwbfxxu.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ivvv.top/gtgkmawecd.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.gogol.net.cn/gtwzbhtlzp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.xziqi.cn/gttdkzleqc.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.fzhhl.top/gtrbalxiem.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.shuidangran.top/gtjfxlacpl.html

[E02] 重复字符串
来源：http://hz.guannengcc.top/gtvszngham.html

Py:   "ab" * 3
来源：http://hz.aibaodan.cn/gtztvgkxba.html

PHP:  str_repeat("ab", 3);
来源：http://hz.hammf.cn/gtbiphrbjl.html

JS:   "ab".repeat(3)
来源：http://hz.shanyushiyangtech.top/gttjnbmgdl.html

TS:   "ab".repeat(3)
来源：http://hz.aibaodan.cn/gtjqvisjrf.html

Java: "ab".repeat(3)
来源：http://hz.yuanzhike.top/gtgdvlntue.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.xingfuxueyuan.xyz/gtcfgqbzyy.html

Ruby: "ab" * 3
来源：http://hz.gaohongyu789.top/gtcwiircmm.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.shanyushiyangkeji.top/gtrtajkzok.html

[E03] 截取子串
来源：http://hz.jianghu66.top/gtkcsxxvsu.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.cqqwz.cn/gtdtwqyhtm.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.yangfankeji.com/gtfcrylanl.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.ywan-chungtsiang.top/gtrenkumpz.html

TS:   s.slice(1, 4)
来源：http://hz.bjfxy.top/gtxhscrnxp.html

Java: s.substring(1, 4)
来源：http://hz.shzxlz.cn/gtoknzfwfl.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.zhaomingkeji.xyz/gtcbtqwtki.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.bjfxy.top/gtegbwmsdw.html

C#:   s.Substring(1, 3)
来源：http://hz.chenjidiqi.icu/gtmtnkmsni.html

[E04] 查找子串位置
来源：http://hz.pycfn.com/gteuxtyyte.html

Py:   s.find("x");  s.index("x")
来源：http://hz.zhongyouzk.top/gtnijzllzd.html

PHP:  strpos($s, "x");
来源：http://hz.yuanzhike.top/gttiwtgmea.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.cdnleiting.top/gtbkyjzyae.html

TS:   s.indexOf("x")
来源：http://hz.chenjidiqi.icu/gtnerwjttz.html

Java: s.indexOf("x")
来源：http://hz.svipenyu.cn/gterowendb.html

Go:   strings.Index(s, "x")
来源：http://hz.daria6918.cn/gtbajjkyhu.html

Ruby: s.index("x")
来源：http://hz.dianchejie.cn/gtyrayhtkm.html

C#:   s.IndexOf("x")
来源：http://hz.zhoulong.xyz/gthwnuceuf.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.daxiang520.top/gthgleanlq.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.hongshengwenyu.top/gtcxsxioeg.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.hnqzz.top/gtdgpqrkhx.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.ydjk.org.cn/gtotudnfwu.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.9152youxi.cn/gtezrmhocm.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.ivvv.top/gtneeyezdt.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.gogol.net.cn/gtyondbech.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.svipenyu.cn/gtjdsliruo.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.jqgfzy.top/gtcsvsccko.html

[E06] 替换子串
来源：http://hz.wangdashe.top/gtmuhsczja.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.9152youxi.cn/gtkqzjtrcc.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.zhengqikj.top/gthebfkgsi.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.hysaishi.cn/gtcghchqlj.html

TS:   s.replaceAll("a", "b")
来源：http://hz.bjfxy.top/gtzmimdwzu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.guannengcc.top/gttmzjezxd.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.ppjwa.cn/gtubihyxva.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.gogol.net.cn/gtrkcgbmao.html

C#:   s.Replace("a", "b")
来源：http://hz.svipenyu.cn/gtucjjrzzp.html

[E07] 按分隔符拆分
来源：http://hz.xinyue.icu/gtstaxduhi.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.jinghuilouyu.cn/gtkwfygmps.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.yuxming.cn/gtsrnfoqrm.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.zycfv.cn/gtjytvhnbm.html

TS:   s.split(",")
来源：http://hz.snrcjt.cn/gtrjlsirbq.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.yanxiufei.cn/gtcrpbmkan.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.aibaodan.cn/gtucszzsjy.html

Ruby: s.split(",");  s.split
来源：http://hz.gotoacloud.top/gtykkznshy.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.cashguo.top/gtuvmapuyf.html

[E08] 数组按分隔符合并
来源：http://hz.ivvv.top/gtholiwmao.html

Py:   ",".join(items)
来源：http://hz.shanyushiyangkeji.top/gtepoqrudh.html

PHP:  implode(",", $items);
来源：http://hz.zhijiandao.cn/gtqbruhtvk.html

JS:   items.join(",")
来源：http://hz.jinqigufen.top/gtckiwiquf.html

TS:   items.join(",")
来源：http://hz.nanxinkj.top/gtrctgxnqp.html

Java: String.join(",", items)
来源：http://hz.xingfuxueyuan.xyz/gtmxlnvxtk.html

Go:   strings.Join(items, ",")
来源：http://hz.mhx1999.top/gtqkrdprmm.html

Ruby: items.join(",")
来源：http://hz.ivvv.top/gtnvbkcsbb.html

C#:   string.Join(",", items)
来源：http://hz.c1oappe.top/gtazinyaqn.html

[E09] 去除所有空白字符
来源：http://hz.cheryme.top/gtjuibbxho.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.aizwys.cn/gtendtsgac.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.shanyushiyangtech.top/gtqoecuhhe.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.ybcxt.top/gtbekwkvlo.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.zycfv.cn/gtwhfboouq.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.xylfe.cn/gtwiqkmepr.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.guowangkeji.top/gtlbarlkfg.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.dianchejie.cn/gtnqitlmla.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.daxiang520.top/gtmyxnhczc.html

[E10] 左侧补零 / 定长填充
来源：http://hz.jianghu66.top/gtfcuyaxap.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.yonumen.top/gtdmahfqac.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.daxiang520.top/gtukbcftmr.html

JS:   "7".padStart(3, "0")
来源：http://hz.birdmap.top/gtwhhplmwd.html

TS:   "7".padStart(3, "0")
来源：http://hz.yj202588.top/gtvihmpurt.html

Java: String.format("%03d", 7)
来源：http://hz.wangshuangyany.cn/gtbijpkbgd.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.smart0.xyz/gtkslcqtga.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.ehwqpu.com/gtmgalocvk.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.aibaodan.cn/gtbxcoqvvf.html

[E11] 反转字符串
来源：http://hz.yueranfly.top/gtzcpimjcw.html

Py:   s[::-1]
来源：http://hz.fzhhl.top/gtnnyxifyo.html

PHP:  strrev($s);
来源：http://hz.hnxiangtu.top/gtlhxskelo.html

JS:   [...s].reverse().join("")
来源：http://hz.dianchejie.cn/gtajjzfdyx.html

TS:   [...s].reverse().join("")
来源：http://hz.shanyushiyangtech.top/gttfwbxmpo.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.ydzc1.top/gtenxjgrhf.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.jiagoushi.top/gthxlibtol.html

Ruby: s.reverse
来源：http://hz.mhx1999.top/gtglfrlkuh.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.zhiwuduotai.top/gtshrrhavq.html

[E12] 统计某字符出现次数
来源：http://hz.aizwys.cn/gthnrzkfhe.html

Py:   s.count("a")
来源：http://hz.chenjidiqi.icu/gtaiqxhhfg.html

PHP:  substr_count($s, "a");
来源：http://hz.quarkkingdee.top/gtizluekeo.html

JS:   s.split("a").length - 1
来源：http://hz.hysaishi.cn/gtfulkvxzp.html

TS:   s.split("a").length - 1
来源：http://hz.c1oappe.top/gttjckewhm.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.snrcjt.cn/gtrvsolrzm.html

Go:   strings.Count(s, "a")
来源：http://hz.yj202588.top/gtlyuabplf.html

Ruby: s.count("a")
来源：http://hz.jiagoushi.top/gtmraxknhr.html

C#:   s.Count(c => c == 'a')
来源：http://hz.shzxlz.cn/gtacyxlthz.html

[E13] 逐字符遍历
来源：http://hz.yangfankeji.com/gtlfqzvlii.html


<!-- 参考信息 -->