代发 wailian999

C#:   list.Insert(0, 0);
来源：http://hz.tian-w.cn/gttvzbtzkq.html

[D04] 删除元素
来源：http://hz.guowangkeji.top/gtxgnkmmxp.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.zhaomingkeji.xyz/gtmrrwoapu.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.yongpay.top/gteidaurau.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.sysykeji.top/gtfwkljwoe.html

TS:   arr.splice(0, 1);
来源：http://hz.yj202588.top/gtvdmzcctu.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.xuetiantiany.cn/gtneiuslmd.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.sysykeji.top/gtxgfqsksz.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.yj20258.top/gtwikeahif.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.aibaodan.cn/gtxdmaxwev.html

[D05] 访问与修改元素
来源：http://hz.gogol.net.cn/gtgfoziksg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhongyouzk.top/gtkkqombgc.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.nanxinkj.top/gtjcvuoslc.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.jinqigfzy.top/gtkkxxcdga.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.sufxvd.cn/gtaabtwmzy.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.aizwys.cn/gtdfsnjkef.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.zhiwuduotai.top/gtsqxuyybz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.smart0.xyz/gtkcprqklt.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.yuanzhike.top/gtjwnxlbra.html

[D06] 数组长度
来源：http://hz.xuanzx.com/gtganxsvtt.html

Py:   len(arr)
来源：http://hz.wangdashe.top/gtdyqgqmbs.html

PHP:  count($arr);
来源：http://hz.redwolf501.top/gtkmzgbwbr.html

JS:   arr.length
来源：http://hz.quarkkingdee.top/gtidpktupp.html

TS:   arr.length
来源：http://hz.xylfe.cn/gtutprvpxd.html

Java: list.size();
来源：http://hz.ivvv.top/gtyalemews.html

Go:   len(arr)
来源：http://hz.sysykeji.top/gthocjrrqn.html

Ruby: arr.length; arr.size
来源：http://hz.snrcjt.cn/gtnsdjhxsw.html

C#:   list.Count;
来源：http://hz.zhoulong.xyz/gtwsyyutcq.html

[D07] 切片 / 取子数组
来源：http://hz.tian-w.cn/gtjebgdkge.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.jlsjyb.cn/gterjirgwt.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.fengsongda.top/gtxzitayrt.html

JS:   arr.slice(1, 4);
来源：http://hz.gzhubu.top/gtfyvjxcmb.html

TS:   arr.slice(1, 4);
来源：http://hz.fzhhl.top/gtsomkgfvd.html

Java: list.subList(1, 4);
来源：http://hz.ppjwa.cn/gtixsbomvj.html

Go:   arr[1:4]
来源：http://hz.ybcxt.top/gtglsqfswv.html

Ruby: arr[1, 3]
来源：http://hz.0kj1m.cn/gtvmjlheai.html

C#:   list.GetRange(1, 3);
来源：http://hz.guowangkeji.top/gtjmzrxfwa.html

[D08] 合并两个数组
来源：http://hz.yonumen.top/gtlulfjkol.html

Py:   a + b;  a.extend(b)
来源：http://hz.smart0.xyz/gtgmclltjc.html

PHP:  array_merge($a, $b);
来源：http://hz.tian-w.cn/gtpcijersx.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.svipenyu.cn/gtnrynikgc.html

TS:   [...a, ...b];
来源：http://hz.tian-w.cn/gtdahiewdq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.yuanzhike.top/gtxhaizxac.html

Go:   append(a, b...)
来源：http://hz.guannengcc.top/gtewceoepb.html

Ruby: a + b;  a.concat(b)
来源：http://hz.hongshengwenyu.top/gtjexvrzhc.html

C#:   a.Concat(b).ToList()
来源：http://hz.sysykeji.top/gticwkmiiz.html

[D09] 排序（升序）
来源：http://hz.guannengcc.top/gtrwpbchez.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ehwqpu.com/gtxvabztlh.html

PHP:  sort($arr);
来源：http://hz.gzhubu.top/gtzgszohgz.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.hongshengwenyu.top/gtbeejnvkm.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.andypj.xyz/gticsoulnd.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.ehwqpu.com/gtquszobrc.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.yuxming.cn/gtxhsefeeb.html

Ruby: arr.sort
来源：http://hz.ydjk.org.cn/gtuvqsnaiq.html

C#:   list.Sort();
来源：http://hz.sxryk.cn/gtczonmuay.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.shuidangran.top/gtusbyacsf.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.xinyue.icu/gtmhuayjij.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yanxiufei.cn/gtqwstjpee.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jqgufenzy.top/gtjoaxdvsk.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zhoulong.xyz/gtjmftyxbg.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.cdnleiting.top/gtlwlfeqfi.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.haohaochexian.top/gtxkcqrmnz.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.fzhhl.top/gtyygodbkx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.kuanghao11.cn/gtlajzcqxf.html

[D11] 反转数组
来源：http://hz.c1oappe.top/gtjscazjab.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.c1oappe.top/gtotwzaomj.html

PHP:  array_reverse($arr);
来源：http://hz.xinyue.icu/gtpdzzndnr.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.aibaodan.cn/gtqgjnaqft.html

TS:   [...arr].reverse();
来源：http://hz.kuanghao11.cn/gtsuixzlgp.html

Java: Collections.reverse(list);
来源：http://hz.xinyue.icu/gtlpeesmua.html

Go:   slices.Reverse(arr)
来源：http://hz.xuetiantiany.cn/gtjjvrmzzq.html

Ruby: arr.reverse
来源：http://hz.yuanzhike.top/gtdyvqvfpz.html

C#:   list.Reverse();
来源：http://hz.hongshengwenyu.top/gtcpktwrer.html

[D12] 查找元素下标
来源：http://hz.daxiang520.top/gtjxfnxksh.html

Py:   arr.index(x);  x in arr
来源：http://hz.guowangkeji.top/gtclirxcgx.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.tian-w.cn/gtsavkvfnt.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zdqjudy.top/gtqercrbtk.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yangfankeji.com/gtwvohaluo.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.gaohongyu789.top/gtozdebsib.html

Go:   slices.Index(arr, x)
来源：http://hz.iojbl.cn/gtmyqzhuex.html

Ruby: arr.index(x)
来源：http://hz.zycfv.cn/gtienynjzu.html

C#:   list.IndexOf(x);
来源：http://hz.hammf.cn/gtfbemuufq.html

[D13] 过滤（保留满足条件的）
来源：http://hz.gotoacloud.top/gtddsihfqa.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.yangfankeji.com/gtrjziqpcj.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.pengpengdd.cyou/gtrjjealnr.html

JS:   arr.filter(x => x > 3)
来源：http://hz.birdmap.top/gtsdxjhplk.html

TS:   arr.filter(x => x > 3)
来源：http://hz.yj20258.top/gtnkzemgay.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.ppjwa.cn/gtkqhvremn.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.jinyuanbaomall.cn/gtvjezwtyr.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.yonumen.top/gtffswnujg.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.sysykeji.top/gtpfsabqeb.html

[D14] 映射转换（每个元素变形）
来源：http://hz.bjfxy.top/gtkrctywhx.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.gaohongyu789.top/gtyckjczta.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.yvedp.cn/gtoazbnnbn.html

JS:   arr.map(x => x * 2)
来源：http://hz.nanxuanxn.top/gttrqgsmxv.html

TS:   arr.map(x => x * 2)
来源：http://hz.cdnleiting.top/gtlzdtlciy.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.yvedp.cn/gtbraphcey.html

Go:   // 手写循环
来源：http://hz.nanxinkj.top/gtcgsbgpcn.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.smart0.xyz/gtmbutzvzq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.sufxvd.cn/gtyojbgmxh.html

[D15] 去重
来源：http://hz.vqdsnc.cn/gtmobwyneu.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.gzhubu.top/gtbxyguuke.html

PHP:  array_unique($arr);
来源：http://hz.yj20258.top/gttmumvoxm.html

JS:   [...new Set(arr)]
来源：http://hz.haohaochexian.top/gtqfmgjoop.html

TS:   [...new Set(arr)]
来源：http://hz.iojbl.cn/gtwulrdoua.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.tian-w.cn/gtuilpptfu.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.jinghuilouyu.cn/gtctvjruyi.html

Ruby: arr.uniq
来源：http://hz.xingfuxueyuan.xyz/gtpykgwnvm.html

C#:   list.Distinct().ToList()
来源：http://hz.yonumen.top/gtofypavlw.html

[D16] 求和与平均值
来源：http://hz.sufxvd.cn/gtpzuqxhqt.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.shuidangran.top/gtnscawrzu.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.xuanzx.com/gteyycxqul.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.xuanzx.com/gtniexzqhf.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.ydjk.org.cn/gtijadtogk.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.yj202588.top/gtsenenymj.html

Go:   // 手写循环累加
来源：http://hz.meibo888.top/gtfpvlyeis.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.nanxuanxn.top/gtbomffpkp.html

C#:   list.Sum();  list.Average()
来源：http://hz.zhixingplan.top/gtmgavbbge.html

[D17] 最大值与最小值
来源：http://hz.cucudq.cn/gtendtszsh.html

Py:   max(arr);  min(arr)
来源：http://hz.jinyuanbaomall.cn/gttcypeohl.html

PHP:  max($arr);  min($arr);
来源：http://hz.cashguo.top/gtcwzutgzs.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.gzhubu.top/gtariwznpy.html

TS:   Math.max(...arr);
来源：http://hz.hnxiangtu.top/gtdqwndyxl.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.yuxming.cn/gtwojuwwjw.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.gzhubu.top/gtljbwgwkz.html

Ruby: arr.max;  arr.min
来源：http://hz.jinqigufen.top/gtyvtezvye.html

C#:   list.Max();  list.Min()
来源：http://hz.ybcxt.top/gtmtwprecc.html

[D18] 扁平化嵌套数组
来源：http://hz.jiagoushi.top/gtfcazpdpz.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.jinqigfzy.top/gtqnedmrfy.html

PHP:  array_merge(...$nested);
来源：http://hz.kuanghao11.cn/gtnyyzjqez.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.tian-w.cn/gtqrzsjxwg.html

TS:   nested.flat();
来源：http://hz.pycfn.com/gtsekaneea.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.sxryk.cn/gtbrjyotqg.html

Go:   // 手写双层循环
来源：http://hz.sweek.top/gtahsiwftt.html

Ruby: nested.flatten
来源：http://hz.jinqigufen.top/gthjtygwao.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.shangyingyoupin.top/gtqyhbmbqm.html

[D19] 按字段分组
来源：http://hz.hfpthk.cn/gtxzxrsnrs.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.xuanzx.com/gtjqcwblni.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.ywan-chungtsiang.top/gtwqejjyiv.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.aibaodan.cn/gtrsppfbyr.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.yonumen.top/gtscyvgkfg.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.jinghuilouyu.cn/gtydsjfllh.html

Go:   // 手写 map[string][]T
来源：http://hz.chenjidiqi.icu/gtmyilmjpx.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.hysaishi.cn/gtmsplqhjd.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.bjfxy.top/gtksfqowmj.html

[D20] 统计每个元素出现次数
来源：http://hz.sweek.top/gtaxfdyazq.html

Py:   Counter(arr)
来源：http://hz.andypj.xyz/gtkgknsmzd.html

PHP:  array_count_values($arr);
来源：http://hz.jiagoushi.top/gtmsvkdhlk.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jianghu66.top/gtujepvstu.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.redwolf501.top/gtiqedzgji.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.ehwqpu.com/gtodvoubpg.html

Go:   // 手写 map[T]int
来源：http://hz.yvedp.cn/gtgiskfyjw.html

Ruby: arr.tally
来源：http://hz.jlsjyb.cn/gtbilrfhxi.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.wangshuangyany.cn/gttprzynxe.html

[D21] 判断是否包含某元素
来源：http://hz.jinyuanbaomall.cn/gtezmpomxu.html

Py:   x in arr
来源：http://hz.ivvv.top/gtitosxxqw.html

PHP:  in_array($x, $arr, true);
来源：http://hz.jinyuanbaomall.cn/gtopbbpmam.html

JS:   arr.includes(x)
来源：http://hz.zhengqikj.top/gtmpkwysvo.html

TS:   arr.includes(x)
来源：http://hz.sufxvd.cn/gtbhabwcfk.html

Java: list.contains(x)
来源：http://hz.jinghuilouyu.cn/gtnnedxrrr.html

Go:   slices.Contains(arr, x)
来源：http://hz.52xcode.cn/gtkcaenhzr.html

Ruby: arr.include?(x)
来源：http://hz.fzhhl.top/gtxwczvsoc.html

C#:   list.Contains(x)
来源：http://hz.mhx1999.top/gtrsfiqefr.html

[D22] 复制数组（避免共享引用）
来源：http://hz.xuanzx.com/gtavsdwrtv.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.yuanzhike.top/gtclgfkmru.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.smart0.xyz/gtzbvtgikp.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.vqdsnc.cn/gtcqlsqyim.html

TS:   [...arr];
来源：http://hz.yuxming.cn/gtpmylzfvz.html

Java: new ArrayList<>(list);
来源：http://hz.zhongyouzk.top/gtrlhzgvcf.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.sufxvd.cn/gtlxlulgmh.html

Ruby: arr.dup;  arr.clone
来源：http://hz.tianlin.xyz/gtcoveedoh.html

C#:   new List<int>(list);
来源：http://hz.gzhubu.top/gtxxcqcwaz.html

[D23] reduce 累积计算
来源：http://hz.hysaishi.cn/gtbrlzkiuh.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.chenlongwang.top/gtnyotabgl.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.wangshuangyany.cn/gtueslwdnf.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.feifeiyinyue.top/gtiiqrotpg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.sufxvd.cn/gtqwqnccup.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.birdmap.top/gtxoqjqruq.html

Go:   // 手写循环
来源：http://hz.aizwys.cn/gtclavpavn.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.shanyushiyangtech.top/gtndhcpcqk.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.chenzaomai.com/gtxsjjftpp.html

[D24] 字典 / Map 基本操作
来源：http://hz.zdqjudy.top/gtccwmcbfg.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.hywenlv.cn/gtzvggobdn.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.cashguo.top/gtfpondxte.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.redwolf501.top/gtmghxadcl.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.ydzc1.top/gtfqgbjkqm.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.cheryme.top/gthvsorfng.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.hywenlv.cn/gtfsbqcmzn.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.zhiwuduotai.top/gtirxmuofm.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.zhaomingkeji.xyz/gtpfsdsqhi.html

[D25] Set 集合去重与交并差
来源：http://hz.ydjk.org.cn/gtiadvodxq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.gzhubu.top/gtbqmrignf.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.hysaishi.cn/gttukqjllh.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.ppjwa.cn/gthupqqrtq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.fengsongda.top/gthyeyduui.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.zdqjudy.top/gtevscqrsp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.hnxiangtu.top/gtajwwhpfb.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.cheryme.top/gteqefrvaw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.nanxuanxn.top/gtggyhqzvc.html

[D26] 数组转字符串
来源：http://hz.yongpay.top/gtvvrjkjbx.html

Py:   ", ".join(map(str, arr))
来源：http://hz.ehwqpu.com/gtsoesyhzs.html

PHP:  implode(", ", $arr);
来源：http://hz.aibaodan.cn/gtponkzwyf.html

JS:   arr.join(", ")
来源：http://hz.feifeiyinyue.top/gtjmxdhkkh.html

TS:   arr.join(", ")
来源：http://hz.xuanzx.com/gtibkmjtnx.html

Java: String.join(", ", list)
来源：http://hz.redwolf501.top/gtqzcsrjdf.html

Go:   strings.Join(strs, ", ")
来源：http://hz.ywan-chungtsiang.top/gtrlplmkgl.html

Ruby: arr.join(", ")
来源：http://hz.aibaodan.cn/gtwthnloen.html

C#:   string.Join(", ", list)
来源：http://hz.meibo888.top/gtqbkqquut.html

================================================================================
来源：http://hz.xuanzx.com/gtteaihncf.html

E. 字符串处理
来源：http://hz.wangshuangyany.cn/gtsgokjlbi.html

================================================================================
来源：http://hz.chenlongwang.top/gtxkubgkfo.html

[E01] 拼接字符串
来源：http://hz.yuanzhike.top/gtwqwydxeg.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.yongpay.top/gtuuuitrfa.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.jinyuanbaomall.cn/gtpepohbnn.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.cdnleiting.top/gtuysbsopj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zhongyouzk.top/gtaigdvype.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.daxiang520.top/gtcrwolgol.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.meibo888.top/gtkvewpgdm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.sxryk.cn/gtjhzyobll.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.gogol.net.cn/gtwjqdivpx.html

[E02] 重复字符串
来源：http://hz.hywenlv.cn/gtxckqelyv.html

Py:   "ab" * 3
来源：http://hz.ydjk.org.cn/gtirygzalh.html

PHP:  str_repeat("ab", 3);
来源：http://hz.jinyuanbaomall.cn/gtlbkokliv.html

JS:   "ab".repeat(3)
来源：http://hz.chenzaomai.com/gtxuyziopr.html

TS:   "ab".repeat(3)
来源：http://hz.aibaodan.cn/gtzuhdkxcp.html

Java: "ab".repeat(3)
来源：http://hz.nanxinkj.top/gtlwrvcrfu.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.zhengqikj.top/gtiejfntqo.html

Ruby: "ab" * 3
来源：http://hz.xylfe.cn/gtiqaixtsd.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.xuetiantiany.cn/gtlbkscsxp.html

[E03] 截取子串
来源：http://hz.sxryk.cn/gtwgzksebq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.sxryk.cn/gtdqqbftnj.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.zhengqikj.top/gthldrqbdm.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.ybcxt.top/gtkgzgldku.html

TS:   s.slice(1, 4)
来源：http://hz.yj20258888.top/gtpnszyybe.html

Java: s.substring(1, 4)
来源：http://hz.birdmap.top/gtsikjntio.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.hammf.cn/gtzzrghdfc.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.xingfuxueyuan.xyz/gtkatllliv.html

C#:   s.Substring(1, 3)
来源：http://hz.birdmap.top/gtotfpncvv.html

[E04] 查找子串位置
来源：http://hz.hammf.cn/gtwvcplukp.html

Py:   s.find("x");  s.index("x")
来源：http://hz.yanxiufei.cn/gtawgajkuq.html

PHP:  strpos($s, "x");
来源：http://hz.shanyushiyangkeji.top/gtedmyuooy.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.sysykeji.top/gtbryihbni.html

TS:   s.indexOf("x")
来源：http://hz.chenlongwang.top/gtazikbcjr.html

Java: s.indexOf("x")
来源：http://hz.cdnleiting.top/gtsdgpafxy.html

Go:   strings.Index(s, "x")
来源：http://hz.aibaodan.cn/gtvlsexuxj.html

Ruby: s.index("x")
来源：http://hz.xuetiantiany.cn/gtpicsrtmf.html

C#:   s.IndexOf("x")
来源：http://hz.ybcxt.top/gteqnseemg.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.ppjwa.cn/gtdqgbywoh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.jinyuanbaomall.cn/gtnhygmhad.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.xinyue.icu/gtphlykfkc.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.hnxiangtu.top/gtyawrajqf.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.hnxiangtu.top/gtpldesmfb.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.aibaodan.cn/gtntzopflb.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.zhiwuduotai.top/gtmwtevobx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.gaohongyu789.top/gtwkrcgckr.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.yuxming.cn/gtmfthazmg.html

[E06] 替换子串
来源：http://hz.ivvv.top/gtdmiygtmi.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.cqqwz.cn/gtbbvmyecp.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.yuxming.cn/gtkphrmanp.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.snrcjt.cn/gtobnhyzyp.html

TS:   s.replaceAll("a", "b")
来源：http://hz.zdqjudy.top/gtzhaospke.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.shzxlz.cn/gtomprzcom.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.xingfuxueyuan.xyz/gtksgycple.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.xylfe.cn/gthrbuedka.html

C#:   s.Replace("a", "b")
来源：http://hz.yj20258.top/gtrldodjft.html

[E07] 按分隔符拆分
来源：http://hz.zhoulong.xyz/gteojpqlda.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.ehwqpu.com/gtotxawirp.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.ppjwa.cn/gtxcwiauhk.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.ywan-chungtsiang.top/gtczdkiewc.html

TS:   s.split(",")
来源：http://hz.fengsongda.top/gtiuwhdzvy.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.pycfn.com/gtlxxmdwzm.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.snrcjt.cn/gtrjlfyhkg.html

Ruby: s.split(",");  s.split
来源：http://hz.hywenlv.cn/gtciggckps.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.jqgufenzy.top/gtpcmzhgtd.html

[E08] 数组按分隔符合并
来源：http://hz.zhoulong.xyz/gtgjhhqfsg.html

Py:   ",".join(items)
来源：http://hz.ppjwa.cn/gtllczdhre.html

PHP:  implode(",", $items);
来源：http://hz.zhongyouzk.top/gtzxrmexzu.html

JS:   items.join(",")
来源：http://hz.zhengqikj.top/gtgfrhijym.html

TS:   items.join(",")
来源：http://hz.xylfe.cn/gtmhbmvtxe.html

Java: String.join(",", items)
来源：http://hz.tian-w.cn/gtbgxvwrqx.html

Go:   strings.Join(items, ",")
来源：http://hz.hammf.cn/gttiauaaec.html

Ruby: items.join(",")
来源：http://hz.jiagoushi.top/gtyojvkjtv.html

C#:   string.Join(",", items)
来源：http://hz.jinqigfzy.top/gtsxlwuhtu.html

[E09] 去除所有空白字符
来源：http://hz.nwbrower.top/gtiyenjhoe.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.wangdashe.top/gticulnoop.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.xuanzx.com/gtncmjvzqr.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.gzhubu.top/gtircevvxh.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.bjfxy.top/gtiqyvwabk.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.gzhubu.top/gtuvspleyq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.jinghuilouyu.cn/gtnlpuasnh.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.ehwqpu.com/gtfcjtuclp.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.cqqwz.cn/gtupvkeodu.html

[E10] 左侧补零 / 定长填充
来源：http://hz.cheryme.top/gtdubssqdf.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.tian-w.cn/gtapxodrnl.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.zhoulong.xyz/gtprilllhi.html

JS:   "7".padStart(3, "0")
来源：http://hz.andypj.xyz/gtlrywdawm.html

TS:   "7".padStart(3, "0")
来源：http://hz.snrcjt.cn/gtczbtwlhe.html

Java: String.format("%03d", 7)
来源：http://hz.sufxvd.cn/gtcpyyicxn.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.iojbl.cn/gtktobkqnl.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.snrcjt.cn/gtvpqcgbxz.html


<!-- 参考信息 -->