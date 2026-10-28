代发 wailian999

Java: list.size();
来源：http://hz.aizwys.cn/gtdqltgoda.html

Go:   len(arr)
来源：http://hz.yanxiufei.cn/gtoehpeqpk.html

Ruby: arr.length; arr.size
来源：http://hz.hnqzz.top/gtehedxbfp.html

C#:   list.Count;
来源：http://hz.ydjk.org.cn/gtdvrypweo.html

[D07] 切片 / 取子数组
来源：http://hz.shanyushiyangtech.top/gttaiwdour.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.jqgufenzy.top/gtpxlvwpbu.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.aizwys.cn/gtugidccdf.html

JS:   arr.slice(1, 4);
来源：http://hz.shuidangran.top/gtwrixeqfl.html

TS:   arr.slice(1, 4);
来源：http://hz.ydjk.org.cn/gtacnqxrei.html

Java: list.subList(1, 4);
来源：http://hz.ydjk.org.cn/gtjftvmadl.html

Go:   arr[1:4]
来源：http://hz.wangshuangyany.cn/gtqvawuxfn.html

Ruby: arr[1, 3]
来源：http://hz.sysykeji.top/gtlmtujlfb.html

C#:   list.GetRange(1, 3);
来源：http://hz.shzxlz.cn/gtziurmjkb.html

[D08] 合并两个数组
来源：http://hz.ehwqpu.com/gtwrkvaqef.html

Py:   a + b;  a.extend(b)
来源：http://hz.tianlin.xyz/gthaclmdlv.html

PHP:  array_merge($a, $b);
来源：http://hz.zdqjudy.top/gttnhcwasw.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.316326.xyz/gtvhuzobzq.html

TS:   [...a, ...b];
来源：http://hz.zhongyouzk.top/gthfjnockx.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.jianghu66.top/gtgxztuhxj.html

Go:   append(a, b...)
来源：http://hz.shuidangran.top/gtqayissuv.html

Ruby: a + b;  a.concat(b)
来源：http://hz.ydzc1.top/gtwkgkcmlx.html

C#:   a.Concat(b).ToList()
来源：http://hz.yanxiufei.cn/gtnkcpktul.html

[D09] 排序（升序）
来源：http://hz.yj202588.top/gtlsuuijyo.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.cqqwz.cn/gtbdkowrll.html

PHP:  sort($arr);
来源：http://hz.iojbl.cn/gtkfooxvqq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.hnqzz.top/gtkmmzlcyp.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.yueranfly.top/gtneswqkjk.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.shangyingyoupin.top/gtrjgyvvsp.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.xuanzx.com/gtucsrgyxz.html

Ruby: arr.sort
来源：http://hz.jlsjyb.cn/gtzfcwnoun.html

C#:   list.Sort();
来源：http://hz.guannengcc.top/gtfcvrvspp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.hywenlv.cn/gtlydcaqwc.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.jiagoushi.top/gtvbjmpzgl.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.0kj1m.cn/gtqfgwzxrc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.ywan-chungtsiang.top/gtsjeofrvu.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.iojbl.cn/gtmdincplr.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.chenzaomai.com/gtjhmnhdjp.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.hongshengwenyu.top/gtukpewxew.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.zycfv.cn/gthmxgvfbr.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.shanyushiyangtech.top/gtwoyltauy.html

[D11] 反转数组
来源：http://hz.feifeiyinyue.top/gtfnyjsytf.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.jianghu66.top/gthmtaocaa.html

PHP:  array_reverse($arr);
来源：http://hz.xuetiantiany.cn/gtseuncnrl.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.hfpthk.cn/gtybnqlxph.html

TS:   [...arr].reverse();
来源：http://hz.sweek.top/gtmmcaofnr.html

Java: Collections.reverse(list);
来源：http://hz.wangshuangyany.cn/gtbcyocqzr.html

Go:   slices.Reverse(arr)
来源：http://hz.shuidangran.top/gtbouhbomc.html

Ruby: arr.reverse
来源：http://hz.hammf.cn/gtruycjtiv.html

C#:   list.Reverse();
来源：http://hz.hnqzz.top/gtulfquwqi.html

[D12] 查找元素下标
来源：http://hz.andypj.xyz/gtqiczugcx.html

Py:   arr.index(x);  x in arr
来源：http://hz.hnqzz.top/gtdubvhnax.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.guowangkeji.top/gtzfrdwion.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.chenzaomai.com/gtukrjyfgt.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.ywan-chungtsiang.top/gtljgavxqv.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.ehwqpu.com/gtlymcixea.html

Go:   slices.Index(arr, x)
来源：http://hz.tanke756.top/gtcahstbdr.html

Ruby: arr.index(x)
来源：http://hz.0kj1m.cn/gtxcisxzwe.html

C#:   list.IndexOf(x);
来源：http://hz.andypj.xyz/gtyonisddf.html

[D13] 过滤（保留满足条件的）
来源：http://hz.jinqigufen.top/gtanhjkchg.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.wangshuangyany.cn/gtvnzwpbae.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.zhoulong.xyz/gtugslpzeu.html

JS:   arr.filter(x => x > 3)
来源：http://hz.zhijiandao.cn/gtfzigjrih.html

TS:   arr.filter(x => x > 3)
来源：http://hz.shanyushiyangkeji.top/gtjwqzeusv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.yanxiufei.cn/gtkaiveblm.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.ivvv.top/gtxgnjlgsx.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.9152youxi.cn/gtroeiqucq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.sysykeji.top/gtkxiekucb.html

[D14] 映射转换（每个元素变形）
来源：http://hz.nanxinkj.top/gtfubkwzgu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.ywan-chungtsiang.top/gtuagliius.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.xylfe.cn/gtepoqkkde.html

JS:   arr.map(x => x * 2)
来源：http://hz.yangfankeji.com/gtholravxu.html

TS:   arr.map(x => x * 2)
来源：http://hz.hnqzz.top/gtigmnieso.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.pengpengdd.cyou/gtxebqndma.html

Go:   // 手写循环
来源：http://hz.cqqwz.cn/gttbjoczcz.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.gzhubu.top/gtgnbfgubq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.jinqigfzy.top/gtpppylxkd.html

[D15] 去重
来源：http://hz.guowangkeji.top/gtwvzatjcz.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.ivvv.top/gtvmfvvydi.html

PHP:  array_unique($arr);
来源：http://hz.zdqjudy.top/gtgtgnuras.html

JS:   [...new Set(arr)]
来源：http://hz.dashuyun.cn/gtiqyjjuxz.html

TS:   [...new Set(arr)]
来源：http://hz.sysykeji.top/gtotmtjdgg.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.wangshuangyany.cn/gtpentbyhs.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.iojbl.cn/gtpvdosjlr.html

Ruby: arr.uniq
来源：http://hz.iojbl.cn/gtmpacgmwb.html

C#:   list.Distinct().ToList()
来源：http://hz.xuanzx.com/gtiqriynyz.html

[D16] 求和与平均值
来源：http://hz.xingfuxueyuan.xyz/gtzaxfjonw.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.shuidangran.top/gtxabhfrqi.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.xuetiantiany.cn/gtlzqyjvpx.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.smart0.xyz/gtusewswpx.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.sufxvd.cn/gtoulcapff.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.shzxlz.cn/gtjrbrbtvy.html

Go:   // 手写循环累加
来源：http://hz.birdmap.top/gtzabuagat.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.shuidangran.top/gtemhpcmnj.html

C#:   list.Sum();  list.Average()
来源：http://hz.tianlin.xyz/gtndpnooeo.html

[D17] 最大值与最小值
来源：http://hz.ehwqpu.com/gtkzxhwjds.html

Py:   max(arr);  min(arr)
来源：http://hz.c1oappe.top/gtdvyzfgbx.html

PHP:  max($arr);  min($arr);
来源：http://hz.meibo888.top/gtisxsgfqo.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.yuanzhike.top/gtwretjesb.html

TS:   Math.max(...arr);
来源：http://hz.aibaodan.cn/gtkxxtsmpk.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.ybcxt.top/gtyjqmebto.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.sweek.top/gtqfjyqfer.html

Ruby: arr.max;  arr.min
来源：http://hz.zdqjudy.top/gtngnhtcfo.html

C#:   list.Max();  list.Min()
来源：http://hz.cqqwz.cn/gthanxqelp.html

[D18] 扁平化嵌套数组
来源：http://hz.hongshengwenyu.top/gtvpnnlmff.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.hnqzz.top/gtviyxaoxo.html

PHP:  array_merge(...$nested);
来源：http://hz.snrcjt.cn/gtrgrcumwm.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.sweek.top/gtfursfhin.html

TS:   nested.flat();
来源：http://hz.haohaochexian.top/gtoeqihnxu.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.zdqjudy.top/gtxobagoaf.html

Go:   // 手写双层循环
来源：http://hz.sxryk.cn/gtzwcdjpgx.html

Ruby: nested.flatten
来源：http://hz.0kj1m.cn/gttwcjigqf.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.ehwqpu.com/gtcdocejrs.html

[D19] 按字段分组
来源：http://hz.sweek.top/gthjxhjosk.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.sweek.top/gtffzsqnjc.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.feifeiyinyue.top/gtcmiuiyup.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.hongshengwenyu.top/gtwxkwvwzg.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.havefunace.top/gthwnigxit.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.hfpthk.cn/gtajoauogs.html

Go:   // 手写 map[string][]T
来源：http://hz.xuetiantiany.cn/gtgtaogbeo.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.gotoacloud.top/gtfusimtdu.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.gogol.net.cn/gthroiihxe.html

[D20] 统计每个元素出现次数
来源：http://hz.bjfxy.top/gtgdqfzikn.html

Py:   Counter(arr)
来源：http://hz.cdnleiting.top/gtpxgkhvui.html

PHP:  array_count_values($arr);
来源：http://hz.ppjwa.cn/gtdavabtxf.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.xinyue.icu/gtiebjsqbs.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.cqqwz.cn/gtqlcaoabc.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.birdmap.top/gtqleykedy.html

Go:   // 手写 map[T]int
来源：http://hz.zhongyouzk.top/gtduypgkve.html

Ruby: arr.tally
来源：http://hz.dashuyun.cn/gtogiqxttp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.aizwys.cn/gtskopgzpz.html

[D21] 判断是否包含某元素
来源：http://hz.yvedp.cn/gtnnqrnctw.html

Py:   x in arr
来源：http://hz.hnxiangtu.top/gtdfykfrrb.html

PHP:  in_array($x, $arr, true);
来源：http://hz.chenzaomai.com/gtygfogbtx.html

JS:   arr.includes(x)
来源：http://hz.ydzc1.top/gtatwohpqj.html

TS:   arr.includes(x)
来源：http://hz.birdmap.top/gtkezpxork.html

Java: list.contains(x)
来源：http://hz.yueranfly.top/gtxxpsnmyl.html

Go:   slices.Contains(arr, x)
来源：http://hz.zdqjudy.top/gtcepmfgbv.html

Ruby: arr.include?(x)
来源：http://hz.daria6918.cn/gtxhtvhbxw.html

C#:   list.Contains(x)
来源：http://hz.guowangkeji.top/gtjbofxeqi.html

[D22] 复制数组（避免共享引用）
来源：http://hz.guowangkeji.top/gtozhpqnke.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.cashguo.top/gtwjfhhcqx.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.yueranfly.top/gtdomwdnyq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.jqgfzy.top/gtwqywmlom.html

TS:   [...arr];
来源：http://hz.zhiwuduotai.top/gtzpznrjcl.html

Java: new ArrayList<>(list);
来源：http://hz.chenjidiqi.icu/gtovkjkhky.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.zhengqikj.top/gtigcegqcf.html

Ruby: arr.dup;  arr.clone
来源：http://hz.yuanzhike.top/gtbvobuars.html

C#:   new List<int>(list);
来源：http://hz.shzxlz.cn/gtssqyfjaj.html

[D23] reduce 累积计算
来源：http://hz.fzhhl.top/gtydfgufbi.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.vqdsnc.cn/gtqrypmkzr.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.gaohongyu789.top/gtcmcdkqyg.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.hnqzz.top/gtasvvowpn.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ydzc1.top/gtarxrvmjd.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.yueranfly.top/gtpgjmnouq.html

Go:   // 手写循环
来源：http://hz.nanxuanxn.top/gtxlrrcmeu.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.shuidangran.top/gtqumkpern.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.ywan-chungtsiang.top/gtrnojxrix.html

[D24] 字典 / Map 基本操作
来源：http://hz.yonumen.top/gtdpcngazp.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.jqgufenzy.top/gtxejirxro.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.zhijiandao.cn/gteesniulm.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.zycfv.cn/gtmfhefgnz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.52xcode.cn/gtdgonkjmj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.aizwys.cn/gtsktkopbc.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.xuetiantiany.cn/gtgyzsavvn.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.dashuyun.cn/gtjfhapikp.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.mhx1999.top/gtiiaiftlb.html

[D25] Set 集合去重与交并差
来源：http://hz.52xcode.cn/gtvrekkazl.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.tianlin.xyz/gtoonabzhc.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.jinghuilouyu.cn/gtiabkiciy.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.shanyushiyangkeji.top/gtnuzqmgyz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.redwolf501.top/gtbfjxllth.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.sufxvd.cn/gtzhrplpam.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.aibaodan.cn/gtjexvjqjj.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.ivvv.top/gtxooibkcn.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.gaohongyu789.top/gthpfrbbcd.html

[D26] 数组转字符串
来源：http://hz.shzxlz.cn/gtxzgpfcod.html

Py:   ", ".join(map(str, arr))
来源：http://hz.nwbrower.top/gtybxwwuzb.html

PHP:  implode(", ", $arr);
来源：http://hz.dashuyun.cn/gtpllzjnqa.html

JS:   arr.join(", ")
来源：http://hz.ywan-chungtsiang.top/gtxfispsaz.html

TS:   arr.join(", ")
来源：http://hz.zhaomingkeji.xyz/gtyqwccgkj.html

Java: String.join(", ", list)
来源：http://hz.hysaishi.cn/gtqwdtjdoc.html

Go:   strings.Join(strs, ", ")
来源：http://hz.yj202588.top/gtudpkcljj.html

Ruby: arr.join(", ")
来源：http://hz.shanyushiyangkeji.top/gtvavdwhuf.html

C#:   string.Join(", ", list)
来源：http://hz.hfpthk.cn/gtkuxdefuv.html

================================================================================
来源：http://hz.daxiang520.top/gtlhmrupvq.html

E. 字符串处理
来源：http://hz.dashuyun.cn/gtjfnlxplw.html

================================================================================
来源：http://hz.zhoulong.xyz/gtjoorzqvn.html

[E01] 拼接字符串
来源：http://hz.zhiwuduotai.top/gttpzfpbcp.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.52xcode.cn/gtwaswyrjl.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.cashguo.top/gtpzbtmxrb.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.feifeiyinyue.top/gtwpcmzmzw.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.0kj1m.cn/gthvtuxqpg.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.quarkkingdee.top/gtweatjtwf.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.quarkkingdee.top/gtkluehkak.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.yj20258888.top/gtmezzokod.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.jqgufenzy.top/gtbkzfajbm.html

[E02] 重复字符串
来源：http://hz.feifeiyinyue.top/gtqvetrsee.html

Py:   "ab" * 3
来源：http://hz.zycfv.cn/gtrckilrdo.html

PHP:  str_repeat("ab", 3);
来源：http://hz.ydjk.org.cn/gtrivwazfx.html

JS:   "ab".repeat(3)
来源：http://hz.sysykeji.top/gtralciibf.html

TS:   "ab".repeat(3)
来源：http://hz.guowangkeji.top/gtcylerskx.html

Java: "ab".repeat(3)
来源：http://hz.jianghu66.top/gtsobiicjj.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.cdnleiting.top/gtmifkudvm.html

Ruby: "ab" * 3
来源：http://hz.yvedp.cn/gtqioxbztt.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.fengsongda.top/gtxxgkgmfs.html

[E03] 截取子串
来源：http://hz.haohaochexian.top/gtoofgpvtw.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.nwbrower.top/gtoofvwbvi.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.chenjidiqi.icu/gtadmooanm.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.vqdsnc.cn/gtdkxbiwzy.html

TS:   s.slice(1, 4)
来源：http://hz.pengpengdd.cyou/gtapftqzri.html

Java: s.substring(1, 4)
来源：http://hz.yj202588.top/gtfurzbwsy.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.hnxiangtu.top/gtpmqrldpi.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.316326.xyz/gtxyzsvdzl.html

C#:   s.Substring(1, 3)
来源：http://hz.shzxlz.cn/gtcllfjujc.html

[E04] 查找子串位置
来源：http://hz.daria6918.cn/gtjfjadqba.html

Py:   s.find("x");  s.index("x")
来源：http://hz.havefunace.top/gtupcumovo.html

PHP:  strpos($s, "x");
来源：http://hz.sysykeji.top/gtueddjlbo.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.wangdashe.top/gtcpzwzgef.html

TS:   s.indexOf("x")
来源：http://hz.daria6918.cn/gtowiponbu.html

Java: s.indexOf("x")
来源：http://hz.yangfankeji.com/gthtuptmla.html

Go:   strings.Index(s, "x")
来源：http://hz.chenjidiqi.icu/gtwqcuqnpp.html

Ruby: s.index("x")
来源：http://hz.meibo888.top/gthzusskwy.html

C#:   s.IndexOf("x")
来源：http://hz.jyoumei.cn/gtvwdtcxfy.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.ivvv.top/gtarntstjt.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.zhengqikj.top/gtydfrlokh.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.hongshengwenyu.top/gteweqkbvk.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.xziqi.cn/gtmxjamfsg.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.cheryme.top/gtdwqbmxit.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.cdnleiting.top/gtlisekhqa.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.tianlin.xyz/gtxtwnlyeu.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.wangshuangyany.cn/gtixkxsahv.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.quarkkingdee.top/gtwmxjjdnh.html

[E06] 替换子串
来源：http://hz.hammf.cn/gtvyqecluw.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.gogol.net.cn/gtfcmyxfon.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.zhijiandao.cn/gtgydgqcxu.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.fzhhl.top/gtgekbwvic.html

TS:   s.replaceAll("a", "b")
来源：http://hz.guowangkeji.top/gtfmiiboja.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.ppjwa.cn/gtgcjbggpx.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.yonumen.top/gttiduaovp.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.andypj.xyz/gtpdepgrzu.html

C#:   s.Replace("a", "b")
来源：http://hz.hnqzz.top/gtbxhfxtnl.html

[E07] 按分隔符拆分
来源：http://hz.yj20258.top/gtbsdjsnxm.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.cucudq.cn/gtsakilxdj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.nanxuanxn.top/gtxwwwgnbg.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.hfpthk.cn/gtkfefgkzs.html

TS:   s.split(",")
来源：http://hz.andypj.xyz/gtbfjzhnpn.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.hongshengwenyu.top/gtsdefqqnv.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.haohaochexian.top/gtlcvzzjvs.html

Ruby: s.split(",");  s.split
来源：http://hz.zhaomingkeji.xyz/gtgvanezwc.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.xinyue.icu/gtayccnkjh.html

[E08] 数组按分隔符合并
来源：http://hz.jiagoushi.top/gtsdftnufi.html

Py:   ",".join(items)
来源：http://hz.daxiang520.top/gtmllemlhb.html

PHP:  implode(",", $items);
来源：http://hz.yuanzhike.top/gtrpdrwqne.html

JS:   items.join(",")
来源：http://hz.wangshuangyany.cn/gtsdqcdurv.html

TS:   items.join(",")
来源：http://hz.tianlin.xyz/gtfzklpggd.html

Java: String.join(",", items)
来源：http://hz.ydjk.org.cn/gtmbcopcgk.html

Go:   strings.Join(items, ",")
来源：http://hz.jiagoushi.top/gtlznhmunk.html

Ruby: items.join(",")
来源：http://hz.zhijiandao.cn/gtocbykehl.html

C#:   string.Join(",", items)
来源：http://hz.zhoulong.xyz/gtecpppzcx.html

[E09] 去除所有空白字符
来源：http://hz.dashuyun.cn/gtkcfcvokj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.zhixingplan.top/gtmjffvghs.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.aibaodan.cn/gtuykhboye.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.nanxuanxn.top/gtqcvodzlc.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.sufxvd.cn/gtfzmcxeit.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.zhoulong.xyz/gtqujbvxhq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.zhiwuduotai.top/gttimesljm.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.sysykeji.top/gtfztlzjjo.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.jqgfzy.top/gtzivnhovn.html

[E10] 左侧补零 / 定长填充
来源：http://hz.hnqzz.top/gtypwdskti.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.jinqigfzy.top/gtxeewxblf.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.gzhubu.top/gtorxqipdc.html

JS:   "7".padStart(3, "0")
来源：http://hz.cqqwz.cn/gtjknnmxjo.html

TS:   "7".padStart(3, "0")
来源：http://hz.yj202588.top/gtyecjdens.html

Java: String.format("%03d", 7)
来源：http://hz.hongshengwenyu.top/gtzyhzrmkz.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.gzhubu.top/gtuoopfgod.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.sufxvd.cn/gtsgmelguc.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.yuxming.cn/gtioplauhu.html

[E11] 反转字符串
来源：http://hz.zhixingplan.top/gtbsrvwjei.html

Py:   s[::-1]
来源：http://hz.hnxiangtu.top/gtnprzazke.html

PHP:  strrev($s);
来源：http://hz.yj20258.top/gtarggfpkg.html

JS:   [...s].reverse().join("")
来源：http://hz.jianghu66.top/gtmkljctzo.html

TS:   [...s].reverse().join("")
来源：http://hz.dashuyun.cn/gtupgoqsia.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.shanyushiyangkeji.top/gtlwtmcfgt.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.svipenyu.cn/gtblfkbatv.html

Ruby: s.reverse
来源：http://hz.gogol.net.cn/gtopwbldir.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.wangdashe.top/gtitegsoas.html

[E12] 统计某字符出现次数
来源：http://hz.bjfxy.top/gttmrcpteu.html

Py:   s.count("a")
来源：http://hz.sweek.top/gtjecibpoc.html

PHP:  substr_count($s, "a");
来源：http://hz.hysaishi.cn/gtgmquwhus.html

JS:   s.split("a").length - 1
来源：http://hz.0kj1m.cn/gthyffqltn.html

TS:   s.split("a").length - 1
来源：http://hz.hnxiangtu.top/gtwlrrjsvo.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.sufxvd.cn/gtyyhbxxjc.html

Go:   strings.Count(s, "a")
来源：http://hz.aibaodan.cn/gtfxcgmhkp.html

Ruby: s.count("a")
来源：http://hz.gogol.net.cn/gtwrphnfcu.html

C#:   s.Count(c => c == 'a')
来源：http://hz.ehwqpu.com/gtvnbbdaxu.html

[E13] 逐字符遍历
来源：http://hz.gaohongyu789.top/gtbhczvpgb.html

Py:   for ch in s: print(ch)
来源：http://hz.hywenlv.cn/gtpjiaksem.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.aizwys.cn/gtqyvbdbph.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.feifeiyinyue.top/gtiyvadkse.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.cashguo.top/gtckayqumt.html


<!-- 参考信息 -->