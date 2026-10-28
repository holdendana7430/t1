代发 wailian999

Py:   len(arr)
来源：http://hz.hnqzz.top/gtglkjpahn.html

PHP:  count($arr);
来源：http://hz.hongshengwenyu.top/gtgqhpyfop.html

JS:   arr.length
来源：http://hz.zhengqikj.top/gtgaqeauly.html

TS:   arr.length
来源：http://hz.xingfuxueyuan.xyz/gtohufrrdb.html

Java: list.size();
来源：http://hz.0kj1m.cn/gtqdspsdnd.html

Go:   len(arr)
来源：http://hz.sweek.top/gtcwxiwcwc.html

Ruby: arr.length; arr.size
来源：http://hz.havefunace.top/gtebviwtzr.html

C#:   list.Count;
来源：http://hz.zdqjudy.top/gtqrcgdteb.html

[D07] 切片 / 取子数组
来源：http://hz.daxiang520.top/gttgxbnett.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.ivvv.top/gtclyorasu.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.yuxming.cn/gtpwvsppeu.html

JS:   arr.slice(1, 4);
来源：http://hz.zdqjudy.top/gtkbrrmcrp.html

TS:   arr.slice(1, 4);
来源：http://hz.shanyushiyangkeji.top/gthttcovxr.html

Java: list.subList(1, 4);
来源：http://hz.316326.xyz/gtkcdsasuu.html

Go:   arr[1:4]
来源：http://hz.zhijiandao.cn/gtgrxaiqsz.html

Ruby: arr[1, 3]
来源：http://hz.meibo888.top/gtigrshtzt.html

C#:   list.GetRange(1, 3);
来源：http://hz.chenjidiqi.icu/gtvmtjbkgt.html

[D08] 合并两个数组
来源：http://hz.gaohongyu789.top/gtgvfhuybx.html

Py:   a + b;  a.extend(b)
来源：http://hz.jlsjyb.cn/gtzdsdlzzl.html

PHP:  array_merge($a, $b);
来源：http://hz.ydzc1.top/gtwrammsql.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.gogol.net.cn/gtrakxsijw.html

TS:   [...a, ...b];
来源：http://hz.tian-w.cn/gtexnkgvjb.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.jlsjyb.cn/gtxnrvhaay.html

Go:   append(a, b...)
来源：http://hz.nwbrower.top/gtcxbgohqi.html

Ruby: a + b;  a.concat(b)
来源：http://hz.haohaochexian.top/gthiwvtmvv.html

C#:   a.Concat(b).ToList()
来源：http://hz.zhoulong.xyz/gtqjdnrpev.html

[D09] 排序（升序）
来源：http://hz.ybcxt.top/gtbmnjwthn.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.gzhubu.top/gtjhwsacdh.html

PHP:  sort($arr);
来源：http://hz.9152youxi.cn/gtpgglruno.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.aizwys.cn/gtovfnguse.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.yanxiufei.cn/gtnsiccxag.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.wangshuangyany.cn/gtwfhwozsi.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.pycfn.com/gtsthsxfyq.html

Ruby: arr.sort
来源：http://hz.wangshuangyany.cn/gtgdqzryxa.html

C#:   list.Sort();
来源：http://hz.ydjk.org.cn/gtyjfzialg.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.xuanzx.com/gtnoncayjl.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.ydzc1.top/gtgbxfatzf.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.hnxiangtu.top/gtfsmucgca.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hongshengwenyu.top/gtdmrtjsdv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.nanxinkj.top/gtqmdhaglp.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.cucudq.cn/gtkhisplkj.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.smart0.xyz/gthcozeesp.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.yueranfly.top/gtalqnwuzd.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.zhixingplan.top/gtdrgqihot.html

[D11] 反转数组
来源：http://hz.cdnleiting.top/gthzcdoepc.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.jlsjyb.cn/gtwaulmhsw.html

PHP:  array_reverse($arr);
来源：http://hz.vqdsnc.cn/gtswlhmayj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.xinyue.icu/gtjzvvredm.html

TS:   [...arr].reverse();
来源：http://hz.52xcode.cn/gtkkprxtfx.html

Java: Collections.reverse(list);
来源：http://hz.jqgfzy.top/gtlgbiyiut.html

Go:   slices.Reverse(arr)
来源：http://hz.jqgfzy.top/gtbmmctsea.html

Ruby: arr.reverse
来源：http://hz.wangshuangyany.cn/gtroazbguu.html

C#:   list.Reverse();
来源：http://hz.shzxlz.cn/gtkzqwuegm.html

[D12] 查找元素下标
来源：http://hz.hnqzz.top/gtwhdhwhfr.html

Py:   arr.index(x);  x in arr
来源：http://hz.shanyushiyangkeji.top/gtvpydyfmb.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.yongpay.top/gtzngyajgo.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zhaomingkeji.xyz/gtelshgwza.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.redwolf501.top/gtxwoqfpfu.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.nanxuanxn.top/gtrjtvvzpk.html

Go:   slices.Index(arr, x)
来源：http://hz.sweek.top/gtcswhmdsz.html

Ruby: arr.index(x)
来源：http://hz.fzhhl.top/gtmxjcyqkm.html

C#:   list.IndexOf(x);
来源：http://hz.chenzaomai.com/gtpmcmeauy.html

[D13] 过滤（保留满足条件的）
来源：http://hz.nanxinkj.top/gtkdaomdcs.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.ppjwa.cn/gtpnybrehx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.pycfn.com/gtxxjfeyfc.html

JS:   arr.filter(x => x > 3)
来源：http://hz.yj202588.top/gtxucvjbzo.html

TS:   arr.filter(x => x > 3)
来源：http://hz.pycfn.com/gtxsgbhoux.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.yuxming.cn/gtqjticqfj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.mhx1999.top/gtttexkxvy.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.cqqwz.cn/gtluszuxjw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.hfpthk.cn/gtmsuhafbu.html

[D14] 映射转换（每个元素变形）
来源：http://hz.pycfn.com/gtgdxpxkxp.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.gzhubu.top/gtmxnjhtjz.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.cucudq.cn/gtoxubvrow.html

JS:   arr.map(x => x * 2)
来源：http://hz.zycfv.cn/gtpzgactmt.html

TS:   arr.map(x => x * 2)
来源：http://hz.shzxlz.cn/gtaejrring.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.jqgfzy.top/gtbesuugqu.html

Go:   // 手写循环
来源：http://hz.tianlin.xyz/gtlnfkxwgg.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.gaohongyu789.top/gtkttqnbly.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.tanke756.top/gtxbatzwjs.html

[D15] 去重
来源：http://hz.hysaishi.cn/gtsqurdjqf.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.gotoacloud.top/gtghclhjta.html

PHP:  array_unique($arr);
来源：http://hz.ehwqpu.com/gtdciswjlq.html

JS:   [...new Set(arr)]
来源：http://hz.smart0.xyz/gtibszzmju.html

TS:   [...new Set(arr)]
来源：http://hz.tian-w.cn/gtpatabyph.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.tianlin.xyz/gtipftfdto.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.snrcjt.cn/gtnrocjafj.html

Ruby: arr.uniq
来源：http://hz.52xcode.cn/gtdqjncnvs.html

C#:   list.Distinct().ToList()
来源：http://hz.sweek.top/gtcayvetbh.html

[D16] 求和与平均值
来源：http://hz.hywenlv.cn/gtfonaksbj.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.jinqigufen.top/gtbidaxert.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.zdqjudy.top/gtfvwatkph.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.cucudq.cn/gthycoybqz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.dashuyun.cn/gtkokkvspc.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.fengsongda.top/gtlissrerl.html

Go:   // 手写循环累加
来源：http://hz.jinqigufen.top/gtcijzvxxx.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.aizwys.cn/gtruehbqlo.html

C#:   list.Sum();  list.Average()
来源：http://hz.zhiwuduotai.top/gtakivqgar.html

[D17] 最大值与最小值
来源：http://hz.316326.xyz/gtkzjldfjt.html

Py:   max(arr);  min(arr)
来源：http://hz.chenjidiqi.icu/gtrnajqicf.html

PHP:  max($arr);  min($arr);
来源：http://hz.daria6918.cn/gturtxrkyk.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.sxryk.cn/gtzappbgtg.html

TS:   Math.max(...arr);
来源：http://hz.ydjk.org.cn/gtahoevbzr.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.guannengcc.top/gtyyldwhcd.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.iojbl.cn/gtdeaihzhy.html

Ruby: arr.max;  arr.min
来源：http://hz.zhengqikj.top/gtoqgrrzqz.html

C#:   list.Max();  list.Min()
来源：http://hz.jinqigufen.top/gthpgalhcr.html

[D18] 扁平化嵌套数组
来源：http://hz.yuxming.cn/gtjbvvprny.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.hammf.cn/gtlvqxgnde.html

PHP:  array_merge(...$nested);
来源：http://hz.ydjk.org.cn/gtkdkshshk.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.jinghuilouyu.cn/gtbmtapfba.html

TS:   nested.flat();
来源：http://hz.zhoulong.xyz/gtifcybwex.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.dashuyun.cn/gtswziwjpp.html

Go:   // 手写双层循环
来源：http://hz.ywan-chungtsiang.top/gtpeshkjfb.html

Ruby: nested.flatten
来源：http://hz.gotoacloud.top/gthqwakirg.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.yongpay.top/gtcskghyyl.html

[D19] 按字段分组
来源：http://hz.yongpay.top/gtoktswsim.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.sxryk.cn/gtypxsmgrj.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.meibo888.top/gtzzsfzuud.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.haohaochexian.top/gtquwxuvui.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.havefunace.top/gtjwmvhnhv.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.xziqi.cn/gtrndufzlk.html

Go:   // 手写 map[string][]T
来源：http://hz.yueranfly.top/gtbnnxejsi.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.jlsjyb.cn/gtnrkftotr.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.aibaodan.cn/gtradojzwv.html

[D20] 统计每个元素出现次数
来源：http://hz.ydjk.org.cn/gtvmkissld.html

Py:   Counter(arr)
来源：http://hz.aizwys.cn/gtewtpfadd.html

PHP:  array_count_values($arr);
来源：http://hz.fzhhl.top/gtkvopuuta.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.ppjwa.cn/gtxljfzdws.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.gotoacloud.top/gtcpbbtvmk.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.zhiwuduotai.top/gtqbgpiimb.html

Go:   // 手写 map[T]int
来源：http://hz.jianghu66.top/gtoxlzhbzw.html

Ruby: arr.tally
来源：http://hz.yj20258.top/gtgegjczfl.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.sxryk.cn/gthgosfkkb.html

[D21] 判断是否包含某元素
来源：http://hz.svipenyu.cn/gtwdbytkky.html

Py:   x in arr
来源：http://hz.yj20258888.top/gtbssvehqh.html

PHP:  in_array($x, $arr, true);
来源：http://hz.yuanzhike.top/gtcsqezfhe.html

JS:   arr.includes(x)
来源：http://hz.jinqigufen.top/gtdadsccyt.html

TS:   arr.includes(x)
来源：http://hz.ydzc1.top/gtyhcncsmh.html

Java: list.contains(x)
来源：http://hz.meibo888.top/gtsmnzqzeq.html

Go:   slices.Contains(arr, x)
来源：http://hz.yuxming.cn/gtrmxvwzoh.html

Ruby: arr.include?(x)
来源：http://hz.pengpengdd.cyou/gtpzepjktl.html

C#:   list.Contains(x)
来源：http://hz.nanxuanxn.top/gtvxzoiqlb.html

[D22] 复制数组（避免共享引用）
来源：http://hz.andypj.xyz/gtxbuwzxfh.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.dashuyun.cn/gtructzkef.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.tian-w.cn/gtapaqtgdf.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.vqdsnc.cn/gtdxpjtcaf.html

TS:   [...arr];
来源：http://hz.cheryme.top/gtxepsfwpq.html

Java: new ArrayList<>(list);
来源：http://hz.yanxiufei.cn/gtykjlcani.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.hnxiangtu.top/gtvjapxwle.html

Ruby: arr.dup;  arr.clone
来源：http://hz.smart0.xyz/gtcvijhlvu.html

C#:   new List<int>(list);
来源：http://hz.jinqigufen.top/gtvkxzotzs.html

[D23] reduce 累积计算
来源：http://hz.sxryk.cn/gtzlkfxhju.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.jinghuilouyu.cn/gtffeecpya.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.shanyushiyangtech.top/gtlqzlvniv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jinqigufen.top/gtirzzgmbu.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhengqikj.top/gtjpsqfbnx.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.birdmap.top/gtfilvwumf.html

Go:   // 手写循环
来源：http://hz.dashuyun.cn/gtuppnbdyu.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.ybcxt.top/gtkpmjeayi.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.pengpengdd.cyou/gtmzitpipr.html

[D24] 字典 / Map 基本操作
来源：http://hz.jlsjyb.cn/gthlcnmfdc.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.ybcxt.top/gtjrdunkly.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.xinyue.icu/gtplspryug.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.zhixingplan.top/gtsaeqmlug.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.kuanghao11.cn/gtwzifpgjf.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.meibo888.top/gtuznkxvqo.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.kuanghao11.cn/gtfmyybmub.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.iojbl.cn/gtkwuxylro.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.yj20258.top/gtdoitcnuo.html

[D25] Set 集合去重与交并差
来源：http://hz.xingfuxueyuan.xyz/gtvevhdxcg.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.cdnleiting.top/gtwbiihaar.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.ydjk.org.cn/gtmwbsemrt.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.hongshengwenyu.top/gthwnxqfcn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.ywan-chungtsiang.top/gtplkibhsp.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.birdmap.top/gtpecnysmy.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.jinqigufen.top/gtrfuffflk.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.cucudq.cn/gtghbrmota.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.gogol.net.cn/gtnmbzlpbk.html

[D26] 数组转字符串
来源：http://hz.ivvv.top/gtinprvinr.html

Py:   ", ".join(map(str, arr))
来源：http://hz.smart0.xyz/gtywspeamk.html

PHP:  implode(", ", $arr);
来源：http://hz.wangshuangyany.cn/gtvpjcgxql.html

JS:   arr.join(", ")
来源：http://hz.cucudq.cn/gteusqoicq.html

TS:   arr.join(", ")
来源：http://hz.zhiwuduotai.top/gtcsklcldg.html

Java: String.join(", ", list)
来源：http://hz.shuidangran.top/gtndhxephp.html

Go:   strings.Join(strs, ", ")
来源：http://hz.52xcode.cn/gttnzrnuhb.html

Ruby: arr.join(", ")
来源：http://hz.zhijiandao.cn/gtdcjnekwh.html

C#:   string.Join(", ", list)
来源：http://hz.xinyue.icu/gthqhiexkm.html

================================================================================
来源：http://hz.jinqigfzy.top/gthrcojqxp.html

E. 字符串处理
来源：http://hz.aibaodan.cn/gtltqosuhp.html

================================================================================
来源：http://hz.quarkkingdee.top/gthlvydpbp.html

[E01] 拼接字符串
来源：http://hz.xziqi.cn/gtyhodcgyt.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.xziqi.cn/gtotfmaqjl.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.nanxinkj.top/gtgxfyzran.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.cdnleiting.top/gtlwcqztwh.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.cdnleiting.top/gtdxspttol.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.yueranfly.top/gttmrqfrjy.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.ppjwa.cn/gtbpximtrm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.zhiwuduotai.top/gtrexumopm.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.yj20258.top/gtzvxsafrq.html

[E02] 重复字符串
来源：http://hz.tian-w.cn/gtfxcdcsro.html

Py:   "ab" * 3
来源：http://hz.vqdsnc.cn/gtvdxhbzxi.html

PHP:  str_repeat("ab", 3);
来源：http://hz.zhoulong.xyz/gtlrfqqjab.html

JS:   "ab".repeat(3)
来源：http://hz.yanxiufei.cn/gtkqqnddtz.html

TS:   "ab".repeat(3)
来源：http://hz.aizwys.cn/gtrhnbxphf.html

Java: "ab".repeat(3)
来源：http://hz.daxiang520.top/gtqzsnfsju.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.shangyingyoupin.top/gtejehlusk.html

Ruby: "ab" * 3
来源：http://hz.ydjk.org.cn/gtkajtrhcj.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.wangdashe.top/gtdlzcoxfl.html

[E03] 截取子串
来源：http://hz.0kj1m.cn/gtjtfonxqx.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.pycfn.com/gtmfsesxbv.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.zdqjudy.top/gtjdjaliur.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.hammf.cn/gtbyyunocj.html

TS:   s.slice(1, 4)
来源：http://hz.hammf.cn/gtsrjylnxh.html

Java: s.substring(1, 4)
来源：http://hz.ydjk.org.cn/gtboasfupl.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.jyoumei.cn/gtajpwmqsc.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.nanxuanxn.top/gtihwoelwc.html

C#:   s.Substring(1, 3)
来源：http://hz.fzhhl.top/gthoqguerv.html

[E04] 查找子串位置
来源：http://hz.jyoumei.cn/gtqknpuxha.html

Py:   s.find("x");  s.index("x")
来源：http://hz.shzxlz.cn/gtdbstcfvp.html

PHP:  strpos($s, "x");
来源：http://hz.52xcode.cn/gtdehjecgd.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.jqgufenzy.top/gtlgqktnxn.html

TS:   s.indexOf("x")
来源：http://hz.chenlongwang.top/gtvtpweeeb.html

Java: s.indexOf("x")
来源：http://hz.zhengqikj.top/gthkycgpze.html

Go:   strings.Index(s, "x")
来源：http://hz.guowangkeji.top/gtwzhhzjjj.html

Ruby: s.index("x")
来源：http://hz.ydzc1.top/gtdigosgij.html

C#:   s.IndexOf("x")
来源：http://hz.daria6918.cn/gtdthvrbyf.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.fzhhl.top/gtiyhmklex.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.shanyushiyangkeji.top/gtphdlizsq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.jiagoushi.top/gtwynyntyv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.xinyue.icu/gtjwrohnla.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.ydzc1.top/gtumhnwlas.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.xuanzx.com/gtekcozkeb.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.aizwys.cn/gtqrslneji.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.yueranfly.top/gtsefmfkoj.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.yuxming.cn/gtesylayfw.html

[E06] 替换子串
来源：http://hz.feifeiyinyue.top/gtcocigtbs.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.wangdashe.top/gtssjdllmo.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.cashguo.top/gtsdfnwyhu.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.chenjidiqi.icu/gtcwvlajis.html

TS:   s.replaceAll("a", "b")
来源：http://hz.tian-w.cn/gtdyhiczzb.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.sxryk.cn/gtftdeypdp.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.nanxinkj.top/gtgghvycqs.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.jqgufenzy.top/gthiwrubzr.html

C#:   s.Replace("a", "b")
来源：http://hz.sweek.top/gtzmupxild.html

[E07] 按分隔符拆分
来源：http://hz.hammf.cn/gtpgukxkpw.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.ehwqpu.com/gtiwiqbtkj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.zhongyouzk.top/gtbkucwpmp.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.wangdashe.top/gtsutufzpl.html

TS:   s.split(",")
来源：http://hz.hongshengwenyu.top/gtucstcerm.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.zhixingplan.top/gtgmlrctam.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.yanxiufei.cn/gtutdxvidr.html

Ruby: s.split(",");  s.split
来源：http://hz.yangfankeji.com/gtxqseutgs.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.cucudq.cn/gtwhedanim.html

[E08] 数组按分隔符合并
来源：http://hz.nanxuanxn.top/gtiixszffw.html

Py:   ",".join(items)
来源：http://hz.jinghuilouyu.cn/gtzqbylgfk.html

PHP:  implode(",", $items);
来源：http://hz.jinqigfzy.top/gtyajmdodf.html

JS:   items.join(",")
来源：http://hz.redwolf501.top/gtkyfgodmm.html

TS:   items.join(",")
来源：http://hz.sweek.top/gtoccwfaix.html

Java: String.join(",", items)
来源：http://hz.jinghuilouyu.cn/gtvgacvyno.html

Go:   strings.Join(items, ",")
来源：http://hz.cqqwz.cn/gtskfhfnwv.html

Ruby: items.join(",")
来源：http://hz.xinyue.icu/gtpsyhqvnl.html

C#:   string.Join(",", items)
来源：http://hz.jqgufenzy.top/gtuehqtoxu.html

[E09] 去除所有空白字符
来源：http://hz.c1oappe.top/gtqoezdyzg.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.ydzc1.top/gtzkdfhjha.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.cheryme.top/gtduvejodh.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.tianlin.xyz/gtshclcwas.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.xinyue.icu/gtmedqduaf.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.zdqjudy.top/gttofbpadw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.daria6918.cn/gtgksheqhz.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.xuanzx.com/gtadtwybep.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.sufxvd.cn/gtbjmhzjkr.html

[E10] 左侧补零 / 定长填充
来源：http://hz.hysaishi.cn/gtdmtbupdq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.yangfankeji.com/gtbgvubbvv.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.yongpay.top/gtimlldzbd.html

JS:   "7".padStart(3, "0")
来源：http://hz.yongpay.top/gthwiozqeg.html

TS:   "7".padStart(3, "0")
来源：http://hz.shanyushiyangkeji.top/gtaodacoxf.html

Java: String.format("%03d", 7)
来源：http://hz.ywan-chungtsiang.top/gtlatrhpgm.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.fzhhl.top/gtbsiallay.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.sweek.top/gtsklktdid.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.nwbrower.top/gtufuyujdb.html

[E11] 反转字符串
来源：http://hz.yongpay.top/gtogeecdos.html

Py:   s[::-1]
来源：http://hz.birdmap.top/gtveigshxn.html

PHP:  strrev($s);
来源：http://hz.yj202588.top/gtfwkfulvo.html

JS:   [...s].reverse().join("")
来源：http://hz.tanke756.top/gtzuluvdku.html

TS:   [...s].reverse().join("")
来源：http://hz.jqgufenzy.top/gtkhzkwtgs.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.cqqwz.cn/gtrjydxhui.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.zycfv.cn/gtczpohemx.html

Ruby: s.reverse
来源：http://hz.0kj1m.cn/gtxegwnkdu.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.cheryme.top/gtekywwgsd.html

[E12] 统计某字符出现次数
来源：http://hz.pycfn.com/gtnmoowovn.html

Py:   s.count("a")
来源：http://hz.yongpay.top/gtieninmzm.html

PHP:  substr_count($s, "a");
来源：http://hz.hysaishi.cn/gtvptsnqkm.html

JS:   s.split("a").length - 1
来源：http://hz.mhx1999.top/gtezqmyjaa.html

TS:   s.split("a").length - 1
来源：http://hz.nanxuanxn.top/gtrgzhwdmf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.tian-w.cn/gtrubfykae.html

Go:   strings.Count(s, "a")
来源：http://hz.yangfankeji.com/gtubtfimok.html

Ruby: s.count("a")
来源：http://hz.jiagoushi.top/gtuwfyryyv.html

C#:   s.Count(c => c == 'a')
来源：http://hz.jinqigufen.top/gthyzgmadc.html

[E13] 逐字符遍历
来源：http://hz.chenlongwang.top/gtzjiujsce.html


<!-- 参考信息 -->