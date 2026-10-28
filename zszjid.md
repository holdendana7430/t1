代发 wailian999

C#:   list.Insert(0, 0);
来源：http://hz.yj20258.top/gtfnyhoxiu.html

[D04] 删除元素
来源：http://hz.xinyue.icu/gtyggnqvgb.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.kuanghao11.cn/gthjfhdatx.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.yueranfly.top/gtjeevgxod.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.gogol.net.cn/gtrtcdguha.html

TS:   arr.splice(0, 1);
来源：http://hz.cdnleiting.top/gtvzgebxxj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.vqdsnc.cn/gtzzrsmnyo.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.cdnleiting.top/gtarofeltf.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.ydjk.org.cn/gtxyukvrpo.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.jinqigufen.top/gtvbnkdjcn.html

[D05] 访问与修改元素
来源：http://hz.sweek.top/gtedjxwmmm.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.cqqwz.cn/gthsefaqxr.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.zhixingplan.top/gthlvmibyj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.ppjwa.cn/gtizcjlejo.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.c1oappe.top/gtwryjkowz.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.andypj.xyz/gtokhthcip.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.xziqi.cn/gtogwxccjj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.chenlongwang.top/gtijnxyzhp.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.ppjwa.cn/gtufkdtegt.html

[D06] 数组长度
来源：http://hz.jianghu66.top/gtdnbnegbl.html

Py:   len(arr)
来源：http://hz.zhaomingkeji.xyz/gtmsdcctwe.html

PHP:  count($arr);
来源：http://hz.chenzaomai.com/gtsuoxvqtm.html

JS:   arr.length
来源：http://hz.zhixingplan.top/gtgzvvdovf.html

TS:   arr.length
来源：http://hz.gaohongyu789.top/gtpqblfgoo.html

Java: list.size();
来源：http://hz.yueranfly.top/gteggswvpt.html

Go:   len(arr)
来源：http://hz.zhongyouzk.top/gtbnigiqfp.html

Ruby: arr.length; arr.size
来源：http://hz.daria6918.cn/gtsopsgglo.html

C#:   list.Count;
来源：http://hz.shzxlz.cn/gtmaybspgb.html

[D07] 切片 / 取子数组
来源：http://hz.redwolf501.top/gtrhqgydkh.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.xuetiantiany.cn/gtksyfaeyn.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.birdmap.top/gtmoqmnsvv.html

JS:   arr.slice(1, 4);
来源：http://hz.yueranfly.top/gtvzezfswy.html

TS:   arr.slice(1, 4);
来源：http://hz.yj202588.top/gtiomqdxbp.html

Java: list.subList(1, 4);
来源：http://hz.xylfe.cn/gteoscdiay.html

Go:   arr[1:4]
来源：http://hz.zdqjudy.top/gtyubztmne.html

Ruby: arr[1, 3]
来源：http://hz.kuanghao11.cn/gtbfwsgpps.html

C#:   list.GetRange(1, 3);
来源：http://hz.zhongyouzk.top/gtnsdhhaqz.html

[D08] 合并两个数组
来源：http://hz.fzhhl.top/gtqisdobgx.html

Py:   a + b;  a.extend(b)
来源：http://hz.nwbrower.top/gtwgrwhvpa.html

PHP:  array_merge($a, $b);
来源：http://hz.meibo888.top/gtjexcxlcc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.sxryk.cn/gtnpzvpkqn.html

TS:   [...a, ...b];
来源：http://hz.tianlin.xyz/gtxcqwhhep.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.quarkkingdee.top/gtsdrlypbb.html

Go:   append(a, b...)
来源：http://hz.hongshengwenyu.top/gthcfniltx.html

Ruby: a + b;  a.concat(b)
来源：http://hz.316326.xyz/gtjlojhcvj.html

C#:   a.Concat(b).ToList()
来源：http://hz.aizwys.cn/gtjnpmrdrx.html

[D09] 排序（升序）
来源：http://hz.jinghuilouyu.cn/gtynqjzcnu.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.tian-w.cn/gterolawrg.html

PHP:  sort($arr);
来源：http://hz.ydzc1.top/gtyrwdpgcg.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.shanyushiyangtech.top/gtqitzkbfa.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.xuetiantiany.cn/gtnsdkhwyi.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.svipenyu.cn/gtfhuguhza.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.yanxiufei.cn/gtcopwjvfs.html

Ruby: arr.sort
来源：http://hz.dianchejie.cn/gtcepfrurt.html

C#:   list.Sort();
来源：http://hz.yuanzhike.top/gtrjshreja.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.sweek.top/gtqzvpxzrc.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.aizwys.cn/gtbyudjens.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jlsjyb.cn/gtaexcdfwv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.shanyushiyangtech.top/gtxcxwwxgg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hongshengwenyu.top/gtirraldof.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.nanxinkj.top/gtjdfnrzhn.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.birdmap.top/gtcnekowwg.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.jqgufenzy.top/gtaldbwoyi.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.tanke756.top/gtvmlbgvep.html

[D11] 反转数组
来源：http://hz.ehwqpu.com/gtzjjczqph.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.pycfn.com/gtujbcinmr.html

PHP:  array_reverse($arr);
来源：http://hz.xuetiantiany.cn/gtorjfmwzp.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.ydjk.org.cn/gtxxzgugqu.html

TS:   [...arr].reverse();
来源：http://hz.hammf.cn/gtnsxkadxy.html

Java: Collections.reverse(list);
来源：http://hz.tian-w.cn/gticpfwkol.html

Go:   slices.Reverse(arr)
来源：http://hz.bjfxy.top/gtgzoqzago.html

Ruby: arr.reverse
来源：http://hz.sxryk.cn/gtrergoxah.html

C#:   list.Reverse();
来源：http://hz.shuidangran.top/gtvktnbfis.html

[D12] 查找元素下标
来源：http://hz.pengpengdd.cyou/gtckkkbbbm.html

Py:   arr.index(x);  x in arr
来源：http://hz.svipenyu.cn/gthlsfkmru.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.tanke756.top/gtnwtjabhu.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.tian-w.cn/gtmchduevg.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.hysaishi.cn/gtuqlkwdfx.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.jinqigufen.top/gtcuvyawkg.html

Go:   slices.Index(arr, x)
来源：http://hz.yongpay.top/gtzcablydm.html

Ruby: arr.index(x)
来源：http://hz.ydzc1.top/gtlfdaeowx.html

C#:   list.IndexOf(x);
来源：http://hz.havefunace.top/gtxykteymv.html

[D13] 过滤（保留满足条件的）
来源：http://hz.jinqigufen.top/gtzrmcpzdq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.bjfxy.top/gtafddikvw.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.aibaodan.cn/gthtxcrnvb.html

JS:   arr.filter(x => x > 3)
来源：http://hz.zhoulong.xyz/gtzbtchewq.html

TS:   arr.filter(x => x > 3)
来源：http://hz.ivvv.top/gtkhhsqjbh.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.sufxvd.cn/gtxjdxjrkq.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.wangdashe.top/gtczffydow.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.hysaishi.cn/gtgwmlhcuu.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.cheryme.top/gthtdensgz.html

[D14] 映射转换（每个元素变形）
来源：http://hz.redwolf501.top/gtrwxfwsob.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.guannengcc.top/gtuvmzlgyq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.chenlongwang.top/gteonjdvod.html

JS:   arr.map(x => x * 2)
来源：http://hz.vqdsnc.cn/gtqbtmzhtr.html

TS:   arr.map(x => x * 2)
来源：http://hz.52xcode.cn/gtrqkxfvyi.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.kuanghao11.cn/gtopkslvtw.html

Go:   // 手写循环
来源：http://hz.hnxiangtu.top/gtctceuykz.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.tian-w.cn/gthjdprhko.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.yonumen.top/gtikvuxicx.html

[D15] 去重
来源：http://hz.svipenyu.cn/gtbbrdnxhh.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.0kj1m.cn/gtjngastwd.html

PHP:  array_unique($arr);
来源：http://hz.nanxuanxn.top/gthpimxzkj.html

JS:   [...new Set(arr)]
来源：http://hz.wangdashe.top/gthoyqxhzi.html

TS:   [...new Set(arr)]
来源：http://hz.guannengcc.top/gtatpahcdt.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.dianchejie.cn/gtpzlqojhc.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.ydjk.org.cn/gtbkknovyu.html

Ruby: arr.uniq
来源：http://hz.cqqwz.cn/gtacjiwqnj.html

C#:   list.Distinct().ToList()
来源：http://hz.aibaodan.cn/gtcqdhzsui.html

[D16] 求和与平均值
来源：http://hz.kuanghao11.cn/gtjglwkgry.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.andypj.xyz/gtzvffxozv.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.sufxvd.cn/gtyaigxvpk.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.guannengcc.top/gtfmbyidmf.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.smart0.xyz/gtlcvtgbip.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.hfpthk.cn/gthhgipsfn.html

Go:   // 手写循环累加
来源：http://hz.bjfxy.top/gtupighxio.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.smart0.xyz/gtdrnbuylp.html

C#:   list.Sum();  list.Average()
来源：http://hz.pycfn.com/gtegelcrcd.html

[D17] 最大值与最小值
来源：http://hz.sysykeji.top/gtewvnqnal.html

Py:   max(arr);  min(arr)
来源：http://hz.wangdashe.top/gtgynxjgmk.html

PHP:  max($arr);  min($arr);
来源：http://hz.zhengqikj.top/gtqmvtzimo.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.ivvv.top/gtesdyaigz.html

TS:   Math.max(...arr);
来源：http://hz.iojbl.cn/gtcazyrrtl.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.gogol.net.cn/gthpmkhwpq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.jinqigufen.top/gtfulsvpbg.html

Ruby: arr.max;  arr.min
来源：http://hz.jinqigufen.top/gthbejfbpa.html

C#:   list.Max();  list.Min()
来源：http://hz.xuetiantiany.cn/gtnrgyexha.html

[D18] 扁平化嵌套数组
来源：http://hz.shanyushiyangkeji.top/gtxjedhklr.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.redwolf501.top/gtsymzziec.html

PHP:  array_merge(...$nested);
来源：http://hz.cucudq.cn/gtyofulthf.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.ydjk.org.cn/gtnqepyubu.html

TS:   nested.flat();
来源：http://hz.xinyue.icu/gtdepmufqp.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.sysykeji.top/gtarrodkia.html

Go:   // 手写双层循环
来源：http://hz.dianchejie.cn/gtqedthdic.html

Ruby: nested.flatten
来源：http://hz.dashuyun.cn/gtjqwowkop.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.cqqwz.cn/gtcrumodth.html

[D19] 按字段分组
来源：http://hz.ydjk.org.cn/gtoocnnlts.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.tianlin.xyz/gtduxwtvjb.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.yuxming.cn/gtkubyzxjd.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.yvedp.cn/gtnzheiqys.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.cqqwz.cn/gtzrqndtue.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.pengpengdd.cyou/gtbcnrovvt.html

Go:   // 手写 map[string][]T
来源：http://hz.jinqigfzy.top/gttquybpzh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.zhoulong.xyz/gtbemvyhol.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.jinqigfzy.top/gtpebksedi.html

[D20] 统计每个元素出现次数
来源：http://hz.zhengqikj.top/gtucdduigp.html

Py:   Counter(arr)
来源：http://hz.birdmap.top/gtxzzstgdh.html

PHP:  array_count_values($arr);
来源：http://hz.cashguo.top/gtuudcmnqs.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yuxming.cn/gtlnoektgd.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.52xcode.cn/gttfktmwli.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.guowangkeji.top/gtfhdfltqa.html

Go:   // 手写 map[T]int
来源：http://hz.nanxuanxn.top/gtczhlrjmn.html

Ruby: arr.tally
来源：http://hz.ydjk.org.cn/gtpjyepihp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.redwolf501.top/gtvcranftl.html

[D21] 判断是否包含某元素
来源：http://hz.wangdashe.top/gthviqsuhj.html

Py:   x in arr
来源：http://hz.dianchejie.cn/gtewedetiu.html

PHP:  in_array($x, $arr, true);
来源：http://hz.andypj.xyz/gtrzdquvpx.html

JS:   arr.includes(x)
来源：http://hz.zhijiandao.cn/gtzpcqelns.html

TS:   arr.includes(x)
来源：http://hz.ybcxt.top/gtvtwxovvh.html

Java: list.contains(x)
来源：http://hz.snrcjt.cn/gtjhfyxhzn.html

Go:   slices.Contains(arr, x)
来源：http://hz.zhijiandao.cn/gtqhatfqks.html

Ruby: arr.include?(x)
来源：http://hz.jlsjyb.cn/gtpcjdjpgw.html

C#:   list.Contains(x)
来源：http://hz.yonumen.top/gtnjbxbpqh.html

[D22] 复制数组（避免共享引用）
来源：http://hz.chenzaomai.com/gtccogjzoa.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.gzhubu.top/gtwufxwygs.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.andypj.xyz/gtfzcnwzqz.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.zycfv.cn/gtqyaolquc.html

TS:   [...arr];
来源：http://hz.shzxlz.cn/gtueiexphh.html

Java: new ArrayList<>(list);
来源：http://hz.yanxiufei.cn/gtzeprvktg.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.shanyushiyangkeji.top/gttsgshxve.html

Ruby: arr.dup;  arr.clone
来源：http://hz.yangfankeji.com/gtobstyefk.html

C#:   new List<int>(list);
来源：http://hz.zhengqikj.top/gtfuoaiodm.html

[D23] reduce 累积计算
来源：http://hz.yj202588.top/gtsshbloqw.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.xuetiantiany.cn/gtdvyyuoke.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.chenlongwang.top/gtopxnyuxm.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yvedp.cn/gtqhylsxou.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.hnqzz.top/gtmzjfmtxg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.zhijiandao.cn/gtsoqbyvmw.html

Go:   // 手写循环
来源：http://hz.guowangkeji.top/gtndmucgnu.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.hfpthk.cn/gtsnxfuozu.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.yuxming.cn/gtpgrqkbdy.html

[D24] 字典 / Map 基本操作
来源：http://hz.daxiang520.top/gtjvczbqod.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.zycfv.cn/gtrrifqdcl.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.c1oappe.top/gtqzkxdnnl.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.nanxinkj.top/gtiplqfswd.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.yj202588.top/gtcrbxvcnm.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.nanxuanxn.top/gtmrayfmlw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.ydjk.org.cn/gtgikwyyib.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.shuidangran.top/gtdxolbjoq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.0kj1m.cn/gtlwgetzrs.html

[D25] Set 集合去重与交并差
来源：http://hz.shangyingyoupin.top/gtbvsjajsw.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.jinyuanbaomall.cn/gtjczdykhh.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.chenlongwang.top/gtfyfhubob.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.zhixingplan.top/gthgalufwl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.shzxlz.cn/gtpoxxoftj.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.snrcjt.cn/gtcqurhyfv.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.hnxiangtu.top/gthddqlmbs.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.meibo888.top/gtdwcauapm.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.iojbl.cn/gtbtkslknp.html

[D26] 数组转字符串
来源：http://hz.tian-w.cn/gtqpjpotgq.html

Py:   ", ".join(map(str, arr))
来源：http://hz.ybcxt.top/gtscrlgjjs.html

PHP:  implode(", ", $arr);
来源：http://hz.nanxuanxn.top/gtkalgqqpm.html

JS:   arr.join(", ")
来源：http://hz.yuanzhike.top/gtdjqmpoyy.html

TS:   arr.join(", ")
来源：http://hz.nwbrower.top/gtvrfvkglv.html

Java: String.join(", ", list)
来源：http://hz.nanxinkj.top/gtnqjsqhnj.html

Go:   strings.Join(strs, ", ")
来源：http://hz.birdmap.top/gtxcjpuzra.html

Ruby: arr.join(", ")
来源：http://hz.yuanzhike.top/gtwdhotqha.html

C#:   string.Join(", ", list)
来源：http://hz.xuetiantiany.cn/gtajtajtyg.html

================================================================================
来源：http://hz.jiagoushi.top/gthymuztty.html

E. 字符串处理
来源：http://hz.daria6918.cn/gtxdpjhpzt.html

================================================================================
来源：http://hz.yj20258.top/gtacpaebxn.html

[E01] 拼接字符串
来源：http://hz.yj20258.top/gtvdzozrxq.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.andypj.xyz/gtmikwqzzk.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.dianchejie.cn/gtvrcmxmst.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.xingfuxueyuan.xyz/gtvojowbio.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yuanzhike.top/gtvnkkeosi.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.guowangkeji.top/gtlfxymwrx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.xziqi.cn/gtfhgxoqjc.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.yuanzhike.top/gthcwjhvvb.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.ehwqpu.com/gtxmplofds.html

[E02] 重复字符串
来源：http://hz.svipenyu.cn/gtarjcskco.html

Py:   "ab" * 3
来源：http://hz.xylfe.cn/gtwjdwhdxj.html

PHP:  str_repeat("ab", 3);
来源：http://hz.yj202588.top/gthoeevunk.html

JS:   "ab".repeat(3)
来源：http://hz.zycfv.cn/gtrklvyato.html

TS:   "ab".repeat(3)
来源：http://hz.gotoacloud.top/gtguqfssid.html

Java: "ab".repeat(3)
来源：http://hz.pengpengdd.cyou/gtclcijqiu.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.cashguo.top/gtchifstcd.html

Ruby: "ab" * 3
来源：http://hz.jinyuanbaomall.cn/gtycvpbkac.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.svipenyu.cn/gtpzbpmvzb.html

[E03] 截取子串
来源：http://hz.dianchejie.cn/gtfpwxlntj.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.guannengcc.top/gtiekntixp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.cdnleiting.top/gtvvlsmsft.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.tanke756.top/gtulcuihgm.html

TS:   s.slice(1, 4)
来源：http://hz.cucudq.cn/gtxolceekt.html

Java: s.substring(1, 4)
来源：http://hz.jinqigufen.top/gtpbrkiesm.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.smart0.xyz/gtlolfsnfx.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.zhixingplan.top/gtvumoqbhb.html

C#:   s.Substring(1, 3)
来源：http://hz.yanxiufei.cn/gtkazxwozk.html

[E04] 查找子串位置
来源：http://hz.hysaishi.cn/gtjrviamnk.html

Py:   s.find("x");  s.index("x")
来源：http://hz.sufxvd.cn/gttartgwkr.html

PHP:  strpos($s, "x");
来源：http://hz.ywan-chungtsiang.top/gttklwmjhe.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.hfpthk.cn/gtyrgdpfga.html

TS:   s.indexOf("x")
来源：http://hz.c1oappe.top/gtisyhxdnz.html

Java: s.indexOf("x")
来源：http://hz.cdnleiting.top/gtrzldhkrx.html

Go:   strings.Index(s, "x")
来源：http://hz.tanke756.top/gthbtfpxls.html

Ruby: s.index("x")
来源：http://hz.dashuyun.cn/gtgaqjupcb.html

C#:   s.IndexOf("x")
来源：http://hz.jinyuanbaomall.cn/gtdyvucqjc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.9152youxi.cn/gtcvqqztqf.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.shanyushiyangkeji.top/gtnlalpumd.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.shanyushiyangkeji.top/gtexuzdmfj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.hfpthk.cn/gtflhqkptd.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.ivvv.top/gthspoopfx.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.xziqi.cn/gtnrsezyax.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.xuanzx.com/gtbxjvlppu.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.dashuyun.cn/gtnusqujhn.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.hfpthk.cn/gtvsaezotq.html

[E06] 替换子串
来源：http://hz.zhoulong.xyz/gtzilrqfef.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.pycfn.com/gtytthyovj.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.sysykeji.top/gtpirywqin.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.cashguo.top/gtpjkvlots.html

TS:   s.replaceAll("a", "b")
来源：http://hz.zhixingplan.top/gtykbkfcyo.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.ppjwa.cn/gtgjkjjmxq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.tian-w.cn/gtdzoxumfv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.jinqigfzy.top/gtqesmhbjp.html

C#:   s.Replace("a", "b")
来源：http://hz.hongshengwenyu.top/gtlunkbxqz.html

[E07] 按分隔符拆分
来源：http://hz.shanyushiyangtech.top/gtzadqhepo.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.hammf.cn/gtqdpftfku.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.zhoulong.xyz/gtjrodvccl.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.0kj1m.cn/gtlsizvbsn.html

TS:   s.split(",")
来源：http://hz.yj20258.top/gtsxmncvnt.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.svipenyu.cn/gtvhtffcqs.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.yueranfly.top/gtfvqzngkw.html

Ruby: s.split(",");  s.split
来源：http://hz.zhaomingkeji.xyz/gtfddqqkjs.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.wangshuangyany.cn/gtgiqtggag.html

[E08] 数组按分隔符合并
来源：http://hz.hysaishi.cn/gtgbppchlw.html

Py:   ",".join(items)
来源：http://hz.nanxuanxn.top/gtarqugowj.html

PHP:  implode(",", $items);
来源：http://hz.fzhhl.top/gttkfobcco.html

JS:   items.join(",")
来源：http://hz.vqdsnc.cn/gtkermcsnp.html

TS:   items.join(",")
来源：http://hz.cucudq.cn/gtbgmbnrhb.html

Java: String.join(",", items)
来源：http://hz.zhengqikj.top/gtlufcbjpy.html

Go:   strings.Join(items, ",")
来源：http://hz.svipenyu.cn/gtiwdxljqk.html

Ruby: items.join(",")
来源：http://hz.aibaodan.cn/gtgscljuru.html

C#:   string.Join(",", items)
来源：http://hz.yj20258888.top/gtvnqeuvyb.html

[E09] 去除所有空白字符
来源：http://hz.yj20258.top/gttvnervmk.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.yj202588.top/gthnszwyth.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.birdmap.top/gtoolklytq.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.jianghu66.top/gtchpmkijn.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.cucudq.cn/gtbrclbytk.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.hnqzz.top/gtapncanjt.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.svipenyu.cn/gtesjwtwog.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.yangfankeji.com/gtpilfhmhq.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.vqdsnc.cn/gtmtvflpmq.html

[E10] 左侧补零 / 定长填充
来源：http://hz.zhijiandao.cn/gtdbnufclo.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.52xcode.cn/gtvnbeioiq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.jianghu66.top/gtnuudetjv.html

JS:   "7".padStart(3, "0")
来源：http://hz.meibo888.top/gtfvgcohpj.html

TS:   "7".padStart(3, "0")
来源：http://hz.snrcjt.cn/gtkkstiukj.html

Java: String.format("%03d", 7)
来源：http://hz.iojbl.cn/gtdymwceym.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.pengpengdd.cyou/gtsvfdjfcz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.jinqigufen.top/gtdvfupqfh.html


<!-- 参考信息 -->