代发 wailian999

Java: list.size();
来源：http://hz.gotoacloud.top/gtjvbztslt.html

Go:   len(arr)
来源：http://hz.shuidangran.top/gtincrjgxs.html

Ruby: arr.length; arr.size
来源：http://hz.jqgufenzy.top/gtstxwxisf.html

C#:   list.Count;
来源：http://hz.yj20258888.top/gtvhgbpdoc.html

[D07] 切片 / 取子数组
来源：http://hz.jinqigfzy.top/gtwrvjybpv.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.zhengqikj.top/gtdkiqfsks.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.svipenyu.cn/gtkshdiqug.html

JS:   arr.slice(1, 4);
来源：http://hz.jqgfzy.top/gtyagvnfuh.html

TS:   arr.slice(1, 4);
来源：http://hz.9152youxi.cn/gtzwpliqhv.html

Java: list.subList(1, 4);
来源：http://hz.cqqwz.cn/gtymiuvxcn.html

Go:   arr[1:4]
来源：http://hz.zhaomingkeji.xyz/gtnpyrgopb.html

Ruby: arr[1, 3]
来源：http://hz.xingfuxueyuan.xyz/gtzooxdeds.html

C#:   list.GetRange(1, 3);
来源：http://hz.xuetiantiany.cn/gtnrekgjpc.html

[D08] 合并两个数组
来源：http://hz.cucudq.cn/gtgxorhydo.html

Py:   a + b;  a.extend(b)
来源：http://hz.c1oappe.top/gtoxmpsnrz.html

PHP:  array_merge($a, $b);
来源：http://hz.shanyushiyangkeji.top/gtcjxbfgbw.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.yanxiufei.cn/gtcwrxorlt.html

TS:   [...a, ...b];
来源：http://hz.zdqjudy.top/gtlftfxnwd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.mhx1999.top/gtuvficqbw.html

Go:   append(a, b...)
来源：http://hz.iojbl.cn/gtnmzlclap.html

Ruby: a + b;  a.concat(b)
来源：http://hz.shangyingyoupin.top/gtgcxmhaub.html

C#:   a.Concat(b).ToList()
来源：http://hz.fzhhl.top/gtrlyirjwz.html

[D09] 排序（升序）
来源：http://hz.snrcjt.cn/gtmbzpgnqb.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.andypj.xyz/gtfauubrwx.html

PHP:  sort($arr);
来源：http://hz.daxiang520.top/gtpfmhuemo.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.52xcode.cn/gtdlvtzccu.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.cdnleiting.top/gtkjokkuwr.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.yanxiufei.cn/gtvqpaeklc.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.bjfxy.top/gthchqxwmb.html

Ruby: arr.sort
来源：http://hz.aibaodan.cn/gthfjwpvwj.html

C#:   list.Sort();
来源：http://hz.shangyingyoupin.top/gtauqiftuz.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.yuanzhike.top/gtjjwpxcdr.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.jqgufenzy.top/gtvgjaduya.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jlsjyb.cn/gtvgpbazlp.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yonumen.top/gtgqtsolmb.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xinyue.icu/gtvrfarjpv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.jqgufenzy.top/gtdjwejrit.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.shanyushiyangtech.top/gtyocemmzh.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.yj20258.top/gtqwdkkark.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.xuetiantiany.cn/gtibiuvtxc.html

[D11] 反转数组
来源：http://hz.sufxvd.cn/gtzregnwwy.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.cdnleiting.top/gtzddbhqtq.html

PHP:  array_reverse($arr);
来源：http://hz.ywan-chungtsiang.top/gtldznlhry.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.xylfe.cn/gtrckvrxxi.html

TS:   [...arr].reverse();
来源：http://hz.gotoacloud.top/gtprqvwjrm.html

Java: Collections.reverse(list);
来源：http://hz.ywan-chungtsiang.top/gtnnwsbmrn.html

Go:   slices.Reverse(arr)
来源：http://hz.zhijiandao.cn/gtwuvllopm.html

Ruby: arr.reverse
来源：http://hz.fzhhl.top/gtjsqcgweo.html

C#:   list.Reverse();
来源：http://hz.sysykeji.top/gtfeteueqn.html

[D12] 查找元素下标
来源：http://hz.zhongyouzk.top/gtbdrgrlax.html

Py:   arr.index(x);  x in arr
来源：http://hz.hysaishi.cn/gtobmtocqd.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.jinqigufen.top/gtxdpmwubf.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zhoulong.xyz/gtrugotfcs.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.haohaochexian.top/gtujwyshqt.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.xylfe.cn/gtpcgzzyrb.html

Go:   slices.Index(arr, x)
来源：http://hz.xuetiantiany.cn/gtixueijcx.html

Ruby: arr.index(x)
来源：http://hz.svipenyu.cn/gtietkiiko.html

C#:   list.IndexOf(x);
来源：http://hz.jianghu66.top/gtylmzltzg.html

[D13] 过滤（保留满足条件的）
来源：http://hz.gzhubu.top/gtzjpaxsjv.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.hongshengwenyu.top/gtfgzzkljm.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.jiagoushi.top/gtrgiurhkz.html

JS:   arr.filter(x => x > 3)
来源：http://hz.meibo888.top/gtwptvnshh.html

TS:   arr.filter(x => x > 3)
来源：http://hz.wangdashe.top/gtsdhspaly.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.yuxming.cn/gtlueckmpw.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.xuanzx.com/gttjcfrbja.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.aizwys.cn/gtutscxhvh.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.tanke756.top/gtnevqerlf.html

[D14] 映射转换（每个元素变形）
来源：http://hz.yangfankeji.com/gtntxmdjrp.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.yj20258.top/gtlmoniwum.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.yvedp.cn/gttdagidza.html

JS:   arr.map(x => x * 2)
来源：http://hz.yj202588.top/gtztfhzsxt.html

TS:   arr.map(x => x * 2)
来源：http://hz.zdqjudy.top/gtnlglnzgr.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.jyoumei.cn/gtojipxvon.html

Go:   // 手写循环
来源：http://hz.shzxlz.cn/gtircofgwj.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.iojbl.cn/gtvmgodtrn.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.yj20258.top/gtpzcebsnu.html

[D15] 去重
来源：http://hz.meibo888.top/gtjldnhise.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.gotoacloud.top/gtsgjcrozr.html

PHP:  array_unique($arr);
来源：http://hz.jinqigufen.top/gtndjlmynd.html

JS:   [...new Set(arr)]
来源：http://hz.hnxiangtu.top/gtyklbfujv.html

TS:   [...new Set(arr)]
来源：http://hz.yonumen.top/gtdjeyijnn.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.andypj.xyz/gtdghlquhe.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.feifeiyinyue.top/gtosdcsgbx.html

Ruby: arr.uniq
来源：http://hz.zycfv.cn/gtrkasptji.html

C#:   list.Distinct().ToList()
来源：http://hz.cucudq.cn/gtiezrqdkg.html

[D16] 求和与平均值
来源：http://hz.yueranfly.top/gtrvklrbdz.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.yj20258888.top/gtmnmoxmkz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.zhengqikj.top/gtoyiaqqty.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zdqjudy.top/gtvddiedxy.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.tian-w.cn/gtxzlwnlnn.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.xuetiantiany.cn/gtjeuejual.html

Go:   // 手写循环累加
来源：http://hz.iojbl.cn/gtwetogvck.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.chenzaomai.com/gthajzrove.html

C#:   list.Sum();  list.Average()
来源：http://hz.hnxiangtu.top/gtnmveclgh.html

[D17] 最大值与最小值
来源：http://hz.havefunace.top/gtdgrvfbru.html

Py:   max(arr);  min(arr)
来源：http://hz.sxryk.cn/gtqhmtiqbc.html

PHP:  max($arr);  min($arr);
来源：http://hz.gogol.net.cn/gtzxvwlqxn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.ydzc1.top/gtllloijie.html

TS:   Math.max(...arr);
来源：http://hz.xuanzx.com/gtxxungvdu.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.jianghu66.top/gtytqsgkrv.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.yongpay.top/gtzphuupqs.html

Ruby: arr.max;  arr.min
来源：http://hz.chenlongwang.top/gtnvbjkybm.html

C#:   list.Max();  list.Min()
来源：http://hz.kuanghao11.cn/gtyhnepxcr.html

[D18] 扁平化嵌套数组
来源：http://hz.shanyushiyangkeji.top/gtlhgxxmos.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.yonumen.top/gtsmchdhmz.html

PHP:  array_merge(...$nested);
来源：http://hz.hongshengwenyu.top/gtcaechfid.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.yuanzhike.top/gtnprrjvjp.html

TS:   nested.flat();
来源：http://hz.jlsjyb.cn/gtlqckjwjx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.yuxming.cn/gtryufipgo.html

Go:   // 手写双层循环
来源：http://hz.jinqigfzy.top/gtwixoovwz.html

Ruby: nested.flatten
来源：http://hz.xziqi.cn/gtmkfstjax.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.ydjk.org.cn/gtiuzqrpco.html

[D19] 按字段分组
来源：http://hz.sysykeji.top/gtjleugxmb.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.yj20258888.top/gtakshxdkh.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.dashuyun.cn/gtuvlfonng.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.tian-w.cn/gtisnoabxo.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.ydzc1.top/gtfxnsusaj.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.pengpengdd.cyou/gtnektqmdy.html

Go:   // 手写 map[string][]T
来源：http://hz.yangfankeji.com/gtxzgdwkyr.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.jinghuilouyu.cn/gtlfajcyva.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.zhijiandao.cn/gteynyozza.html

[D20] 统计每个元素出现次数
来源：http://hz.xylfe.cn/gtnkqgdizi.html

Py:   Counter(arr)
来源：http://hz.jiagoushi.top/gtzemqxyjq.html

PHP:  array_count_values($arr);
来源：http://hz.gotoacloud.top/gtptzvtmqr.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.bjfxy.top/gtyywkwirk.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jinyuanbaomall.cn/gteipmtuhy.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.ywan-chungtsiang.top/gtvxmiplkl.html

Go:   // 手写 map[T]int
来源：http://hz.316326.xyz/gtcbfenjcl.html

Ruby: arr.tally
来源：http://hz.haohaochexian.top/gtacngrqgn.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.ywan-chungtsiang.top/gtnpbtibwm.html

[D21] 判断是否包含某元素
来源：http://hz.yvedp.cn/gttpuwijcl.html

Py:   x in arr
来源：http://hz.havefunace.top/gtipxhaevu.html

PHP:  in_array($x, $arr, true);
来源：http://hz.ybcxt.top/gtcgkrwctn.html

JS:   arr.includes(x)
来源：http://hz.daxiang520.top/gtgjajnivh.html

TS:   arr.includes(x)
来源：http://hz.zhixingplan.top/gtstsggvsf.html

Java: list.contains(x)
来源：http://hz.birdmap.top/gtkgawioqc.html

Go:   slices.Contains(arr, x)
来源：http://hz.aibaodan.cn/gtahwkrihh.html

Ruby: arr.include?(x)
来源：http://hz.quarkkingdee.top/gtkfynnjay.html

C#:   list.Contains(x)
来源：http://hz.shanyushiyangtech.top/gtilneuuqv.html

[D22] 复制数组（避免共享引用）
来源：http://hz.svipenyu.cn/gtmivgjppr.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.tanke756.top/gtifsitztt.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.sufxvd.cn/gtrgdkipnh.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.dashuyun.cn/gttxhfhsbo.html

TS:   [...arr];
来源：http://hz.cashguo.top/gtmnmwxhca.html

Java: new ArrayList<>(list);
来源：http://hz.cheryme.top/gtabwgcwny.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.feifeiyinyue.top/gtpzggowna.html

Ruby: arr.dup;  arr.clone
来源：http://hz.bjfxy.top/gtwgvlumxx.html

C#:   new List<int>(list);
来源：http://hz.jqgfzy.top/gtwhheftix.html

[D23] reduce 累积计算
来源：http://hz.hnqzz.top/gtwwpjkuaq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.yonumen.top/gtdsllmowa.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.hammf.cn/gtjmqtwvfo.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.havefunace.top/gtvekijbxk.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yueranfly.top/gtfqrwvqdm.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.hnqzz.top/gtkhqnizrs.html

Go:   // 手写循环
来源：http://hz.52xcode.cn/gtwmesfyco.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.pycfn.com/gthlqiljxp.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.bjfxy.top/gtywxlaiqj.html

[D24] 字典 / Map 基本操作
来源：http://hz.zhengqikj.top/gtvxovunac.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.zhixingplan.top/gtsiouywam.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.yangfankeji.com/gtpoynduim.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.andypj.xyz/gtqiitdonz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.nanxinkj.top/gtxeacvepz.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.bjfxy.top/gtessuofma.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.0kj1m.cn/gtwbzjrway.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.yonumen.top/gtlqtmammf.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.feifeiyinyue.top/gtxbviovbp.html

[D25] Set 集合去重与交并差
来源：http://hz.cqqwz.cn/gtpkretznu.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.yonumen.top/gthxjotocc.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.wangdashe.top/gtdzszhvsx.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.meibo888.top/gtbkupibbu.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.hnqzz.top/gttrcnaybf.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.snrcjt.cn/gttvrxsphk.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.cdnleiting.top/gtnzbrkcha.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.yanxiufei.cn/gtyzmboahf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.smart0.xyz/gtkabnrwok.html

[D26] 数组转字符串
来源：http://hz.jqgfzy.top/gtdzoxfjui.html

Py:   ", ".join(map(str, arr))
来源：http://hz.shangyingyoupin.top/gtwpxoztam.html

PHP:  implode(", ", $arr);
来源：http://hz.jinyuanbaomall.cn/gttgxtfvrc.html

JS:   arr.join(", ")
来源：http://hz.svipenyu.cn/gtyjzuvgan.html

TS:   arr.join(", ")
来源：http://hz.sxryk.cn/gtsjjscxcx.html

Java: String.join(", ", list)
来源：http://hz.daria6918.cn/gtjswnjxak.html

Go:   strings.Join(strs, ", ")
来源：http://hz.kuanghao11.cn/gtblyvdyrd.html

Ruby: arr.join(", ")
来源：http://hz.ehwqpu.com/gtvnhhzplv.html

C#:   string.Join(", ", list)
来源：http://hz.jinyuanbaomall.cn/gteoqkdpxf.html

================================================================================
来源：http://hz.xinyue.icu/gteoivgzvu.html

E. 字符串处理
来源：http://hz.xuetiantiany.cn/gtgcqganfu.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtwirdscuo.html

[E01] 拼接字符串
来源：http://hz.xinyue.icu/gtguwmthda.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.jlsjyb.cn/gtxrxibilc.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.zhiwuduotai.top/gtkjtgkzyy.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.guannengcc.top/gtfceqbjbb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yuxming.cn/gtzkaeorhu.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.0kj1m.cn/gtmsqypqxb.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.jinqigfzy.top/gtwhedxclk.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.gotoacloud.top/gtigfhjuhq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.chenzaomai.com/gtfzxngevx.html

[E02] 重复字符串
来源：http://hz.zhixingplan.top/gtwsneogtv.html

Py:   "ab" * 3
来源：http://hz.aizwys.cn/gtcdeioczk.html

PHP:  str_repeat("ab", 3);
来源：http://hz.gaohongyu789.top/gtmjgsisuo.html

JS:   "ab".repeat(3)
来源：http://hz.iojbl.cn/gtckuhdwjo.html

TS:   "ab".repeat(3)
来源：http://hz.nanxuanxn.top/gtxlydfqoo.html

Java: "ab".repeat(3)
来源：http://hz.iojbl.cn/gtsqyjnszg.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.nanxinkj.top/gtuhstgkgt.html

Ruby: "ab" * 3
来源：http://hz.yanxiufei.cn/gtroumqlmv.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.yj20258.top/gtjlkukjky.html

[E03] 截取子串
来源：http://hz.daxiang520.top/gtuvpgvxmz.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.jyoumei.cn/gtmzmuppjk.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.bjfxy.top/gtpezakize.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.zhiwuduotai.top/gtsdzkwoqd.html

TS:   s.slice(1, 4)
来源：http://hz.tanke756.top/gtkhzojjnm.html

Java: s.substring(1, 4)
来源：http://hz.wangdashe.top/gtxsazwgiu.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.hysaishi.cn/gtzxuthwzw.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.xuanzx.com/gtltxglvjc.html

C#:   s.Substring(1, 3)
来源：http://hz.gaohongyu789.top/gtjsiqisfe.html

[E04] 查找子串位置
来源：http://hz.chenjidiqi.icu/gtlfaoggmn.html

Py:   s.find("x");  s.index("x")
来源：http://hz.jianghu66.top/gtzsbiihcd.html

PHP:  strpos($s, "x");
来源：http://hz.shzxlz.cn/gtqfosvxnd.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.shangyingyoupin.top/gtlfcrbxts.html

TS:   s.indexOf("x")
来源：http://hz.svipenyu.cn/gtrjkifgbq.html

Java: s.indexOf("x")
来源：http://hz.hysaishi.cn/gtbqnetmuu.html

Go:   strings.Index(s, "x")
来源：http://hz.haohaochexian.top/gthmtmlnfi.html

Ruby: s.index("x")
来源：http://hz.jyoumei.cn/gthnijkogz.html

C#:   s.IndexOf("x")
来源：http://hz.birdmap.top/gtlfcsahel.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.0kj1m.cn/gtxuhefgeg.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.tanke756.top/gtktkeifnq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.havefunace.top/gtlpeujswk.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.havefunace.top/gtodnsdtib.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.jqgfzy.top/gtjmnefgqv.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jinghuilouyu.cn/gtlbwuvmmp.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.havefunace.top/gtwlorufgu.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.ydjk.org.cn/gtuvgxzblt.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.sufxvd.cn/gtazxitibc.html

[E06] 替换子串
来源：http://hz.andypj.xyz/gtcaldgrwd.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.redwolf501.top/gttnyavckq.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.vqdsnc.cn/gtlzmgqcak.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.xylfe.cn/gtowraapgr.html

TS:   s.replaceAll("a", "b")
来源：http://hz.cashguo.top/gtnpenonfd.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.chenlongwang.top/gtuisggipn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.zycfv.cn/gtvnxzrmgc.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.bjfxy.top/gtyciqmubg.html

C#:   s.Replace("a", "b")
来源：http://hz.mhx1999.top/gtuhxqwqgo.html

[E07] 按分隔符拆分
来源：http://hz.sxryk.cn/gtqkajyong.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.yvedp.cn/gtlqcwqdug.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.snrcjt.cn/gtyehpnrrj.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.yuanzhike.top/gtqblratwz.html

TS:   s.split(",")
来源：http://hz.ydjk.org.cn/gtbemcqqhv.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.0kj1m.cn/gtmfusmsbq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.jinyuanbaomall.cn/gtxpqktmyo.html

Ruby: s.split(",");  s.split
来源：http://hz.wangdashe.top/gtnjpjulgi.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.dianchejie.cn/gtezkrtndz.html

[E08] 数组按分隔符合并
来源：http://hz.hfpthk.cn/gtegvadlie.html

Py:   ",".join(items)
来源：http://hz.hammf.cn/gtvykppjkl.html

PHP:  implode(",", $items);
来源：http://hz.gogol.net.cn/gtkkmdbels.html

JS:   items.join(",")
来源：http://hz.nwbrower.top/gtkyqxtrow.html

TS:   items.join(",")
来源：http://hz.yongpay.top/gtjlhvkxzj.html

Java: String.join(",", items)
来源：http://hz.52xcode.cn/gtvcpetfri.html

Go:   strings.Join(items, ",")
来源：http://hz.andypj.xyz/gtdprrapfp.html

Ruby: items.join(",")
来源：http://hz.chenjidiqi.icu/gtiadxotml.html

C#:   string.Join(",", items)
来源：http://hz.wangshuangyany.cn/gthxafwucz.html

[E09] 去除所有空白字符
来源：http://hz.ehwqpu.com/gtuvrfncvs.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.ywan-chungtsiang.top/gtsihktsin.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.jyoumei.cn/gtxkigyehn.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.vqdsnc.cn/gtfwaanrkr.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.feifeiyinyue.top/gtlcfvapic.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.sweek.top/gtqjrvqsgm.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.ppjwa.cn/gtnqqllqoa.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.yuanzhike.top/gthierduko.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.dashuyun.cn/gtlcionczq.html

[E10] 左侧补零 / 定长填充
来源：http://hz.yj20258.top/gtbpnnwxjm.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.shzxlz.cn/gtttfbodzx.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.yj202588.top/gtpfzxmdzz.html

JS:   "7".padStart(3, "0")
来源：http://hz.andypj.xyz/gtntckbhwq.html

TS:   "7".padStart(3, "0")
来源：http://hz.52xcode.cn/gtoajvpqck.html

Java: String.format("%03d", 7)
来源：http://hz.shanyushiyangtech.top/gtqbziajlt.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.yuxming.cn/gtgvbgnvmq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.cucudq.cn/gtesatnkmc.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.aizwys.cn/gtpcxtcbvu.html

[E11] 反转字符串
来源：http://hz.jianghu66.top/gtnwucxbsl.html

Py:   s[::-1]
来源：http://hz.wangshuangyany.cn/gtxstpowqp.html

PHP:  strrev($s);
来源：http://hz.hfpthk.cn/gtqzdxaofu.html

JS:   [...s].reverse().join("")
来源：http://hz.cashguo.top/gtndgfeqiz.html

TS:   [...s].reverse().join("")
来源：http://hz.nwbrower.top/gtloubtdjy.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.shzxlz.cn/gtdkcfonqi.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.9152youxi.cn/gtqkweplwl.html

Ruby: s.reverse
来源：http://hz.chenzaomai.com/gtzenpsnlc.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.nanxinkj.top/gtpljsgtpe.html

[E12] 统计某字符出现次数
来源：http://hz.iojbl.cn/gtupwjexxk.html

Py:   s.count("a")
来源：http://hz.fengsongda.top/gtqypzpeao.html

PHP:  substr_count($s, "a");
来源：http://hz.jinyuanbaomall.cn/gtnfcarhbb.html

JS:   s.split("a").length - 1
来源：http://hz.yongpay.top/gtlgupbjrl.html

TS:   s.split("a").length - 1
来源：http://hz.sufxvd.cn/gtjwhiaxxz.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.xingfuxueyuan.xyz/gtrrrnlkzb.html

Go:   strings.Count(s, "a")
来源：http://hz.jinqigfzy.top/gtypdjrlrr.html

Ruby: s.count("a")
来源：http://hz.hfpthk.cn/gtgrieykmh.html

C#:   s.Count(c => c == 'a')
来源：http://hz.shanyushiyangkeji.top/gtpgbcjwxp.html

[E13] 逐字符遍历
来源：http://hz.hnqzz.top/gtaqrwfqxd.html

Py:   for ch in s: print(ch)
来源：http://hz.gaohongyu789.top/gtfjjeftpp.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.zhijiandao.cn/gtzxqljgki.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.shzxlz.cn/gtujoyztta.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.meibo888.top/gtezbymbio.html


<!-- 参考信息 -->