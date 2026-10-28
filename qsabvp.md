代发 wailian999

Java: list.size();
来源：http://hz.wangshuangyany.cn/gtgetgzjli.html

Go:   len(arr)
来源：http://hz.ydjk.org.cn/gtrgtnkbjj.html

Ruby: arr.length; arr.size
来源：http://hz.yanxiufei.cn/gtirqkcbye.html

C#:   list.Count;
来源：http://hz.cheryme.top/gtzvebiyra.html

[D07] 切片 / 取子数组
来源：http://hz.quarkkingdee.top/gtbbumzqxp.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.bjfxy.top/gtujwyngad.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.shanyushiyangkeji.top/gtbidyhwcm.html

JS:   arr.slice(1, 4);
来源：http://hz.daria6918.cn/gtnabkaapj.html

TS:   arr.slice(1, 4);
来源：http://hz.gotoacloud.top/gtkoxyiveq.html

Java: list.subList(1, 4);
来源：http://hz.xziqi.cn/gtdxyfjsgh.html

Go:   arr[1:4]
来源：http://hz.havefunace.top/gteamwfjps.html

Ruby: arr[1, 3]
来源：http://hz.daxiang520.top/gtpskudnbi.html

C#:   list.GetRange(1, 3);
来源：http://hz.gotoacloud.top/gtldbslwaw.html

[D08] 合并两个数组
来源：http://hz.jlsjyb.cn/gtlylybtgs.html

Py:   a + b;  a.extend(b)
来源：http://hz.zhongyouzk.top/gtrmpakuad.html

PHP:  array_merge($a, $b);
来源：http://hz.zdqjudy.top/gtxulfxmfc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.sweek.top/gtovpsyfdm.html

TS:   [...a, ...b];
来源：http://hz.yvedp.cn/gtkkedmsuy.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.xingfuxueyuan.xyz/gttwhiooer.html

Go:   append(a, b...)
来源：http://hz.chenlongwang.top/gtuzryrshp.html

Ruby: a + b;  a.concat(b)
来源：http://hz.iojbl.cn/gtwnbyhwuy.html

C#:   a.Concat(b).ToList()
来源：http://hz.nwbrower.top/gthmacvtzd.html

[D09] 排序（升序）
来源：http://hz.cucudq.cn/gtkiclntcm.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.wangshuangyany.cn/gthcipqsji.html

PHP:  sort($arr);
来源：http://hz.birdmap.top/gtcyfqkjlb.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.jqgufenzy.top/gtmgaubghe.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.ivvv.top/gtzrztzboe.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.xinyue.icu/gthwbwgxrl.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.zhaomingkeji.xyz/gtlcvwuzaa.html

Ruby: arr.sort
来源：http://hz.yuanzhike.top/gtsxxpkzbw.html

C#:   list.Sort();
来源：http://hz.ehwqpu.com/gtcgwbcezk.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.9152youxi.cn/gtisbeitcp.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.zdqjudy.top/gtikvwragm.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.andypj.xyz/gtxytdfloq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xuanzx.com/gtqgeksaxo.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.tianlin.xyz/gtftyirtqb.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.xingfuxueyuan.xyz/gtpdtzvujd.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.cheryme.top/gtoobpmesb.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.9152youxi.cn/gtrbandlca.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.shanyushiyangtech.top/gtvklzbazh.html

[D11] 反转数组
来源：http://hz.shanyushiyangkeji.top/gtahwslequ.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.yvedp.cn/gtwmthjqjc.html

PHP:  array_reverse($arr);
来源：http://hz.wangdashe.top/gtjzdhvnun.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.fengsongda.top/gtgdimkkeu.html

TS:   [...arr].reverse();
来源：http://hz.shanyushiyangkeji.top/gtkxjoubzt.html

Java: Collections.reverse(list);
来源：http://hz.zhaomingkeji.xyz/gteohhubqf.html

Go:   slices.Reverse(arr)
来源：http://hz.yangfankeji.com/gtptstkmsw.html

Ruby: arr.reverse
来源：http://hz.yonumen.top/gtvqdezjjv.html

C#:   list.Reverse();
来源：http://hz.zhengqikj.top/gtsecronro.html

[D12] 查找元素下标
来源：http://hz.gotoacloud.top/gtrrhsjvqf.html

Py:   arr.index(x);  x in arr
来源：http://hz.svipenyu.cn/gthqbxycdj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.snrcjt.cn/gthbxlmksx.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.xylfe.cn/gtklrlokad.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.xinyue.icu/gtbwjehvmf.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.zhixingplan.top/gthencdqdv.html

Go:   slices.Index(arr, x)
来源：http://hz.meibo888.top/gtplwuggsl.html

Ruby: arr.index(x)
来源：http://hz.sweek.top/gtjczcyqhn.html

C#:   list.IndexOf(x);
来源：http://hz.shzxlz.cn/gtmjnatdkk.html

[D13] 过滤（保留满足条件的）
来源：http://hz.yj20258.top/gtukgionln.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.andypj.xyz/gtpggbzxcz.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.hysaishi.cn/gtshvjjkja.html

JS:   arr.filter(x => x > 3)
来源：http://hz.jianghu66.top/gtbxyebpld.html

TS:   arr.filter(x => x > 3)
来源：http://hz.wangdashe.top/gtcszqvrud.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.xuetiantiany.cn/gtwwhqgjxw.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.andypj.xyz/gtgktsolxa.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.pycfn.com/gtcbumowma.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.cdnleiting.top/gtduwuybzu.html

[D14] 映射转换（每个元素变形）
来源：http://hz.jqgfzy.top/gtnvoosgrm.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.hywenlv.cn/gtknzznjov.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.gotoacloud.top/gtglscnpky.html

JS:   arr.map(x => x * 2)
来源：http://hz.andypj.xyz/gtgramhupz.html

TS:   arr.map(x => x * 2)
来源：http://hz.svipenyu.cn/gtycddwfra.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.daria6918.cn/gtrjvnkdob.html

Go:   // 手写循环
来源：http://hz.jyoumei.cn/gtoqigtcpw.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.feifeiyinyue.top/gtzavhiruf.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.cdnleiting.top/gtocuuhgnb.html

[D15] 去重
来源：http://hz.pycfn.com/gtjqjjruvj.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.zdqjudy.top/gtwbjtmxtv.html

PHP:  array_unique($arr);
来源：http://hz.guannengcc.top/gtzuryvccw.html

JS:   [...new Set(arr)]
来源：http://hz.ydjk.org.cn/gtsovmtfxy.html

TS:   [...new Set(arr)]
来源：http://hz.cucudq.cn/gtocpyknkt.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.cucudq.cn/gtvmstlybe.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.smart0.xyz/gtcwmphiji.html

Ruby: arr.uniq
来源：http://hz.yj20258.top/gttsuqzomu.html

C#:   list.Distinct().ToList()
来源：http://hz.yangfankeji.com/gtspxedqdy.html

[D16] 求和与平均值
来源：http://hz.aibaodan.cn/gtwzctqgwp.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.hammf.cn/gtheoxdxnp.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.tanke756.top/gtlrgyutxi.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yonumen.top/gtjfcakjoa.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zdqjudy.top/gtdxinxxfo.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.xingfuxueyuan.xyz/gtbuytlmvr.html

Go:   // 手写循环累加
来源：http://hz.chenzaomai.com/gtaseucniy.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.cqqwz.cn/gtksurakbq.html

C#:   list.Sum();  list.Average()
来源：http://hz.kuanghao11.cn/gtgrzdqtoo.html

[D17] 最大值与最小值
来源：http://hz.shuidangran.top/gtbdufwkpo.html

Py:   max(arr);  min(arr)
来源：http://hz.redwolf501.top/gtswqzpwtk.html

PHP:  max($arr);  min($arr);
来源：http://hz.meibo888.top/gtiwusvbmf.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.bjfxy.top/gtdokcsfpg.html

TS:   Math.max(...arr);
来源：http://hz.jlsjyb.cn/gtgialfxoh.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.jqgfzy.top/gtqhcnoqnu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.daxiang520.top/gtomblfzmk.html

Ruby: arr.max;  arr.min
来源：http://hz.gogol.net.cn/gtkwccukny.html

C#:   list.Max();  list.Min()
来源：http://hz.316326.xyz/gtonhjbmbq.html

[D18] 扁平化嵌套数组
来源：http://hz.shangyingyoupin.top/gtvnwrokwk.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.zhiwuduotai.top/gttnewplmj.html

PHP:  array_merge(...$nested);
来源：http://hz.xziqi.cn/gttjacdgmb.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.andypj.xyz/gtnfucsmzq.html

TS:   nested.flat();
来源：http://hz.xinyue.icu/gtqlusycyb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.birdmap.top/gtmlahdhtz.html

Go:   // 手写双层循环
来源：http://hz.gotoacloud.top/gtotslrggz.html

Ruby: nested.flatten
来源：http://hz.xuanzx.com/gtofxnjsix.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.dashuyun.cn/gtaewfzpcs.html

[D19] 按字段分组
来源：http://hz.yonumen.top/gtfthhkfbj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.hywenlv.cn/gtpoctflpp.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.xylfe.cn/gtjgvhwhzw.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.hysaishi.cn/gtknibtmwy.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.wangshuangyany.cn/gtkqhrcave.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.smart0.xyz/gttbzdsgza.html

Go:   // 手写 map[string][]T
来源：http://hz.ivvv.top/gtjkaxtmlq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.snrcjt.cn/gtqzvqasav.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.mhx1999.top/gtzieefeoc.html

[D20] 统计每个元素出现次数
来源：http://hz.0kj1m.cn/gtpcnbzmmo.html

Py:   Counter(arr)
来源：http://hz.yuxming.cn/gtydpobvxs.html

PHP:  array_count_values($arr);
来源：http://hz.zycfv.cn/gtemwhrfkd.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.wangdashe.top/gtrtotatck.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.shzxlz.cn/gtuzvltcbv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.cucudq.cn/gtanamyobt.html

Go:   // 手写 map[T]int
来源：http://hz.iojbl.cn/gtwvmnpjeu.html

Ruby: arr.tally
来源：http://hz.xziqi.cn/gtnoqhujas.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.hysaishi.cn/gttzqwzemf.html

[D21] 判断是否包含某元素
来源：http://hz.ivvv.top/gtwmvvreih.html

Py:   x in arr
来源：http://hz.vqdsnc.cn/gtjlsjogfb.html

PHP:  in_array($x, $arr, true);
来源：http://hz.fengsongda.top/gtjkrooeta.html

JS:   arr.includes(x)
来源：http://hz.gogol.net.cn/gtkgqqrsxz.html

TS:   arr.includes(x)
来源：http://hz.pengpengdd.cyou/gtimvvtyni.html

Java: list.contains(x)
来源：http://hz.bjfxy.top/gtdrtngidl.html

Go:   slices.Contains(arr, x)
来源：http://hz.yj20258.top/gtzpdylovl.html

Ruby: arr.include?(x)
来源：http://hz.kuanghao11.cn/gtmipvljzp.html

C#:   list.Contains(x)
来源：http://hz.tianlin.xyz/gtngguhezz.html

[D22] 复制数组（避免共享引用）
来源：http://hz.shanyushiyangtech.top/gtmbmmqprd.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.xziqi.cn/gtawwcrpnv.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.jinqigfzy.top/gtixtmdkay.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.cheryme.top/gtjhgrjjhj.html

TS:   [...arr];
来源：http://hz.birdmap.top/gtzdtjujos.html

Java: new ArrayList<>(list);
来源：http://hz.xziqi.cn/gtbpvsjhit.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.yj20258888.top/gtqbjyxmpc.html

Ruby: arr.dup;  arr.clone
来源：http://hz.jinqigfzy.top/gtfigexnvj.html

C#:   new List<int>(list);
来源：http://hz.sysykeji.top/gtguymteoo.html

[D23] reduce 累积计算
来源：http://hz.quarkkingdee.top/gtxjwuvnvp.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.jianghu66.top/gtapunhxgh.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.xuetiantiany.cn/gtjpxbuhtz.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.snrcjt.cn/gtfblbvshq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.shuidangran.top/gtyxrersce.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.quarkkingdee.top/gtqfhhhdlx.html

Go:   // 手写循环
来源：http://hz.chenjidiqi.icu/gtakvepcln.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.hongshengwenyu.top/gtrdmlzewq.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.zhengqikj.top/gtnuuifsei.html

[D24] 字典 / Map 基本操作
来源：http://hz.chenlongwang.top/gtliwzdnfl.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.fengsongda.top/gtwqgkcjxd.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.fzhhl.top/gtwfelygkg.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.nanxinkj.top/gtfvgssxue.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.tian-w.cn/gtjqyjemjj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.guannengcc.top/gthjrzdlqq.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.wangdashe.top/gtktyiqdex.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.haohaochexian.top/gtlnbzshta.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.guowangkeji.top/gtqfsypjku.html

[D25] Set 集合去重与交并差
来源：http://hz.jqgufenzy.top/gtsspxlwxm.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.daria6918.cn/gtzglmcqfl.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.hnxiangtu.top/gtskowqour.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.daxiang520.top/gtjazlknfh.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.cqqwz.cn/gthzjodzny.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.jianghu66.top/gtazhzybio.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.smart0.xyz/gthrdxyvxh.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.sxryk.cn/gtvvmctkbf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.redwolf501.top/gteonusxxn.html

[D26] 数组转字符串
来源：http://hz.hnqzz.top/gtgxeemlor.html

Py:   ", ".join(map(str, arr))
来源：http://hz.hnxiangtu.top/gtkmtuwxgd.html

PHP:  implode(", ", $arr);
来源：http://hz.daxiang520.top/gtpvwhmwts.html

JS:   arr.join(", ")
来源：http://hz.daria6918.cn/gtonwkkjns.html

TS:   arr.join(", ")
来源：http://hz.gotoacloud.top/gtvcsexnym.html

Java: String.join(", ", list)
来源：http://hz.zhaomingkeji.xyz/gteyonphha.html

Go:   strings.Join(strs, ", ")
来源：http://hz.vqdsnc.cn/gtedbcpwiy.html

Ruby: arr.join(", ")
来源：http://hz.c1oappe.top/gtaggeyumz.html

C#:   string.Join(", ", list)
来源：http://hz.hysaishi.cn/gtgjwbuszk.html

================================================================================
来源：http://hz.yvedp.cn/gtfouhbtpg.html

E. 字符串处理
来源：http://hz.guannengcc.top/gtwrnatakb.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtsqxunddp.html

[E01] 拼接字符串
来源：http://hz.ivvv.top/gtmsudfdab.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.birdmap.top/gtwrwyxzfc.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.ydjk.org.cn/gtkbwinfte.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.bjfxy.top/gtndjyoheb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.birdmap.top/gtjarstlzh.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.redwolf501.top/gtbqtvulib.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.yueranfly.top/gtprinvoiu.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.daxiang520.top/gtautfzyrl.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.hysaishi.cn/gthftirqsm.html

[E02] 重复字符串
来源：http://hz.gogol.net.cn/gtvkaajjgl.html

Py:   "ab" * 3
来源：http://hz.yuxming.cn/gtxrdpdkrj.html

PHP:  str_repeat("ab", 3);
来源：http://hz.ybcxt.top/gtjimxrdtw.html

JS:   "ab".repeat(3)
来源：http://hz.0kj1m.cn/gtrkvswpth.html

TS:   "ab".repeat(3)
来源：http://hz.gzhubu.top/gtrjgmgchy.html

Java: "ab".repeat(3)
来源：http://hz.cheryme.top/gtvnrddbjp.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.guannengcc.top/gtnmuqwdrm.html

Ruby: "ab" * 3
来源：http://hz.hammf.cn/gtnmgvfckb.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.andypj.xyz/gtkaqpssym.html

[E03] 截取子串
来源：http://hz.zhaomingkeji.xyz/gtfikgcgss.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.jqgfzy.top/gtholjhalw.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.guannengcc.top/gtrgnaqkui.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.yj202588.top/gtpiincmfo.html

TS:   s.slice(1, 4)
来源：http://hz.hnxiangtu.top/gtbdxlzbmn.html

Java: s.substring(1, 4)
来源：http://hz.shanyushiyangtech.top/gtwozhlrbw.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.sweek.top/gtcqhgjanj.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.c1oappe.top/gtmmunsomg.html

C#:   s.Substring(1, 3)
来源：http://hz.xylfe.cn/gtugwznpdn.html

[E04] 查找子串位置
来源：http://hz.ivvv.top/gtgwavfvcl.html

Py:   s.find("x");  s.index("x")
来源：http://hz.gogol.net.cn/gtdhdrmtzv.html

PHP:  strpos($s, "x");
来源：http://hz.snrcjt.cn/gtrzztqlzs.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.xingfuxueyuan.xyz/gtbccvggbh.html

TS:   s.indexOf("x")
来源：http://hz.vqdsnc.cn/gteujcnlll.html

Java: s.indexOf("x")
来源：http://hz.gzhubu.top/gtmilmldzx.html

Go:   strings.Index(s, "x")
来源：http://hz.316326.xyz/gtcnsrzhbo.html

Ruby: s.index("x")
来源：http://hz.chenjidiqi.icu/gtiunzzyqy.html

C#:   s.IndexOf("x")
来源：http://hz.cdnleiting.top/gtwbihuyng.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.wangshuangyany.cn/gtlqfnluux.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.gogol.net.cn/gttjfbxlgn.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.chenzaomai.com/gtbztakcrz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.shzxlz.cn/gtlanzcrqt.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.wangdashe.top/gtlwgxvaer.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.sufxvd.cn/gtxjwyolis.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.jlsjyb.cn/gteomfxair.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.sxryk.cn/gteywuhrji.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.vqdsnc.cn/gtkxlnwtgl.html

[E06] 替换子串
来源：http://hz.birdmap.top/gtnbdemyfv.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.tian-w.cn/gtwipbolmj.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.guowangkeji.top/gttukommpk.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jyoumei.cn/gtferghlpt.html

TS:   s.replaceAll("a", "b")
来源：http://hz.gotoacloud.top/gtmocgchyb.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.iojbl.cn/gtquqwuwts.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.dashuyun.cn/gtanuixcie.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.wangshuangyany.cn/gtvzbxfvom.html

C#:   s.Replace("a", "b")
来源：http://hz.dianchejie.cn/gtniblzeez.html

[E07] 按分隔符拆分
来源：http://hz.cheryme.top/gtxmtfdndx.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.yanxiufei.cn/gtjznfmvig.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.andypj.xyz/gtmfsvkxyn.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.zhiwuduotai.top/gttmprsqgi.html

TS:   s.split(",")
来源：http://hz.xuanzx.com/gtfhpopput.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.fengsongda.top/gttglddzyb.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.shanyushiyangtech.top/gtwcawrnrp.html

Ruby: s.split(",");  s.split
来源：http://hz.pycfn.com/gttbjrfdfu.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.sweek.top/gtqlqyhprr.html

[E08] 数组按分隔符合并
来源：http://hz.chenjidiqi.icu/gtxssjeezu.html

Py:   ",".join(items)
来源：http://hz.haohaochexian.top/gtdebfxhnz.html

PHP:  implode(",", $items);
来源：http://hz.daxiang520.top/gtxujoiwcl.html

JS:   items.join(",")
来源：http://hz.ivvv.top/gtxjludcbz.html

TS:   items.join(",")
来源：http://hz.havefunace.top/gtlkiztdaa.html

Java: String.join(",", items)
来源：http://hz.ybcxt.top/gtsormeuvs.html

Go:   strings.Join(items, ",")
来源：http://hz.yj20258.top/gtrifnnqbj.html

Ruby: items.join(",")
来源：http://hz.zhijiandao.cn/gtogybpxva.html

C#:   string.Join(",", items)
来源：http://hz.sufxvd.cn/gthqjzgrzq.html

[E09] 去除所有空白字符
来源：http://hz.havefunace.top/gtpehjqjxq.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.zhongyouzk.top/gtrhhibhxv.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.ywan-chungtsiang.top/gtncrmrjte.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.jqgfzy.top/gtnjbmxvpn.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.nwbrower.top/gtpxsomaae.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.bjfxy.top/gtqnqpvcis.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.ehwqpu.com/gtgviinghv.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.gogol.net.cn/gtnozvcodv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.aizwys.cn/gtgtlavjml.html

[E10] 左侧补零 / 定长填充
来源：http://hz.nanxuanxn.top/gtamkdqtuc.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.xziqi.cn/gtpxtzbqdy.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.snrcjt.cn/gtjqodnnnl.html

JS:   "7".padStart(3, "0")
来源：http://hz.zhixingplan.top/gtpmmeldrm.html

TS:   "7".padStart(3, "0")
来源：http://hz.52xcode.cn/gtvvqbpdfp.html

Java: String.format("%03d", 7)
来源：http://hz.daxiang520.top/gthjuhcila.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.jiagoushi.top/gtatwocnnj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.yj202588.top/gtdipymgow.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.sysykeji.top/gtmffpydpx.html

[E11] 反转字符串
来源：http://hz.shanyushiyangkeji.top/gtgipktngn.html

Py:   s[::-1]
来源：http://hz.quarkkingdee.top/gtrcbmteky.html

PHP:  strrev($s);
来源：http://hz.sufxvd.cn/gthirztecy.html

JS:   [...s].reverse().join("")
来源：http://hz.xziqi.cn/gtyncypepm.html

TS:   [...s].reverse().join("")
来源：http://hz.9152youxi.cn/gthqgfnptb.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.meibo888.top/gttgmbwpjw.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.jiagoushi.top/gthvxuywuw.html

Ruby: s.reverse
来源：http://hz.jqgufenzy.top/gtdareeeeq.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.cheryme.top/gttwxgkxpl.html

[E12] 统计某字符出现次数
来源：http://hz.yanxiufei.cn/gtkyegtvld.html

Py:   s.count("a")
来源：http://hz.xinyue.icu/gtplfgwtqt.html

PHP:  substr_count($s, "a");
来源：http://hz.cqqwz.cn/gthyrwggrw.html

JS:   s.split("a").length - 1
来源：http://hz.zhiwuduotai.top/gtrjjlozzi.html

TS:   s.split("a").length - 1
来源：http://hz.daxiang520.top/gtusylulrr.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.shuidangran.top/gtemmptgni.html

Go:   strings.Count(s, "a")
来源：http://hz.jinqigfzy.top/gthxdbgwna.html

Ruby: s.count("a")
来源：http://hz.cheryme.top/gtvuswzhic.html

C#:   s.Count(c => c == 'a')
来源：http://hz.yvedp.cn/gtmvkxmmes.html

[E13] 逐字符遍历
来源：http://hz.c1oappe.top/gtexsvsoke.html

Py:   for ch in s: print(ch)
来源：http://hz.wangshuangyany.cn/gtdaxdslun.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.nanxinkj.top/gtxpjhtafa.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yuxming.cn/gtbkvksnxc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yonumen.top/gtpgalnjih.html


<!-- 参考信息 -->