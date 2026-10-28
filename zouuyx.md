代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.yonumen.top/gtyzwjcxkr.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.ppjwa.cn/gtfygjiafw.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.wangdashe.top/gtrmyonewt.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.fengsongda.top/gthxfngnar.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.gogol.net.cn/gtrzmatjht.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.chenlongwang.top/gtqsrrojlp.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.hnxiangtu.top/gtnrwzehux.html

[D06] 数组长度
来源：http://hz.birdmap.top/gtjopofqrz.html

Py:   len(arr)
来源：http://hz.shuidangran.top/gtvxcmdwia.html

PHP:  count($arr);
来源：http://hz.sweek.top/gtaqrkgmvo.html

JS:   arr.length
来源：http://hz.birdmap.top/gtwfkrrhwb.html

TS:   arr.length
来源：http://hz.xinyue.icu/gtagjmnyrs.html

Java: list.size();
来源：http://hz.pycfn.com/gtwxaietoh.html

Go:   len(arr)
来源：http://hz.xuanzx.com/gtrjsumcqy.html

Ruby: arr.length; arr.size
来源：http://hz.cheryme.top/gtbkscgjir.html

C#:   list.Count;
来源：http://hz.yvedp.cn/gtdedpfzam.html

[D07] 切片 / 取子数组
来源：http://hz.hfpthk.cn/gtwaemgmxn.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.zycfv.cn/gtqlfzxlcp.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.yj20258.top/gtflykxaqs.html

JS:   arr.slice(1, 4);
来源：http://hz.pengpengdd.cyou/gtasoqmnzq.html

TS:   arr.slice(1, 4);
来源：http://hz.jianghu66.top/gtyvtbuuxw.html

Java: list.subList(1, 4);
来源：http://hz.aibaodan.cn/gtqlzxivgk.html

Go:   arr[1:4]
来源：http://hz.yonumen.top/gtdxhnggnv.html

Ruby: arr[1, 3]
来源：http://hz.haohaochexian.top/gtzngndgql.html

C#:   list.GetRange(1, 3);
来源：http://hz.hongshengwenyu.top/gtkkkexwfp.html

[D08] 合并两个数组
来源：http://hz.cdnleiting.top/gtzjpiruaq.html

Py:   a + b;  a.extend(b)
来源：http://hz.yj202588.top/gtqorfqwcw.html

PHP:  array_merge($a, $b);
来源：http://hz.jinqigufen.top/gtjlyqcnzl.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.snrcjt.cn/gtdnqqrkmi.html

TS:   [...a, ...b];
来源：http://hz.yongpay.top/gtxrnrijcc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.ydjk.org.cn/gtkxavurni.html

Go:   append(a, b...)
来源：http://hz.meibo888.top/gtcvukkhis.html

Ruby: a + b;  a.concat(b)
来源：http://hz.hywenlv.cn/gtyxrgpcjw.html

C#:   a.Concat(b).ToList()
来源：http://hz.cucudq.cn/gtnyxboahp.html

[D09] 排序（升序）
来源：http://hz.gotoacloud.top/gterhxnzmp.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.iojbl.cn/gtqpoahmlh.html

PHP:  sort($arr);
来源：http://hz.c1oappe.top/gtmsiahlkp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.316326.xyz/gtddtzvbtk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.cqqwz.cn/gtizpklchv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.zycfv.cn/gtypiojuzy.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.mhx1999.top/gtbkruuoxx.html

Ruby: arr.sort
来源：http://hz.xuetiantiany.cn/gtcwfmftgt.html

C#:   list.Sort();
来源：http://hz.jyoumei.cn/gtzltlasjp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.havefunace.top/gtfagjewpd.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.vqdsnc.cn/gtnvrxmbgi.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yangfankeji.com/gtafytesul.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.ppjwa.cn/gtkhlhwpii.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hfpthk.cn/gtyfodwkkd.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.xuanzx.com/gthjfrbzue.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.yuxming.cn/gtarutjteq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.316326.xyz/gtwuijgcbo.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.jiagoushi.top/gtoqvfbqoa.html

[D11] 反转数组
来源：http://hz.meibo888.top/gtpazvktqm.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.xylfe.cn/gtzgvxirsv.html

PHP:  array_reverse($arr);
来源：http://hz.guannengcc.top/gtoemdfmzl.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.chenlongwang.top/gtamqqcnaj.html

TS:   [...arr].reverse();
来源：http://hz.chenzaomai.com/gtgtwzesii.html

Java: Collections.reverse(list);
来源：http://hz.ehwqpu.com/gtnsheozia.html

Go:   slices.Reverse(arr)
来源：http://hz.nanxuanxn.top/gtvlyujsla.html

Ruby: arr.reverse
来源：http://hz.ehwqpu.com/gtsnipqmtv.html

C#:   list.Reverse();
来源：http://hz.yvedp.cn/gthnsaqgte.html

[D12] 查找元素下标
来源：http://hz.gaohongyu789.top/gtlfgxuxyb.html

Py:   arr.index(x);  x in arr
来源：http://hz.hfpthk.cn/gthoatlwts.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.aibaodan.cn/gtzktvvuxt.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.shanyushiyangkeji.top/gtqtnkkehk.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zhongyouzk.top/gtngdzfrtl.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.tianlin.xyz/gtvdmkbvjk.html

Go:   slices.Index(arr, x)
来源：http://hz.aizwys.cn/gtvyymkjap.html

Ruby: arr.index(x)
来源：http://hz.cashguo.top/gtyhsqnqox.html

C#:   list.IndexOf(x);
来源：http://hz.yj20258888.top/gtatxxdbhb.html

[D13] 过滤（保留满足条件的）
来源：http://hz.sufxvd.cn/gtwcdazrnj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.yj202588.top/gteabwxdxw.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.shzxlz.cn/gtbsmhiolt.html

JS:   arr.filter(x => x > 3)
来源：http://hz.shangyingyoupin.top/gtrmhatvit.html

TS:   arr.filter(x => x > 3)
来源：http://hz.gotoacloud.top/gtpeyuzflx.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.ydzc1.top/gtmrewrxtb.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.dashuyun.cn/gtokikswco.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.zdqjudy.top/gtolbmhffx.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.cqqwz.cn/gtuyeopuki.html

[D14] 映射转换（每个元素变形）
来源：http://hz.gaohongyu789.top/gtnlmiaxpo.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.jlsjyb.cn/gtnankiugc.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.52xcode.cn/gtdmuastgo.html

JS:   arr.map(x => x * 2)
来源：http://hz.zhijiandao.cn/gtmpfgoras.html

TS:   arr.map(x => x * 2)
来源：http://hz.haohaochexian.top/gtvgwcfcat.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.yanxiufei.cn/gtovxduozg.html

Go:   // 手写循环
来源：http://hz.tanke756.top/gtkmpqrlai.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.c1oappe.top/gtgmufvlay.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.jinyuanbaomall.cn/gthrrajgll.html

[D15] 去重
来源：http://hz.nwbrower.top/gtxqjertkk.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.hysaishi.cn/gtrmcgstmf.html

PHP:  array_unique($arr);
来源：http://hz.yonumen.top/gtazhwczrm.html

JS:   [...new Set(arr)]
来源：http://hz.cashguo.top/gtcksgrhke.html

TS:   [...new Set(arr)]
来源：http://hz.svipenyu.cn/gtvslotnrv.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.yj202588.top/gthckkgoza.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.redwolf501.top/gtghqbemww.html

Ruby: arr.uniq
来源：http://hz.shanyushiyangkeji.top/gtfjqsjwvi.html

C#:   list.Distinct().ToList()
来源：http://hz.316326.xyz/gtgsvgxwai.html

[D16] 求和与平均值
来源：http://hz.jqgufenzy.top/gtbaoffmal.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.smart0.xyz/gtxmxhdktv.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.yanxiufei.cn/gtqullytku.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.meibo888.top/gtthjigciv.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.pycfn.com/gtjdvzcfdm.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.ppjwa.cn/gtqedgnnzf.html

Go:   // 手写循环累加
来源：http://hz.gaohongyu789.top/gtyvweiqpk.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.zhengqikj.top/gtholfrxxr.html

C#:   list.Sum();  list.Average()
来源：http://hz.zhoulong.xyz/gtrtbtmaal.html

[D17] 最大值与最小值
来源：http://hz.sxryk.cn/gtawpgqgje.html

Py:   max(arr);  min(arr)
来源：http://hz.nanxuanxn.top/gtumurdgaq.html

PHP:  max($arr);  min($arr);
来源：http://hz.tanke756.top/gtdfjlopce.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.hfpthk.cn/gtelzzgnpg.html

TS:   Math.max(...arr);
来源：http://hz.zhengqikj.top/gtxcgwcqiq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.svipenyu.cn/gtcyleyciu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.chenzaomai.com/gtyzdffnxy.html

Ruby: arr.max;  arr.min
来源：http://hz.wangdashe.top/gtxrasxahu.html

C#:   list.Max();  list.Min()
来源：http://hz.jqgfzy.top/gthcyuywip.html

[D18] 扁平化嵌套数组
来源：http://hz.sysykeji.top/gttqmpmhvu.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.yj20258.top/gtvjujpnkc.html

PHP:  array_merge(...$nested);
来源：http://hz.yangfankeji.com/gtcnavmhvh.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.bjfxy.top/gtaejwxgqv.html

TS:   nested.flat();
来源：http://hz.xziqi.cn/gtjcfygtcq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.sweek.top/gtfveksflm.html

Go:   // 手写双层循环
来源：http://hz.jinghuilouyu.cn/gtegbdoshx.html

Ruby: nested.flatten
来源：http://hz.feifeiyinyue.top/gtuhrmpfqf.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.iojbl.cn/gtobhruwbf.html

[D19] 按字段分组
来源：http://hz.nanxuanxn.top/gtwtinxymb.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.chenjidiqi.icu/gtyqwivtpa.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.cdnleiting.top/gtagduheoe.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.hammf.cn/gtotsvsjnk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.c1oappe.top/gtpwrkvptm.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.zhixingplan.top/gtatsqdtfb.html

Go:   // 手写 map[string][]T
来源：http://hz.havefunace.top/gtcxqlgrqf.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.yanxiufei.cn/gtibfeqjvh.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.cashguo.top/gtgsshjosj.html

[D20] 统计每个元素出现次数
来源：http://hz.dianchejie.cn/gtscqkdghv.html

Py:   Counter(arr)
来源：http://hz.xinyue.icu/gtvdhkkzwl.html

PHP:  array_count_values($arr);
来源：http://hz.316326.xyz/gtwbewmpzz.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hywenlv.cn/gtdemcnmux.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.gogol.net.cn/gtbxmrnwzu.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.ehwqpu.com/gtygazabkp.html

Go:   // 手写 map[T]int
来源：http://hz.jianghu66.top/gtsqbgmfuf.html

Ruby: arr.tally
来源：http://hz.svipenyu.cn/gtoelwuecn.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.guowangkeji.top/gtwzdhrebt.html

[D21] 判断是否包含某元素
来源：http://hz.shuidangran.top/gtquqsnbvj.html

Py:   x in arr
来源：http://hz.sweek.top/gtnlkpotsw.html

PHP:  in_array($x, $arr, true);
来源：http://hz.chenzaomai.com/gtqkibnsff.html

JS:   arr.includes(x)
来源：http://hz.ehwqpu.com/gtixqaheij.html

TS:   arr.includes(x)
来源：http://hz.pycfn.com/gtrokjudtn.html

Java: list.contains(x)
来源：http://hz.hywenlv.cn/gtothyjyps.html

Go:   slices.Contains(arr, x)
来源：http://hz.ppjwa.cn/gtdiewbbkr.html

Ruby: arr.include?(x)
来源：http://hz.52xcode.cn/gtqgurldgr.html

C#:   list.Contains(x)
来源：http://hz.chenzaomai.com/gttnznvquw.html

[D22] 复制数组（避免共享引用）
来源：http://hz.xinyue.icu/gtyawjqxlb.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.nanxinkj.top/gteasfsnob.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.snrcjt.cn/gtgzgtdtem.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.tian-w.cn/gthawdbxnx.html

TS:   [...arr];
来源：http://hz.aizwys.cn/gtqtgkylsg.html

Java: new ArrayList<>(list);
来源：http://hz.hnqzz.top/gtgjgpgkot.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.gogol.net.cn/gtbiwappbq.html

Ruby: arr.dup;  arr.clone
来源：http://hz.smart0.xyz/gtdhowcszj.html

C#:   new List<int>(list);
来源：http://hz.zycfv.cn/gtwzrkpvru.html

[D23] reduce 累积计算
来源：http://hz.jinghuilouyu.cn/gtyywtfvob.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.pycfn.com/gtxscdqbtk.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.xylfe.cn/gtmxmzbiqw.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhaomingkeji.xyz/gtvbojdnbq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.pengpengdd.cyou/gtooxnrhyn.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.zhongyouzk.top/gtbjzsztxz.html

Go:   // 手写循环
来源：http://hz.jiagoushi.top/gtlhakfewg.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.yuxming.cn/gtjjcbvlxd.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.0kj1m.cn/gtvwqaamnv.html

[D24] 字典 / Map 基本操作
来源：http://hz.guowangkeji.top/gtbyfcehkj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.chenzaomai.com/gtkfldbjqu.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.hnxiangtu.top/gtyasoowkk.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.svipenyu.cn/gtivtozypq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.jiagoushi.top/gtgjyjdedd.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.jqgufenzy.top/gtntmcvmbr.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.chenjidiqi.icu/gtwilnxazs.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.gogol.net.cn/gtrfidwklj.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.guowangkeji.top/gtfepnomls.html

[D25] Set 集合去重与交并差
来源：http://hz.hfpthk.cn/gtdagvhqax.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.yj202588.top/gthwmljovt.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.tianlin.xyz/gtaaxmipdw.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.havefunace.top/gtfkojkoeq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.hammf.cn/gtxvioxdhg.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.sxryk.cn/gtvuujdxgc.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.sysykeji.top/gtpurygveo.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.ydzc1.top/gtpmxviagg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.snrcjt.cn/gtdgdhjccf.html

[D26] 数组转字符串
来源：http://hz.bjfxy.top/gtqyzdpyfq.html

Py:   ", ".join(map(str, arr))
来源：http://hz.zhongyouzk.top/gtgphvxkbh.html

PHP:  implode(", ", $arr);
来源：http://hz.hnqzz.top/gttobfskbv.html

JS:   arr.join(", ")
来源：http://hz.hammf.cn/gtkxxboabw.html

TS:   arr.join(", ")
来源：http://hz.zhoulong.xyz/gtziuomxaj.html

Java: String.join(", ", list)
来源：http://hz.tianlin.xyz/gtbsjsznvu.html

Go:   strings.Join(strs, ", ")
来源：http://hz.andypj.xyz/gtwogirjeq.html

Ruby: arr.join(", ")
来源：http://hz.hongshengwenyu.top/gtxlvivisj.html

C#:   string.Join(", ", list)
来源：http://hz.zycfv.cn/gtptasenkk.html

================================================================================
来源：http://hz.birdmap.top/gtfhjtswxj.html

E. 字符串处理
来源：http://hz.jiagoushi.top/gtsnesnrsi.html

================================================================================
来源：http://hz.hnxiangtu.top/gtdqqroxka.html

[E01] 拼接字符串
来源：http://hz.0kj1m.cn/gtrtzbeicz.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.0kj1m.cn/gtrixjtqsv.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.jinqigfzy.top/gtpjcugtww.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.sweek.top/gtfniwihpu.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.tianlin.xyz/gtldnuyzzk.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.snrcjt.cn/gtguwopffn.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.ivvv.top/gtazbrgale.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.iojbl.cn/gtjfymffrw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.zhoulong.xyz/gtkrzawxep.html

[E02] 重复字符串
来源：http://hz.316326.xyz/gtouxqlwhv.html

Py:   "ab" * 3
来源：http://hz.guannengcc.top/gtqmpczswu.html

PHP:  str_repeat("ab", 3);
来源：http://hz.shuidangran.top/gtokwaeoik.html

JS:   "ab".repeat(3)
来源：http://hz.meibo888.top/gtdgibvcax.html

TS:   "ab".repeat(3)
来源：http://hz.yvedp.cn/gtgfohvwta.html

Java: "ab".repeat(3)
来源：http://hz.gogol.net.cn/gtkmgjbxja.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.jinyuanbaomall.cn/gtaxensyny.html

Ruby: "ab" * 3
来源：http://hz.xuetiantiany.cn/gtwdysvtsu.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.gotoacloud.top/gtxeiordlf.html

[E03] 截取子串
来源：http://hz.sysykeji.top/gtbmmorqqo.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.yueranfly.top/gtldtedxxd.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.zhengqikj.top/gtuqzpzklo.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.sysykeji.top/gtckuyaqbe.html

TS:   s.slice(1, 4)
来源：http://hz.dianchejie.cn/gtkzevqnsu.html

Java: s.substring(1, 4)
来源：http://hz.zhiwuduotai.top/gtygksxdtn.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.sufxvd.cn/gtygfhcjmf.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.yj20258.top/gtdozjivrd.html

C#:   s.Substring(1, 3)
来源：http://hz.cucudq.cn/gtzykjoirj.html

[E04] 查找子串位置
来源：http://hz.jinyuanbaomall.cn/gtdiicvzbu.html

Py:   s.find("x");  s.index("x")
来源：http://hz.zhoulong.xyz/gtmpfabxaf.html

PHP:  strpos($s, "x");
来源：http://hz.jqgfzy.top/gtcuzaojdg.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.hnxiangtu.top/gtfetpqbil.html

TS:   s.indexOf("x")
来源：http://hz.aibaodan.cn/gtgiyvynxx.html

Java: s.indexOf("x")
来源：http://hz.yuanzhike.top/gtyokpfnpw.html

Go:   strings.Index(s, "x")
来源：http://hz.gaohongyu789.top/gtwscjhygf.html

Ruby: s.index("x")
来源：http://hz.daxiang520.top/gthpxjchek.html

C#:   s.IndexOf("x")
来源：http://hz.hongshengwenyu.top/gtucvfjlod.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.hammf.cn/gtaduqestj.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.yj20258.top/gtdzdcfvyc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.zhijiandao.cn/gteydsxtkd.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zhiwuduotai.top/gtmacgsfxk.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.jlsjyb.cn/gtasbawoyy.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.chenlongwang.top/gteoippzqs.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.havefunace.top/gtcrvalowx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.hammf.cn/gtyvvxlold.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.jinqigufen.top/gtfnsldzhu.html

[E06] 替换子串
来源：http://hz.gaohongyu789.top/gtcfyhavgq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.cucudq.cn/gtlxlxyozc.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.meibo888.top/gtlmrsbqoe.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.pycfn.com/gtslcirwmj.html

TS:   s.replaceAll("a", "b")
来源：http://hz.ehwqpu.com/gtyuddxwag.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.nwbrower.top/gtrjuxglom.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.jlsjyb.cn/gtgomxfpeb.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.jqgfzy.top/gtjlizrfdz.html

C#:   s.Replace("a", "b")
来源：http://hz.nwbrower.top/gtledskfzd.html

[E07] 按分隔符拆分
来源：http://hz.shanyushiyangtech.top/gtldwihlpf.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.fzhhl.top/gtuxxykfwg.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.cqqwz.cn/gtruripyyx.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.yj202588.top/gtvglnethi.html

TS:   s.split(",")
来源：http://hz.feifeiyinyue.top/gtqimtdvoa.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.ybcxt.top/gtixxovtpc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.yuanzhike.top/gtbuftqbdr.html

Ruby: s.split(",");  s.split
来源：http://hz.hongshengwenyu.top/gtveoknxdb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.jianghu66.top/gtxfbqvvuy.html

[E08] 数组按分隔符合并
来源：http://hz.316326.xyz/gtotbdganc.html

Py:   ",".join(items)
来源：http://hz.yj202588.top/gtkrjzgvwy.html

PHP:  implode(",", $items);
来源：http://hz.jqgufenzy.top/gthtaauqqw.html

JS:   items.join(",")
来源：http://hz.xylfe.cn/gtqxmmoobm.html

TS:   items.join(",")
来源：http://hz.zhengqikj.top/gteynuwaps.html

Java: String.join(",", items)
来源：http://hz.jinqigufen.top/gtribhkeve.html

Go:   strings.Join(items, ",")
来源：http://hz.zhixingplan.top/gtykczesug.html

Ruby: items.join(",")
来源：http://hz.svipenyu.cn/gtpbhlewdb.html

C#:   string.Join(",", items)
来源：http://hz.iojbl.cn/gtoajbzxyt.html

[E09] 去除所有空白字符
来源：http://hz.gotoacloud.top/gtkhfqyrex.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.quarkkingdee.top/gtttqhothi.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.ppjwa.cn/gtrqugehvw.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.yonumen.top/gttrtoxtxe.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.52xcode.cn/gtrxhmbbjm.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.yvedp.cn/gtezpgmaaj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.ivvv.top/gtkyubgohr.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.jqgufenzy.top/gtlmyqdoai.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.meibo888.top/gtusdtwquq.html

[E10] 左侧补零 / 定长填充
来源：http://hz.cucudq.cn/gtjzdcqppb.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.havefunace.top/gtxrmljybz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.sweek.top/gtbrgqmtme.html

JS:   "7".padStart(3, "0")
来源：http://hz.sysykeji.top/gtsrobthbi.html

TS:   "7".padStart(3, "0")
来源：http://hz.nwbrower.top/gtyzribvxl.html

Java: String.format("%03d", 7)
来源：http://hz.sysykeji.top/gtvzvuotcl.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.aibaodan.cn/gtbddmarqp.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.yuxming.cn/gtqlixqjgs.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.jinqigufen.top/gteplmzaod.html

[E11] 反转字符串
来源：http://hz.hfpthk.cn/gtvamygucc.html

Py:   s[::-1]
来源：http://hz.shzxlz.cn/gtmgznbuvz.html

PHP:  strrev($s);
来源：http://hz.fzhhl.top/gtccgafsfv.html

JS:   [...s].reverse().join("")
来源：http://hz.jyoumei.cn/gtvwhbvrpp.html

TS:   [...s].reverse().join("")
来源：http://hz.redwolf501.top/gtjyaqvfly.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.ywan-chungtsiang.top/gthavrxrjx.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.hongshengwenyu.top/gtbrnekopk.html

Ruby: s.reverse
来源：http://hz.cucudq.cn/gtijceuavx.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.hfpthk.cn/gtsoinsebm.html

[E12] 统计某字符出现次数
来源：http://hz.wangdashe.top/gttvdxtzey.html

Py:   s.count("a")
来源：http://hz.bjfxy.top/gtlnltlrqf.html


<!-- 参考信息 -->