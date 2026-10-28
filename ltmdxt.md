代发 wailian999

[D07] 切片 / 取子数组
来源：http://hz.jlsjyb.cn/gthqwsaglu.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.hywenlv.cn/gtrudojfbn.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.ywan-chungtsiang.top/gtsdozzpuu.html

JS:   arr.slice(1, 4);
来源：http://hz.yanxiufei.cn/gtyfoptffv.html

TS:   arr.slice(1, 4);
来源：http://hz.jinyuanbaomall.cn/gtclfvjjul.html

Java: list.subList(1, 4);
来源：http://hz.hysaishi.cn/gttqlstnbu.html

Go:   arr[1:4]
来源：http://hz.xingfuxueyuan.xyz/gteqbujemx.html

Ruby: arr[1, 3]
来源：http://hz.iojbl.cn/gttpypxliu.html

C#:   list.GetRange(1, 3);
来源：http://hz.ydzc1.top/gtrqmfjazw.html

[D08] 合并两个数组
来源：http://hz.yj202588.top/gteddqgzlx.html

Py:   a + b;  a.extend(b)
来源：http://hz.jinghuilouyu.cn/gtybudeokc.html

PHP:  array_merge($a, $b);
来源：http://hz.jyoumei.cn/gtujllstbs.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.chenjidiqi.icu/gtcpsicxqd.html

TS:   [...a, ...b];
来源：http://hz.iojbl.cn/gtyrtloygl.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.yanxiufei.cn/gtcvvaxzjl.html

Go:   append(a, b...)
来源：http://hz.hnqzz.top/gtmigrotop.html

Ruby: a + b;  a.concat(b)
来源：http://hz.yueranfly.top/gtupkwyehh.html

C#:   a.Concat(b).ToList()
来源：http://hz.chenjidiqi.icu/gtczqxpyft.html

[D09] 排序（升序）
来源：http://hz.shanyushiyangkeji.top/gtpnzajqku.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.birdmap.top/gtfvyxhdpw.html

PHP:  sort($arr);
来源：http://hz.feifeiyinyue.top/gtvdhnezuu.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.mhx1999.top/gtqtezlwae.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.cheryme.top/gtkefpcodi.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.jinyuanbaomall.cn/gthizdshpj.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.hnqzz.top/gtmigubsbn.html

Ruby: arr.sort
来源：http://hz.zhijiandao.cn/gtwknxktzb.html

C#:   list.Sort();
来源：http://hz.snrcjt.cn/gtcgionfhh.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.fzhhl.top/gtabohsnrz.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.jinqigfzy.top/gtxmlgwkaj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.shuidangran.top/gthjlvmlkw.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yvedp.cn/gtyfzkbkvn.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jinyuanbaomall.cn/gtddcyocwf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.jlsjyb.cn/gtenlmmqmg.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.chenzaomai.com/gtcogyaejk.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.xingfuxueyuan.xyz/gtndecolnr.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.jlsjyb.cn/gtlvxyzfmv.html

[D11] 反转数组
来源：http://hz.sxryk.cn/gtaoyipzcs.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.shuidangran.top/gtrjeyxiem.html

PHP:  array_reverse($arr);
来源：http://hz.zycfv.cn/gtxsvnjswc.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.yj20258888.top/gtalseicde.html

TS:   [...arr].reverse();
来源：http://hz.haohaochexian.top/gtbzixiphe.html

Java: Collections.reverse(list);
来源：http://hz.andypj.xyz/gtumtpoxua.html

Go:   slices.Reverse(arr)
来源：http://hz.zhixingplan.top/gtxynwyivy.html

Ruby: arr.reverse
来源：http://hz.c1oappe.top/gtknqfmhwc.html

C#:   list.Reverse();
来源：http://hz.birdmap.top/gtrcnynbkk.html

[D12] 查找元素下标
来源：http://hz.zhongyouzk.top/gtdzynotvo.html

Py:   arr.index(x);  x in arr
来源：http://hz.zhengqikj.top/gtrbvqmikj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.sweek.top/gtyktnrlwt.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zhaomingkeji.xyz/gtarrlyojs.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zhixingplan.top/gteadldlzq.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.meibo888.top/gtdeugqqdb.html

Go:   slices.Index(arr, x)
来源：http://hz.svipenyu.cn/gthlxwncpn.html

Ruby: arr.index(x)
来源：http://hz.9152youxi.cn/gtegtltalh.html

C#:   list.IndexOf(x);
来源：http://hz.yj20258.top/gtutyvcqmb.html

[D13] 过滤（保留满足条件的）
来源：http://hz.yj202588.top/gtmrxqzzuu.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.sufxvd.cn/gtesukwwee.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.wangshuangyany.cn/gtxxcppyfg.html

JS:   arr.filter(x => x > 3)
来源：http://hz.shzxlz.cn/gtvhczupha.html

TS:   arr.filter(x => x > 3)
来源：http://hz.daria6918.cn/gthebjqgri.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.gogol.net.cn/gtsqvrrfen.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.tianlin.xyz/gtznvtqcpo.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.jiagoushi.top/gtwqwzmcdo.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.xylfe.cn/gttzznbzbn.html

[D14] 映射转换（每个元素变形）
来源：http://hz.feifeiyinyue.top/gtdodpwbzc.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.sufxvd.cn/gtuwhdnxuh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.yueranfly.top/gtbioypihp.html

JS:   arr.map(x => x * 2)
来源：http://hz.zhixingplan.top/gtgolkxdvk.html

TS:   arr.map(x => x * 2)
来源：http://hz.yuanzhike.top/gteornancx.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.feifeiyinyue.top/gthykxvyie.html

Go:   // 手写循环
来源：http://hz.chenzaomai.com/gtxgkknpar.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.jianghu66.top/gtccjcytfw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.tianlin.xyz/gtvwvwqjvd.html

[D15] 去重
来源：http://hz.jqgfzy.top/gtgvzktobr.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.jlsjyb.cn/gtkzrxmejo.html

PHP:  array_unique($arr);
来源：http://hz.nanxinkj.top/gtjapmhyba.html

JS:   [...new Set(arr)]
来源：http://hz.zhiwuduotai.top/gtkwxvuobz.html

TS:   [...new Set(arr)]
来源：http://hz.xuetiantiany.cn/gtgwupaclh.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.xinyue.icu/gtasqmtups.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.0kj1m.cn/gtwybpfmjg.html

Ruby: arr.uniq
来源：http://hz.aizwys.cn/gtfwnhjtjh.html

C#:   list.Distinct().ToList()
来源：http://hz.sysykeji.top/gttakabwcw.html

[D16] 求和与平均值
来源：http://hz.zhaomingkeji.xyz/gtkqtguyyn.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.havefunace.top/gtjnidmuny.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.gotoacloud.top/gtdailtooz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.iojbl.cn/gthqzdgvup.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hywenlv.cn/gtwemiogbe.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.316326.xyz/gtnyhynqqw.html

Go:   // 手写循环累加
来源：http://hz.c1oappe.top/gtodnwjfnl.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.jianghu66.top/gtxzsruzze.html

C#:   list.Sum();  list.Average()
来源：http://hz.52xcode.cn/gtlouccvll.html

[D17] 最大值与最小值
来源：http://hz.fzhhl.top/gtipcyabnz.html

Py:   max(arr);  min(arr)
来源：http://hz.jyoumei.cn/gtsnwfizvq.html

PHP:  max($arr);  min($arr);
来源：http://hz.cashguo.top/gtglhbgqlx.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.xingfuxueyuan.xyz/gthrjmwuuh.html

TS:   Math.max(...arr);
来源：http://hz.zhiwuduotai.top/gtsbfymikr.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.tian-w.cn/gtyxirbjus.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.9152youxi.cn/gtqixbyaal.html

Ruby: arr.max;  arr.min
来源：http://hz.hammf.cn/gtpxmpxupi.html

C#:   list.Max();  list.Min()
来源：http://hz.dianchejie.cn/gtijsmzcnr.html

[D18] 扁平化嵌套数组
来源：http://hz.bjfxy.top/gtgmtoyfoz.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.wangdashe.top/gtwlndmhxj.html

PHP:  array_merge(...$nested);
来源：http://hz.cashguo.top/gtsacpjxbi.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.cqqwz.cn/gtpeuxcvdj.html

TS:   nested.flat();
来源：http://hz.nanxinkj.top/gtexxrgmjn.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.wangdashe.top/gtseekfmzu.html

Go:   // 手写双层循环
来源：http://hz.ywan-chungtsiang.top/gtoeyompvn.html

Ruby: nested.flatten
来源：http://hz.sxryk.cn/gtdcsimtpj.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.hfpthk.cn/gtgoizqzqh.html

[D19] 按字段分组
来源：http://hz.feifeiyinyue.top/gtqzknvlzz.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.ivvv.top/gtlzxkzwac.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.aizwys.cn/gthmvyikbk.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.jlsjyb.cn/gtoaaunfur.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.c1oappe.top/gtabvptinh.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.snrcjt.cn/gtjydudftv.html

Go:   // 手写 map[string][]T
来源：http://hz.xuanzx.com/gteydzvqbu.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.zhaomingkeji.xyz/gtnuxjtmjm.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.shangyingyoupin.top/gtjdkdkhuq.html

[D20] 统计每个元素出现次数
来源：http://hz.yanxiufei.cn/gtnofsrvhi.html

Py:   Counter(arr)
来源：http://hz.ybcxt.top/gticbwzgph.html

PHP:  array_count_values($arr);
来源：http://hz.xingfuxueyuan.xyz/gtziohtheb.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.xinyue.icu/gththlgpgp.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.aizwys.cn/gtxocamrrw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.jinghuilouyu.cn/gtwodrnghl.html

Go:   // 手写 map[T]int
来源：http://hz.smart0.xyz/gtwisfjcye.html

Ruby: arr.tally
来源：http://hz.meibo888.top/gtqrjqkpta.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.jinyuanbaomall.cn/gteeugtjho.html

[D21] 判断是否包含某元素
来源：http://hz.hywenlv.cn/gtcirmxhpw.html

Py:   x in arr
来源：http://hz.shanyushiyangtech.top/gtuxwnroxt.html

PHP:  in_array($x, $arr, true);
来源：http://hz.tanke756.top/gtvbvrmvzd.html

JS:   arr.includes(x)
来源：http://hz.ppjwa.cn/gtzlkiluqi.html

TS:   arr.includes(x)
来源：http://hz.nanxinkj.top/gtwkyhpxlj.html

Java: list.contains(x)
来源：http://hz.hnqzz.top/gtntrupcxq.html

Go:   slices.Contains(arr, x)
来源：http://hz.wangdashe.top/gtjcxpptza.html

Ruby: arr.include?(x)
来源：http://hz.sufxvd.cn/gtyuedukxr.html

C#:   list.Contains(x)
来源：http://hz.wangshuangyany.cn/gtdarhorea.html

[D22] 复制数组（避免共享引用）
来源：http://hz.xingfuxueyuan.xyz/gtovxbixft.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.gaohongyu789.top/gtdtocavji.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.jqgfzy.top/gthcbzekti.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.tanke756.top/gtkkpilzis.html

TS:   [...arr];
来源：http://hz.jqgfzy.top/gtuwtswrxj.html

Java: new ArrayList<>(list);
来源：http://hz.xingfuxueyuan.xyz/gtcmtyfsbz.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.yueranfly.top/gtwlfwgvfk.html

Ruby: arr.dup;  arr.clone
来源：http://hz.hongshengwenyu.top/gtgvitotst.html

C#:   new List<int>(list);
来源：http://hz.birdmap.top/gtbgjpheos.html

[D23] reduce 累积计算
来源：http://hz.xylfe.cn/gtpnbaqaop.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.zhiwuduotai.top/gtmprabvqp.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.meibo888.top/gtdzparamz.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.hnqzz.top/gtaumsumbf.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.meibo888.top/gtwagslxzz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.hnxiangtu.top/gtfiezoqkx.html

Go:   // 手写循环
来源：http://hz.xingfuxueyuan.xyz/gtlrcjvepw.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.dianchejie.cn/gtyigmrijh.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.zdqjudy.top/gtwlwfrees.html

[D24] 字典 / Map 基本操作
来源：http://hz.xylfe.cn/gtqdjyeeyi.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.feifeiyinyue.top/gtsinxzwrd.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.tian-w.cn/gtvnoxpman.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.jinqigfzy.top/gtxsbxbeki.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.cdnleiting.top/gtrsqtntpy.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.tianlin.xyz/gtsmyrttsi.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.yj20258888.top/gtotvmzthm.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.pengpengdd.cyou/gtoynbjkvn.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.jinqigfzy.top/gtfupvifeq.html

[D25] Set 集合去重与交并差
来源：http://hz.pycfn.com/gtefmtgsjm.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.sxryk.cn/gtxrullytc.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.aizwys.cn/gtnxqyeiyl.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.jiagoushi.top/gtpdawksls.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.sysykeji.top/gtuoilmniu.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.pengpengdd.cyou/gtihummsrd.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.ydjk.org.cn/gtfpipxtci.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.meibo888.top/gthhqpajqk.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.cqqwz.cn/gteffozsob.html

[D26] 数组转字符串
来源：http://hz.gotoacloud.top/gtkctgrxej.html

Py:   ", ".join(map(str, arr))
来源：http://hz.pengpengdd.cyou/gtqzptnlim.html

PHP:  implode(", ", $arr);
来源：http://hz.shzxlz.cn/gtwcpirnal.html

JS:   arr.join(", ")
来源：http://hz.yongpay.top/gtkqvlktgr.html

TS:   arr.join(", ")
来源：http://hz.gogol.net.cn/gthdfomxqy.html

Java: String.join(", ", list)
来源：http://hz.cqqwz.cn/gtjztgunou.html

Go:   strings.Join(strs, ", ")
来源：http://hz.yuanzhike.top/gtcrmuassh.html

Ruby: arr.join(", ")
来源：http://hz.daxiang520.top/gtbhbqjkqj.html

C#:   string.Join(", ", list)
来源：http://hz.chenlongwang.top/gttllbzmjr.html

================================================================================
来源：http://hz.nwbrower.top/gtrriplprp.html

E. 字符串处理
来源：http://hz.ydzc1.top/gtmqbcvjrp.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtwzeonjty.html

[E01] 拼接字符串
来源：http://hz.yuxming.cn/gtdngzudwx.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.tian-w.cn/gtibknmyil.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.ivvv.top/gtdnhsorxx.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.tianlin.xyz/gtfdnxvson.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.daria6918.cn/gtisdcizfe.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.chenzaomai.com/gtwvtprmib.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.zhaomingkeji.xyz/gtkezmhona.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.daxiang520.top/gtxyjbrcbg.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.aibaodan.cn/gtdyabndxa.html

[E02] 重复字符串
来源：http://hz.yuxming.cn/gtkougtvim.html

Py:   "ab" * 3
来源：http://hz.hammf.cn/gtvmuezllw.html

PHP:  str_repeat("ab", 3);
来源：http://hz.xziqi.cn/gtgbxvhpbv.html

JS:   "ab".repeat(3)
来源：http://hz.tianlin.xyz/gtabuwefjv.html

TS:   "ab".repeat(3)
来源：http://hz.aizwys.cn/gtdqyolizk.html

Java: "ab".repeat(3)
来源：http://hz.jlsjyb.cn/gthwijqirb.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.shanyushiyangtech.top/gtnkuilwjs.html

Ruby: "ab" * 3
来源：http://hz.pengpengdd.cyou/gtaytlyacf.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.ydzc1.top/gtigpsuuxk.html

[E03] 截取子串
来源：http://hz.gotoacloud.top/gtbunxdudd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.dashuyun.cn/gteizymsya.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.tianlin.xyz/gtvfmqibmp.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.yvedp.cn/gtkhkpykkq.html

TS:   s.slice(1, 4)
来源：http://hz.meibo888.top/gtcnrxnesv.html

Java: s.substring(1, 4)
来源：http://hz.xingfuxueyuan.xyz/gtagglvbsv.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.sweek.top/gtotqqskfm.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.gogol.net.cn/gtpfwzrzpu.html

C#:   s.Substring(1, 3)
来源：http://hz.chenjidiqi.icu/gtmcbtaviv.html

[E04] 查找子串位置
来源：http://hz.svipenyu.cn/gthvignnbo.html

Py:   s.find("x");  s.index("x")
来源：http://hz.pycfn.com/gtnhmtzoym.html

PHP:  strpos($s, "x");
来源：http://hz.chenzaomai.com/gtajtwmyaq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.tanke756.top/gtnfuqomkw.html

TS:   s.indexOf("x")
来源：http://hz.jqgufenzy.top/gtaezertnq.html

Java: s.indexOf("x")
来源：http://hz.dashuyun.cn/gtguhzumen.html

Go:   strings.Index(s, "x")
来源：http://hz.xinyue.icu/gtvfdvigwr.html

Ruby: s.index("x")
来源：http://hz.redwolf501.top/gtxjogubuj.html

C#:   s.IndexOf("x")
来源：http://hz.xuanzx.com/gtdcwnulcs.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.snrcjt.cn/gtbqpnncbm.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.jlsjyb.cn/gtgvktggbc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.yvedp.cn/gtfvaoqbdu.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yuanzhike.top/gtzdlabqsj.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.ydjk.org.cn/gtkskdkigk.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.bjfxy.top/gtorbulxhn.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.daxiang520.top/gtcmewrlhq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.dianchejie.cn/gtysufrysd.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.316326.xyz/gtxiuicbkp.html

[E06] 替换子串
来源：http://hz.zycfv.cn/gtwmbszygn.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.aizwys.cn/gtnzljymcl.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.nanxinkj.top/gtigwbraik.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jinghuilouyu.cn/gtsgofdrls.html

TS:   s.replaceAll("a", "b")
来源：http://hz.wangdashe.top/gtnjxszeuh.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.ehwqpu.com/gtxmuhjkka.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.smart0.xyz/gtemsvmfel.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.zycfv.cn/gtdgokiuyw.html

C#:   s.Replace("a", "b")
来源：http://hz.aibaodan.cn/gtngtcnhkq.html

[E07] 按分隔符拆分
来源：http://hz.nwbrower.top/gthxctovoa.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.jlsjyb.cn/gtteneabxy.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.snrcjt.cn/gtgxcutajf.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.9152youxi.cn/gtgodarhrm.html

TS:   s.split(",")
来源：http://hz.aibaodan.cn/gtxsfaqpnk.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.yj202588.top/gthpqutzgr.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.316326.xyz/gtolecierf.html

Ruby: s.split(",");  s.split
来源：http://hz.fengsongda.top/gtfyymtvfy.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.sxryk.cn/gtwdoemgar.html

[E08] 数组按分隔符合并
来源：http://hz.haohaochexian.top/gtyitshkmr.html

Py:   ",".join(items)
来源：http://hz.nanxinkj.top/gtxvxtskft.html

PHP:  implode(",", $items);
来源：http://hz.sysykeji.top/gteafzklug.html

JS:   items.join(",")
来源：http://hz.daria6918.cn/gthgluuove.html

TS:   items.join(",")
来源：http://hz.ehwqpu.com/gtouwnkpnj.html

Java: String.join(",", items)
来源：http://hz.tian-w.cn/gtnjqjhvmb.html

Go:   strings.Join(items, ",")
来源：http://hz.birdmap.top/gtowkukfyc.html

Ruby: items.join(",")
来源：http://hz.sufxvd.cn/gttefhaosq.html

C#:   string.Join(",", items)
来源：http://hz.chenlongwang.top/gtdbcphvde.html

[E09] 去除所有空白字符
来源：http://hz.snrcjt.cn/gthxaquhuz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.ywan-chungtsiang.top/gtmzfstgcb.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.fengsongda.top/gthabepjkp.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.yueranfly.top/gtnkjbekjw.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.vqdsnc.cn/gtwyofsgio.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.pycfn.com/gtakvfwozi.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.sufxvd.cn/gtdvhiuidt.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.zhongyouzk.top/gtijotjcdj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.ydjk.org.cn/gttcrrtezn.html

[E10] 左侧补零 / 定长填充
来源：http://hz.redwolf501.top/gtxrzegumz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.0kj1m.cn/gtnnperblt.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.jinqigufen.top/gtlzsmwphp.html

JS:   "7".padStart(3, "0")
来源：http://hz.andypj.xyz/gtmelrsumn.html

TS:   "7".padStart(3, "0")
来源：http://hz.yongpay.top/gtpqavbpkn.html

Java: String.format("%03d", 7)
来源：http://hz.chenjidiqi.icu/gtxvtweilw.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.jqgfzy.top/gtyhkbisvp.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.zhaomingkeji.xyz/gttjlsjhty.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.wangdashe.top/gtyrariwqs.html

[E11] 反转字符串
来源：http://hz.jqgfzy.top/gtcvztesub.html

Py:   s[::-1]
来源：http://hz.yuanzhike.top/gtltgrncze.html

PHP:  strrev($s);
来源：http://hz.xuetiantiany.cn/gtgldzkfwt.html

JS:   [...s].reverse().join("")
来源：http://hz.zhixingplan.top/gtphaackzd.html

TS:   [...s].reverse().join("")
来源：http://hz.sweek.top/gtuipumxwy.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.xuetiantiany.cn/gttaahoykq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.nwbrower.top/gtbptlniyn.html

Ruby: s.reverse
来源：http://hz.iojbl.cn/gtpdjokogs.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.iojbl.cn/gtoeznaanp.html

[E12] 统计某字符出现次数
来源：http://hz.jinghuilouyu.cn/gtehynbkqs.html

Py:   s.count("a")
来源：http://hz.chenjidiqi.icu/gtmzswazkk.html

PHP:  substr_count($s, "a");
来源：http://hz.xylfe.cn/gtiryxjqan.html

JS:   s.split("a").length - 1
来源：http://hz.52xcode.cn/gtvvrupsmo.html

TS:   s.split("a").length - 1
来源：http://hz.hammf.cn/gtfvrmrorj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.ybcxt.top/gtnhlzigvc.html

Go:   strings.Count(s, "a")
来源：http://hz.pengpengdd.cyou/gthbhzencm.html

Ruby: s.count("a")
来源：http://hz.daxiang520.top/gtzgdxtbdm.html

C#:   s.Count(c => c == 'a')
来源：http://hz.dianchejie.cn/gtsqwpvqro.html

[E13] 逐字符遍历
来源：http://hz.316326.xyz/gtjfuewjzd.html

Py:   for ch in s: print(ch)
来源：http://hz.andypj.xyz/gtdlytbkka.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.cheryme.top/gtmtjsooud.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.52xcode.cn/gtajdnrkai.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jinqigufen.top/gtoicuqnmw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.shanyushiyangtech.top/gtrrucsaoe.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.daria6918.cn/gtftxafopq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.sxryk.cn/gtmgntwkjs.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.sufxvd.cn/gtpmwdutep.html


<!-- 参考信息 -->