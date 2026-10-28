代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.tianlin.xyz/gtfyqyzfmi.html

TS:   [...a, ...b];
来源：http://hz.xingfuxueyuan.xyz/gtfmuvxosl.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.gzhubu.top/gtbcpoyipz.html

Go:   append(a, b...)
来源：http://hz.jiagoushi.top/gtfuuacqzu.html

Ruby: a + b;  a.concat(b)
来源：http://hz.guowangkeji.top/gtdaooziyg.html

C#:   a.Concat(b).ToList()
来源：http://hz.yvedp.cn/gttjdriiut.html

[D09] 排序（升序）
来源：http://hz.vqdsnc.cn/gtolyxkoom.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yj202588.top/gtfghzojye.html

PHP:  sort($arr);
来源：http://hz.xylfe.cn/gtumakpkgg.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.smart0.xyz/gtldqvcnel.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.hnxiangtu.top/gtittxapwc.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.cashguo.top/gtuwlkxxgw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.yj202588.top/gteczbdgbw.html

Ruby: arr.sort
来源：http://hz.gogol.net.cn/gtnbljzbom.html

C#:   list.Sort();
来源：http://hz.yuanzhike.top/gthrjcslfg.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.52xcode.cn/gtbfctyyfb.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.vqdsnc.cn/gtzomhuxyo.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.daxiang520.top/gtnxwvqkko.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yonumen.top/gtaavfpqep.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.aibaodan.cn/gtqxokwmee.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.dashuyun.cn/gtiegsicnr.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.jqgfzy.top/gtrujexsds.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.316326.xyz/gtcenftmoe.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.quarkkingdee.top/gtjxyamhbk.html

[D11] 反转数组
来源：http://hz.yj20258888.top/gtxxhxhlsg.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.chenzaomai.com/gtqmnptxux.html

PHP:  array_reverse($arr);
来源：http://hz.haohaochexian.top/gtglwixgka.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.fzhhl.top/gttjpzqyst.html

TS:   [...arr].reverse();
来源：http://hz.hnqzz.top/gtwnbmnyvc.html

Java: Collections.reverse(list);
来源：http://hz.chenzaomai.com/gttohwuurr.html

Go:   slices.Reverse(arr)
来源：http://hz.jinghuilouyu.cn/gtptwhpsgi.html

Ruby: arr.reverse
来源：http://hz.ppjwa.cn/gtyemwpyyk.html

C#:   list.Reverse();
来源：http://hz.daria6918.cn/gtznkfanrn.html

[D12] 查找元素下标
来源：http://hz.cashguo.top/gtzwbofhtu.html

Py:   arr.index(x);  x in arr
来源：http://hz.guannengcc.top/gttabzcylt.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.svipenyu.cn/gtmtncvzqc.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jinghuilouyu.cn/gtuoowzwfj.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.guowangkeji.top/gtmreaxoan.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.kuanghao11.cn/gtcffgcgvd.html

Go:   slices.Index(arr, x)
来源：http://hz.ydjk.org.cn/gtvphixvos.html

Ruby: arr.index(x)
来源：http://hz.chenjidiqi.icu/gttcjevgma.html

C#:   list.IndexOf(x);
来源：http://hz.yangfankeji.com/gtmjobknps.html

[D13] 过滤（保留满足条件的）
来源：http://hz.shuidangran.top/gtwzajildf.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.feifeiyinyue.top/gtptwlprqj.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.hfpthk.cn/gtajbxyzsf.html

JS:   arr.filter(x => x > 3)
来源：http://hz.shuidangran.top/gtfdjdirjj.html

TS:   arr.filter(x => x > 3)
来源：http://hz.wangdashe.top/gtlhtboasu.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.wangshuangyany.cn/gtsdyftwaz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.yonumen.top/gtrjpkdfvk.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.ydzc1.top/gtmbpkrjwj.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.haohaochexian.top/gtpzgqdlje.html

[D14] 映射转换（每个元素变形）
来源：http://hz.zhoulong.xyz/gtclrqllbj.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.sysykeji.top/gtjpxkinym.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.yj202588.top/gtmhsawkok.html

JS:   arr.map(x => x * 2)
来源：http://hz.hammf.cn/gtcivrfnzg.html

TS:   arr.map(x => x * 2)
来源：http://hz.cucudq.cn/gttvlvmalo.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.sysykeji.top/gtxtoikcfv.html

Go:   // 手写循环
来源：http://hz.tianlin.xyz/gtetkwxidv.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.zhijiandao.cn/gtjgzyumkb.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.quarkkingdee.top/gtqdtkutcm.html

[D15] 去重
来源：http://hz.jinqigfzy.top/gtcnbknyza.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.svipenyu.cn/gtzgjsxorb.html

PHP:  array_unique($arr);
来源：http://hz.ehwqpu.com/gtssonvmns.html

JS:   [...new Set(arr)]
来源：http://hz.0kj1m.cn/gticcsybzg.html

TS:   [...new Set(arr)]
来源：http://hz.hywenlv.cn/gtmrmiwktq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.chenlongwang.top/gtpgfxbhtv.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.jlsjyb.cn/gtohrzpdrg.html

Ruby: arr.uniq
来源：http://hz.xziqi.cn/gtbdzqgtap.html

C#:   list.Distinct().ToList()
来源：http://hz.cqqwz.cn/gtspotddsa.html

[D16] 求和与平均值
来源：http://hz.jinyuanbaomall.cn/gtozeqozrd.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.shangyingyoupin.top/gtorrwyojo.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.ivvv.top/gtncpdvfgj.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.tanke756.top/gtecogylyx.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.daria6918.cn/gtovigwrtl.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.nwbrower.top/gtousrnwih.html

Go:   // 手写循环累加
来源：http://hz.nanxuanxn.top/gthijpgpam.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.gotoacloud.top/gtnaysjait.html

C#:   list.Sum();  list.Average()
来源：http://hz.svipenyu.cn/gtrysirgwc.html

[D17] 最大值与最小值
来源：http://hz.yj202588.top/gtplooemdb.html

Py:   max(arr);  min(arr)
来源：http://hz.jqgufenzy.top/gtirppgqdl.html

PHP:  max($arr);  min($arr);
来源：http://hz.ehwqpu.com/gtexeuhxsr.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.yonumen.top/gtfcozvujz.html

TS:   Math.max(...arr);
来源：http://hz.316326.xyz/gtgkckvnal.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.jinghuilouyu.cn/gtutanmncq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.jqgfzy.top/gtclkfgexv.html

Ruby: arr.max;  arr.min
来源：http://hz.wangdashe.top/gtvnmovham.html

C#:   list.Max();  list.Min()
来源：http://hz.ywan-chungtsiang.top/gtnbaflfkr.html

[D18] 扁平化嵌套数组
来源：http://hz.jinqigufen.top/gtqcbjwbrb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.wangshuangyany.cn/gtajeauufg.html

PHP:  array_merge(...$nested);
来源：http://hz.wangdashe.top/gtgymfzxni.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.gaohongyu789.top/gtveiuckkg.html

TS:   nested.flat();
来源：http://hz.hysaishi.cn/gtilsninns.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.havefunace.top/gthfkjhvav.html

Go:   // 手写双层循环
来源：http://hz.sufxvd.cn/gtfebseump.html

Ruby: nested.flatten
来源：http://hz.mhx1999.top/gtmpyjrtlg.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.nanxinkj.top/gttsxvexec.html

[D19] 按字段分组
来源：http://hz.gzhubu.top/gtoelqmghd.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.jianghu66.top/gtjjylvffu.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.jianghu66.top/gtaegbblvl.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.nwbrower.top/gtkxzoqbry.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.jinghuilouyu.cn/gtrglfhlqj.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.zhaomingkeji.xyz/gttnjinrao.html

Go:   // 手写 map[string][]T
来源：http://hz.zhoulong.xyz/gtnvswvawc.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.quarkkingdee.top/gtneackrej.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.havefunace.top/gtzbcbwrue.html

[D20] 统计每个元素出现次数
来源：http://hz.xziqi.cn/gtuzzpnlny.html

Py:   Counter(arr)
来源：http://hz.yuxming.cn/gtrzznsxpu.html

PHP:  array_count_values($arr);
来源：http://hz.jinghuilouyu.cn/gtalucobuh.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.cashguo.top/gtnohceaiz.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yvedp.cn/gtypnnggwz.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.xuetiantiany.cn/gtxhqnkwtr.html

Go:   // 手写 map[T]int
来源：http://hz.nanxuanxn.top/gtpevwzmiy.html

Ruby: arr.tally
来源：http://hz.xylfe.cn/gttwxmnfbz.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.zhaomingkeji.xyz/gtgyuschah.html

[D21] 判断是否包含某元素
来源：http://hz.316326.xyz/gtduewnemy.html

Py:   x in arr
来源：http://hz.ybcxt.top/gtizreenqu.html

PHP:  in_array($x, $arr, true);
来源：http://hz.hfpthk.cn/gtckxhfyoh.html

JS:   arr.includes(x)
来源：http://hz.xinyue.icu/gtotrwunbw.html

TS:   arr.includes(x)
来源：http://hz.jqgufenzy.top/gtvaekazpw.html

Java: list.contains(x)
来源：http://hz.yj20258888.top/gtyhsiwlxu.html

Go:   slices.Contains(arr, x)
来源：http://hz.zdqjudy.top/gtplpjlfjf.html

Ruby: arr.include?(x)
来源：http://hz.gotoacloud.top/gtzolyobbw.html

C#:   list.Contains(x)
来源：http://hz.jianghu66.top/gtcjcmojuy.html

[D22] 复制数组（避免共享引用）
来源：http://hz.havefunace.top/gtdiwhrhmb.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.sweek.top/gtmvygatlo.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.sxryk.cn/gtfnnsiyhf.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.xuanzx.com/gtezeseemt.html

TS:   [...arr];
来源：http://hz.zhoulong.xyz/gtdfzascgn.html

Java: new ArrayList<>(list);
来源：http://hz.jyoumei.cn/gteromgmto.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.hongshengwenyu.top/gtlsemtkxf.html

Ruby: arr.dup;  arr.clone
来源：http://hz.jianghu66.top/gtgmhogevp.html

C#:   new List<int>(list);
来源：http://hz.hfpthk.cn/gtcoufiayc.html

[D23] reduce 累积计算
来源：http://hz.sxryk.cn/gtaotsmivm.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.ydzc1.top/gtaajhtrkf.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.quarkkingdee.top/gtgogisgqm.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.kuanghao11.cn/gtpueulypp.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yj20258888.top/gttbfoyrax.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.jyoumei.cn/gtkceqpjle.html

Go:   // 手写循环
来源：http://hz.andypj.xyz/gtsbvqbwuu.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.zhoulong.xyz/gtqmvvqoaf.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.xingfuxueyuan.xyz/gtmtzokqwr.html

[D24] 字典 / Map 基本操作
来源：http://hz.9152youxi.cn/gtgmwnktbb.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.chenjidiqi.icu/gtwkjwmygx.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.hongshengwenyu.top/gtqouatpkq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.0kj1m.cn/gtiupsdble.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.hongshengwenyu.top/gtumgcibiy.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.yangfankeji.com/gthjsesima.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.yueranfly.top/gthqpmbhud.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.hnqzz.top/gtvreuqfgs.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.yj20258.top/gtqjdsnstr.html

[D25] Set 集合去重与交并差
来源：http://hz.guannengcc.top/gteavxuenj.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.nanxinkj.top/gtsacwutdl.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.gaohongyu789.top/gtqknxavms.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.52xcode.cn/gtcbhwwwga.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.ywan-chungtsiang.top/gttsjoindl.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.pycfn.com/gtudsvughh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.redwolf501.top/gteqowregb.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.cucudq.cn/gtouczeopz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.redwolf501.top/gteraspblt.html

[D26] 数组转字符串
来源：http://hz.cdnleiting.top/gtkejttfjb.html

Py:   ", ".join(map(str, arr))
来源：http://hz.gotoacloud.top/gtyapifwsb.html

PHP:  implode(", ", $arr);
来源：http://hz.zhongyouzk.top/gtuochwuju.html

JS:   arr.join(", ")
来源：http://hz.sysykeji.top/gtfnburkbi.html

TS:   arr.join(", ")
来源：http://hz.sufxvd.cn/gtbfybwpjn.html

Java: String.join(", ", list)
来源：http://hz.tian-w.cn/gtklxrxaji.html

Go:   strings.Join(strs, ", ")
来源：http://hz.shzxlz.cn/gtqksnjkpe.html

Ruby: arr.join(", ")
来源：http://hz.hfpthk.cn/gtuikqzzaf.html

C#:   string.Join(", ", list)
来源：http://hz.yuxming.cn/gtfjhlpqfs.html

================================================================================
来源：http://hz.jyoumei.cn/gtjcbvtvvz.html

E. 字符串处理
来源：http://hz.c1oappe.top/gtrzgjries.html

================================================================================
来源：http://hz.cqqwz.cn/gtfvsqyuhv.html

[E01] 拼接字符串
来源：http://hz.c1oappe.top/gtrgknyjji.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.ybcxt.top/gtqxvtrmzn.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.quarkkingdee.top/gtxgecntij.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.hywenlv.cn/gtzhorkjxw.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.xuanzx.com/gtuuqhkdwc.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.yonumen.top/gtdzgltsmg.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.yvedp.cn/gtlmeihfmr.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.tanke756.top/gttzkfcdmh.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.yueranfly.top/gtkcibexru.html

[E02] 重复字符串
来源：http://hz.daxiang520.top/gtnuthruvm.html

Py:   "ab" * 3
来源：http://hz.yongpay.top/gtantntroo.html

PHP:  str_repeat("ab", 3);
来源：http://hz.aizwys.cn/gtzvkgjmme.html

JS:   "ab".repeat(3)
来源：http://hz.quarkkingdee.top/gtrksrummf.html

TS:   "ab".repeat(3)
来源：http://hz.aibaodan.cn/gtdaglnfwf.html

Java: "ab".repeat(3)
来源：http://hz.tianlin.xyz/gtpgdcalaz.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.haohaochexian.top/gtlwiazebb.html

Ruby: "ab" * 3
来源：http://hz.316326.xyz/gtawcbyiom.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.ppjwa.cn/gthgmmozlx.html

[E03] 截取子串
来源：http://hz.guowangkeji.top/gtgunutwoe.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.jyoumei.cn/gtrtssgauq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.kuanghao11.cn/gtmrnetdmr.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.zhixingplan.top/gtgddvhkgr.html

TS:   s.slice(1, 4)
来源：http://hz.xuanzx.com/gtxkubdjdz.html

Java: s.substring(1, 4)
来源：http://hz.cashguo.top/gtoznvscqo.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.jqgufenzy.top/gtyygnucoa.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.jinyuanbaomall.cn/gtmcwpymvg.html

C#:   s.Substring(1, 3)
来源：http://hz.yj20258888.top/gtayzokfwe.html

[E04] 查找子串位置
来源：http://hz.zhaomingkeji.xyz/gtjshrkndl.html

Py:   s.find("x");  s.index("x")
来源：http://hz.vqdsnc.cn/gtchtatkjd.html

PHP:  strpos($s, "x");
来源：http://hz.guannengcc.top/gtrkgbzjji.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.yj20258888.top/gtayzqelik.html

TS:   s.indexOf("x")
来源：http://hz.svipenyu.cn/gtliqmxmbj.html

Java: s.indexOf("x")
来源：http://hz.yuanzhike.top/gtihbokgzv.html

Go:   strings.Index(s, "x")
来源：http://hz.nwbrower.top/gtrddgxviq.html

Ruby: s.index("x")
来源：http://hz.hywenlv.cn/gtyvysnmsq.html

C#:   s.IndexOf("x")
来源：http://hz.daria6918.cn/gtfmfnlpib.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.nanxinkj.top/gtnerlefui.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.daxiang520.top/gtohajamkz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.jinqigfzy.top/gtwoujxcqx.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.xylfe.cn/gtfmxvjdkw.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.jinqigfzy.top/gtzkbirzir.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.c1oappe.top/gtghnptjxe.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.jianghu66.top/gtobyluaga.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.smart0.xyz/gthyfuelfc.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.hongshengwenyu.top/gtkmyjujog.html

[E06] 替换子串
来源：http://hz.mhx1999.top/gtnxxzrizn.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.nwbrower.top/gtqrrcrlcd.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.zdqjudy.top/gtyvqjyevx.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.nanxuanxn.top/gtmtnaqocd.html

TS:   s.replaceAll("a", "b")
来源：http://hz.bjfxy.top/gtneltrccp.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.svipenyu.cn/gthfkurmos.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.daria6918.cn/gtxqzgchoq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.andypj.xyz/gtxbquxkqy.html

C#:   s.Replace("a", "b")
来源：http://hz.jiagoushi.top/gtvxllghep.html

[E07] 按分隔符拆分
来源：http://hz.sysykeji.top/gtugasqrey.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.xylfe.cn/gtgwfknvhn.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.cdnleiting.top/gteyyuwtjv.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.gogol.net.cn/gthcetibrz.html

TS:   s.split(",")
来源：http://hz.yongpay.top/gttbqtkizt.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.shanyushiyangtech.top/gtcavmbcoj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.cqqwz.cn/gtrwraipyo.html

Ruby: s.split(",");  s.split
来源：http://hz.nwbrower.top/gthtdvzdth.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.nwbrower.top/gtfbmcfgzr.html

[E08] 数组按分隔符合并
来源：http://hz.aizwys.cn/gtmxbeokkp.html

Py:   ",".join(items)
来源：http://hz.nanxinkj.top/gtrrnezbkz.html

PHP:  implode(",", $items);
来源：http://hz.sufxvd.cn/gtddojobzn.html

JS:   items.join(",")
来源：http://hz.gotoacloud.top/gtqolndzqt.html

TS:   items.join(",")
来源：http://hz.daxiang520.top/gtxsqjazuj.html

Java: String.join(",", items)
来源：http://hz.tanke756.top/gttkvssfui.html

Go:   strings.Join(items, ",")
来源：http://hz.ydzc1.top/gtclpujydo.html

Ruby: items.join(",")
来源：http://hz.tanke756.top/gtzpdqetoa.html

C#:   string.Join(",", items)
来源：http://hz.kuanghao11.cn/gtxeexcnga.html

[E09] 去除所有空白字符
来源：http://hz.shanyushiyangkeji.top/gtstifccwz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.redwolf501.top/gtkkmjizit.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.bjfxy.top/gtmbmjwbqq.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.tanke756.top/gtxhtbbcry.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.pycfn.com/gtpzhacrer.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.yueranfly.top/gtsqyxnpgr.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.shuidangran.top/gtqrdfirky.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.tanke756.top/gtfibpvdvh.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.sxryk.cn/gtesnnacuc.html

[E10] 左侧补零 / 定长填充
来源：http://hz.tian-w.cn/gtutljapbl.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.yangfankeji.com/gtoorbmokv.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.kuanghao11.cn/gtrlhaanyx.html

JS:   "7".padStart(3, "0")
来源：http://hz.chenzaomai.com/gtjhlvcsrk.html

TS:   "7".padStart(3, "0")
来源：http://hz.zhixingplan.top/gtxqefwwyn.html

Java: String.format("%03d", 7)
来源：http://hz.jianghu66.top/gtfsfiolpt.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.xuetiantiany.cn/gtdemvfowe.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.jqgufenzy.top/gtczpgvkzu.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.chenzaomai.com/gtonhigkia.html

[E11] 反转字符串
来源：http://hz.zhongyouzk.top/gtspdqmalr.html

Py:   s[::-1]
来源：http://hz.gaohongyu789.top/gtyyamwdtv.html

PHP:  strrev($s);
来源：http://hz.cheryme.top/gthxeozaxk.html

JS:   [...s].reverse().join("")
来源：http://hz.gaohongyu789.top/gtyotxujfo.html

TS:   [...s].reverse().join("")
来源：http://hz.smart0.xyz/gtwylxsypp.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.jqgufenzy.top/gtfdcdqzrp.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.nanxinkj.top/gttjydmpxy.html

Ruby: s.reverse
来源：http://hz.cdnleiting.top/gtktxzvomn.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.yongpay.top/gttazotxkz.html

[E12] 统计某字符出现次数
来源：http://hz.cashguo.top/gtnzcljgaz.html

Py:   s.count("a")
来源：http://hz.0kj1m.cn/gtlgbujvov.html

PHP:  substr_count($s, "a");
来源：http://hz.yvedp.cn/gtterhrkhb.html

JS:   s.split("a").length - 1
来源：http://hz.feifeiyinyue.top/gtfwbltpad.html

TS:   s.split("a").length - 1
来源：http://hz.tanke756.top/gtehwbenqw.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.chenlongwang.top/gtectghsoy.html

Go:   strings.Count(s, "a")
来源：http://hz.fengsongda.top/gtecjvsmus.html

Ruby: s.count("a")
来源：http://hz.xuanzx.com/gtkouoblvr.html

C#:   s.Count(c => c == 'a')
来源：http://hz.gotoacloud.top/gtyosewkrc.html

[E13] 逐字符遍历
来源：http://hz.cashguo.top/gtciyrfbcq.html

Py:   for ch in s: print(ch)
来源：http://hz.shzxlz.cn/gtveaiktdb.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.feifeiyinyue.top/gtmagsksvo.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.cheryme.top/gtsfzcruft.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ywan-chungtsiang.top/gtoceyllid.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.yuanzhike.top/gthraxxpmg.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.shuidangran.top/gtucndlvqc.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.zhixingplan.top/gtiyfhynno.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.gotoacloud.top/gtgahyvrun.html

[E14] URL 编码与 Base64
来源：http://hz.jiagoushi.top/gtjlavwxtp.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.mhx1999.top/gtnjtjgfuk.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.xuanzx.com/gtkilkvmpv.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.xuanzx.com/gtajmmlkaz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.cheryme.top/gtnbphtaea.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.zhixingplan.top/gtoyivqhfn.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.svipenyu.cn/gtuzkjaoen.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.meibo888.top/gtsvjnjycz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.gzhubu.top/gtdqmaeuib.html

[E15] HTML 转义 / 反转义
来源：http://hz.c1oappe.top/gtupawcdgb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.jqgufenzy.top/gtyidnhxuz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.nanxuanxn.top/gtgcvyjpvv.html


<!-- 参考信息 -->