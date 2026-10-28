代发 wailian999

[D07] 切片 / 取子数组
来源：http://hz.tianlin.xyz/gtgkzsxcmr.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.yuanzhike.top/gtdqklwxxr.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.vqdsnc.cn/gtpwaukjkn.html

JS:   arr.slice(1, 4);
来源：http://hz.xuetiantiany.cn/gtgtwqyccw.html

TS:   arr.slice(1, 4);
来源：http://hz.tian-w.cn/gtwvuqjutq.html

Java: list.subList(1, 4);
来源：http://hz.redwolf501.top/gtaftuufsd.html

Go:   arr[1:4]
来源：http://hz.hongshengwenyu.top/gtmvmyzqvp.html

Ruby: arr[1, 3]
来源：http://hz.shuidangran.top/gtndxjwkzt.html

C#:   list.GetRange(1, 3);
来源：http://hz.9152youxi.cn/gtnhuchiat.html

[D08] 合并两个数组
来源：http://hz.cqqwz.cn/gtvkikjhpu.html

Py:   a + b;  a.extend(b)
来源：http://hz.wangshuangyany.cn/gtqorqkrqs.html

PHP:  array_merge($a, $b);
来源：http://hz.smart0.xyz/gtnlwjaqfc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.andypj.xyz/gteqiegbxw.html

TS:   [...a, ...b];
来源：http://hz.c1oappe.top/gtrsvnbuxy.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.nanxuanxn.top/gtvjcxrfzg.html

Go:   append(a, b...)
来源：http://hz.xuetiantiany.cn/gtsuztpsfu.html

Ruby: a + b;  a.concat(b)
来源：http://hz.xinyue.icu/gtjctffsth.html

C#:   a.Concat(b).ToList()
来源：http://hz.yj20258888.top/gtosmhfmmn.html

[D09] 排序（升序）
来源：http://hz.xylfe.cn/gtrbtwzlji.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.cucudq.cn/gtqaitfrwg.html

PHP:  sort($arr);
来源：http://hz.cdnleiting.top/gtcduulwca.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.bjfxy.top/gtanbomfuv.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.zhongyouzk.top/gtqbonnyhy.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.aibaodan.cn/gtsuiennfa.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.hywenlv.cn/gtrfmlmmhe.html

Ruby: arr.sort
来源：http://hz.snrcjt.cn/gtypqthegm.html

C#:   list.Sort();
来源：http://hz.dashuyun.cn/gtpqxisokx.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.hammf.cn/gtzvcsccqq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.zhixingplan.top/gtbrgoqrmk.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.pengpengdd.cyou/gtduwtxydj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.cashguo.top/gtqbofxedi.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zhoulong.xyz/gtizvvigzn.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.havefunace.top/gtegsvnccm.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.jlsjyb.cn/gtisixyhfj.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.zhiwuduotai.top/gtcascebas.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.svipenyu.cn/gtjbnincdk.html

[D11] 反转数组
来源：http://hz.haohaochexian.top/gtymetcffe.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.jinqigfzy.top/gthfljobfz.html

PHP:  array_reverse($arr);
来源：http://hz.zhongyouzk.top/gtxfkramvm.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.hywenlv.cn/gtzopcqphw.html

TS:   [...arr].reverse();
来源：http://hz.ppjwa.cn/gtnwwhiwak.html

Java: Collections.reverse(list);
来源：http://hz.c1oappe.top/gtzimxmzub.html

Go:   slices.Reverse(arr)
来源：http://hz.vqdsnc.cn/gtupecfrqf.html

Ruby: arr.reverse
来源：http://hz.yonumen.top/gtnbmrgent.html

C#:   list.Reverse();
来源：http://hz.jlsjyb.cn/gtnqkvzvam.html

[D12] 查找元素下标
来源：http://hz.nanxuanxn.top/gtcrqqkwkv.html

Py:   arr.index(x);  x in arr
来源：http://hz.zhengqikj.top/gtqrsorozt.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.9152youxi.cn/gtursgymfx.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.hywenlv.cn/gtfmomjfrs.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.ydjk.org.cn/gtqqbnrrtx.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.jqgfzy.top/gtfsxeeyzi.html

Go:   slices.Index(arr, x)
来源：http://hz.316326.xyz/gteowgqrwm.html

Ruby: arr.index(x)
来源：http://hz.yueranfly.top/gtmxludwej.html

C#:   list.IndexOf(x);
来源：http://hz.jinqigufen.top/gtnpcxohsh.html

[D13] 过滤（保留满足条件的）
来源：http://hz.xylfe.cn/gtbzgwrymn.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.ydzc1.top/gtvvkrximr.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.shzxlz.cn/gtilvfbdsv.html

JS:   arr.filter(x => x > 3)
来源：http://hz.fzhhl.top/gtapkeabiz.html

TS:   arr.filter(x => x > 3)
来源：http://hz.sweek.top/gtkrcjnnhg.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.hnqzz.top/gtirbcafnj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.zhongyouzk.top/gtqejtbnwu.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.shangyingyoupin.top/gtfhyaxibv.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.pengpengdd.cyou/gtjgodaxdr.html

[D14] 映射转换（每个元素变形）
来源：http://hz.chenlongwang.top/gtfqnmeuul.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.yj20258888.top/gtezgmifxp.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.sysykeji.top/gtkeiutpgm.html

JS:   arr.map(x => x * 2)
来源：http://hz.xylfe.cn/gtsocuyrkz.html

TS:   arr.map(x => x * 2)
来源：http://hz.aibaodan.cn/gtpxhzpsdk.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.jyoumei.cn/gtvvorctce.html

Go:   // 手写循环
来源：http://hz.9152youxi.cn/gtmwkhncvh.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.cqqwz.cn/gtdzymocfw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.cheryme.top/gtujsizdik.html

[D15] 去重
来源：http://hz.cucudq.cn/gtxsfbhwxm.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.0kj1m.cn/gtuvbaxhnb.html

PHP:  array_unique($arr);
来源：http://hz.yonumen.top/gtymhxzlxn.html

JS:   [...new Set(arr)]
来源：http://hz.shanyushiyangtech.top/gtgtspiqtm.html

TS:   [...new Set(arr)]
来源：http://hz.quarkkingdee.top/gtdwjatgmh.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.yangfankeji.com/gtedrvsidq.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.aizwys.cn/gtaegtgitc.html

Ruby: arr.uniq
来源：http://hz.sysykeji.top/gtehckdqnm.html

C#:   list.Distinct().ToList()
来源：http://hz.aizwys.cn/gtxsbiotfg.html

[D16] 求和与平均值
来源：http://hz.pengpengdd.cyou/gtggpciboh.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.guowangkeji.top/gtxitxqtkk.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.xylfe.cn/gtpnwispih.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.wangshuangyany.cn/gtcndnisws.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.dianchejie.cn/gtreinybbr.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.ybcxt.top/gtbolceenw.html

Go:   // 手写循环累加
来源：http://hz.yuxming.cn/gtftkbcrse.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.jiagoushi.top/gtcslrwmtr.html

C#:   list.Sum();  list.Average()
来源：http://hz.sysykeji.top/gtmcvikxih.html

[D17] 最大值与最小值
来源：http://hz.jyoumei.cn/gtaqjrsbbx.html

Py:   max(arr);  min(arr)
来源：http://hz.yj20258.top/gtuuilfrva.html

PHP:  max($arr);  min($arr);
来源：http://hz.cucudq.cn/gtzfcojkfp.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.jlsjyb.cn/gtvealdjwy.html

TS:   Math.max(...arr);
来源：http://hz.yj202588.top/gttuilxvok.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.daxiang520.top/gtmfckoqem.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.hammf.cn/gtbwdvrijs.html

Ruby: arr.max;  arr.min
来源：http://hz.shanyushiyangkeji.top/gtlvruzhdh.html

C#:   list.Max();  list.Min()
来源：http://hz.sweek.top/gtctvnvzly.html

[D18] 扁平化嵌套数组
来源：http://hz.yanxiufei.cn/gtduxtssdx.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.nanxuanxn.top/gtdongtrnp.html

PHP:  array_merge(...$nested);
来源：http://hz.wangshuangyany.cn/gtxmfixfnz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.kuanghao11.cn/gtvogcwqzg.html

TS:   nested.flat();
来源：http://hz.nwbrower.top/gtewbfcxdg.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.nanxuanxn.top/gtqumkczke.html

Go:   // 手写双层循环
来源：http://hz.shanyushiyangtech.top/gtwxgjxzfs.html

Ruby: nested.flatten
来源：http://hz.0kj1m.cn/gtjqcqernr.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.9152youxi.cn/gtyuvpxrgb.html

[D19] 按字段分组
来源：http://hz.aizwys.cn/gtiuxgbaip.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.yj20258888.top/gtubgdbwkd.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.yj202588.top/gtvtgndoaq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.gotoacloud.top/gtjoryjlxa.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.havefunace.top/gtsobwvnkg.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.yueranfly.top/gtitqomzhe.html

Go:   // 手写 map[string][]T
来源：http://hz.sysykeji.top/gtvcpubqsp.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.cucudq.cn/gtyxlenxyp.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.yueranfly.top/gtscfcoudl.html

[D20] 统计每个元素出现次数
来源：http://hz.zhoulong.xyz/gtntkjapqt.html

Py:   Counter(arr)
来源：http://hz.nanxuanxn.top/gtapuxkcnz.html

PHP:  array_count_values($arr);
来源：http://hz.xuanzx.com/gtmftyayiv.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.xinyue.icu/gtlhdluxom.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hnxiangtu.top/gtuhacgpjo.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.jlsjyb.cn/gtuwipyyve.html

Go:   // 手写 map[T]int
来源：http://hz.zhijiandao.cn/gthfapspjl.html

Ruby: arr.tally
来源：http://hz.daria6918.cn/gtjjgjnoxr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.hongshengwenyu.top/gtgdplxpnp.html

[D21] 判断是否包含某元素
来源：http://hz.xinyue.icu/gtowqqdcbr.html

Py:   x in arr
来源：http://hz.mhx1999.top/gtubwswibd.html

PHP:  in_array($x, $arr, true);
来源：http://hz.gotoacloud.top/gtoisednpc.html

JS:   arr.includes(x)
来源：http://hz.aibaodan.cn/gtoahnkcqd.html

TS:   arr.includes(x)
来源：http://hz.wangdashe.top/gtvkbxtaxp.html

Java: list.contains(x)
来源：http://hz.cucudq.cn/gtddnjiseg.html

Go:   slices.Contains(arr, x)
来源：http://hz.tianlin.xyz/gtebbswdrk.html

Ruby: arr.include?(x)
来源：http://hz.guannengcc.top/gtausjpmmu.html

C#:   list.Contains(x)
来源：http://hz.jlsjyb.cn/gtytdmcjvu.html

[D22] 复制数组（避免共享引用）
来源：http://hz.shanyushiyangtech.top/gtcoejehfg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.jinqigfzy.top/gtshargodg.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.gogol.net.cn/gtrgdmnbhz.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.0kj1m.cn/gtxkcosvcx.html

TS:   [...arr];
来源：http://hz.yuanzhike.top/gtoonnjqey.html

Java: new ArrayList<>(list);
来源：http://hz.daria6918.cn/gtxrxchmzp.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.ppjwa.cn/gtgjnwrfcw.html

Ruby: arr.dup;  arr.clone
来源：http://hz.daxiang520.top/gtyfueobrl.html

C#:   new List<int>(list);
来源：http://hz.yueranfly.top/gtdmyepory.html

[D23] reduce 累积计算
来源：http://hz.yj20258.top/gtbuziyjda.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.cdnleiting.top/gtgnequjet.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.yuanzhike.top/gtxzdmawyd.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.pycfn.com/gtoofozdwy.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.aibaodan.cn/gtehbxbheu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.xuetiantiany.cn/gtyzgeywze.html

Go:   // 手写循环
来源：http://hz.jyoumei.cn/gtororqacq.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.fengsongda.top/gtmoabxrka.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.jinqigfzy.top/gtrthuqzcl.html

[D24] 字典 / Map 基本操作
来源：http://hz.sweek.top/gtvwatokhe.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.cqqwz.cn/gtuexipujw.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.hywenlv.cn/gtdxpwhnvk.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.svipenyu.cn/gtcbtdtrko.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.ywan-chungtsiang.top/gtbprpeqyd.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.zhoulong.xyz/gtrfmyxhkj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.xinyue.icu/gtznefypet.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.9152youxi.cn/gtzkljfitn.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.ppjwa.cn/gtzspizrve.html

[D25] Set 集合去重与交并差
来源：http://hz.jqgfzy.top/gtjpmicygl.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.zhiwuduotai.top/gtdrufbaed.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.yonumen.top/gtnkjggate.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.hongshengwenyu.top/gthahdwlyw.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.nwbrower.top/gtjvivwgbr.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.gogol.net.cn/gtdfijspnl.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.ehwqpu.com/gtiwqghhcz.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.c1oappe.top/gtndsmrmyh.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.xinyue.icu/gtuggwjmge.html

[D26] 数组转字符串
来源：http://hz.ivvv.top/gtzwwnskbq.html

Py:   ", ".join(map(str, arr))
来源：http://hz.jianghu66.top/gtjvhubwsc.html

PHP:  implode(", ", $arr);
来源：http://hz.yanxiufei.cn/gtmxxafzdo.html

JS:   arr.join(", ")
来源：http://hz.cdnleiting.top/gtvtbuauyc.html

TS:   arr.join(", ")
来源：http://hz.havefunace.top/gtwjqeowyi.html

Java: String.join(", ", list)
来源：http://hz.kuanghao11.cn/gthnjguioq.html

Go:   strings.Join(strs, ", ")
来源：http://hz.wangshuangyany.cn/gtmovtsuvj.html

Ruby: arr.join(", ")
来源：http://hz.aizwys.cn/gtdtqbuoxz.html

C#:   string.Join(", ", list)
来源：http://hz.nanxinkj.top/gtsncuqspv.html

================================================================================
来源：http://hz.guannengcc.top/gtxudueiph.html

E. 字符串处理
来源：http://hz.gogol.net.cn/gtnkxrmpxk.html

================================================================================
来源：http://hz.yvedp.cn/gtccoyzxni.html

[E01] 拼接字符串
来源：http://hz.yj20258.top/gtnesdzegs.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.yvedp.cn/gtebhlwvtt.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.cashguo.top/gtafilhkmb.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yj202588.top/gtgxrymnjh.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ywan-chungtsiang.top/gtfjmexihf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.chenjidiqi.icu/gtmigfcwhc.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.shanyushiyangtech.top/gtwlpjwhsw.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.havefunace.top/gtagwhvzcq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.yanxiufei.cn/gtdxpcjwwb.html

[E02] 重复字符串
来源：http://hz.sweek.top/gtlqujsgia.html

Py:   "ab" * 3
来源：http://hz.jlsjyb.cn/gtesguwhwf.html

PHP:  str_repeat("ab", 3);
来源：http://hz.daria6918.cn/gtxkdlzfyr.html

JS:   "ab".repeat(3)
来源：http://hz.yueranfly.top/gtxqhteirb.html

TS:   "ab".repeat(3)
来源：http://hz.9152youxi.cn/gtphlquewf.html

Java: "ab".repeat(3)
来源：http://hz.zdqjudy.top/gtlheuovfb.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.yangfankeji.com/gtyddxtdgd.html

Ruby: "ab" * 3
来源：http://hz.daria6918.cn/gtkkmtrncf.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.ivvv.top/gtrwlkokcl.html

[E03] 截取子串
来源：http://hz.xylfe.cn/gthdnjuemw.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.cashguo.top/gtxdgsmoyf.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.0kj1m.cn/gtfnknmnno.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.yanxiufei.cn/gtsfxwwhrn.html

TS:   s.slice(1, 4)
来源：http://hz.nanxuanxn.top/gtrzbaaqgy.html

Java: s.substring(1, 4)
来源：http://hz.zhengqikj.top/gtvabxmvjk.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.yonumen.top/gtziqhqeau.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.hysaishi.cn/gtxncerbww.html

C#:   s.Substring(1, 3)
来源：http://hz.chenzaomai.com/gtdtjmrjdg.html

[E04] 查找子串位置
来源：http://hz.pengpengdd.cyou/gteqbxpmjs.html

Py:   s.find("x");  s.index("x")
来源：http://hz.52xcode.cn/gtpnsljbzf.html

PHP:  strpos($s, "x");
来源：http://hz.9152youxi.cn/gtejrdtfnw.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.shzxlz.cn/gttdrorslx.html

TS:   s.indexOf("x")
来源：http://hz.yuxming.cn/gtivrocyuq.html

Java: s.indexOf("x")
来源：http://hz.gogol.net.cn/gtzdddkbus.html

Go:   strings.Index(s, "x")
来源：http://hz.gaohongyu789.top/gtgvedfsnp.html

Ruby: s.index("x")
来源：http://hz.haohaochexian.top/gtjkfabeiy.html

C#:   s.IndexOf("x")
来源：http://hz.yongpay.top/gtlhmhtatx.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.xuanzx.com/gtcanyhbwd.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.birdmap.top/gtewtibryt.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.zhengqikj.top/gtrrqmeutf.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jianghu66.top/gtzyapmtff.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.gzhubu.top/gtgificmua.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.xinyue.icu/gtqwuukkjn.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.shzxlz.cn/gtgpsoihog.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.ivvv.top/gtectjrplq.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.feifeiyinyue.top/gtfijccogd.html

[E06] 替换子串
来源：http://hz.yuxming.cn/gtaonzzlxp.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.sysykeji.top/gtmckambkt.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.haohaochexian.top/gtoxefnkhm.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.shuidangran.top/gtomxesabk.html

TS:   s.replaceAll("a", "b")
来源：http://hz.jiagoushi.top/gtcfbxyblb.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.redwolf501.top/gtuspovoye.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.shuidangran.top/gtcmdcstzn.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.xuanzx.com/gtceoxswcd.html

C#:   s.Replace("a", "b")
来源：http://hz.snrcjt.cn/gtcvzknnof.html

[E07] 按分隔符拆分
来源：http://hz.jqgufenzy.top/gtxuuylxdu.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.xuanzx.com/gtliokcmjm.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.0kj1m.cn/gttlizlsli.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.dashuyun.cn/gtyojsofwu.html

TS:   s.split(",")
来源：http://hz.c1oappe.top/gttagmjwta.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.tanke756.top/gtauzwyqry.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.zhixingplan.top/gtoqonuxtj.html

Ruby: s.split(",");  s.split
来源：http://hz.yonumen.top/gtswtbucqe.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.jiagoushi.top/gtvdsxnkno.html

[E08] 数组按分隔符合并
来源：http://hz.wangdashe.top/gtomcgzdhm.html

Py:   ",".join(items)
来源：http://hz.gogol.net.cn/gtyqoduhub.html

PHP:  implode(",", $items);
来源：http://hz.jinyuanbaomall.cn/gtimbggwyg.html

JS:   items.join(",")
来源：http://hz.ydjk.org.cn/gtsujhmqru.html

TS:   items.join(",")
来源：http://hz.smart0.xyz/gtrvfmtgnb.html

Java: String.join(",", items)
来源：http://hz.cheryme.top/gtzabbydwu.html

Go:   strings.Join(items, ",")
来源：http://hz.zhongyouzk.top/gthpxotusq.html

Ruby: items.join(",")
来源：http://hz.zhoulong.xyz/gtchfroqxn.html

C#:   string.Join(",", items)
来源：http://hz.ybcxt.top/gtflcxqkli.html

[E09] 去除所有空白字符
来源：http://hz.vqdsnc.cn/gtgjbrgrhc.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.svipenyu.cn/gtqasekvcw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.svipenyu.cn/gtpkwhepcp.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.hammf.cn/gtexmgsmnx.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.xingfuxueyuan.xyz/gtbyyxjnxw.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.xinyue.icu/gtlzkczmvy.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.zhoulong.xyz/gtmyztdkdj.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.guannengcc.top/gtnouhzqcf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.hnqzz.top/gtimlfupot.html

[E10] 左侧补零 / 定长填充
来源：http://hz.bjfxy.top/gtzuktqjim.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.shzxlz.cn/gtgykldrep.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.yueranfly.top/gtarsojgjl.html

JS:   "7".padStart(3, "0")
来源：http://hz.vqdsnc.cn/gtxrlvanvk.html

TS:   "7".padStart(3, "0")
来源：http://hz.jqgfzy.top/gtoqumbgps.html

Java: String.format("%03d", 7)
来源：http://hz.meibo888.top/gtcnaxxwmd.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.jiagoushi.top/gtlkeiqejl.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.sxryk.cn/gtrzkrapur.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.kuanghao11.cn/gtafpeayjb.html

[E11] 反转字符串
来源：http://hz.havefunace.top/gtptdekbnx.html

Py:   s[::-1]
来源：http://hz.guowangkeji.top/gtdycnkntz.html

PHP:  strrev($s);
来源：http://hz.yuanzhike.top/gtqouvnguo.html

JS:   [...s].reverse().join("")
来源：http://hz.zhaomingkeji.xyz/gtkcozyfgy.html

TS:   [...s].reverse().join("")
来源：http://hz.dianchejie.cn/gtbonyqeat.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.hfpthk.cn/gtvarznlmy.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.shanyushiyangkeji.top/gtfeqagvgq.html

Ruby: s.reverse
来源：http://hz.xingfuxueyuan.xyz/gttgqvowus.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.hammf.cn/gtkeuktlyn.html

[E12] 统计某字符出现次数
来源：http://hz.shanyushiyangkeji.top/gtuxgakhla.html

Py:   s.count("a")
来源：http://hz.yj202588.top/gtccoxrnzl.html

PHP:  substr_count($s, "a");
来源：http://hz.aibaodan.cn/gtpvuclotm.html

JS:   s.split("a").length - 1
来源：http://hz.cqqwz.cn/gtgzlnqqdf.html

TS:   s.split("a").length - 1
来源：http://hz.yj202588.top/gtgqcgekjo.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.tianlin.xyz/gtdvplpjel.html

Go:   strings.Count(s, "a")
来源：http://hz.gotoacloud.top/gtseqgcsmn.html

Ruby: s.count("a")
来源：http://hz.chenzaomai.com/gtoxznanfs.html

C#:   s.Count(c => c == 'a')
来源：http://hz.xingfuxueyuan.xyz/gtioswzwyu.html

[E13] 逐字符遍历
来源：http://hz.hnqzz.top/gtaljfekky.html

Py:   for ch in s: print(ch)
来源：http://hz.sysykeji.top/gtjeqtnbar.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.guannengcc.top/gtowmirnay.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.nanxuanxn.top/gttlrcqdzu.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.tian-w.cn/gtnmxrnmiv.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.ydzc1.top/gtquthqtxp.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.ivvv.top/gtnjccithj.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.cheryme.top/gtuyqnxtcs.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.316326.xyz/gtxibrtpdg.html


<!-- 参考信息 -->