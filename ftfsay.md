代发 wailian999

Py:   len(arr)
来源：http://hz.jinqigfzy.top/gtxldrmeyr.html

PHP:  count($arr);
来源：http://hz.pengpengdd.cyou/gtqerhpjeb.html

JS:   arr.length
来源：http://hz.cashguo.top/gtzmaspbbk.html

TS:   arr.length
来源：http://hz.yuanzhike.top/gtjthquulj.html

Java: list.size();
来源：http://hz.bjfxy.top/gtqamgasah.html

Go:   len(arr)
来源：http://hz.hysaishi.cn/gtinqmosit.html

Ruby: arr.length; arr.size
来源：http://hz.chenzaomai.com/gtsdjcpgrs.html

C#:   list.Count;
来源：http://hz.cashguo.top/gtphwwyabo.html

[D07] 切片 / 取子数组
来源：http://hz.316326.xyz/gtagztczer.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.chenjidiqi.icu/gthiesbqad.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.feifeiyinyue.top/gtdivxiaie.html

JS:   arr.slice(1, 4);
来源：http://hz.tanke756.top/gtmnfdyqnu.html

TS:   arr.slice(1, 4);
来源：http://hz.hnxiangtu.top/gtkmkrayoj.html

Java: list.subList(1, 4);
来源：http://hz.jinyuanbaomall.cn/gthgzkupzl.html

Go:   arr[1:4]
来源：http://hz.ydjk.org.cn/gtpsxchxny.html

Ruby: arr[1, 3]
来源：http://hz.cucudq.cn/gtemigtced.html

C#:   list.GetRange(1, 3);
来源：http://hz.bjfxy.top/gtptrxopva.html

[D08] 合并两个数组
来源：http://hz.jqgfzy.top/gtqaetvvae.html

Py:   a + b;  a.extend(b)
来源：http://hz.chenjidiqi.icu/gtzyzsdksk.html

PHP:  array_merge($a, $b);
来源：http://hz.316326.xyz/gtxblsczdu.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.0kj1m.cn/gtsewlknhf.html

TS:   [...a, ...b];
来源：http://hz.52xcode.cn/gtvmqvqlnp.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.cqqwz.cn/gthweemrvq.html

Go:   append(a, b...)
来源：http://hz.gogol.net.cn/gtqfywgqza.html

Ruby: a + b;  a.concat(b)
来源：http://hz.tanke756.top/gtfwssjjxh.html

C#:   a.Concat(b).ToList()
来源：http://hz.gotoacloud.top/gtwngwxtxr.html

[D09] 排序（升序）
来源：http://hz.hnxiangtu.top/gtnabcrory.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.feifeiyinyue.top/gtruhqfhtz.html

PHP:  sort($arr);
来源：http://hz.ybcxt.top/gtukfurkyg.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.quarkkingdee.top/gtmbvhkyyw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.nwbrower.top/gtilyytlmq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.tian-w.cn/gtrxuepniu.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.daria6918.cn/gtyxsnpsxl.html

Ruby: arr.sort
来源：http://hz.zhijiandao.cn/gtnrhovkuj.html

C#:   list.Sort();
来源：http://hz.zhiwuduotai.top/gtkdadrady.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.zhongyouzk.top/gtytremjvb.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.hnxiangtu.top/gtmetlghpj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.tianlin.xyz/gtdvcvbosn.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.ydjk.org.cn/gtlgeosykq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.shzxlz.cn/gtytjxpuri.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.svipenyu.cn/gtiznhrxie.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.guowangkeji.top/gthhxniscf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.yvedp.cn/gtmzfxdkmt.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.zhijiandao.cn/gtxrykgnei.html

[D11] 反转数组
来源：http://hz.52xcode.cn/gtzebtjmvh.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.ehwqpu.com/gtvdsmpuxc.html

PHP:  array_reverse($arr);
来源：http://hz.xuanzx.com/gtexfzmshs.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.guowangkeji.top/gtiadoxfay.html

TS:   [...arr].reverse();
来源：http://hz.pycfn.com/gtbhdpqdau.html

Java: Collections.reverse(list);
来源：http://hz.wangshuangyany.cn/gtahvjartv.html

Go:   slices.Reverse(arr)
来源：http://hz.pycfn.com/gtrknkxgvh.html

Ruby: arr.reverse
来源：http://hz.zhongyouzk.top/gttbpcsohl.html

C#:   list.Reverse();
来源：http://hz.fzhhl.top/gtyddeavyr.html

[D12] 查找元素下标
来源：http://hz.svipenyu.cn/gtpkgdoesd.html

Py:   arr.index(x);  x in arr
来源：http://hz.tianlin.xyz/gtyejvvwaw.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.yuanzhike.top/gtkfwzszer.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.cheryme.top/gtodrlsvle.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zhongyouzk.top/gtddrxnwzp.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.tian-w.cn/gtagnnxtur.html

Go:   slices.Index(arr, x)
来源：http://hz.yj202588.top/gtjqcezqtw.html

Ruby: arr.index(x)
来源：http://hz.bjfxy.top/gtrjpeidms.html

C#:   list.IndexOf(x);
来源：http://hz.cashguo.top/gtyyclzerv.html

[D13] 过滤（保留满足条件的）
来源：http://hz.9152youxi.cn/gtzoncmmnv.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.hnqzz.top/gtkdtoiimf.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.yonumen.top/gtwgylimwm.html

JS:   arr.filter(x => x > 3)
来源：http://hz.yj20258.top/gtqfrbsvcd.html

TS:   arr.filter(x => x > 3)
来源：http://hz.redwolf501.top/gtnmtslbxz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.hysaishi.cn/gtasqqzkcq.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.bjfxy.top/gtdkpjcyol.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.shangyingyoupin.top/gtzvqopyie.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.snrcjt.cn/gtqchtsenn.html

[D14] 映射转换（每个元素变形）
来源：http://hz.mhx1999.top/gtoynesmvm.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.yvedp.cn/gtdoaikzvu.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.hfpthk.cn/gtlvxpubsz.html

JS:   arr.map(x => x * 2)
来源：http://hz.jyoumei.cn/gtnxjonsem.html

TS:   arr.map(x => x * 2)
来源：http://hz.hammf.cn/gtpmrzmbui.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.gogol.net.cn/gtcqlkpiuv.html

Go:   // 手写循环
来源：http://hz.316326.xyz/gttnqncqng.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.zhixingplan.top/gtmwpqxlvf.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.jiagoushi.top/gtpthlzgym.html

[D15] 去重
来源：http://hz.sxryk.cn/gtkyxsxigc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.cashguo.top/gtngovgubz.html

PHP:  array_unique($arr);
来源：http://hz.yvedp.cn/gtonxrukbg.html

JS:   [...new Set(arr)]
来源：http://hz.c1oappe.top/gtjeukpxfz.html

TS:   [...new Set(arr)]
来源：http://hz.yangfankeji.com/gtudmvevbu.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.shangyingyoupin.top/gtbpnqltnn.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.yueranfly.top/gtnxfmwnly.html

Ruby: arr.uniq
来源：http://hz.yj202588.top/gthbrehbiu.html

C#:   list.Distinct().ToList()
来源：http://hz.dashuyun.cn/gtcbapgdod.html

[D16] 求和与平均值
来源：http://hz.gogol.net.cn/gtmnrvshnb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.hnqzz.top/gtfgzlrmaf.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.bjfxy.top/gtrgdablhm.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hnqzz.top/gtnnzbwiru.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.chenjidiqi.icu/gtlvqspdli.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.yueranfly.top/gtaypecuuq.html

Go:   // 手写循环累加
来源：http://hz.c1oappe.top/gtjcmtonrx.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.yvedp.cn/gthqqruras.html

C#:   list.Sum();  list.Average()
来源：http://hz.yvedp.cn/gtanabtytc.html

[D17] 最大值与最小值
来源：http://hz.tianlin.xyz/gtvvtuqgpf.html

Py:   max(arr);  min(arr)
来源：http://hz.zhaomingkeji.xyz/gtmnjatniy.html

PHP:  max($arr);  min($arr);
来源：http://hz.xuetiantiany.cn/gtifxjldoa.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.aibaodan.cn/gtaeaycjwz.html

TS:   Math.max(...arr);
来源：http://hz.chenzaomai.com/gtjeevegps.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.smart0.xyz/gtacqomnpv.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.c1oappe.top/gtcxrofrmt.html

Ruby: arr.max;  arr.min
来源：http://hz.jinqigufen.top/gtznerljal.html

C#:   list.Max();  list.Min()
来源：http://hz.ydzc1.top/gtydbhfyaw.html

[D18] 扁平化嵌套数组
来源：http://hz.gogol.net.cn/gtzsrkxcxy.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.yongpay.top/gtchvqxnlj.html

PHP:  array_merge(...$nested);
来源：http://hz.shanyushiyangtech.top/gtbpewghbr.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.c1oappe.top/gtztaoovcr.html

TS:   nested.flat();
来源：http://hz.svipenyu.cn/gtmuliagqa.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.tianlin.xyz/gtilyyjdqh.html

Go:   // 手写双层循环
来源：http://hz.jyoumei.cn/gtnodbgtpr.html

Ruby: nested.flatten
来源：http://hz.gotoacloud.top/gtneyzfujr.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.smart0.xyz/gtvlpxdhbl.html

[D19] 按字段分组
来源：http://hz.jiagoushi.top/gtbahigtvq.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.redwolf501.top/gtpxztqxau.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.jinghuilouyu.cn/gtwlrceddb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.yuanzhike.top/gtvhzqdxfn.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.cheryme.top/gtmtlxqvfw.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.wangshuangyany.cn/gtcviidsmk.html

Go:   // 手写 map[string][]T
来源：http://hz.xinyue.icu/gtpruukkzt.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.hammf.cn/gtevxinaty.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.pycfn.com/gteqgpywfm.html

[D20] 统计每个元素出现次数
来源：http://hz.iojbl.cn/gthpgjajls.html

Py:   Counter(arr)
来源：http://hz.bjfxy.top/gttbafnunp.html

PHP:  array_count_values($arr);
来源：http://hz.cdnleiting.top/gtkojcjwtl.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.shanyushiyangtech.top/gtpnxogcec.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hnxiangtu.top/gtmzoteufp.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.mhx1999.top/gtpfnhsrgr.html

Go:   // 手写 map[T]int
来源：http://hz.hywenlv.cn/gtlstpznsf.html

Ruby: arr.tally
来源：http://hz.snrcjt.cn/gtxkcmaxzk.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.guannengcc.top/gtynivjvbh.html

[D21] 判断是否包含某元素
来源：http://hz.jqgufenzy.top/gtmdmovaxx.html

Py:   x in arr
来源：http://hz.xziqi.cn/gtvrjadikk.html

PHP:  in_array($x, $arr, true);
来源：http://hz.316326.xyz/gthrvtarvw.html

JS:   arr.includes(x)
来源：http://hz.aibaodan.cn/gteqnmoeou.html

TS:   arr.includes(x)
来源：http://hz.fzhhl.top/gtfqqiihea.html

Java: list.contains(x)
来源：http://hz.yonumen.top/gtojfieeeq.html

Go:   slices.Contains(arr, x)
来源：http://hz.ydzc1.top/gtplipwbwm.html

Ruby: arr.include?(x)
来源：http://hz.xziqi.cn/gthiflfyus.html

C#:   list.Contains(x)
来源：http://hz.yuanzhike.top/gtmlplyjuk.html

[D22] 复制数组（避免共享引用）
来源：http://hz.birdmap.top/gtntfmmzjn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.yueranfly.top/gttvyfdmpd.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.shzxlz.cn/gtaeogjchj.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.chenlongwang.top/gttyjxmlqh.html

TS:   [...arr];
来源：http://hz.zdqjudy.top/gtkamblhlc.html

Java: new ArrayList<>(list);
来源：http://hz.xuetiantiany.cn/gtxisatiwd.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.mhx1999.top/gtqyuggyfs.html

Ruby: arr.dup;  arr.clone
来源：http://hz.zhijiandao.cn/gtyqbiylrh.html

C#:   new List<int>(list);
来源：http://hz.yueranfly.top/gtzvhqimfy.html

[D23] reduce 累积计算
来源：http://hz.tanke756.top/gtjgfrrkxe.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.hammf.cn/gtjzhwhfdn.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.yuanzhike.top/gtzvkovsel.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.wangshuangyany.cn/gtaavxunby.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yonumen.top/gthmiwyywu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.zhongyouzk.top/gtrkaicifn.html

Go:   // 手写循环
来源：http://hz.pycfn.com/gtiamllxsi.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.yj20258.top/gtplycwcuj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.ybcxt.top/gtdnbxtdut.html

[D24] 字典 / Map 基本操作
来源：http://hz.jinghuilouyu.cn/gtwpnpwggh.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.yongpay.top/gtbkisflly.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.feifeiyinyue.top/gtvdgdgtwx.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.hongshengwenyu.top/gtedjxgyty.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.yangfankeji.com/gtnxwatlpm.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.zhengqikj.top/gtskrwfvoq.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.dashuyun.cn/gtpvrnybdb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.haohaochexian.top/gtuyoyyoss.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.nanxuanxn.top/gturczbpyc.html

[D25] Set 集合去重与交并差
来源：http://hz.jianghu66.top/gtblkrxvid.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.shanyushiyangtech.top/gtzvnzmicg.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.chenzaomai.com/gtsivhwvcq.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.zdqjudy.top/gtvumqhxpk.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.guannengcc.top/gtavyfveag.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.redwolf501.top/gtfdpkvinp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.cqqwz.cn/gtchliktaf.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.ybcxt.top/gtuakmfxck.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.shzxlz.cn/gtuzuuaxot.html

[D26] 数组转字符串
来源：http://hz.andypj.xyz/gtweebjjkv.html

Py:   ", ".join(map(str, arr))
来源：http://hz.zhiwuduotai.top/gtrnvyjbhx.html

PHP:  implode(", ", $arr);
来源：http://hz.yongpay.top/gtgnizmtro.html

JS:   arr.join(", ")
来源：http://hz.yj20258.top/gtanapdfuh.html

TS:   arr.join(", ")
来源：http://hz.pengpengdd.cyou/gtdjkfmgia.html

Java: String.join(", ", list)
来源：http://hz.yj202588.top/gtctjqirmi.html

Go:   strings.Join(strs, ", ")
来源：http://hz.tian-w.cn/gtbbguccqr.html

Ruby: arr.join(", ")
来源：http://hz.c1oappe.top/gttdgiqfyg.html

C#:   string.Join(", ", list)
来源：http://hz.gaohongyu789.top/gtuljrlxei.html

================================================================================
来源：http://hz.tianlin.xyz/gtezanwqtx.html

E. 字符串处理
来源：http://hz.mhx1999.top/gtzocylxpw.html

================================================================================
来源：http://hz.jqgfzy.top/gtkbhhkfey.html

[E01] 拼接字符串
来源：http://hz.iojbl.cn/gtfbvrzevt.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.kuanghao11.cn/gttflqimmm.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.sufxvd.cn/gtzxaaqebk.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jinyuanbaomall.cn/gtmspwdibx.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.hnxiangtu.top/gtiaydlhhl.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.ivvv.top/gtfvyztlbl.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.jlsjyb.cn/gtqxblptxy.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.wangdashe.top/gtceosdjbw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.birdmap.top/gtsshubpma.html

[E02] 重复字符串
来源：http://hz.52xcode.cn/gtgwpxgfie.html

Py:   "ab" * 3
来源：http://hz.guannengcc.top/gtfvehindu.html

PHP:  str_repeat("ab", 3);
来源：http://hz.zhijiandao.cn/gtrpcesrol.html

JS:   "ab".repeat(3)
来源：http://hz.feifeiyinyue.top/gtdfxxtslm.html

TS:   "ab".repeat(3)
来源：http://hz.ppjwa.cn/gtluhlicee.html

Java: "ab".repeat(3)
来源：http://hz.zhongyouzk.top/gtpbmhthbq.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.pengpengdd.cyou/gtckzhmdzn.html

Ruby: "ab" * 3
来源：http://hz.wangshuangyany.cn/gtgchjlsbh.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.cheryme.top/gtrrxmvssm.html

[E03] 截取子串
来源：http://hz.cucudq.cn/gtbfbgiwin.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.yj202588.top/gtgsxncbjm.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.gaohongyu789.top/gtopgdnths.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.zhaomingkeji.xyz/gtybsionps.html

TS:   s.slice(1, 4)
来源：http://hz.zhengqikj.top/gtxflzljgp.html

Java: s.substring(1, 4)
来源：http://hz.pycfn.com/gtishkewwz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.zdqjudy.top/gtmttxrgyb.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.hammf.cn/gttrxovjjz.html

C#:   s.Substring(1, 3)
来源：http://hz.xingfuxueyuan.xyz/gtkrffbyif.html

[E04] 查找子串位置
来源：http://hz.yj20258888.top/gtndubfrfx.html

Py:   s.find("x");  s.index("x")
来源：http://hz.ehwqpu.com/gttfhcgnpj.html

PHP:  strpos($s, "x");
来源：http://hz.zhongyouzk.top/gtxjxytgiq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.zhongyouzk.top/gtmsmrhqxc.html

TS:   s.indexOf("x")
来源：http://hz.haohaochexian.top/gtcclvculm.html

Java: s.indexOf("x")
来源：http://hz.cqqwz.cn/gtnbbpoazi.html

Go:   strings.Index(s, "x")
来源：http://hz.hnqzz.top/gthovwujgb.html

Ruby: s.index("x")
来源：http://hz.chenlongwang.top/gtwapaoesp.html

C#:   s.IndexOf("x")
来源：http://hz.xylfe.cn/gtqnmnlvgj.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.guannengcc.top/gtsxjlmppy.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.wangdashe.top/gtmgzubpbq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.sweek.top/gtywediozt.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.52xcode.cn/gtmjylkctv.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.ywan-chungtsiang.top/gtydlycynt.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.bjfxy.top/gtbptyhrlx.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.chenjidiqi.icu/gtnfgcdjpj.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.jinqigufen.top/gtyjnrclag.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.ydzc1.top/gtxudnnqcq.html

[E06] 替换子串
来源：http://hz.guowangkeji.top/gtqgxyruze.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.chenlongwang.top/gtqgdwnfkh.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.shangyingyoupin.top/gtnlixgkke.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yonumen.top/gtdjmksakh.html

TS:   s.replaceAll("a", "b")
来源：http://hz.fzhhl.top/gtalbyaios.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.sysykeji.top/gtnomnpaoc.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.ybcxt.top/gtndwkbjus.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.ydjk.org.cn/gtuddzvhbo.html

C#:   s.Replace("a", "b")
来源：http://hz.xziqi.cn/gtezizwjix.html

[E07] 按分隔符拆分
来源：http://hz.ehwqpu.com/gtrmmtbreq.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.shanyushiyangtech.top/gtbhutbdya.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.smart0.xyz/gtzlmphpxn.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.ybcxt.top/gtolcfpypb.html

TS:   s.split(",")
来源：http://hz.316326.xyz/gtczhtrgjc.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.daria6918.cn/gtheeiaxad.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.svipenyu.cn/gtsyjgiyeu.html

Ruby: s.split(",");  s.split
来源：http://hz.fzhhl.top/gtxkbynebs.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.jinqigfzy.top/gttohgsfrx.html

[E08] 数组按分隔符合并
来源：http://hz.yonumen.top/gtwefiyyjo.html

Py:   ",".join(items)
来源：http://hz.hongshengwenyu.top/gtunjjpjyo.html

PHP:  implode(",", $items);
来源：http://hz.redwolf501.top/gtzxdjbcaj.html

JS:   items.join(",")
来源：http://hz.jinghuilouyu.cn/gtotwxxjjm.html

TS:   items.join(",")
来源：http://hz.gzhubu.top/gtpdstfhio.html

Java: String.join(",", items)
来源：http://hz.xuanzx.com/gtdodxrpct.html

Go:   strings.Join(items, ",")
来源：http://hz.yangfankeji.com/gtrphvzmnb.html

Ruby: items.join(",")
来源：http://hz.xuetiantiany.cn/gthligenon.html

C#:   string.Join(",", items)
来源：http://hz.ivvv.top/gtblzvviul.html

[E09] 去除所有空白字符
来源：http://hz.ydjk.org.cn/gtolnueqnm.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.ehwqpu.com/gtncpzkvhw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.birdmap.top/gtpxyxeyau.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.birdmap.top/gtrkdzjcoi.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.zycfv.cn/gtgxnisxyt.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.chenlongwang.top/gtkwcqpexc.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.xingfuxueyuan.xyz/gtaipdbyxi.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.52xcode.cn/gtpqtxagcv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.jqgufenzy.top/gtbmfjibrn.html

[E10] 左侧补零 / 定长填充
来源：http://hz.xuetiantiany.cn/gtnjgjiqrf.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.nanxinkj.top/gtvjhtcqgs.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.ybcxt.top/gtoymwldts.html

JS:   "7".padStart(3, "0")
来源：http://hz.tian-w.cn/gtprmyiaae.html

TS:   "7".padStart(3, "0")
来源：http://hz.zhengqikj.top/gttnkaysvf.html

Java: String.format("%03d", 7)
来源：http://hz.guannengcc.top/gtcjzdjysr.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.svipenyu.cn/gthpcgvyjc.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.tianlin.xyz/gtkscgtwyv.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.feifeiyinyue.top/gthnjazvmf.html

[E11] 反转字符串
来源：http://hz.ywan-chungtsiang.top/gtgnfemdin.html

Py:   s[::-1]
来源：http://hz.xinyue.icu/gtuslflyfe.html

PHP:  strrev($s);
来源：http://hz.tanke756.top/gtemjobuxc.html

JS:   [...s].reverse().join("")
来源：http://hz.yueranfly.top/gtafqnyias.html

TS:   [...s].reverse().join("")
来源：http://hz.chenjidiqi.icu/gtbgglazkg.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.jqgufenzy.top/gtegzhbaev.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.hnqzz.top/gtutinhiby.html

Ruby: s.reverse
来源：http://hz.guannengcc.top/gtqmwjzrki.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.sxryk.cn/gtmeirreux.html

[E12] 统计某字符出现次数
来源：http://hz.aibaodan.cn/gtwnlenfzr.html

Py:   s.count("a")
来源：http://hz.kuanghao11.cn/gtxddsmlec.html

PHP:  substr_count($s, "a");
来源：http://hz.daria6918.cn/gtcfbvqlll.html

JS:   s.split("a").length - 1
来源：http://hz.tian-w.cn/gtcldizmcu.html

TS:   s.split("a").length - 1
来源：http://hz.fengsongda.top/gtmjpyigdl.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.hysaishi.cn/gtzbirjgxc.html

Go:   strings.Count(s, "a")
来源：http://hz.yj20258888.top/gthmgcbals.html

Ruby: s.count("a")
来源：http://hz.sxryk.cn/gtmvtywhhs.html

C#:   s.Count(c => c == 'a')
来源：http://hz.shanyushiyangtech.top/gthzypoydb.html

[E13] 逐字符遍历
来源：http://hz.shanyushiyangtech.top/gtrmvjbcwm.html


<!-- 参考信息 -->