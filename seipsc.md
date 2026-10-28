代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.birdmap.top/gthohmjsqf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.zhongyouzk.top/gthsetdiha.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.cashguo.top/gtoprjbixa.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.jqgufenzy.top/gtqapofgow.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.xuanzx.com/gtplrbikap.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.wangdashe.top/gtzwmusxdb.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.cheryme.top/gtxkngnmgb.html

[D06] 数组长度
来源：http://hz.jinyuanbaomall.cn/gthhqweilk.html

Py:   len(arr)
来源：http://hz.xinyue.icu/gtplbiiyhd.html

PHP:  count($arr);
来源：http://hz.yvedp.cn/gtydbfounh.html

JS:   arr.length
来源：http://hz.jiagoushi.top/gtyhfnzqih.html

TS:   arr.length
来源：http://hz.andypj.xyz/gtjolcnliz.html

Java: list.size();
来源：http://hz.chenzaomai.com/gtacgqzlmm.html

Go:   len(arr)
来源：http://hz.redwolf501.top/gtrhvipjcb.html

Ruby: arr.length; arr.size
来源：http://hz.wangshuangyany.cn/gtgjbzcgrf.html

C#:   list.Count;
来源：http://hz.chenjidiqi.icu/gtepcuehqx.html

[D07] 切片 / 取子数组
来源：http://hz.tanke756.top/gtririaidd.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.cdnleiting.top/gthcrfvpsu.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.quarkkingdee.top/gtskdefatr.html

JS:   arr.slice(1, 4);
来源：http://hz.pycfn.com/gtmpqbyyht.html

TS:   arr.slice(1, 4);
来源：http://hz.xziqi.cn/gtdhuaqmlv.html

Java: list.subList(1, 4);
来源：http://hz.hysaishi.cn/gtimvjqwdm.html

Go:   arr[1:4]
来源：http://hz.jinghuilouyu.cn/gtbqiyofyh.html

Ruby: arr[1, 3]
来源：http://hz.hysaishi.cn/gttodambja.html

C#:   list.GetRange(1, 3);
来源：http://hz.yj20258888.top/gthdhshicv.html

[D08] 合并两个数组
来源：http://hz.fzhhl.top/gtmvrgenck.html

Py:   a + b;  a.extend(b)
来源：http://hz.sweek.top/gtwjoubbrk.html

PHP:  array_merge($a, $b);
来源：http://hz.hywenlv.cn/gttzgyviib.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.meibo888.top/gtwrtyxovg.html

TS:   [...a, ...b];
来源：http://hz.zhoulong.xyz/gtrupmmmue.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.gogol.net.cn/gtgjsozgzl.html

Go:   append(a, b...)
来源：http://hz.fengsongda.top/gtvoeoslyu.html

Ruby: a + b;  a.concat(b)
来源：http://hz.gaohongyu789.top/gtoaixlydh.html

C#:   a.Concat(b).ToList()
来源：http://hz.zhixingplan.top/gtvvwtulwa.html

[D09] 排序（升序）
来源：http://hz.jqgufenzy.top/gtiswxfssb.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yongpay.top/gtdhztuxag.html

PHP:  sort($arr);
来源：http://hz.snrcjt.cn/gtscscwyrl.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.hnqzz.top/gtjnmuvzrw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.yangfankeji.com/gtjxnsdqxx.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.jqgfzy.top/gtpvzxgliy.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.dashuyun.cn/gtvbfyfilw.html

Ruby: arr.sort
来源：http://hz.jinqigufen.top/gtemnwydld.html

C#:   list.Sort();
来源：http://hz.c1oappe.top/gtxzaytbpa.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.aizwys.cn/gtlcvuzewj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.redwolf501.top/gtfygqmaht.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zhoulong.xyz/gtpcpvukhc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xingfuxueyuan.xyz/gtnspbappd.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yuxming.cn/gtzgurodta.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.ehwqpu.com/gteyvfqgxk.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.sysykeji.top/gtrzjqxdnr.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.yanxiufei.cn/gtekbrazuz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.andypj.xyz/gtkskcflmf.html

[D11] 反转数组
来源：http://hz.hnqzz.top/gtarmfmjsr.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.zycfv.cn/gtsbbqlaue.html

PHP:  array_reverse($arr);
来源：http://hz.snrcjt.cn/gthzyzijeb.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.hfpthk.cn/gtauhkushg.html

TS:   [...arr].reverse();
来源：http://hz.chenzaomai.com/gtoixeosnk.html

Java: Collections.reverse(list);
来源：http://hz.jianghu66.top/gtozznfyfq.html

Go:   slices.Reverse(arr)
来源：http://hz.chenzaomai.com/gteqcimoao.html

Ruby: arr.reverse
来源：http://hz.yanxiufei.cn/gtrgtvyxht.html

C#:   list.Reverse();
来源：http://hz.nanxinkj.top/gtywvdhrve.html

[D12] 查找元素下标
来源：http://hz.iojbl.cn/gtseverqnp.html

Py:   arr.index(x);  x in arr
来源：http://hz.xinyue.icu/gtbqbpbfbj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.yj20258888.top/gtnrpqsnha.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zdqjudy.top/gtgordcdam.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.guowangkeji.top/gtrpqfaegn.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.feifeiyinyue.top/gtulichplq.html

Go:   slices.Index(arr, x)
来源：http://hz.fzhhl.top/gtsaalwgjn.html

Ruby: arr.index(x)
来源：http://hz.jianghu66.top/gtmuasvmyl.html

C#:   list.IndexOf(x);
来源：http://hz.redwolf501.top/gthcfnnalw.html

[D13] 过滤（保留满足条件的）
来源：http://hz.jqgfzy.top/gtsyqucmbr.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.hywenlv.cn/gtrokhpfhn.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.zhiwuduotai.top/gtyvwglclr.html

JS:   arr.filter(x => x > 3)
来源：http://hz.ivvv.top/gtlodlczoe.html

TS:   arr.filter(x => x > 3)
来源：http://hz.sysykeji.top/gtozpgrhsc.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.bjfxy.top/gtgkjxurhu.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.nwbrower.top/gttklfdbuh.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.hysaishi.cn/gtzrgrnenn.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.sxryk.cn/gtxcxbrlld.html

[D14] 映射转换（每个元素变形）
来源：http://hz.cashguo.top/gthmnuhlrt.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.aizwys.cn/gtlqwmfnwc.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.sxryk.cn/gtkypvnvmf.html

JS:   arr.map(x => x * 2)
来源：http://hz.yj20258.top/gthybfnpwb.html

TS:   arr.map(x => x * 2)
来源：http://hz.fzhhl.top/gtziuyqdqy.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.daria6918.cn/gtsesacgmr.html

Go:   // 手写循环
来源：http://hz.quarkkingdee.top/gtccfkjbne.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.yuanzhike.top/gtahusagok.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.ydzc1.top/gtsgnqatwu.html

[D15] 去重
来源：http://hz.xylfe.cn/gtlhllhfvy.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.birdmap.top/gtowcixrzy.html

PHP:  array_unique($arr);
来源：http://hz.ppjwa.cn/gtvgmyiigk.html

JS:   [...new Set(arr)]
来源：http://hz.jqgufenzy.top/gtwafbsolg.html

TS:   [...new Set(arr)]
来源：http://hz.chenjidiqi.icu/gtwfxiddly.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.tian-w.cn/gttsxfaqfg.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.chenzaomai.com/gttcnljkyv.html

Ruby: arr.uniq
来源：http://hz.jyoumei.cn/gtgqhnkedz.html

C#:   list.Distinct().ToList()
来源：http://hz.smart0.xyz/gtibnekpxn.html

[D16] 求和与平均值
来源：http://hz.yueranfly.top/gttchdoidy.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.wangshuangyany.cn/gtchkjjfyg.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.fzhhl.top/gtxwtwjych.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zhiwuduotai.top/gtxrhhjjmk.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.sxryk.cn/gtmxmdzsts.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.birdmap.top/gtbluscven.html

Go:   // 手写循环累加
来源：http://hz.zhaomingkeji.xyz/gtprcctckh.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.zycfv.cn/gtecjhoeqm.html

C#:   list.Sum();  list.Average()
来源：http://hz.chenlongwang.top/gtjfvwghbu.html

[D17] 最大值与最小值
来源：http://hz.xinyue.icu/gthroebmyg.html

Py:   max(arr);  min(arr)
来源：http://hz.jyoumei.cn/gtniqwwbrt.html

PHP:  max($arr);  min($arr);
来源：http://hz.yvedp.cn/gtkmsjeguu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.xziqi.cn/gtuumqmltb.html

TS:   Math.max(...arr);
来源：http://hz.aizwys.cn/gtozdhybac.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.zhijiandao.cn/gtrqkacvxl.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.xinyue.icu/gttgehqmqz.html

Ruby: arr.max;  arr.min
来源：http://hz.yonumen.top/gtnnltqbkb.html

C#:   list.Max();  list.Min()
来源：http://hz.cdnleiting.top/gtsxzivzcm.html

[D18] 扁平化嵌套数组
来源：http://hz.yj20258888.top/gtphgvlhzd.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.ybcxt.top/gtxorkxlcx.html

PHP:  array_merge(...$nested);
来源：http://hz.guannengcc.top/gtjddttfjs.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.xziqi.cn/gtuczumoiy.html

TS:   nested.flat();
来源：http://hz.snrcjt.cn/gtcmldyecl.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.pycfn.com/gtldvizvtp.html

Go:   // 手写双层循环
来源：http://hz.kuanghao11.cn/gtxcrgwgwa.html

Ruby: nested.flatten
来源：http://hz.aizwys.cn/gtoykyfnyv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.cdnleiting.top/gtbdgsgtxk.html

[D19] 按字段分组
来源：http://hz.jyoumei.cn/gtkxliewoy.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.wangshuangyany.cn/gttaovcfsy.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.tianlin.xyz/gtewpdngry.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.daxiang520.top/gtlijzjpkq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.ywan-chungtsiang.top/gtgcfzzxrp.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.gotoacloud.top/gtjxgjtaxj.html

Go:   // 手写 map[string][]T
来源：http://hz.yanxiufei.cn/gtfuxvgkxm.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.jqgfzy.top/gtgbfzrgvh.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.jqgfzy.top/gtgjffpjdd.html

[D20] 统计每个元素出现次数
来源：http://hz.ydjk.org.cn/gtlgvyofor.html

Py:   Counter(arr)
来源：http://hz.wangdashe.top/gtxkvtntuo.html

PHP:  array_count_values($arr);
来源：http://hz.redwolf501.top/gtumpfugyc.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.haohaochexian.top/gtjjdwyoip.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yangfankeji.com/gtbtqmqyzu.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.jinqigufen.top/gtkrsjwjms.html

Go:   // 手写 map[T]int
来源：http://hz.fzhhl.top/gttsnjjlkg.html

Ruby: arr.tally
来源：http://hz.wangshuangyany.cn/gtayqlfatw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.fzhhl.top/gtodxzgiqa.html

[D21] 判断是否包含某元素
来源：http://hz.hongshengwenyu.top/gtxfwhdfjv.html

Py:   x in arr
来源：http://hz.yj202588.top/gtpvlsktbl.html

PHP:  in_array($x, $arr, true);
来源：http://hz.chenlongwang.top/gtafpbrrae.html

JS:   arr.includes(x)
来源：http://hz.hnqzz.top/gtihvlnmpz.html

TS:   arr.includes(x)
来源：http://hz.jinqigfzy.top/gtwwwqmopf.html

Java: list.contains(x)
来源：http://hz.ehwqpu.com/gtzhornpnw.html

Go:   slices.Contains(arr, x)
来源：http://hz.pengpengdd.cyou/gtbkifmlse.html

Ruby: arr.include?(x)
来源：http://hz.nanxinkj.top/gtpjuzsbae.html

C#:   list.Contains(x)
来源：http://hz.c1oappe.top/gtimzldwuv.html

[D22] 复制数组（避免共享引用）
来源：http://hz.aizwys.cn/gtzpnfrqun.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.hfpthk.cn/gtbonhdbtp.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.jiagoushi.top/gtkqpdzvjr.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.ydzc1.top/gtrlvgukvs.html

TS:   [...arr];
来源：http://hz.andypj.xyz/gtjycsltyb.html

Java: new ArrayList<>(list);
来源：http://hz.cdnleiting.top/gtnqqfvgcu.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.xylfe.cn/gtpfccdexm.html

Ruby: arr.dup;  arr.clone
来源：http://hz.ybcxt.top/gtrkelyxhf.html

C#:   new List<int>(list);
来源：http://hz.nwbrower.top/gtmdjhlond.html

[D23] reduce 累积计算
来源：http://hz.9152youxi.cn/gtwxgttyvb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.quarkkingdee.top/gtuvtsbpva.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.jqgufenzy.top/gtbjctlmly.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yangfankeji.com/gtodtuywwj.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.snrcjt.cn/gtnikhavvy.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.yj202588.top/gtbetjvhec.html

Go:   // 手写循环
来源：http://hz.haohaochexian.top/gtvhkqbile.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.svipenyu.cn/gtfgclatvb.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.ywan-chungtsiang.top/gtwnsonlzv.html

[D24] 字典 / Map 基本操作
来源：http://hz.redwolf501.top/gtrxqqbytv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.zycfv.cn/gtkvteazbn.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.meibo888.top/gtahckdggj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.havefunace.top/gtggoahgou.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.shzxlz.cn/gtugjjcwyi.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.yangfankeji.com/gtuuqcwjhy.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.gotoacloud.top/gtfezwncnc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.shanyushiyangkeji.top/gtvnyduysg.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.zhoulong.xyz/gtuidzfdes.html

[D25] Set 集合去重与交并差
来源：http://hz.haohaochexian.top/gtsdbrupei.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.yj20258.top/gtrhyvhcbc.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.jinqigufen.top/gtxzlqhbzy.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.yangfankeji.com/gtkkkhlwlq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.tanke756.top/gtdabbcaqy.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.jinqigfzy.top/gtuealvntc.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.dashuyun.cn/gtpwxkdsgc.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.hnxiangtu.top/gtgftawlab.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.pengpengdd.cyou/gtghmmoxkn.html

[D26] 数组转字符串
来源：http://hz.cdnleiting.top/gtzdkdxoqn.html

Py:   ", ".join(map(str, arr))
来源：http://hz.9152youxi.cn/gthrxokeho.html

PHP:  implode(", ", $arr);
来源：http://hz.ybcxt.top/gtyfgpouay.html

JS:   arr.join(", ")
来源：http://hz.nanxuanxn.top/gtoysuqtui.html

TS:   arr.join(", ")
来源：http://hz.shuidangran.top/gthdadqjpt.html

Java: String.join(", ", list)
来源：http://hz.andypj.xyz/gtoldwyzqd.html

Go:   strings.Join(strs, ", ")
来源：http://hz.nanxuanxn.top/gtgwetzuwj.html

Ruby: arr.join(", ")
来源：http://hz.shzxlz.cn/gtecptskwn.html

C#:   string.Join(", ", list)
来源：http://hz.yuanzhike.top/gtrddzunpx.html

================================================================================
来源：http://hz.zhoulong.xyz/gtnfaujrgw.html

E. 字符串处理
来源：http://hz.xziqi.cn/gtgvqsgwyg.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtrwszfkgj.html

[E01] 拼接字符串
来源：http://hz.zhaomingkeji.xyz/gtmozvzgne.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.ehwqpu.com/gtqtxjumib.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.xuanzx.com/gthhwmuhcs.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jyoumei.cn/gtfmsirrcx.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ivvv.top/gtgbsezkzl.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.yj202588.top/gtlsjztaep.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.zhengqikj.top/gtregwybrw.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.yuxming.cn/gtcmwoqinu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.52xcode.cn/gtauppedst.html

[E02] 重复字符串
来源：http://hz.yanxiufei.cn/gtzcujftod.html

Py:   "ab" * 3
来源：http://hz.ehwqpu.com/gtgkdfckjc.html

PHP:  str_repeat("ab", 3);
来源：http://hz.shanyushiyangtech.top/gtlsjxppda.html

JS:   "ab".repeat(3)
来源：http://hz.hfpthk.cn/gtypaioayx.html

TS:   "ab".repeat(3)
来源：http://hz.hysaishi.cn/gtnsmgryix.html

Java: "ab".repeat(3)
来源：http://hz.jinqigufen.top/gtcyefpgup.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.yvedp.cn/gtmajvjvfu.html

Ruby: "ab" * 3
来源：http://hz.jlsjyb.cn/gtuwtmcvzc.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.shzxlz.cn/gtiezhbzgv.html

[E03] 截取子串
来源：http://hz.dianchejie.cn/gtkidkbcsz.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.cashguo.top/gtutlukbzv.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.fzhhl.top/gtdnrhaqpv.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.ywan-chungtsiang.top/gtjxyxbeiz.html

TS:   s.slice(1, 4)
来源：http://hz.mhx1999.top/gtvhsfiryr.html

Java: s.substring(1, 4)
来源：http://hz.fengsongda.top/gtaxljamte.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.hongshengwenyu.top/gtwsuqlkkw.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.tian-w.cn/gthxcmjing.html

C#:   s.Substring(1, 3)
来源：http://hz.jinqigufen.top/gtuspxcfpk.html

[E04] 查找子串位置
来源：http://hz.chenzaomai.com/gtgzalympn.html

Py:   s.find("x");  s.index("x")
来源：http://hz.ydjk.org.cn/gtcrlpiboy.html

PHP:  strpos($s, "x");
来源：http://hz.xuetiantiany.cn/gtyntmijav.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.52xcode.cn/gthxppqsfx.html

TS:   s.indexOf("x")
来源：http://hz.jlsjyb.cn/gtxwtldgtw.html

Java: s.indexOf("x")
来源：http://hz.jinqigfzy.top/gtaanqmetz.html

Go:   strings.Index(s, "x")
来源：http://hz.andypj.xyz/gtmcmcjyio.html

Ruby: s.index("x")
来源：http://hz.yvedp.cn/gtugokvfxu.html

C#:   s.IndexOf("x")
来源：http://hz.jinqigfzy.top/gtbrlbksfs.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.shzxlz.cn/gtusupsxmq.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.zhaomingkeji.xyz/gtfyffbumm.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.yvedp.cn/gtleawlrgh.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yj20258.top/gtwzspjrld.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.yj202588.top/gtytanohae.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zhixingplan.top/gtckmymolw.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.guowangkeji.top/gttvswmnrl.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.pycfn.com/gtkismssav.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.cashguo.top/gthsiyrbid.html

[E06] 替换子串
来源：http://hz.shangyingyoupin.top/gtxbotvocf.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.fzhhl.top/gtyawtebxi.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.9152youxi.cn/gtrkdkdbzo.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.redwolf501.top/gtbxrgumzq.html

TS:   s.replaceAll("a", "b")
来源：http://hz.zycfv.cn/gtbnzxrtat.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.tanke756.top/gtzmufmpdz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.jinqigfzy.top/gtahmijbiz.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.dianchejie.cn/gtksklmbph.html

C#:   s.Replace("a", "b")
来源：http://hz.jinqigfzy.top/gtfaazzjde.html

[E07] 按分隔符拆分
来源：http://hz.wangshuangyany.cn/gtwmqdfjpe.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.cdnleiting.top/gtghvhgjfl.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.snrcjt.cn/gtptexvjog.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.yueranfly.top/gtigldjjxo.html

TS:   s.split(",")
来源：http://hz.zhixingplan.top/gthqlojtvt.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.bjfxy.top/gtmezwytdx.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.birdmap.top/gtiqkrfuud.html

Ruby: s.split(",");  s.split
来源：http://hz.52xcode.cn/gtbitkxlqh.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.hnxiangtu.top/gtmheuyacb.html

[E08] 数组按分隔符合并
来源：http://hz.yj20258.top/gtmijhutwp.html

Py:   ",".join(items)
来源：http://hz.hongshengwenyu.top/gtbzihaxjz.html

PHP:  implode(",", $items);
来源：http://hz.shzxlz.cn/gtwudpswmn.html

JS:   items.join(",")
来源：http://hz.52xcode.cn/gtypmdmrsi.html

TS:   items.join(",")
来源：http://hz.bjfxy.top/gtsirgpjom.html

Java: String.join(",", items)
来源：http://hz.sufxvd.cn/gtswrltiem.html

Go:   strings.Join(items, ",")
来源：http://hz.sweek.top/gtoswyhvdh.html

Ruby: items.join(",")
来源：http://hz.aizwys.cn/gtymlkjzdw.html

C#:   string.Join(",", items)
来源：http://hz.shanyushiyangkeji.top/gtdjbrxzag.html

[E09] 去除所有空白字符
来源：http://hz.yonumen.top/gtmkfwwxcm.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.iojbl.cn/gtmwrqcliv.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.shzxlz.cn/gtdkcndtzt.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.chenzaomai.com/gtzjbtrhws.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.pycfn.com/gtxtjtednc.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.jinghuilouyu.cn/gtnkbpkxyu.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.jinghuilouyu.cn/gtgjyvgvrv.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.hnqzz.top/gtaznjwcwd.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.xziqi.cn/gtueosrmmy.html

[E10] 左侧补零 / 定长填充
来源：http://hz.fengsongda.top/gtwfzlcvgx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.pengpengdd.cyou/gtevaexwqb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.chenlongwang.top/gtwogdpmqf.html

JS:   "7".padStart(3, "0")
来源：http://hz.jianghu66.top/gtbwryxhfk.html

TS:   "7".padStart(3, "0")
来源：http://hz.aizwys.cn/gtijnprekk.html

Java: String.format("%03d", 7)
来源：http://hz.zdqjudy.top/gtvaeckzmc.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.nwbrower.top/gtwwwzvimu.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.hywenlv.cn/gtqyczkaxh.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.pycfn.com/gtlhrhkrbc.html

[E11] 反转字符串
来源：http://hz.wangdashe.top/gtyrgcypfm.html

Py:   s[::-1]
来源：http://hz.hongshengwenyu.top/gtphxnsdxq.html

PHP:  strrev($s);
来源：http://hz.gotoacloud.top/gtcvmkewxz.html

JS:   [...s].reverse().join("")
来源：http://hz.shzxlz.cn/gtxcctnfpl.html

TS:   [...s].reverse().join("")
来源：http://hz.meibo888.top/gteexjrxzq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.316326.xyz/gtltvgrwyd.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.ppjwa.cn/gtwdoompfn.html

Ruby: s.reverse
来源：http://hz.xinyue.icu/gtmarpklec.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.hnxiangtu.top/gtcvhykkct.html

[E12] 统计某字符出现次数
来源：http://hz.zhongyouzk.top/gttonrphyw.html

Py:   s.count("a")
来源：http://hz.jqgufenzy.top/gtuktmghun.html


<!-- 参考信息 -->