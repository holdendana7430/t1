代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.hammf.cn/gtdzympyqt.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.hammf.cn/gtqmbmfiww.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.sufxvd.cn/gtojdlqmco.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.c1oappe.top/gtlhwbejvk.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.yueranfly.top/gtkebxfhle.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.tanke756.top/gtnpimjcxm.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.wangshuangyany.cn/gtuvgjtskl.html

[D06] 数组长度
来源：http://hz.jinqigufen.top/gtbbnksbhl.html

Py:   len(arr)
来源：http://hz.jqgfzy.top/gtofdvijks.html

PHP:  count($arr);
来源：http://hz.vqdsnc.cn/gtvmbbueuy.html

JS:   arr.length
来源：http://hz.vqdsnc.cn/gtzehbeefg.html

TS:   arr.length
来源：http://hz.chenzaomai.com/gttqjqfisj.html

Java: list.size();
来源：http://hz.cdnleiting.top/gttjxbwkfx.html

Go:   len(arr)
来源：http://hz.hnqzz.top/gtsdnqdezb.html

Ruby: arr.length; arr.size
来源：http://hz.smart0.xyz/gtczwjxooi.html

C#:   list.Count;
来源：http://hz.ydzc1.top/gtesipdvar.html

[D07] 切片 / 取子数组
来源：http://hz.birdmap.top/gtkbdbhjqv.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.sysykeji.top/gtakeertuz.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.xuanzx.com/gtbytcsbki.html

JS:   arr.slice(1, 4);
来源：http://hz.dianchejie.cn/gtcrujzxqe.html

TS:   arr.slice(1, 4);
来源：http://hz.guannengcc.top/gtqmbyjpuz.html

Java: list.subList(1, 4);
来源：http://hz.yongpay.top/gtbefslunm.html

Go:   arr[1:4]
来源：http://hz.sweek.top/gtezwexahq.html

Ruby: arr[1, 3]
来源：http://hz.birdmap.top/gtcpodghoz.html

C#:   list.GetRange(1, 3);
来源：http://hz.iojbl.cn/gtczirwuls.html

[D08] 合并两个数组
来源：http://hz.ivvv.top/gtbxzzaivt.html

Py:   a + b;  a.extend(b)
来源：http://hz.zhixingplan.top/gttlcnrckl.html

PHP:  array_merge($a, $b);
来源：http://hz.chenlongwang.top/gtxcglfdbe.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.jiagoushi.top/gtmoqifuot.html

TS:   [...a, ...b];
来源：http://hz.quarkkingdee.top/gtbdkumhbh.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.ppjwa.cn/gtibvwaxcn.html

Go:   append(a, b...)
来源：http://hz.cheryme.top/gtbjohbdpb.html

Ruby: a + b;  a.concat(b)
来源：http://hz.pengpengdd.cyou/gtmxwkdrhw.html

C#:   a.Concat(b).ToList()
来源：http://hz.jinyuanbaomall.cn/gtxilcrmxx.html

[D09] 排序（升序）
来源：http://hz.ivvv.top/gtzntwxksl.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jinqigfzy.top/gtjeandpvp.html

PHP:  sort($arr);
来源：http://hz.jinyuanbaomall.cn/gtfpyxnzug.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.smart0.xyz/gtuuiytiwp.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.dianchejie.cn/gtqbsngsov.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.yj20258.top/gtvkwqontk.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.0kj1m.cn/gtqjmkleoj.html

Ruby: arr.sort
来源：http://hz.snrcjt.cn/gtlldnncrw.html

C#:   list.Sort();
来源：http://hz.yueranfly.top/gtwywwhzkr.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.tian-w.cn/gtumggsnbj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.yuxming.cn/gtiytgvwud.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zhiwuduotai.top/gtquboapyl.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.aibaodan.cn/gtlzvshapv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.chenjidiqi.icu/gtoiefovqy.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.haohaochexian.top/gtgtgjkjoq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.xinyue.icu/gtibcvtzgg.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.hfpthk.cn/gtryffonrv.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.hnqzz.top/gtgojtqtmc.html

[D11] 反转数组
来源：http://hz.yvedp.cn/gtrvyhhzia.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.chenjidiqi.icu/gtmrrhqeuq.html

PHP:  array_reverse($arr);
来源：http://hz.nanxuanxn.top/gtwtmqamlq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.hfpthk.cn/gtfkqdprod.html

TS:   [...arr].reverse();
来源：http://hz.xinyue.icu/gtrishprmf.html

Java: Collections.reverse(list);
来源：http://hz.chenlongwang.top/gtcqvznsxl.html

Go:   slices.Reverse(arr)
来源：http://hz.pengpengdd.cyou/gthntcyvth.html

Ruby: arr.reverse
来源：http://hz.yj202588.top/gtinqdgioi.html

C#:   list.Reverse();
来源：http://hz.zhixingplan.top/gtvuynrbnf.html

[D12] 查找元素下标
来源：http://hz.zhijiandao.cn/gtyvwewdil.html

Py:   arr.index(x);  x in arr
来源：http://hz.sxryk.cn/gtaubixajm.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.yj20258888.top/gtyeqnamxe.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jiagoushi.top/gtflduarpk.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.ybcxt.top/gthlwftscp.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.ppjwa.cn/gtrydqeipd.html

Go:   slices.Index(arr, x)
来源：http://hz.sufxvd.cn/gtxysuazyi.html

Ruby: arr.index(x)
来源：http://hz.fengsongda.top/gtwaxjifhs.html

C#:   list.IndexOf(x);
来源：http://hz.snrcjt.cn/gtkdtchaoi.html

[D13] 过滤（保留满足条件的）
来源：http://hz.jiagoushi.top/gtyboipiyj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.gotoacloud.top/gtepgmulae.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.yj202588.top/gtqathmhqe.html

JS:   arr.filter(x => x > 3)
来源：http://hz.zhoulong.xyz/gtrjuxbrcp.html

TS:   arr.filter(x => x > 3)
来源：http://hz.ehwqpu.com/gtjuvaidnl.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.zhaomingkeji.xyz/gtwwxbrhzi.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.hnxiangtu.top/gtksutqaqg.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.9152youxi.cn/gtayrdlzwd.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.shanyushiyangkeji.top/gtrgfhyvva.html

[D14] 映射转换（每个元素变形）
来源：http://hz.ydjk.org.cn/gtcotuyzpj.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.yuxming.cn/gtjnczwwqs.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.aibaodan.cn/gtjtqswzit.html

JS:   arr.map(x => x * 2)
来源：http://hz.andypj.xyz/gtbhcbcnwr.html

TS:   arr.map(x => x * 2)
来源：http://hz.yuxming.cn/gtrazfdjgr.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.gotoacloud.top/gthtsvwahu.html

Go:   // 手写循环
来源：http://hz.jiagoushi.top/gtdgmbvzvt.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.jlsjyb.cn/gtexwlzoss.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.yanxiufei.cn/gtwlcngoeh.html

[D15] 去重
来源：http://hz.snrcjt.cn/gtgjuakbti.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.iojbl.cn/gtknssrhti.html

PHP:  array_unique($arr);
来源：http://hz.zycfv.cn/gtxrsmnjnp.html

JS:   [...new Set(arr)]
来源：http://hz.9152youxi.cn/gtcyhbgkwc.html

TS:   [...new Set(arr)]
来源：http://hz.ehwqpu.com/gtxbhbrxdm.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.guowangkeji.top/gtcikughek.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.pengpengdd.cyou/gttcxaaghw.html

Ruby: arr.uniq
来源：http://hz.zhengqikj.top/gtypzdykrt.html

C#:   list.Distinct().ToList()
来源：http://hz.yanxiufei.cn/gtcdnyvlwm.html

[D16] 求和与平均值
来源：http://hz.guowangkeji.top/gtktkcszvn.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.c1oappe.top/gtxeionvsq.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.guannengcc.top/gttaffptgh.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.mhx1999.top/gtaauvdezp.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.mhx1999.top/gtxtnriayz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.nanxinkj.top/gtpplnrgtx.html

Go:   // 手写循环累加
来源：http://hz.yuxming.cn/gtbtoqrtpi.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.ydzc1.top/gtjnidivqv.html

C#:   list.Sum();  list.Average()
来源：http://hz.sxryk.cn/gtbavjkczu.html

[D17] 最大值与最小值
来源：http://hz.jqgfzy.top/gtgkqtspxp.html

Py:   max(arr);  min(arr)
来源：http://hz.zhiwuduotai.top/gtqkgyseek.html

PHP:  max($arr);  min($arr);
来源：http://hz.jinqigfzy.top/gtxmmyyvsp.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.iojbl.cn/gtauulxktn.html

TS:   Math.max(...arr);
来源：http://hz.dashuyun.cn/gtddfoymet.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.jinqigfzy.top/gtkbbjgcmx.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.shzxlz.cn/gtwlrnywwz.html

Ruby: arr.max;  arr.min
来源：http://hz.cashguo.top/gtlkscknno.html

C#:   list.Max();  list.Min()
来源：http://hz.kuanghao11.cn/gtkakqxgzd.html

[D18] 扁平化嵌套数组
来源：http://hz.shzxlz.cn/gtsnddwaaq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.sufxvd.cn/gtndxzllgh.html

PHP:  array_merge(...$nested);
来源：http://hz.9152youxi.cn/gtmkwyebku.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.316326.xyz/gtrfhugxal.html

TS:   nested.flat();
来源：http://hz.wangshuangyany.cn/gthckufckg.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.nwbrower.top/gtltillttp.html

Go:   // 手写双层循环
来源：http://hz.jinyuanbaomall.cn/gtcnqjldys.html

Ruby: nested.flatten
来源：http://hz.wangdashe.top/gtxctzsjwc.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.havefunace.top/gtywhvqvrw.html

[D19] 按字段分组
来源：http://hz.dianchejie.cn/gtowqiqkko.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.cucudq.cn/gtmogqoedv.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.smart0.xyz/gtpxgmwilk.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.feifeiyinyue.top/gtaddvqvzw.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.zdqjudy.top/gtgwfhfbza.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.nanxuanxn.top/gtxzccclvy.html

Go:   // 手写 map[string][]T
来源：http://hz.sufxvd.cn/gtbsvmibnc.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.shuidangran.top/gtwrpbgyvh.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.jqgfzy.top/gtoogqnoey.html

[D20] 统计每个元素出现次数
来源：http://hz.jyoumei.cn/gtomqfvgix.html

Py:   Counter(arr)
来源：http://hz.fengsongda.top/gttejlzmmu.html

PHP:  array_count_values($arr);
来源：http://hz.jinghuilouyu.cn/gtbstuweub.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.52xcode.cn/gtjpcksvds.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.andypj.xyz/gtrdnovsgj.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.cqqwz.cn/gtycmypmxy.html

Go:   // 手写 map[T]int
来源：http://hz.hfpthk.cn/gtrbabintx.html

Ruby: arr.tally
来源：http://hz.sysykeji.top/gtoxkxyqim.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.sufxvd.cn/gtyunvbhus.html

[D21] 判断是否包含某元素
来源：http://hz.jqgfzy.top/gtrxvhtnye.html

Py:   x in arr
来源：http://hz.havefunace.top/gtbakarzvz.html

PHP:  in_array($x, $arr, true);
来源：http://hz.pycfn.com/gtqwggtdcg.html

JS:   arr.includes(x)
来源：http://hz.dashuyun.cn/gtfmyhepzo.html

TS:   arr.includes(x)
来源：http://hz.cdnleiting.top/gtksdqjrqw.html

Java: list.contains(x)
来源：http://hz.mhx1999.top/gtyluzkfvj.html

Go:   slices.Contains(arr, x)
来源：http://hz.tian-w.cn/gttthycduh.html

Ruby: arr.include?(x)
来源：http://hz.cashguo.top/gtlkkegpmb.html

C#:   list.Contains(x)
来源：http://hz.xylfe.cn/gtvtlahoic.html

[D22] 复制数组（避免共享引用）
来源：http://hz.cqqwz.cn/gthneduecj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.yj20258888.top/gtkaoypzgr.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.jinqigfzy.top/gtpnqocedu.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.jqgufenzy.top/gtvwgmidvj.html

TS:   [...arr];
来源：http://hz.chenlongwang.top/gtngfhrtcd.html

Java: new ArrayList<>(list);
来源：http://hz.vqdsnc.cn/gtojpsarud.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.jinqigfzy.top/gtxdvmsics.html

Ruby: arr.dup;  arr.clone
来源：http://hz.nwbrower.top/gtreywtgyf.html

C#:   new List<int>(list);
来源：http://hz.yj20258.top/gtlfngizsu.html

[D23] reduce 累积计算
来源：http://hz.chenjidiqi.icu/gtjsxvpnzt.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.cdnleiting.top/gteqlmbjjw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.jyoumei.cn/gtiurlhqjn.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yuanzhike.top/gtssuocfof.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.chenjidiqi.icu/gtnsqphamx.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.c1oappe.top/gttgxrcqvb.html

Go:   // 手写循环
来源：http://hz.zhiwuduotai.top/gtrvscealz.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.guannengcc.top/gteippotwj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.yuxming.cn/gtzrsxzris.html

[D24] 字典 / Map 基本操作
来源：http://hz.fzhhl.top/gtmbfjcixi.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.hammf.cn/gtjipdslhi.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.0kj1m.cn/gthdthhgfo.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.nanxuanxn.top/gtqmeovvkq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.hnxiangtu.top/gtoaedgqlg.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.daria6918.cn/gtmadifnrg.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.gaohongyu789.top/gtxgcsgbsp.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.sxryk.cn/gtgcpdwxgg.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.xylfe.cn/gteqgrkaxo.html

[D25] Set 集合去重与交并差
来源：http://hz.zhaomingkeji.xyz/gtiwqhiipb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.meibo888.top/gtbbesgcut.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.hnxiangtu.top/gtbslwiqgy.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.yuanzhike.top/gttzfdabyp.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.cashguo.top/gtbhjsqqse.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.havefunace.top/gtwedvukyu.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.haohaochexian.top/gtjfbsccjo.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.yangfankeji.com/gttpyhtrgf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.gzhubu.top/gtmxcafwht.html

[D26] 数组转字符串
来源：http://hz.dashuyun.cn/gtdzvvzjuh.html

Py:   ", ".join(map(str, arr))
来源：http://hz.hongshengwenyu.top/gtndtjnlln.html

PHP:  implode(", ", $arr);
来源：http://hz.jlsjyb.cn/gturupjmnd.html

JS:   arr.join(", ")
来源：http://hz.yangfankeji.com/gtmwjexkqw.html

TS:   arr.join(", ")
来源：http://hz.ywan-chungtsiang.top/gtfllcavbi.html

Java: String.join(", ", list)
来源：http://hz.cashguo.top/gthoamrqwz.html

Go:   strings.Join(strs, ", ")
来源：http://hz.xingfuxueyuan.xyz/gttvfbghxd.html

Ruby: arr.join(", ")
来源：http://hz.xylfe.cn/gthhiyxtqt.html

C#:   string.Join(", ", list)
来源：http://hz.nanxinkj.top/gtzpswhbxy.html

================================================================================
来源：http://hz.andypj.xyz/gtimxndbke.html

E. 字符串处理
来源：http://hz.sweek.top/gthtgdtweu.html

================================================================================
来源：http://hz.0kj1m.cn/gtyllpezgd.html

[E01] 拼接字符串
来源：http://hz.jinqigufen.top/gtketflndf.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.shanyushiyangtech.top/gtzcxrikdw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.ybcxt.top/gtzhcoyvrs.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.vqdsnc.cn/gtxbgfvmig.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.316326.xyz/gtgmocrsuz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.sufxvd.cn/gteaclrhna.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.cucudq.cn/gtocwybeal.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.yj20258888.top/gtphholdmy.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.yj20258.top/gtvszxkzij.html

[E02] 重复字符串
来源：http://hz.zhiwuduotai.top/gtwnfxddia.html

Py:   "ab" * 3
来源：http://hz.jqgufenzy.top/gthvnvdpvj.html

PHP:  str_repeat("ab", 3);
来源：http://hz.fzhhl.top/gtaxftotzy.html

JS:   "ab".repeat(3)
来源：http://hz.cqqwz.cn/gtptvuwnvb.html

TS:   "ab".repeat(3)
来源：http://hz.yanxiufei.cn/gtxxvprhxd.html

Java: "ab".repeat(3)
来源：http://hz.daxiang520.top/gtypvayvfo.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.yvedp.cn/gtslwcbxwn.html

Ruby: "ab" * 3
来源：http://hz.ydjk.org.cn/gtvotbuitk.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.daxiang520.top/gtyvaiwgke.html

[E03] 截取子串
来源：http://hz.shzxlz.cn/gtmdompuig.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.jyoumei.cn/gtpokfggbk.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.zhoulong.xyz/gtjrhtdffp.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.chenlongwang.top/gtsxkvgyid.html

TS:   s.slice(1, 4)
来源：http://hz.svipenyu.cn/gtotzpttza.html

Java: s.substring(1, 4)
来源：http://hz.dashuyun.cn/gtdfdkdgfn.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.redwolf501.top/gtucjeqbuo.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.redwolf501.top/gtfvojhkkk.html

C#:   s.Substring(1, 3)
来源：http://hz.quarkkingdee.top/gtwlwabztp.html

[E04] 查找子串位置
来源：http://hz.yj202588.top/gtubuffveh.html

Py:   s.find("x");  s.index("x")
来源：http://hz.jlsjyb.cn/gtwnhbxuhi.html

PHP:  strpos($s, "x");
来源：http://hz.hywenlv.cn/gtvmwuqglq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.jianghu66.top/gtogkrzcfz.html

TS:   s.indexOf("x")
来源：http://hz.fengsongda.top/gttyrjnukk.html

Java: s.indexOf("x")
来源：http://hz.hysaishi.cn/gtrortkhot.html

Go:   strings.Index(s, "x")
来源：http://hz.shuidangran.top/gtissxmcpg.html

Ruby: s.index("x")
来源：http://hz.smart0.xyz/gtjxplsygj.html

C#:   s.IndexOf("x")
来源：http://hz.xinyue.icu/gtwxufiwve.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.cqqwz.cn/gtshshhrab.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.yuanzhike.top/gtkvynoued.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.zycfv.cn/gtgwmphqlx.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.guowangkeji.top/gtuvjjunua.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.cdnleiting.top/gtswivuyqh.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.smart0.xyz/gtgghovelx.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.redwolf501.top/gtrothrzze.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.sweek.top/gtrxqfdawh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.aibaodan.cn/gtdagzpgzy.html

[E06] 替换子串
来源：http://hz.hfpthk.cn/gtjtfnocpv.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.wangdashe.top/gtdiogxfft.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.redwolf501.top/gtmvuvdqko.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.mhx1999.top/gtmsjjryqt.html

TS:   s.replaceAll("a", "b")
来源：http://hz.guannengcc.top/gtpbtgtcxm.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.nanxuanxn.top/gtktnmupva.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.shanyushiyangkeji.top/gtvqgwlvty.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.svipenyu.cn/gticnwcudg.html

C#:   s.Replace("a", "b")
来源：http://hz.zdqjudy.top/gtaotzzmam.html

[E07] 按分隔符拆分
来源：http://hz.jinqigufen.top/gtjqmrjjcm.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.hnqzz.top/gtpvnfwpkz.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.andypj.xyz/gtsxrmpyol.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.birdmap.top/gtfcyllmvq.html

TS:   s.split(",")
来源：http://hz.fzhhl.top/gtdlkvfojw.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.52xcode.cn/gttcigbaxa.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.redwolf501.top/gtocxnhlhn.html

Ruby: s.split(",");  s.split
来源：http://hz.bjfxy.top/gtudclpywt.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.iojbl.cn/gtmjjeffza.html

[E08] 数组按分隔符合并
来源：http://hz.yanxiufei.cn/gtuuxyhvcd.html

Py:   ",".join(items)
来源：http://hz.guowangkeji.top/gtixiaveth.html

PHP:  implode(",", $items);
来源：http://hz.0kj1m.cn/gtujgstzyp.html

JS:   items.join(",")
来源：http://hz.chenlongwang.top/gtpfznurei.html

TS:   items.join(",")
来源：http://hz.yj20258.top/gtkboqpuuq.html

Java: String.join(",", items)
来源：http://hz.smart0.xyz/gtvjjhhqtf.html

Go:   strings.Join(items, ",")
来源：http://hz.ppjwa.cn/gtgcjewnvb.html

Ruby: items.join(",")
来源：http://hz.wangshuangyany.cn/gthvemjtir.html

C#:   string.Join(",", items)
来源：http://hz.zhoulong.xyz/gtljggbddi.html

[E09] 去除所有空白字符
来源：http://hz.ydjk.org.cn/gtvdycgovz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.sxryk.cn/gthezlrnmq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.yueranfly.top/gtijlxndnm.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.shangyingyoupin.top/gtmvtmurit.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.xinyue.icu/gtaiqwhaas.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.redwolf501.top/gtdnjzogfu.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.xingfuxueyuan.xyz/gtkddwzatx.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.iojbl.cn/gtpoxqvvak.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.ivvv.top/gtlsyxddhv.html

[E10] 左侧补零 / 定长填充
来源：http://hz.ydzc1.top/gtnpkjkgbz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.jianghu66.top/gtenrvbrvp.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.yongpay.top/gtfgzzzymu.html

JS:   "7".padStart(3, "0")
来源：http://hz.fzhhl.top/gtorkorapn.html

TS:   "7".padStart(3, "0")
来源：http://hz.ybcxt.top/gtxpozbdfo.html

Java: String.format("%03d", 7)
来源：http://hz.hammf.cn/gtkwnqikxl.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.ehwqpu.com/gtotgxljuy.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.chenjidiqi.icu/gtnidvjpkk.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.jinqigfzy.top/gtfuzxzgzf.html

[E11] 反转字符串
来源：http://hz.birdmap.top/gtuazgdakn.html

Py:   s[::-1]
来源：http://hz.mhx1999.top/gtaxwxgokh.html

PHP:  strrev($s);
来源：http://hz.bjfxy.top/gtwiidhgwq.html

JS:   [...s].reverse().join("")
来源：http://hz.yongpay.top/gtaxnxeyvl.html

TS:   [...s].reverse().join("")
来源：http://hz.jiagoushi.top/gtzcumonxm.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.shangyingyoupin.top/gtrhhxccsy.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.chenjidiqi.icu/gtrndcsozc.html

Ruby: s.reverse
来源：http://hz.guowangkeji.top/gtaakxkiqk.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.snrcjt.cn/gtseifielb.html

[E12] 统计某字符出现次数
来源：http://hz.svipenyu.cn/gtpoycfxlw.html

Py:   s.count("a")
来源：http://hz.zycfv.cn/gtsxgguhqc.html


<!-- 参考信息 -->