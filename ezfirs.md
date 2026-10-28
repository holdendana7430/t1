代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://hz.dianchejie.cn/gtxvywpefs.html

C#:   a.Concat(b).ToList()
来源：http://hz.9152youxi.cn/gtarwlyvmn.html

[D09] 排序（升序）
来源：http://hz.havefunace.top/gtikiscpga.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.dianchejie.cn/gtpodaeyhc.html

PHP:  sort($arr);
来源：http://hz.zdqjudy.top/gtaiskgfrg.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.yj20258.top/gteehlnniq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.hnqzz.top/gtercfrthv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.nanxinkj.top/gtslwrdttq.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.feifeiyinyue.top/gtqmeobiay.html

Ruby: arr.sort
来源：http://hz.zhoulong.xyz/gtlbvjqclf.html

C#:   list.Sort();
来源：http://hz.yonumen.top/gtptgtqvup.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.quarkkingdee.top/gtejqkhcgx.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.yueranfly.top/gtlxpdiohj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.hammf.cn/gtclyeokbr.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.iojbl.cn/gtpqewivvu.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hnqzz.top/gtgwuuwsor.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.chenjidiqi.icu/gtyemfidyn.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.ivvv.top/gtwwdyhnei.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.chenjidiqi.icu/gtdrvlruge.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.shangyingyoupin.top/gtvgtspaxz.html

[D11] 反转数组
来源：http://hz.snrcjt.cn/gtltucfksn.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.chenjidiqi.icu/gtgpyibmpy.html

PHP:  array_reverse($arr);
来源：http://hz.dashuyun.cn/gtyiyzwxpn.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.yuanzhike.top/gtpmbemkkv.html

TS:   [...arr].reverse();
来源：http://hz.ybcxt.top/gtedefbadj.html

Java: Collections.reverse(list);
来源：http://hz.yangfankeji.com/gthlstpciw.html

Go:   slices.Reverse(arr)
来源：http://hz.tanke756.top/gtiybbfnkg.html

Ruby: arr.reverse
来源：http://hz.cucudq.cn/gtugethpgt.html

C#:   list.Reverse();
来源：http://hz.wangdashe.top/gtmlfhcsob.html

[D12] 查找元素下标
来源：http://hz.gaohongyu789.top/gtacznexpa.html

Py:   arr.index(x);  x in arr
来源：http://hz.gzhubu.top/gtlnnwpvwe.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.shuidangran.top/gtbszztcxc.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.aibaodan.cn/gtjzhzeizs.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.iojbl.cn/gtiboujsha.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.sysykeji.top/gtvvexujax.html

Go:   slices.Index(arr, x)
来源：http://hz.jqgufenzy.top/gtxmnwrrpi.html

Ruby: arr.index(x)
来源：http://hz.feifeiyinyue.top/gtgawiekzm.html

C#:   list.IndexOf(x);
来源：http://hz.yuanzhike.top/gthgwplgko.html

[D13] 过滤（保留满足条件的）
来源：http://hz.zdqjudy.top/gtbdadrbfr.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.kuanghao11.cn/gtgglcorah.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.kuanghao11.cn/gtdxormibi.html

JS:   arr.filter(x => x > 3)
来源：http://hz.yueranfly.top/gtzshmnmwx.html

TS:   arr.filter(x => x > 3)
来源：http://hz.shangyingyoupin.top/gttnrtcaeo.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.snrcjt.cn/gthilftxxa.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.zhixingplan.top/gtavvljacd.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.jiagoushi.top/gtgkpoacok.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.daria6918.cn/gtwytqexjt.html

[D14] 映射转换（每个元素变形）
来源：http://hz.chenlongwang.top/gtxsdokprx.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.jqgufenzy.top/gthzujtgde.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.jqgufenzy.top/gtxxqwntoe.html

JS:   arr.map(x => x * 2)
来源：http://hz.316326.xyz/gtvwherjqu.html

TS:   arr.map(x => x * 2)
来源：http://hz.yj202588.top/gtphsiyupd.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.svipenyu.cn/gtlgkanoqc.html

Go:   // 手写循环
来源：http://hz.52xcode.cn/gtaevgdgtx.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.tian-w.cn/gtaeeqapmq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.havefunace.top/gtppxowmiv.html

[D15] 去重
来源：http://hz.dianchejie.cn/gtcoeaxdos.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.yanxiufei.cn/gtzskfsime.html

PHP:  array_unique($arr);
来源：http://hz.redwolf501.top/gttxwfzpdt.html

JS:   [...new Set(arr)]
来源：http://hz.shanyushiyangtech.top/gttzpvzzay.html

TS:   [...new Set(arr)]
来源：http://hz.jinqigufen.top/gtvwkjmann.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.zycfv.cn/gtlkiaujka.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.c1oappe.top/gtdbmqcztn.html

Ruby: arr.uniq
来源：http://hz.sweek.top/gtbxabebjx.html

C#:   list.Distinct().ToList()
来源：http://hz.yuanzhike.top/gtbxwepchv.html

[D16] 求和与平均值
来源：http://hz.ybcxt.top/gttywqmtbx.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.yj20258888.top/gtaghlcnxz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.redwolf501.top/gtceidgwxm.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.aibaodan.cn/gtzqdxoqzw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yanxiufei.cn/gtodhcswch.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.jqgfzy.top/gtyhyvvovu.html

Go:   // 手写循环累加
来源：http://hz.gaohongyu789.top/gtbmwtggte.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.cqqwz.cn/gtwkmhvawv.html

C#:   list.Sum();  list.Average()
来源：http://hz.cqqwz.cn/gttflduchm.html

[D17] 最大值与最小值
来源：http://hz.0kj1m.cn/gttyghtwnv.html

Py:   max(arr);  min(arr)
来源：http://hz.ydjk.org.cn/gtqlvdfjtc.html

PHP:  max($arr);  min($arr);
来源：http://hz.cdnleiting.top/gttkcixtsr.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.zhoulong.xyz/gtbnpeoetm.html

TS:   Math.max(...arr);
来源：http://hz.sxryk.cn/gttadvbxwg.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.redwolf501.top/gtpoplruxf.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.tian-w.cn/gtqbqtyqbi.html

Ruby: arr.max;  arr.min
来源：http://hz.chenzaomai.com/gtppddqpiz.html

C#:   list.Max();  list.Min()
来源：http://hz.andypj.xyz/gtucymmume.html

[D18] 扁平化嵌套数组
来源：http://hz.xuanzx.com/gtxzdswpzq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.ppjwa.cn/gtebuyiytu.html

PHP:  array_merge(...$nested);
来源：http://hz.yj202588.top/gtrhfrslgp.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.zhixingplan.top/gtzrdnmjwp.html

TS:   nested.flat();
来源：http://hz.zhongyouzk.top/gtyfvucarl.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.iojbl.cn/gtesbergnc.html

Go:   // 手写双层循环
来源：http://hz.zdqjudy.top/gtcjyaaolf.html

Ruby: nested.flatten
来源：http://hz.birdmap.top/gtjuypydhv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.nanxinkj.top/gtphdctblh.html

[D19] 按字段分组
来源：http://hz.yuxming.cn/gtbjopeyem.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.jinyuanbaomall.cn/gtxttqbfgt.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.chenzaomai.com/gtrbwwzekh.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.dashuyun.cn/gtcsplximn.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.cashguo.top/gtxmgsxnxh.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.jinqigfzy.top/gtrvgbpbrj.html

Go:   // 手写 map[string][]T
来源：http://hz.guowangkeji.top/gtxdtbrhtu.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.tanke756.top/gtbwmdazri.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.jinyuanbaomall.cn/gtptoxqytl.html

[D20] 统计每个元素出现次数
来源：http://hz.cucudq.cn/gtkjoqfibi.html

Py:   Counter(arr)
来源：http://hz.zycfv.cn/gtfluedfpy.html

PHP:  array_count_values($arr);
来源：http://hz.yangfankeji.com/gtgcnjiaak.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yangfankeji.com/gtdfzlaabw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yongpay.top/gtmdqqwygu.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.jyoumei.cn/gtavihwysu.html

Go:   // 手写 map[T]int
来源：http://hz.daxiang520.top/gtccxmqmjl.html

Ruby: arr.tally
来源：http://hz.xuetiantiany.cn/gttpjgphdh.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.cdnleiting.top/gtjlqsatxp.html

[D21] 判断是否包含某元素
来源：http://hz.shanyushiyangkeji.top/gtedgqzqkn.html

Py:   x in arr
来源：http://hz.havefunace.top/gtzoknniqa.html

PHP:  in_array($x, $arr, true);
来源：http://hz.xuetiantiany.cn/gtznfjfkyq.html

JS:   arr.includes(x)
来源：http://hz.ppjwa.cn/gtfkjzivvg.html

TS:   arr.includes(x)
来源：http://hz.dashuyun.cn/gtbuazbqbu.html

Java: list.contains(x)
来源：http://hz.vqdsnc.cn/gtpxgebhkf.html

Go:   slices.Contains(arr, x)
来源：http://hz.yvedp.cn/gtxvigapid.html

Ruby: arr.include?(x)
来源：http://hz.xuetiantiany.cn/gtjtcwtgmq.html

C#:   list.Contains(x)
来源：http://hz.ydzc1.top/gtrrfldsxp.html

[D22] 复制数组（避免共享引用）
来源：http://hz.jinyuanbaomall.cn/gtmovsahao.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.tianlin.xyz/gtrjbjulox.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.xinyue.icu/gtdcandukr.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.haohaochexian.top/gtuwsnqsyc.html

TS:   [...arr];
来源：http://hz.ppjwa.cn/gtmlgolouc.html

Java: new ArrayList<>(list);
来源：http://hz.bjfxy.top/gtrujxndnx.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.ywan-chungtsiang.top/gttuclmpvi.html

Ruby: arr.dup;  arr.clone
来源：http://hz.wangdashe.top/gtuhmoqigj.html

C#:   new List<int>(list);
来源：http://hz.chenzaomai.com/gtlzqpysjl.html

[D23] reduce 累积计算
来源：http://hz.yvedp.cn/gtlotixvtw.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.cqqwz.cn/gtcumdxwjt.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.sysykeji.top/gtubjonztw.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yuxming.cn/gtmupytewc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.hongshengwenyu.top/gttniwtznz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.tanke756.top/gtxqhlnvmq.html

Go:   // 手写循环
来源：http://hz.chenlongwang.top/gtbztppkwd.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.svipenyu.cn/gtzeglpnch.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.hywenlv.cn/gtxdlvyrcc.html

[D24] 字典 / Map 基本操作
来源：http://hz.hywenlv.cn/gtcijqeqnc.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.shangyingyoupin.top/gtxlzlbtdh.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.yongpay.top/gtlnssaxfk.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.jyoumei.cn/gtknmhfxra.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.fengsongda.top/gtoedyposl.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.ppjwa.cn/gtvscpovdh.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.smart0.xyz/gtbwumnutu.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.tian-w.cn/gtgodrdoyk.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.zycfv.cn/gtsqezfozz.html

[D25] Set 集合去重与交并差
来源：http://hz.yj20258888.top/gtdqtxenyg.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.pycfn.com/gtptdrzqkp.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.bjfxy.top/gthomwpivs.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.redwolf501.top/gtgzocagfw.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.yj202588.top/gttmpisxoc.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.havefunace.top/gtxtamgadi.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.nwbrower.top/gtjgwgkjfv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.hysaishi.cn/gtkethvolp.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.nanxuanxn.top/gtrylqhetj.html

[D26] 数组转字符串
来源：http://hz.zhongyouzk.top/gtsuzailof.html

Py:   ", ".join(map(str, arr))
来源：http://hz.nanxuanxn.top/gtngiblggp.html

PHP:  implode(", ", $arr);
来源：http://hz.yanxiufei.cn/gtinfilupw.html

JS:   arr.join(", ")
来源：http://hz.52xcode.cn/gtqkhipxkw.html

TS:   arr.join(", ")
来源：http://hz.sysykeji.top/gtrvzgrcie.html

Java: String.join(", ", list)
来源：http://hz.ehwqpu.com/gtwrghbecv.html

Go:   strings.Join(strs, ", ")
来源：http://hz.aizwys.cn/gtpfugnxgz.html

Ruby: arr.join(", ")
来源：http://hz.cheryme.top/gtukfhtooo.html

C#:   string.Join(", ", list)
来源：http://hz.hysaishi.cn/gthsonnxkw.html

================================================================================
来源：http://hz.svipenyu.cn/gtsdlaafpt.html

E. 字符串处理
来源：http://hz.cheryme.top/gtvvwgyxqe.html

================================================================================
来源：http://hz.iojbl.cn/gtprxtdbgo.html

[E01] 拼接字符串
来源：http://hz.9152youxi.cn/gthmkcesdo.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.daria6918.cn/gtejcibjfk.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.wangdashe.top/gtfsvghjzn.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ywan-chungtsiang.top/gtvweqwmkp.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.snrcjt.cn/gtoefzlrpc.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.nanxinkj.top/gtqagkjetn.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.nanxuanxn.top/gttaxchwlc.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.ywan-chungtsiang.top/gtnunyeuta.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.sysykeji.top/gtlkadpugp.html

[E02] 重复字符串
来源：http://hz.zycfv.cn/gttnicdsrp.html

Py:   "ab" * 3
来源：http://hz.nanxinkj.top/gtxcogrjud.html

PHP:  str_repeat("ab", 3);
来源：http://hz.fzhhl.top/gtksegkmtg.html

JS:   "ab".repeat(3)
来源：http://hz.vqdsnc.cn/gtwvetwzyd.html

TS:   "ab".repeat(3)
来源：http://hz.bjfxy.top/gtbtrqjipf.html

Java: "ab".repeat(3)
来源：http://hz.feifeiyinyue.top/gtjsapdleh.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.tanke756.top/gtsknwnbst.html

Ruby: "ab" * 3
来源：http://hz.xuetiantiany.cn/gtdtxwrqpy.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.zycfv.cn/gtiictmehf.html

[E03] 截取子串
来源：http://hz.yj202588.top/gtyqdehxon.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.daria6918.cn/gthujrbxio.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.hnxiangtu.top/gtwsuuwyup.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.yj20258888.top/gtauxcnjsg.html

TS:   s.slice(1, 4)
来源：http://hz.zhixingplan.top/gtczjxvfkw.html

Java: s.substring(1, 4)
来源：http://hz.hywenlv.cn/gtpehrlicc.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.ivvv.top/gtsqzfbucg.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.jinqigufen.top/gtffxqqgms.html

C#:   s.Substring(1, 3)
来源：http://hz.snrcjt.cn/gtgynvnvlr.html

[E04] 查找子串位置
来源：http://hz.daria6918.cn/gttmcnytel.html

Py:   s.find("x");  s.index("x")
来源：http://hz.ywan-chungtsiang.top/gtkgujqorb.html

PHP:  strpos($s, "x");
来源：http://hz.hywenlv.cn/gtymoyipic.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.sweek.top/gtuadisxhu.html

TS:   s.indexOf("x")
来源：http://hz.daria6918.cn/gtuqafcpoa.html

Java: s.indexOf("x")
来源：http://hz.quarkkingdee.top/gtedhhnscm.html

Go:   strings.Index(s, "x")
来源：http://hz.tianlin.xyz/gteygscxbm.html

Ruby: s.index("x")
来源：http://hz.ybcxt.top/gttyysuycn.html

C#:   s.IndexOf("x")
来源：http://hz.gaohongyu789.top/gtgyznupfk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.tianlin.xyz/gtejsempxk.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.yuanzhike.top/gtlistosec.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.yanxiufei.cn/gtwccvpiyq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.smart0.xyz/gtpkfxdexn.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.mhx1999.top/gtxmevulwa.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.tian-w.cn/gtmcutzdrj.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.tianlin.xyz/gtnjcotied.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.zhoulong.xyz/gtasgebdyd.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.gogol.net.cn/gtuqasfded.html

[E06] 替换子串
来源：http://hz.yonumen.top/gtzqaxipiu.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.yonumen.top/gtqfonkvcv.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.yuanzhike.top/gtjqrdjdhs.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jinghuilouyu.cn/gtllieqhpx.html

TS:   s.replaceAll("a", "b")
来源：http://hz.sweek.top/gtwxjhzrgg.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhixingplan.top/gtmcowthst.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.ehwqpu.com/gtbbsrterf.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.gzhubu.top/gtuxrotnji.html

C#:   s.Replace("a", "b")
来源：http://hz.iojbl.cn/gtzndzjujk.html

[E07] 按分隔符拆分
来源：http://hz.yj20258888.top/gttfricrcn.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.sufxvd.cn/gtfasvqdge.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.ehwqpu.com/gtppmysujs.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.havefunace.top/gtsfgtbvlh.html

TS:   s.split(",")
来源：http://hz.hammf.cn/gtzcjjfoms.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.pycfn.com/gtaygvzugy.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.iojbl.cn/gtdrosgpzx.html

Ruby: s.split(",");  s.split
来源：http://hz.zdqjudy.top/gtbbvbsvxj.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.ybcxt.top/gtubnflsfn.html

[E08] 数组按分隔符合并
来源：http://hz.gzhubu.top/gtabikptph.html

Py:   ",".join(items)
来源：http://hz.gzhubu.top/gtcgcdlxle.html

PHP:  implode(",", $items);
来源：http://hz.sysykeji.top/gtczbngmai.html

JS:   items.join(",")
来源：http://hz.yangfankeji.com/gtyyeiezuf.html

TS:   items.join(",")
来源：http://hz.jinqigufen.top/gtitchtifp.html

Java: String.join(",", items)
来源：http://hz.iojbl.cn/gtnwdrytcg.html

Go:   strings.Join(items, ",")
来源：http://hz.birdmap.top/gtkfqgazgj.html

Ruby: items.join(",")
来源：http://hz.nanxinkj.top/gtfoqyntqa.html

C#:   string.Join(",", items)
来源：http://hz.chenlongwang.top/gtueakgcif.html

[E09] 去除所有空白字符
来源：http://hz.pengpengdd.cyou/gtmztzpnxh.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.xinyue.icu/gtaygfaala.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.9152youxi.cn/gtwnzsgntg.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.andypj.xyz/gtwfcfttgw.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.zhongyouzk.top/gtpahhplvz.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.tian-w.cn/gtujdbsttz.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.hysaishi.cn/gtokjptdnf.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.iojbl.cn/gtkzulachu.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.jinghuilouyu.cn/gtientfuxh.html

[E10] 左侧补零 / 定长填充
来源：http://hz.jiagoushi.top/gtgvrnhkfs.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.snrcjt.cn/gtoeasdlsa.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.yongpay.top/gtryloaxwp.html

JS:   "7".padStart(3, "0")
来源：http://hz.zhoulong.xyz/gticcydeya.html

TS:   "7".padStart(3, "0")
来源：http://hz.fzhhl.top/gtarkcjhnk.html

Java: String.format("%03d", 7)
来源：http://hz.hammf.cn/gtbcwtivco.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.jinyuanbaomall.cn/gtanfeqzrp.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.yangfankeji.com/gtqgvvjels.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.316326.xyz/gtkvwcitnh.html

[E11] 反转字符串
来源：http://hz.zhiwuduotai.top/gtmajxufjr.html

Py:   s[::-1]
来源：http://hz.aizwys.cn/gtsengzdjk.html

PHP:  strrev($s);
来源：http://hz.gaohongyu789.top/gtvycisqvj.html

JS:   [...s].reverse().join("")
来源：http://hz.cucudq.cn/gtfcwzcldf.html

TS:   [...s].reverse().join("")
来源：http://hz.cqqwz.cn/gtehsgltpw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.yuxming.cn/gtjxwtambq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.pycfn.com/gtospubrst.html

Ruby: s.reverse
来源：http://hz.cheryme.top/gtwgjtpvvs.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.ppjwa.cn/gtttycctnn.html

[E12] 统计某字符出现次数
来源：http://hz.iojbl.cn/gtugdwkdyt.html

Py:   s.count("a")
来源：http://hz.redwolf501.top/gtuxgcfhjo.html

PHP:  substr_count($s, "a");
来源：http://hz.meibo888.top/gtmbjiczbn.html

JS:   s.split("a").length - 1
来源：http://hz.jianghu66.top/gtxkekmsxr.html

TS:   s.split("a").length - 1
来源：http://hz.tanke756.top/gtzfweuzsp.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.shzxlz.cn/gtyuxbhemn.html

Go:   strings.Count(s, "a")
来源：http://hz.gzhubu.top/gttvvgrjlr.html

Ruby: s.count("a")
来源：http://hz.shangyingyoupin.top/gtdhxdvjvv.html

C#:   s.Count(c => c == 'a')
来源：http://hz.ydzc1.top/gtjekcalvo.html

[E13] 逐字符遍历
来源：http://hz.yongpay.top/gtqbbtcxab.html

Py:   for ch in s: print(ch)
来源：http://hz.guannengcc.top/gtanacvzgn.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.jinyuanbaomall.cn/gtnhuwfibb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yj20258888.top/gtgsknomkm.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.fengsongda.top/gthaezrqur.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.zhaomingkeji.xyz/gtbhkbgvfk.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.hammf.cn/gtzqovgcyr.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.52xcode.cn/gthmwwkbll.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.andypj.xyz/gtegwljwjh.html

[E14] URL 编码与 Base64
来源：http://hz.zhaomingkeji.xyz/gtnpfchnzy.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.nanxinkj.top/gtcmflnmnb.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.nanxuanxn.top/gtdroamksb.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.mhx1999.top/gtumqmldtx.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.dashuyun.cn/gtkoidydtu.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.fengsongda.top/gtrypiygxh.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.yueranfly.top/gtuyempbdo.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.ywan-chungtsiang.top/gtqcgnanlv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.havefunace.top/gtsltcacfw.html

[E15] HTML 转义 / 反转义
来源：http://hz.cashguo.top/gtghofbgqn.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.jqgfzy.top/gtxvhxjdoy.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.shanyushiyangkeji.top/gteoncjmjy.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.mhx1999.top/gtthkmlwhg.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.xziqi.cn/gtguzkfbnn.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.kuanghao11.cn/gtrtbesodg.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.pycfn.com/gtdjajaqkb.html


<!-- 参考信息 -->