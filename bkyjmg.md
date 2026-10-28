代发 wailian999

Java: list.size();
来源：http://hz.cucudq.cn/gtkhstskzq.html

Go:   len(arr)
来源：http://hz.zhengqikj.top/gtxdtgpger.html

Ruby: arr.length; arr.size
来源：http://hz.zhoulong.xyz/gtmmxwtltc.html

C#:   list.Count;
来源：http://hz.pycfn.com/gtvndzgmxt.html

[D07] 切片 / 取子数组
来源：http://hz.nanxuanxn.top/gtsmyejmsx.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.andypj.xyz/gtaozadjwt.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.yuxming.cn/gtuqyouaaw.html

JS:   arr.slice(1, 4);
来源：http://hz.guowangkeji.top/gtxgbzonmw.html

TS:   arr.slice(1, 4);
来源：http://hz.9152youxi.cn/gttdenlnax.html

Java: list.subList(1, 4);
来源：http://hz.zhixingplan.top/gtmholfwfx.html

Go:   arr[1:4]
来源：http://hz.zhiwuduotai.top/gtgyzxyvnp.html

Ruby: arr[1, 3]
来源：http://hz.jyoumei.cn/gteimpapnd.html

C#:   list.GetRange(1, 3);
来源：http://hz.cqqwz.cn/gttzkuauwz.html

[D08] 合并两个数组
来源：http://hz.chenjidiqi.icu/gtvkreeilr.html

Py:   a + b;  a.extend(b)
来源：http://hz.wangshuangyany.cn/gtciqcyeze.html

PHP:  array_merge($a, $b);
来源：http://hz.aibaodan.cn/gtulhjdylg.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.ydzc1.top/gtlbuktvyj.html

TS:   [...a, ...b];
来源：http://hz.jinyuanbaomall.cn/gtfhwlwhwx.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.ivvv.top/gtwhsaiuxe.html

Go:   append(a, b...)
来源：http://hz.hywenlv.cn/gtrpjfszwe.html

Ruby: a + b;  a.concat(b)
来源：http://hz.cheryme.top/gtlskkrqax.html

C#:   a.Concat(b).ToList()
来源：http://hz.chenzaomai.com/gtmpkahdnb.html

[D09] 排序（升序）
来源：http://hz.mhx1999.top/gtvqzimkjs.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.shangyingyoupin.top/gtidmnfqpo.html

PHP:  sort($arr);
来源：http://hz.fengsongda.top/gtjjreavkv.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.yanxiufei.cn/gtqwlzutar.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.zdqjudy.top/gtrjhcgvdw.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.dianchejie.cn/gtdzhjpoht.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.ydzc1.top/gtukuqjoyv.html

Ruby: arr.sort
来源：http://hz.guannengcc.top/gtrywmahsu.html

C#:   list.Sort();
来源：http://hz.316326.xyz/gtjwkwcdki.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.feifeiyinyue.top/gtgnfopqwi.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.gogol.net.cn/gtwoynvkeh.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jyoumei.cn/gtqvxvzmha.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hongshengwenyu.top/gtlweljpru.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.iojbl.cn/gthhtbeshk.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.zhijiandao.cn/gteytjqldw.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.shuidangran.top/gttmkmmpnq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.nanxuanxn.top/gtaauarjpm.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.andypj.xyz/gtzltfocqs.html

[D11] 反转数组
来源：http://hz.svipenyu.cn/gttvoggeao.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.nanxuanxn.top/gtttoxvkrw.html

PHP:  array_reverse($arr);
来源：http://hz.xinyue.icu/gtksngrpgx.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.yj20258888.top/gtfckwhyvz.html

TS:   [...arr].reverse();
来源：http://hz.ppjwa.cn/gtsygfowgv.html

Java: Collections.reverse(list);
来源：http://hz.sxryk.cn/gtmvjslbst.html

Go:   slices.Reverse(arr)
来源：http://hz.redwolf501.top/gtzkzfjlha.html

Ruby: arr.reverse
来源：http://hz.dianchejie.cn/gtfgxsocjq.html

C#:   list.Reverse();
来源：http://hz.meibo888.top/gtjiaoivns.html

[D12] 查找元素下标
来源：http://hz.sxryk.cn/gtdfhxugdi.html

Py:   arr.index(x);  x in arr
来源：http://hz.dashuyun.cn/gtfxdxevto.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.smart0.xyz/gteelcoszl.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.fzhhl.top/gteaohqmfp.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.cucudq.cn/gtdqokjkhq.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.yuxming.cn/gtksoejwtl.html

Go:   slices.Index(arr, x)
来源：http://hz.xuetiantiany.cn/gtmdgygpyu.html

Ruby: arr.index(x)
来源：http://hz.shzxlz.cn/gtbayascud.html

C#:   list.IndexOf(x);
来源：http://hz.shuidangran.top/gttcaxvzjf.html

[D13] 过滤（保留满足条件的）
来源：http://hz.tian-w.cn/gtgrmhcvoa.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.bjfxy.top/gttxlgqkmf.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.jiagoushi.top/gtfmchpzkv.html

JS:   arr.filter(x => x > 3)
来源：http://hz.hywenlv.cn/gtakhvvuja.html

TS:   arr.filter(x => x > 3)
来源：http://hz.ppjwa.cn/gtdfybdeum.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.yonumen.top/gtaagoehqt.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.jinyuanbaomall.cn/gtktmjzsuy.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.feifeiyinyue.top/gtremrsmpw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.cdnleiting.top/gtnlvsbgad.html

[D14] 映射转换（每个元素变形）
来源：http://hz.jinqigfzy.top/gtvwxlegyd.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.0kj1m.cn/gtimlyrnic.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.daxiang520.top/gtwpsinamo.html

JS:   arr.map(x => x * 2)
来源：http://hz.cheryme.top/gtctjfkyvj.html

TS:   arr.map(x => x * 2)
来源：http://hz.cucudq.cn/gtavipxrqg.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.zhengqikj.top/gtkjdubluj.html

Go:   // 手写循环
来源：http://hz.gaohongyu789.top/gtvmcxodzz.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.jqgfzy.top/gtcgimjcio.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.gotoacloud.top/gttzbymctt.html

[D15] 去重
来源：http://hz.jlsjyb.cn/gtztvpozxq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.sysykeji.top/gtoqvtifiz.html

PHP:  array_unique($arr);
来源：http://hz.jinghuilouyu.cn/gtwljieacu.html

JS:   [...new Set(arr)]
来源：http://hz.sufxvd.cn/gtskokklnn.html

TS:   [...new Set(arr)]
来源：http://hz.zycfv.cn/gtkkczayex.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.yangfankeji.com/gtopugmgrh.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.zhixingplan.top/gtcnxzuwul.html

Ruby: arr.uniq
来源：http://hz.xuetiantiany.cn/gtrunbilgo.html

C#:   list.Distinct().ToList()
来源：http://hz.sufxvd.cn/gtodcyirxx.html

[D16] 求和与平均值
来源：http://hz.smart0.xyz/gtecoixkvn.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.cashguo.top/gtojplmbea.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.xingfuxueyuan.xyz/gthrbsqrfm.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.cheryme.top/gtbhauonku.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.shuidangran.top/gtvompuiqw.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.jqgfzy.top/gtsjpvjvcy.html

Go:   // 手写循环累加
来源：http://hz.aibaodan.cn/gteajcglkb.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.sweek.top/gtwwyabedc.html

C#:   list.Sum();  list.Average()
来源：http://hz.jyoumei.cn/gtfjcjprwc.html

[D17] 最大值与最小值
来源：http://hz.52xcode.cn/gtezrkhais.html

Py:   max(arr);  min(arr)
来源：http://hz.ehwqpu.com/gthtnxyoqn.html

PHP:  max($arr);  min($arr);
来源：http://hz.chenzaomai.com/gtstimytdp.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.sufxvd.cn/gttrxmhdvu.html

TS:   Math.max(...arr);
来源：http://hz.yonumen.top/gtbxsttvhb.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.guannengcc.top/gttrkslnmb.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.gogol.net.cn/gthztehruw.html

Ruby: arr.max;  arr.min
来源：http://hz.birdmap.top/gtovphspsj.html

C#:   list.Max();  list.Min()
来源：http://hz.cdnleiting.top/gtojqhcjrt.html

[D18] 扁平化嵌套数组
来源：http://hz.yongpay.top/gtcdkzfdsm.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.dashuyun.cn/gttlphryqt.html

PHP:  array_merge(...$nested);
来源：http://hz.shangyingyoupin.top/gttfhdhybd.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.ybcxt.top/gtaazhqvqk.html

TS:   nested.flat();
来源：http://hz.chenlongwang.top/gtditdkmfy.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.xingfuxueyuan.xyz/gtdlbfeqho.html

Go:   // 手写双层循环
来源：http://hz.ydjk.org.cn/gtcwjkabsw.html

Ruby: nested.flatten
来源：http://hz.ehwqpu.com/gtxzkahcvq.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.cqqwz.cn/gtjlswznrp.html

[D19] 按字段分组
来源：http://hz.yuanzhike.top/gtcgbcuozg.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.shanyushiyangkeji.top/gtqeyqmtgj.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.chenlongwang.top/gtkehpfpef.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.smart0.xyz/gtetnfebgb.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.yanxiufei.cn/gtsaarpsnd.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.yonumen.top/gtxwksawib.html

Go:   // 手写 map[string][]T
来源：http://hz.gogol.net.cn/gtpzxxwuqq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.guannengcc.top/gtiheodeww.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.zhiwuduotai.top/gtbuvqgscu.html

[D20] 统计每个元素出现次数
来源：http://hz.zhiwuduotai.top/gtqgfkaypf.html

Py:   Counter(arr)
来源：http://hz.jqgfzy.top/gtivdbcfec.html

PHP:  array_count_values($arr);
来源：http://hz.meibo888.top/gtanelhicv.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.sysykeji.top/gtxrbrrfmt.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.aizwys.cn/gtljibyjwm.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.yongpay.top/gtnnfemhey.html

Go:   // 手写 map[T]int
来源：http://hz.sufxvd.cn/gtygitjmfs.html

Ruby: arr.tally
来源：http://hz.guannengcc.top/gtgnsqcamq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.chenzaomai.com/gtnorcmkds.html

[D21] 判断是否包含某元素
来源：http://hz.yongpay.top/gtfndmgjpz.html

Py:   x in arr
来源：http://hz.meibo888.top/gtgbaovxml.html

PHP:  in_array($x, $arr, true);
来源：http://hz.aizwys.cn/gtnaygcdao.html

JS:   arr.includes(x)
来源：http://hz.xingfuxueyuan.xyz/gtbqqkzevl.html

TS:   arr.includes(x)
来源：http://hz.jinghuilouyu.cn/gtiveipwbk.html

Java: list.contains(x)
来源：http://hz.quarkkingdee.top/gtqqaggpks.html

Go:   slices.Contains(arr, x)
来源：http://hz.aizwys.cn/gtqsjcqedh.html

Ruby: arr.include?(x)
来源：http://hz.cucudq.cn/gtclmosdxk.html

C#:   list.Contains(x)
来源：http://hz.yj20258.top/gtrdkkobjj.html

[D22] 复制数组（避免共享引用）
来源：http://hz.jinyuanbaomall.cn/gtuglazwfr.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.tianlin.xyz/gtiwvgsvee.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.yangfankeji.com/gtqfrszkbn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.gaohongyu789.top/gtgwynddfh.html

TS:   [...arr];
来源：http://hz.hywenlv.cn/gtprimtcsp.html

Java: new ArrayList<>(list);
来源：http://hz.hongshengwenyu.top/gtmigzytus.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.jiagoushi.top/gtuioymryz.html

Ruby: arr.dup;  arr.clone
来源：http://hz.zhoulong.xyz/gtlvxzutcg.html

C#:   new List<int>(list);
来源：http://hz.dashuyun.cn/gtsykrgjei.html

[D23] reduce 累积计算
来源：http://hz.ydjk.org.cn/gtujfvhsyy.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.zhixingplan.top/gtrsiigobx.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.xingfuxueyuan.xyz/gtuembkbgt.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.sysykeji.top/gtcpmpoesa.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.chenzaomai.com/gttuomgxsu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.ydjk.org.cn/gtbnacqwfq.html

Go:   // 手写循环
来源：http://hz.wangdashe.top/gtiudijxpb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.vqdsnc.cn/gtrafkfxhc.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.0kj1m.cn/gtbmkhjeux.html

[D24] 字典 / Map 基本操作
来源：http://hz.dashuyun.cn/gtrfkowcob.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.yangfankeji.com/gtbzsnqcjl.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.yj202588.top/gtelrbsjwi.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.zhixingplan.top/gtbgvurjou.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.yangfankeji.com/gtzvydepqd.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.wangdashe.top/gtaxvypzpp.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.nanxuanxn.top/gtkrgcnllu.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.jinghuilouyu.cn/gtylprrtwa.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.cucudq.cn/gtcsrlnxia.html

[D25] Set 集合去重与交并差
来源：http://hz.hammf.cn/gtubtpyjwk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.zhaomingkeji.xyz/gtrnykwrms.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.jiagoushi.top/gtbmcrypho.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.nanxinkj.top/gtjnsnycuc.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.xingfuxueyuan.xyz/gthdurwomy.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.yanxiufei.cn/gtafrmrflr.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.ivvv.top/gtgvqqzoar.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.tian-w.cn/gtlwwbjafl.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.316326.xyz/gtzfvwuckz.html

[D26] 数组转字符串
来源：http://hz.mhx1999.top/gtfkqqayqv.html

Py:   ", ".join(map(str, arr))
来源：http://hz.redwolf501.top/gtwybcoust.html

PHP:  implode(", ", $arr);
来源：http://hz.iojbl.cn/gtiddhuolb.html

JS:   arr.join(", ")
来源：http://hz.dashuyun.cn/gtzrujuhor.html

TS:   arr.join(", ")
来源：http://hz.cqqwz.cn/gtrspmrvzn.html

Java: String.join(", ", list)
来源：http://hz.yj20258.top/gtlsvmdtoj.html

Go:   strings.Join(strs, ", ")
来源：http://hz.gotoacloud.top/gtbhgzivgt.html

Ruby: arr.join(", ")
来源：http://hz.pengpengdd.cyou/gtyzdiypbz.html

C#:   string.Join(", ", list)
来源：http://hz.sysykeji.top/gtwaiafsih.html

================================================================================
来源：http://hz.jqgufenzy.top/gtooyyfdjw.html

E. 字符串处理
来源：http://hz.ybcxt.top/gtcogvvmhb.html

================================================================================
来源：http://hz.xziqi.cn/gtbtalyycr.html

[E01] 拼接字符串
来源：http://hz.tanke756.top/gtixewhcma.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.pycfn.com/gtpbltfili.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.daxiang520.top/gtyudeqmbc.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zycfv.cn/gtvpkydsjq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ehwqpu.com/gtitcqymmr.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.vqdsnc.cn/gtdvwrbqok.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.jinghuilouyu.cn/gteoniuwwr.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.gaohongyu789.top/gtlrfovdfz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.ywan-chungtsiang.top/gtfbaqvguj.html

[E02] 重复字符串
来源：http://hz.wangdashe.top/gtaqyavjkk.html

Py:   "ab" * 3
来源：http://hz.yuanzhike.top/gtlzksfddu.html

PHP:  str_repeat("ab", 3);
来源：http://hz.kuanghao11.cn/gtjhlryglv.html

JS:   "ab".repeat(3)
来源：http://hz.chenjidiqi.icu/gtgybmokjx.html

TS:   "ab".repeat(3)
来源：http://hz.yangfankeji.com/gtejzmfqbq.html

Java: "ab".repeat(3)
来源：http://hz.yuanzhike.top/gtskmdrjqm.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.aizwys.cn/gtqxcrmksk.html

Ruby: "ab" * 3
来源：http://hz.ehwqpu.com/gtzhwmiybi.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.aibaodan.cn/gtgtkxjayc.html

[E03] 截取子串
来源：http://hz.yj20258.top/gtzkzlpofs.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.hongshengwenyu.top/gtrzadpmrm.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.xziqi.cn/gtjnjjfhfw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.havefunace.top/gtzyvypznx.html

TS:   s.slice(1, 4)
来源：http://hz.hnxiangtu.top/gtqhglacvk.html

Java: s.substring(1, 4)
来源：http://hz.sufxvd.cn/gtihqqwdzq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.zhixingplan.top/gtzajhsjsg.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.ivvv.top/gtqzfitepu.html

C#:   s.Substring(1, 3)
来源：http://hz.fengsongda.top/gtnzfeuwmk.html

[E04] 查找子串位置
来源：http://hz.yangfankeji.com/gtrnrvmgnx.html

Py:   s.find("x");  s.index("x")
来源：http://hz.sweek.top/gtrxjiosdy.html

PHP:  strpos($s, "x");
来源：http://hz.9152youxi.cn/gtfxpycgpl.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.xingfuxueyuan.xyz/gtxvkclvfb.html

TS:   s.indexOf("x")
来源：http://hz.jianghu66.top/gtbzrijoch.html

Java: s.indexOf("x")
来源：http://hz.hysaishi.cn/gtrhwcqkfh.html

Go:   strings.Index(s, "x")
来源：http://hz.hysaishi.cn/gttgllpkgx.html

Ruby: s.index("x")
来源：http://hz.cqqwz.cn/gtqubnqmwh.html

C#:   s.IndexOf("x")
来源：http://hz.hammf.cn/gtsfdukrdv.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.xuetiantiany.cn/gtzbvszonn.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.c1oappe.top/gtnxsqblay.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.yonumen.top/gtqmsccdof.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.kuanghao11.cn/gtmnmvvgid.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.havefunace.top/gtppqsjwpu.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jqgufenzy.top/gtwtitmhdp.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.vqdsnc.cn/gtschyxfsc.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.hnqzz.top/gtwxssveel.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.ehwqpu.com/gtzjxceqof.html

[E06] 替换子串
来源：http://hz.ydzc1.top/gtholmgyvx.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.tanke756.top/gtolnsrotl.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.nwbrower.top/gtnmcqkzhp.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.mhx1999.top/gtkkdbzroa.html

TS:   s.replaceAll("a", "b")
来源：http://hz.sufxvd.cn/gtjyrhuwdb.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yj202588.top/gtrghydxfy.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.zhijiandao.cn/gthvekritw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.sxryk.cn/gtfpxjnasf.html

C#:   s.Replace("a", "b")
来源：http://hz.feifeiyinyue.top/gtykmiswug.html

[E07] 按分隔符拆分
来源：http://hz.9152youxi.cn/gthvsvnyim.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.sxryk.cn/gtrxfjhiwk.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.hysaishi.cn/gtmkcvgibo.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.jiagoushi.top/gtlsfpvkqf.html

TS:   s.split(",")
来源：http://hz.jianghu66.top/gtqglubtmq.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.yuxming.cn/gtwccastno.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.iojbl.cn/gtqcbgoarj.html

Ruby: s.split(",");  s.split
来源：http://hz.cashguo.top/gtjyvvuqsa.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.vqdsnc.cn/gteqogyrgo.html

[E08] 数组按分隔符合并
来源：http://hz.sysykeji.top/gtgahztcsg.html

Py:   ",".join(items)
来源：http://hz.yonumen.top/gtoleqqyin.html

PHP:  implode(",", $items);
来源：http://hz.kuanghao11.cn/gtrfvpwokv.html

JS:   items.join(",")
来源：http://hz.xuanzx.com/gtljbnvzup.html

TS:   items.join(",")
来源：http://hz.pengpengdd.cyou/gthdvjetbp.html

Java: String.join(",", items)
来源：http://hz.xylfe.cn/gtqmozbnlj.html

Go:   strings.Join(items, ",")
来源：http://hz.zhaomingkeji.xyz/gtufezmzaq.html

Ruby: items.join(",")
来源：http://hz.jianghu66.top/gtuersdiwn.html

C#:   string.Join(",", items)
来源：http://hz.kuanghao11.cn/gtdugkkgyh.html

[E09] 去除所有空白字符
来源：http://hz.yongpay.top/gthsbhvtbz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.chenjidiqi.icu/gtgnqongwx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.ppjwa.cn/gtgmmazbpv.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.hfpthk.cn/gtfhptssju.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.yangfankeji.com/gtwlgjniqc.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.iojbl.cn/gtypzdsuvv.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.xingfuxueyuan.xyz/gtzbexhuql.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.chenzaomai.com/gtrgmnkyez.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.bjfxy.top/gtpjwhzdcq.html

[E10] 左侧补零 / 定长填充
来源：http://hz.wangshuangyany.cn/gtrhrdoxyp.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.hongshengwenyu.top/gtgvhxypie.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.iojbl.cn/gtkmchkekb.html

JS:   "7".padStart(3, "0")
来源：http://hz.cdnleiting.top/gtgcouvjue.html

TS:   "7".padStart(3, "0")
来源：http://hz.wangshuangyany.cn/gtstqkrtad.html

Java: String.format("%03d", 7)
来源：http://hz.kuanghao11.cn/gtfbgwndna.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.316326.xyz/gtagwvxcrn.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.gogol.net.cn/gtdnkiufsb.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.52xcode.cn/gtafhwuwzb.html

[E11] 反转字符串
来源：http://hz.zhoulong.xyz/gtcuwwtbyu.html

Py:   s[::-1]
来源：http://hz.chenzaomai.com/gtkbhgowld.html

PHP:  strrev($s);
来源：http://hz.svipenyu.cn/gtjebbxurd.html

JS:   [...s].reverse().join("")
来源：http://hz.hfpthk.cn/gtltexnkye.html

TS:   [...s].reverse().join("")
来源：http://hz.hywenlv.cn/gtjolnzxzy.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.gaohongyu789.top/gtuymumdyc.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.hfpthk.cn/gtkqvxtdum.html

Ruby: s.reverse
来源：http://hz.meibo888.top/gtbasoqblh.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.shangyingyoupin.top/gtsyiwzpqq.html

[E12] 统计某字符出现次数
来源：http://hz.shzxlz.cn/gtvnejzqej.html

Py:   s.count("a")
来源：http://hz.xuetiantiany.cn/gtvshfxnhq.html

PHP:  substr_count($s, "a");
来源：http://hz.sweek.top/gtyackntul.html

JS:   s.split("a").length - 1
来源：http://hz.yj202588.top/gtikvkdzus.html

TS:   s.split("a").length - 1
来源：http://hz.shanyushiyangtech.top/gthmjqxxhk.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.vqdsnc.cn/gtkxpbfcgd.html

Go:   strings.Count(s, "a")
来源：http://hz.guowangkeji.top/gtmmzaxtoj.html

Ruby: s.count("a")
来源：http://hz.yueranfly.top/gtajocaowk.html

C#:   s.Count(c => c == 'a')
来源：http://hz.wangshuangyany.cn/gtrvajexik.html

[E13] 逐字符遍历
来源：http://hz.kuanghao11.cn/gtrbpsetgi.html

Py:   for ch in s: print(ch)
来源：http://hz.jqgfzy.top/gtlvnzepxv.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.gaohongyu789.top/gtyvwkhrnb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yonumen.top/gtmyyipxpd.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.nanxinkj.top/gtvrmeuzhr.html


<!-- 参考信息 -->