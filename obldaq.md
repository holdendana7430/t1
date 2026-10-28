代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.redwolf501.top/gtdxpeodtk.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.yueranfly.top/gtycqbwkpo.html

[D05] 访问与修改元素
来源：http://hz.andypj.xyz/gtemhxibbk.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jinqigfzy.top/gtynozmboz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.jinqigufen.top/gtszjuqvtm.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.tanke756.top/gtkohukhcj.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.daxiang520.top/gtvryxcxwa.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.ybcxt.top/gtcefeaqxk.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.chenlongwang.top/gtyjvgiwdt.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.ivvv.top/gtyrvhiuwv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.ydjk.org.cn/gtwluteuzl.html

[D06] 数组长度
来源：http://hz.zycfv.cn/gtjvhltmnl.html

Py:   len(arr)
来源：http://hz.jqgfzy.top/gtyvmievdc.html

PHP:  count($arr);
来源：http://hz.jinqigufen.top/gtphktslsp.html

JS:   arr.length
来源：http://hz.wangdashe.top/gtppytucci.html

TS:   arr.length
来源：http://hz.nanxuanxn.top/gtdlbmaxnw.html

Java: list.size();
来源：http://hz.jinqigfzy.top/gtiutpiumb.html

Go:   len(arr)
来源：http://hz.ybcxt.top/gtxeupdyql.html

Ruby: arr.length; arr.size
来源：http://hz.zhaomingkeji.xyz/gtngbheuuq.html

C#:   list.Count;
来源：http://hz.hnxiangtu.top/gtktksbuhb.html

[D07] 切片 / 取子数组
来源：http://hz.zhiwuduotai.top/gtnpbqavmn.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.jiagoushi.top/gtzevupmjo.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.gogol.net.cn/gtgrwdgdtl.html

JS:   arr.slice(1, 4);
来源：http://hz.gogol.net.cn/gtlcgwlfqx.html

TS:   arr.slice(1, 4);
来源：http://hz.yuanzhike.top/gtffoiigku.html

Java: list.subList(1, 4);
来源：http://hz.ehwqpu.com/gtcekuwcrv.html

Go:   arr[1:4]
来源：http://hz.hongshengwenyu.top/gtryxiqdmp.html

Ruby: arr[1, 3]
来源：http://hz.sxryk.cn/gtegdyrrll.html

C#:   list.GetRange(1, 3);
来源：http://hz.cheryme.top/gtpcaqzegt.html

[D08] 合并两个数组
来源：http://hz.c1oappe.top/gtqiuozond.html

Py:   a + b;  a.extend(b)
来源：http://hz.iojbl.cn/gtadczwhdy.html

PHP:  array_merge($a, $b);
来源：http://hz.guannengcc.top/gtunudenvv.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.aizwys.cn/gtqofmmrxd.html

TS:   [...a, ...b];
来源：http://hz.gaohongyu789.top/gtwxltpgdm.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.cucudq.cn/gtkexswczx.html

Go:   append(a, b...)
来源：http://hz.fengsongda.top/gteyhcjkni.html

Ruby: a + b;  a.concat(b)
来源：http://hz.wangshuangyany.cn/gtosbgwfxd.html

C#:   a.Concat(b).ToList()
来源：http://hz.xinyue.icu/gtktriahts.html

[D09] 排序（升序）
来源：http://hz.zhijiandao.cn/gtddiuppwb.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.vqdsnc.cn/gtrclwwwkp.html

PHP:  sort($arr);
来源：http://hz.zhixingplan.top/gtbtvospch.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.jiagoushi.top/gtfhfzdthn.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.tianlin.xyz/gtcapvaxoh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.snrcjt.cn/gtovvknplb.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.hysaishi.cn/gtzmtvygvt.html

Ruby: arr.sort
来源：http://hz.iojbl.cn/gtdthttpaw.html

C#:   list.Sort();
来源：http://hz.0kj1m.cn/gtcjmfgpgv.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.jqgufenzy.top/gtebidgplz.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.chenlongwang.top/gtqjnhwxnz.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yuanzhike.top/gtwjztpood.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.cashguo.top/gtycxbnjal.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yj20258.top/gtshroocdp.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.wangshuangyany.cn/gtwpiawydg.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.chenlongwang.top/gtjlkonjck.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.vqdsnc.cn/gtijdequkw.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.cqqwz.cn/gtfhiltsno.html

[D11] 反转数组
来源：http://hz.52xcode.cn/gtdxkognhe.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.xingfuxueyuan.xyz/gtvgudkylg.html

PHP:  array_reverse($arr);
来源：http://hz.wangshuangyany.cn/gtprqblgkz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.jinghuilouyu.cn/gtxtpbfpkj.html

TS:   [...arr].reverse();
来源：http://hz.xingfuxueyuan.xyz/gtbjrsqqxo.html

Java: Collections.reverse(list);
来源：http://hz.sysykeji.top/gtzqczmnxo.html

Go:   slices.Reverse(arr)
来源：http://hz.aizwys.cn/gtcaelpgkh.html

Ruby: arr.reverse
来源：http://hz.fengsongda.top/gtmntvmqfu.html

C#:   list.Reverse();
来源：http://hz.kuanghao11.cn/gtksdhhxsu.html

[D12] 查找元素下标
来源：http://hz.daria6918.cn/gtlqjqnsgw.html

Py:   arr.index(x);  x in arr
来源：http://hz.guannengcc.top/gtxcmgbohu.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.iojbl.cn/gtjwttchbw.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.meibo888.top/gtubtonquv.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zhiwuduotai.top/gtpceomclg.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.hnqzz.top/gtzjuvznxu.html

Go:   slices.Index(arr, x)
来源：http://hz.yueranfly.top/gtwyqckuth.html

Ruby: arr.index(x)
来源：http://hz.quarkkingdee.top/gtjrnbfimn.html

C#:   list.IndexOf(x);
来源：http://hz.shuidangran.top/gtndonfbqy.html

[D13] 过滤（保留满足条件的）
来源：http://hz.yuanzhike.top/gtcsehvgni.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.shuidangran.top/gtkngfamdn.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.chenzaomai.com/gtdkvgncrx.html

JS:   arr.filter(x => x > 3)
来源：http://hz.zdqjudy.top/gtllkpwdhj.html

TS:   arr.filter(x => x > 3)
来源：http://hz.hywenlv.cn/gtxtlngvaf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.xziqi.cn/gtcbogzkwg.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.jyoumei.cn/gtmkrtmkad.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.havefunace.top/gtaeiwaaua.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.hnxiangtu.top/gtxbnxcieq.html

[D14] 映射转换（每个元素变形）
来源：http://hz.pengpengdd.cyou/gtpnqemoth.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.zdqjudy.top/gtlvbfhyvh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.sweek.top/gtucjogsjl.html

JS:   arr.map(x => x * 2)
来源：http://hz.shuidangran.top/gtzykmzbcx.html

TS:   arr.map(x => x * 2)
来源：http://hz.zdqjudy.top/gtqaqwoaly.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.shanyushiyangkeji.top/gteogepmbx.html

Go:   // 手写循环
来源：http://hz.birdmap.top/gtihhwijdc.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.9152youxi.cn/gtimpmnwqo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.zhengqikj.top/gtwilclppp.html

[D15] 去重
来源：http://hz.ydjk.org.cn/gtdwwhiyjo.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.wangdashe.top/gtmrvmhsgd.html

PHP:  array_unique($arr);
来源：http://hz.wangdashe.top/gtkvgxejvp.html

JS:   [...new Set(arr)]
来源：http://hz.yanxiufei.cn/gtyaepwnuh.html

TS:   [...new Set(arr)]
来源：http://hz.jyoumei.cn/gtrysrsayk.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.dianchejie.cn/gtazvrlupj.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.zdqjudy.top/gtudyzkxvj.html

Ruby: arr.uniq
来源：http://hz.zhijiandao.cn/gtjxcdqvqp.html

C#:   list.Distinct().ToList()
来源：http://hz.xuetiantiany.cn/gtztxnjuja.html

[D16] 求和与平均值
来源：http://hz.jinqigufen.top/gtuknrtbgd.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.chenlongwang.top/gthfhohhmd.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.c1oappe.top/gtrjjroxxq.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hongshengwenyu.top/gtlkciozoi.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yonumen.top/gtwhlavhmh.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.xylfe.cn/gtpyfplfhc.html

Go:   // 手写循环累加
来源：http://hz.hysaishi.cn/gtrjfushug.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.nanxuanxn.top/gtmqrrbtov.html

C#:   list.Sum();  list.Average()
来源：http://hz.wangshuangyany.cn/gtzairiaoz.html

[D17] 最大值与最小值
来源：http://hz.zhiwuduotai.top/gtouukvvdo.html

Py:   max(arr);  min(arr)
来源：http://hz.pycfn.com/gthykclbjm.html

PHP:  max($arr);  min($arr);
来源：http://hz.mhx1999.top/gtbrqqqwyx.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.xingfuxueyuan.xyz/gttlcgguwr.html

TS:   Math.max(...arr);
来源：http://hz.guowangkeji.top/gtqiyozchm.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.shanyushiyangkeji.top/gtazmrsipw.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.dashuyun.cn/gtqjnsfyaw.html

Ruby: arr.max;  arr.min
来源：http://hz.xuanzx.com/gtuxrbwocz.html

C#:   list.Max();  list.Min()
来源：http://hz.hywenlv.cn/gteailnovj.html

[D18] 扁平化嵌套数组
来源：http://hz.yueranfly.top/gtycwchudz.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.tianlin.xyz/gthtujvmze.html

PHP:  array_merge(...$nested);
来源：http://hz.gotoacloud.top/gtjwwsleir.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.guowangkeji.top/gtbystrnpm.html

TS:   nested.flat();
来源：http://hz.gotoacloud.top/gtldlzohqh.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.andypj.xyz/gtwntpvwbw.html

Go:   // 手写双层循环
来源：http://hz.vqdsnc.cn/gtaperdhzq.html

Ruby: nested.flatten
来源：http://hz.zhaomingkeji.xyz/gtlclovaph.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.zhijiandao.cn/gtadmigwby.html

[D19] 按字段分组
来源：http://hz.0kj1m.cn/gtphwrgnwt.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.zhiwuduotai.top/gtrrlxonnw.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.hnxiangtu.top/gtlqpspptu.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.xingfuxueyuan.xyz/gtmtfirrel.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.yj20258.top/gtemnddqnl.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.zhongyouzk.top/gtjpjwaamr.html

Go:   // 手写 map[string][]T
来源：http://hz.xylfe.cn/gtcisayivx.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.smart0.xyz/gtybnndcjl.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.guannengcc.top/gtdutakjrt.html

[D20] 统计每个元素出现次数
来源：http://hz.jyoumei.cn/gtjjpbgrwi.html

Py:   Counter(arr)
来源：http://hz.jinghuilouyu.cn/gtwtnxvdnx.html

PHP:  array_count_values($arr);
来源：http://hz.yj202588.top/gtymglqxgt.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.dianchejie.cn/gtdnqtzrya.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zhoulong.xyz/gtcboadvug.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.0kj1m.cn/gtnnsrfwit.html

Go:   // 手写 map[T]int
来源：http://hz.jinghuilouyu.cn/gttftfyecd.html

Ruby: arr.tally
来源：http://hz.chenlongwang.top/gtbpkdynjj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.dianchejie.cn/gtphqwosxt.html

[D21] 判断是否包含某元素
来源：http://hz.ywan-chungtsiang.top/gtvgycxrnr.html

Py:   x in arr
来源：http://hz.yangfankeji.com/gtzkhhuybz.html

PHP:  in_array($x, $arr, true);
来源：http://hz.aibaodan.cn/gtyemxgara.html

JS:   arr.includes(x)
来源：http://hz.c1oappe.top/gtpyoxdsbc.html

TS:   arr.includes(x)
来源：http://hz.havefunace.top/gtefsimwtw.html

Java: list.contains(x)
来源：http://hz.yanxiufei.cn/gtadwkmlnp.html

Go:   slices.Contains(arr, x)
来源：http://hz.jqgufenzy.top/gtsmupjtnz.html

Ruby: arr.include?(x)
来源：http://hz.sysykeji.top/gtfzlsspkb.html

C#:   list.Contains(x)
来源：http://hz.jqgfzy.top/gtewiggibb.html

[D22] 复制数组（避免共享引用）
来源：http://hz.jianghu66.top/gtvcdknskv.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.zhongyouzk.top/gtwikxxnct.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.ydjk.org.cn/gtdfsaigon.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.birdmap.top/gtaulbbqlw.html

TS:   [...arr];
来源：http://hz.bjfxy.top/gtdfeepjvd.html

Java: new ArrayList<>(list);
来源：http://hz.ywan-chungtsiang.top/gtpiqwlete.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.zhengqikj.top/gtkdigprhv.html

Ruby: arr.dup;  arr.clone
来源：http://hz.jlsjyb.cn/gtgeugjyjf.html

C#:   new List<int>(list);
来源：http://hz.9152youxi.cn/gtjvzkuley.html

[D23] reduce 累积计算
来源：http://hz.jinqigfzy.top/gtotjrhmnm.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.daxiang520.top/gtwhvnmmpq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.yvedp.cn/gthoyvecwl.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.dianchejie.cn/gtgkihqwys.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.cashguo.top/gtnnwelycy.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.snrcjt.cn/gtoxmumbml.html

Go:   // 手写循环
来源：http://hz.zdqjudy.top/gttwvkiiyf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.jqgfzy.top/gtnqiukulg.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.chenjidiqi.icu/gtpghgcevi.html

[D24] 字典 / Map 基本操作
来源：http://hz.iojbl.cn/gtxxadrbjx.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.gaohongyu789.top/gtscqibbbb.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.yueranfly.top/gtbfqvkumd.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.shuidangran.top/gtxulutaqf.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.yj20258888.top/gthzmuempq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.ybcxt.top/gtomkbiasa.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.hnqzz.top/gtmamjdfhs.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.nanxinkj.top/gtcflthduv.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.hnqzz.top/gtvaqabyub.html

[D25] Set 集合去重与交并差
来源：http://hz.yuxming.cn/gtybeutpqu.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.xylfe.cn/gtevbzrqcw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.daria6918.cn/gtrckslmvy.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.yangfankeji.com/gttfaspjmf.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.zhengqikj.top/gtsarplfyw.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.ppjwa.cn/gtcpugphzt.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.kuanghao11.cn/gtefzburru.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.nanxinkj.top/gtumacflbt.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.jqgfzy.top/gtxhqjpjma.html

[D26] 数组转字符串
来源：http://hz.chenlongwang.top/gtutxffmkr.html

Py:   ", ".join(map(str, arr))
来源：http://hz.shanyushiyangtech.top/gtknynjxzs.html

PHP:  implode(", ", $arr);
来源：http://hz.ivvv.top/gtdqmvcrqx.html

JS:   arr.join(", ")
来源：http://hz.redwolf501.top/gtgwmsrcrh.html

TS:   arr.join(", ")
来源：http://hz.9152youxi.cn/gtctxuxinz.html

Java: String.join(", ", list)
来源：http://hz.vqdsnc.cn/gtnugsheqa.html

Go:   strings.Join(strs, ", ")
来源：http://hz.tian-w.cn/gtvtwzyogr.html

Ruby: arr.join(", ")
来源：http://hz.52xcode.cn/gtrhjdvxhb.html

C#:   string.Join(", ", list)
来源：http://hz.yj20258.top/gtqpsjjngr.html

================================================================================
来源：http://hz.hammf.cn/gtgrdniehi.html

E. 字符串处理
来源：http://hz.cdnleiting.top/gtkeptrbef.html

================================================================================
来源：http://hz.sxryk.cn/gtdhupjdpc.html

[E01] 拼接字符串
来源：http://hz.xinyue.icu/gtmxmrzkao.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.xuetiantiany.cn/gtcszwbdyz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.yj20258.top/gtaujguqml.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.havefunace.top/gtikrwgyev.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ydzc1.top/gtikylwhka.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.zycfv.cn/gtweguybnu.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.redwolf501.top/gthxmwkzls.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.shzxlz.cn/gtvngarcur.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.zhaomingkeji.xyz/gtfqxbrdfo.html

[E02] 重复字符串
来源：http://hz.ppjwa.cn/gtpiulkygx.html

Py:   "ab" * 3
来源：http://hz.wangshuangyany.cn/gtigaegipd.html

PHP:  str_repeat("ab", 3);
来源：http://hz.dashuyun.cn/gtbbakqqtv.html

JS:   "ab".repeat(3)
来源：http://hz.hammf.cn/gtkaftuwuw.html

TS:   "ab".repeat(3)
来源：http://hz.shuidangran.top/gtcarzfheb.html

Java: "ab".repeat(3)
来源：http://hz.hammf.cn/gtovimhdhn.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.ybcxt.top/gtonoeccsy.html

Ruby: "ab" * 3
来源：http://hz.cucudq.cn/gtlhrnlaea.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.jinghuilouyu.cn/gtfdspxfxd.html

[E03] 截取子串
来源：http://hz.dashuyun.cn/gtdrmkljiu.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.quarkkingdee.top/gtalahyqmf.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.0kj1m.cn/gttjayzmgh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.nanxinkj.top/gtgqnqzuvh.html

TS:   s.slice(1, 4)
来源：http://hz.jqgufenzy.top/gtlzjgmyai.html

Java: s.substring(1, 4)
来源：http://hz.redwolf501.top/gtfwilocou.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.jqgfzy.top/gtczjbepme.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.chenjidiqi.icu/gtyyvxfdrp.html

C#:   s.Substring(1, 3)
来源：http://hz.gotoacloud.top/gtqmnvqxuo.html

[E04] 查找子串位置
来源：http://hz.haohaochexian.top/gttycuvlao.html

Py:   s.find("x");  s.index("x")
来源：http://hz.ydjk.org.cn/gtjhqyuuzl.html

PHP:  strpos($s, "x");
来源：http://hz.kuanghao11.cn/gtgcrjyehv.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.feifeiyinyue.top/gtsbtgsdzh.html

TS:   s.indexOf("x")
来源：http://hz.hammf.cn/gtdaznvahq.html

Java: s.indexOf("x")
来源：http://hz.fzhhl.top/gtpqgruhqn.html

Go:   strings.Index(s, "x")
来源：http://hz.zhijiandao.cn/gtsiastdsh.html

Ruby: s.index("x")
来源：http://hz.cucudq.cn/gtluksfejf.html

C#:   s.IndexOf("x")
来源：http://hz.kuanghao11.cn/gtqrotzwzl.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.52xcode.cn/gtzqobtlej.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.hysaishi.cn/gtbbvjinkr.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.zycfv.cn/gtxjtgdedb.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.quarkkingdee.top/gtjdyrjhzz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.zhoulong.xyz/gtpvrhknhn.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.quarkkingdee.top/gtglmpgwdb.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.yvedp.cn/gtxeuwdqio.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.hongshengwenyu.top/gtezfahkvh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.yj20258.top/gtbbntbkmj.html

[E06] 替换子串
来源：http://hz.jiagoushi.top/gtsjtwdxvt.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.jlsjyb.cn/gtnewzwpcg.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.hysaishi.cn/gtxydzcysd.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.svipenyu.cn/gtekmynqkq.html

TS:   s.replaceAll("a", "b")
来源：http://hz.mhx1999.top/gtsyrqubdo.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jiagoushi.top/gtfnnfitse.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.52xcode.cn/gtgsieskwt.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.gaohongyu789.top/gtyloitrde.html

C#:   s.Replace("a", "b")
来源：http://hz.zhengqikj.top/gtztfruscc.html

[E07] 按分隔符拆分
来源：http://hz.zycfv.cn/gtlpavqxma.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.ppjwa.cn/gtwqmgfbkr.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.yongpay.top/gtwjfjuctm.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.jianghu66.top/gtzonitslh.html

TS:   s.split(",")
来源：http://hz.gaohongyu789.top/gtdimfldgp.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.jinghuilouyu.cn/gtlmvjvfik.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.jinqigufen.top/gtookygmhh.html

Ruby: s.split(",");  s.split
来源：http://hz.ybcxt.top/gtgvzjdeha.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.pycfn.com/gtsdbfjcts.html

[E08] 数组按分隔符合并
来源：http://hz.mhx1999.top/gtdmwrcedr.html

Py:   ",".join(items)
来源：http://hz.meibo888.top/gtsymwkbez.html

PHP:  implode(",", $items);
来源：http://hz.fengsongda.top/gtfosvfgkn.html

JS:   items.join(",")
来源：http://hz.yangfankeji.com/gtptwmqavn.html

TS:   items.join(",")
来源：http://hz.52xcode.cn/gthapmtqpu.html

Java: String.join(",", items)
来源：http://hz.jlsjyb.cn/gtdbhsqupp.html

Go:   strings.Join(items, ",")
来源：http://hz.yangfankeji.com/gththwvcwj.html

Ruby: items.join(",")
来源：http://hz.yangfankeji.com/gtofvxvdqw.html

C#:   string.Join(",", items)
来源：http://hz.yuxming.cn/gtvmkcuunw.html

[E09] 去除所有空白字符
来源：http://hz.andypj.xyz/gtcicslaac.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.zhixingplan.top/gtxugelpzq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.ivvv.top/gtbewehwvo.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.zycfv.cn/gtyhcmhwqd.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.nwbrower.top/gtcfxzsbjw.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.ydjk.org.cn/gtrgpfddvh.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.daxiang520.top/gtsveaqvnb.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.snrcjt.cn/gtfhvsdzkp.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.jinqigfzy.top/gtzbmkhhvj.html

[E10] 左侧补零 / 定长填充
来源：http://hz.hammf.cn/gtnhskbxnm.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.vqdsnc.cn/gtdlrsiszc.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.cqqwz.cn/gtzkxmfszq.html

JS:   "7".padStart(3, "0")
来源：http://hz.jyoumei.cn/gtncdicymy.html

TS:   "7".padStart(3, "0")
来源：http://hz.wangshuangyany.cn/gtvreyqgvm.html

Java: String.format("%03d", 7)
来源：http://hz.aizwys.cn/gtbbbjymcm.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.gzhubu.top/gtfmjftrsg.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.shzxlz.cn/gtyigigkbv.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.sysykeji.top/gtmxuxudwp.html

[E11] 反转字符串
来源：http://hz.yueranfly.top/gtfpptfbaq.html

Py:   s[::-1]
来源：http://hz.svipenyu.cn/gtsheiffux.html

PHP:  strrev($s);
来源：http://hz.meibo888.top/gtwdmagobq.html

JS:   [...s].reverse().join("")
来源：http://hz.jinqigfzy.top/gtpwdfdzup.html

TS:   [...s].reverse().join("")
来源：http://hz.xuetiantiany.cn/gtrregudvz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.yueranfly.top/gtiavhduil.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.gaohongyu789.top/gtcpmlcqyi.html


<!-- 参考信息 -->