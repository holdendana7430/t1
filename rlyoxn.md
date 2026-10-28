代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://hz.ydzc1.top/gthxcdxrlp.html

[D08] 合并两个数组
来源：http://hz.yuanzhike.top/gtajxhtlvz.html

Py:   a + b;  a.extend(b)
来源：http://hz.chenlongwang.top/gtkyzrmorb.html

PHP:  array_merge($a, $b);
来源：http://hz.ywan-chungtsiang.top/gtfokjsdrn.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.yangfankeji.com/gtqyzhbxyj.html

TS:   [...a, ...b];
来源：http://hz.xziqi.cn/gtlbpgqjve.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.yj202588.top/gtmuodjylf.html

Go:   append(a, b...)
来源：http://hz.tianlin.xyz/gtornasqto.html

Ruby: a + b;  a.concat(b)
来源：http://hz.xinyue.icu/gtgktzjagl.html

C#:   a.Concat(b).ToList()
来源：http://hz.ywan-chungtsiang.top/gtxpedjkkz.html

[D09] 排序（升序）
来源：http://hz.ehwqpu.com/gtdfqlriqa.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.chenlongwang.top/gtldlpepnk.html

PHP:  sort($arr);
来源：http://hz.yongpay.top/gtkvcvnxcb.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.cqqwz.cn/gtdjntkpyw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.tianlin.xyz/gtswocimsr.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.jqgufenzy.top/gtteyswvgq.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.iojbl.cn/gtgpcswpja.html

Ruby: arr.sort
来源：http://hz.haohaochexian.top/gtiasqtdqi.html

C#:   list.Sort();
来源：http://hz.hysaishi.cn/gtaoiiusgm.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.yvedp.cn/gtapzshctf.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.ydzc1.top/gtrpluihtw.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.bjfxy.top/gtctreadpb.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.ehwqpu.com/gtspucbkax.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yj202588.top/gtofostvbh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.smart0.xyz/gtcmtdhhwo.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.gzhubu.top/gttgspdxxd.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.feifeiyinyue.top/gtczgbhsto.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.andypj.xyz/gtobpcdnlx.html

[D11] 反转数组
来源：http://hz.hongshengwenyu.top/gtykayeilz.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.snrcjt.cn/gtgdicqhdk.html

PHP:  array_reverse($arr);
来源：http://hz.chenjidiqi.icu/gtseqmmqng.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.chenlongwang.top/gtgnkymdcy.html

TS:   [...arr].reverse();
来源：http://hz.hongshengwenyu.top/gtktilivor.html

Java: Collections.reverse(list);
来源：http://hz.gzhubu.top/gtduebpbgu.html

Go:   slices.Reverse(arr)
来源：http://hz.dashuyun.cn/gtatearbhf.html

Ruby: arr.reverse
来源：http://hz.wangdashe.top/gtropzeknk.html

C#:   list.Reverse();
来源：http://hz.sysykeji.top/gtwxzmzxib.html

[D12] 查找元素下标
来源：http://hz.hfpthk.cn/gtpmuyirkq.html

Py:   arr.index(x);  x in arr
来源：http://hz.shanyushiyangkeji.top/gtwdybrpfl.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.zhoulong.xyz/gtayhiklsx.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.svipenyu.cn/gtafsispbp.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jinghuilouyu.cn/gtqkvfhdyu.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.chenjidiqi.icu/gtbwovzjqy.html

Go:   slices.Index(arr, x)
来源：http://hz.feifeiyinyue.top/gtacdefpbq.html

Ruby: arr.index(x)
来源：http://hz.jqgufenzy.top/gtemarqejv.html

C#:   list.IndexOf(x);
来源：http://hz.nwbrower.top/gtedthtycx.html

[D13] 过滤（保留满足条件的）
来源：http://hz.hysaishi.cn/gttaktatmg.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.nanxuanxn.top/gtuuorevbz.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.yanxiufei.cn/gtlojxszkn.html

JS:   arr.filter(x => x > 3)
来源：http://hz.yuanzhike.top/gtmcvonykw.html

TS:   arr.filter(x => x > 3)
来源：http://hz.chenjidiqi.icu/gtjmetxlih.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.aizwys.cn/gtaxjthayl.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.wangshuangyany.cn/gtkssyrpyu.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.nanxinkj.top/gtgjujjlwc.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.jinyuanbaomall.cn/gtfyqytfrh.html

[D14] 映射转换（每个元素变形）
来源：http://hz.jinyuanbaomall.cn/gtlesvpfgs.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.meibo888.top/gtftsrhvhl.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.jinqigfzy.top/gtajlknohx.html

JS:   arr.map(x => x * 2)
来源：http://hz.ydjk.org.cn/gtuzfmbgof.html

TS:   arr.map(x => x * 2)
来源：http://hz.aizwys.cn/gtieadnbxs.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.daria6918.cn/gtyzjwezxz.html

Go:   // 手写循环
来源：http://hz.feifeiyinyue.top/gtinxouosp.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.chenzaomai.com/gtncymwlix.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.shanyushiyangkeji.top/gtjeahwfrs.html

[D15] 去重
来源：http://hz.hywenlv.cn/gtwlzdgnub.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.jqgfzy.top/gtojaianav.html

PHP:  array_unique($arr);
来源：http://hz.52xcode.cn/gtrstbdysd.html

JS:   [...new Set(arr)]
来源：http://hz.0kj1m.cn/gtqvsczabu.html

TS:   [...new Set(arr)]
来源：http://hz.pycfn.com/gtoctogskn.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.feifeiyinyue.top/gtjadwixhb.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.ehwqpu.com/gtqhpwyxhz.html

Ruby: arr.uniq
来源：http://hz.haohaochexian.top/gtvlgbprav.html

C#:   list.Distinct().ToList()
来源：http://hz.redwolf501.top/gtocmcawgk.html

[D16] 求和与平均值
来源：http://hz.fzhhl.top/gtvktywqaz.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.9152youxi.cn/gtwhsqjadk.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.hammf.cn/gthdsqdsdy.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zhongyouzk.top/gtmutvunsm.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hfpthk.cn/gtfjvtlfvp.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.guowangkeji.top/gtqcoyrwhv.html

Go:   // 手写循环累加
来源：http://hz.smart0.xyz/gtyjuzgsjf.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.cucudq.cn/gtkbjwgysb.html

C#:   list.Sum();  list.Average()
来源：http://hz.shzxlz.cn/gtqowtioqq.html

[D17] 最大值与最小值
来源：http://hz.ppjwa.cn/gtuxchqlpa.html

Py:   max(arr);  min(arr)
来源：http://hz.iojbl.cn/gtksparycy.html

PHP:  max($arr);  min($arr);
来源：http://hz.hywenlv.cn/gtutvzivyy.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.shanyushiyangtech.top/gtaooqzhhx.html

TS:   Math.max(...arr);
来源：http://hz.yueranfly.top/gtlhjnjhkw.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.yvedp.cn/gtxliohlnu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.cheryme.top/gtevzrkqck.html

Ruby: arr.max;  arr.min
来源：http://hz.zhengqikj.top/gtrpbdsckd.html

C#:   list.Max();  list.Min()
来源：http://hz.jiagoushi.top/gtbcieacnm.html

[D18] 扁平化嵌套数组
来源：http://hz.chenlongwang.top/gtilqraaib.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.yongpay.top/gtqzyxiwpd.html

PHP:  array_merge(...$nested);
来源：http://hz.redwolf501.top/gtfmwvikwu.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.zhiwuduotai.top/gthfbspmws.html

TS:   nested.flat();
来源：http://hz.cdnleiting.top/gtlkzedhsj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.shzxlz.cn/gtvniiijia.html

Go:   // 手写双层循环
来源：http://hz.ybcxt.top/gtrwxodlsm.html

Ruby: nested.flatten
来源：http://hz.9152youxi.cn/gtemsthltt.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.yangfankeji.com/gtaerkknxn.html

[D19] 按字段分组
来源：http://hz.yj20258888.top/gtakyuqqoz.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.sxryk.cn/gtlwhrpjnd.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.shangyingyoupin.top/gtcboobpnr.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.9152youxi.cn/gtzvlovyce.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.redwolf501.top/gtjwlfweut.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.yuxming.cn/gtqvafivto.html

Go:   // 手写 map[string][]T
来源：http://hz.aizwys.cn/gtsazbuqky.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.316326.xyz/gtvxzmfycu.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.gogol.net.cn/gtrwniuept.html

[D20] 统计每个元素出现次数
来源：http://hz.jqgfzy.top/gtpfnszqtd.html

Py:   Counter(arr)
来源：http://hz.ydjk.org.cn/gtpaghbdyr.html

PHP:  array_count_values($arr);
来源：http://hz.aizwys.cn/gtlaqigxol.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.fzhhl.top/gtiurjsnzx.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.52xcode.cn/gtzgluomkb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.gaohongyu789.top/gtnekdkljz.html

Go:   // 手写 map[T]int
来源：http://hz.smart0.xyz/gtdftoukoz.html

Ruby: arr.tally
来源：http://hz.ydjk.org.cn/gtfsjqjuzo.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.zhaomingkeji.xyz/gtvhxbobov.html

[D21] 判断是否包含某元素
来源：http://hz.hongshengwenyu.top/gtklcxefxs.html

Py:   x in arr
来源：http://hz.daxiang520.top/gtdzrcddvs.html

PHP:  in_array($x, $arr, true);
来源：http://hz.cheryme.top/gtafpwasbm.html

JS:   arr.includes(x)
来源：http://hz.hywenlv.cn/gtujnkewww.html

TS:   arr.includes(x)
来源：http://hz.vqdsnc.cn/gtvukiznwn.html

Java: list.contains(x)
来源：http://hz.shanyushiyangkeji.top/gtwcsvwkaz.html

Go:   slices.Contains(arr, x)
来源：http://hz.ppjwa.cn/gttflqvfbi.html

Ruby: arr.include?(x)
来源：http://hz.zhiwuduotai.top/gtybarrpkh.html

C#:   list.Contains(x)
来源：http://hz.mhx1999.top/gtcbrefybt.html

[D22] 复制数组（避免共享引用）
来源：http://hz.wangshuangyany.cn/gtrokzalxr.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.hywenlv.cn/gtdxblddpc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.hywenlv.cn/gtnurlevuy.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.aizwys.cn/gtmfejelfn.html

TS:   [...arr];
来源：http://hz.wangshuangyany.cn/gtetaikjqg.html

Java: new ArrayList<>(list);
来源：http://hz.guowangkeji.top/gtvghhtcfj.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.yvedp.cn/gtawebuhrm.html

Ruby: arr.dup;  arr.clone
来源：http://hz.bjfxy.top/gtpdjsibvm.html

C#:   new List<int>(list);
来源：http://hz.tianlin.xyz/gtffrzooje.html

[D23] reduce 累积计算
来源：http://hz.yueranfly.top/gtmdqzuuxb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.hywenlv.cn/gtyslhbvzi.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.hysaishi.cn/gtpuaytxkq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.xuetiantiany.cn/gtdntjkilw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ywan-chungtsiang.top/gtxhubffgd.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.mhx1999.top/gthvvtyqdk.html

Go:   // 手写循环
来源：http://hz.haohaochexian.top/gtbonvmfnr.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.zhaomingkeji.xyz/gtqnxdhgqi.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.aizwys.cn/gtyylvjnzf.html

[D24] 字典 / Map 基本操作
来源：http://hz.chenlongwang.top/gtrvfgonrv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.52xcode.cn/gtwwtintiy.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.9152youxi.cn/gtntcrotmv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.zhaomingkeji.xyz/gtskanqude.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.jlsjyb.cn/gtvldebncc.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.jlsjyb.cn/gtvtwqtxpv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.yvedp.cn/gtwacjetil.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.cdnleiting.top/gtaprcdbmc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.chenlongwang.top/gtdcangzpk.html

[D25] Set 集合去重与交并差
来源：http://hz.shzxlz.cn/gtwhbbxwmm.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.9152youxi.cn/gtsxgzgvbj.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.nanxuanxn.top/gtcrzjamro.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.tian-w.cn/gtubolateg.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.yuxming.cn/gtdqzykgvq.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.shanyushiyangkeji.top/gtwhiqpeie.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.jlsjyb.cn/gtoepibmmj.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.shangyingyoupin.top/gtvngqrejj.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.cdnleiting.top/gtjqdnubvc.html

[D26] 数组转字符串
来源：http://hz.tian-w.cn/gtmmzdcqnj.html

Py:   ", ".join(map(str, arr))
来源：http://hz.zycfv.cn/gtjphrhmvo.html

PHP:  implode(", ", $arr);
来源：http://hz.hammf.cn/gtqcpgmbnx.html

JS:   arr.join(", ")
来源：http://hz.yongpay.top/gtyvbpmuqr.html

TS:   arr.join(", ")
来源：http://hz.wangshuangyany.cn/gttryzvdgg.html

Java: String.join(", ", list)
来源：http://hz.daria6918.cn/gtbpzgcfhs.html

Go:   strings.Join(strs, ", ")
来源：http://hz.yj20258.top/gtllcihryt.html

Ruby: arr.join(", ")
来源：http://hz.gotoacloud.top/gtejfitplh.html

C#:   string.Join(", ", list)
来源：http://hz.zdqjudy.top/gtrdhjsiwb.html

================================================================================
来源：http://hz.yj202588.top/gtemdslhmh.html

E. 字符串处理
来源：http://hz.chenzaomai.com/gtklevopqh.html

================================================================================
来源：http://hz.cdnleiting.top/gtjfbdadwj.html

[E01] 拼接字符串
来源：http://hz.0kj1m.cn/gtfcumjeqn.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.zhijiandao.cn/gtexalsqod.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.hnxiangtu.top/gtxriptpsq.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zhongyouzk.top/gtxpacozuk.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zdqjudy.top/gttbxmdqgg.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.nanxuanxn.top/gtuteblsyq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.andypj.xyz/gtguftplfe.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.ehwqpu.com/gtnopoupfo.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.aibaodan.cn/gtveldlpbe.html

[E02] 重复字符串
来源：http://hz.zhongyouzk.top/gtxbryepfu.html

Py:   "ab" * 3
来源：http://hz.gogol.net.cn/gtorsuxgks.html

PHP:  str_repeat("ab", 3);
来源：http://hz.gogol.net.cn/gtzaeikrzx.html

JS:   "ab".repeat(3)
来源：http://hz.jinqigufen.top/gtgtkhsnpq.html

TS:   "ab".repeat(3)
来源：http://hz.yueranfly.top/gttgdeqlvy.html

Java: "ab".repeat(3)
来源：http://hz.daxiang520.top/gtxhpjqygc.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.gaohongyu789.top/gtwqwjpxza.html

Ruby: "ab" * 3
来源：http://hz.cdnleiting.top/gtfncktujz.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.xziqi.cn/gtygdprdys.html

[E03] 截取子串
来源：http://hz.daria6918.cn/gtypztbigr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.gotoacloud.top/gtvbwttkop.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.nwbrower.top/gtajsnridi.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.svipenyu.cn/gtmtnnbrum.html

TS:   s.slice(1, 4)
来源：http://hz.mhx1999.top/gtxzqgoxkk.html

Java: s.substring(1, 4)
来源：http://hz.guowangkeji.top/gtxzwwzvhm.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.hammf.cn/gtrfrqyikj.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.redwolf501.top/gtubsjttam.html

C#:   s.Substring(1, 3)
来源：http://hz.gotoacloud.top/gtdmowqwob.html

[E04] 查找子串位置
来源：http://hz.yvedp.cn/gtdxinzelx.html

Py:   s.find("x");  s.index("x")
来源：http://hz.ydjk.org.cn/gtacefjley.html

PHP:  strpos($s, "x");
来源：http://hz.jianghu66.top/gtixvldcpo.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.daxiang520.top/gtcmznnpnz.html

TS:   s.indexOf("x")
来源：http://hz.hammf.cn/gtgqrgpjqe.html

Java: s.indexOf("x")
来源：http://hz.zhongyouzk.top/gtszhimudq.html

Go:   strings.Index(s, "x")
来源：http://hz.zhongyouzk.top/gtmvktpxpz.html

Ruby: s.index("x")
来源：http://hz.vqdsnc.cn/gtonakkzmo.html

C#:   s.IndexOf("x")
来源：http://hz.jyoumei.cn/gtwdwufmrv.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.yvedp.cn/gtcxmdeccf.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.yj20258888.top/gtphujekos.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.wangdashe.top/gtwyiokhgt.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.sufxvd.cn/gtzxmdupue.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.quarkkingdee.top/gtjaecycrj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.haohaochexian.top/gtrwvvoicd.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.smart0.xyz/gtalfvzhpe.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.daria6918.cn/gtyosveohl.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.snrcjt.cn/gtyknlbnat.html

[E06] 替换子串
来源：http://hz.shanyushiyangtech.top/gthemqeoeg.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.hywenlv.cn/gtwmzdsccw.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.sufxvd.cn/gtnhjpyuvz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yj202588.top/gtxbmzcscv.html

TS:   s.replaceAll("a", "b")
来源：http://hz.zhaomingkeji.xyz/gtnazshkjf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.bjfxy.top/gtmfugjobm.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.sweek.top/gtnwkbvtgk.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.xingfuxueyuan.xyz/gtfpykakap.html

C#:   s.Replace("a", "b")
来源：http://hz.vqdsnc.cn/gtaoquuztg.html

[E07] 按分隔符拆分
来源：http://hz.yonumen.top/gtepvmxcre.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.birdmap.top/gtqqyrkegt.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.shzxlz.cn/gtxjlosgxy.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.zycfv.cn/gtwsalwgpb.html

TS:   s.split(",")
来源：http://hz.xinyue.icu/gtviziujsn.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.daxiang520.top/gtgvmnmuso.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.haohaochexian.top/gtlrmdlbvh.html

Ruby: s.split(",");  s.split
来源：http://hz.zhijiandao.cn/gtxeqkyjwz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.316326.xyz/gtddugpsjh.html

[E08] 数组按分隔符合并
来源：http://hz.zhoulong.xyz/gtblzpuqnz.html

Py:   ",".join(items)
来源：http://hz.hysaishi.cn/gtndakaqri.html

PHP:  implode(",", $items);
来源：http://hz.cashguo.top/gtvrvyfyan.html

JS:   items.join(",")
来源：http://hz.meibo888.top/gtofuubisj.html

TS:   items.join(",")
来源：http://hz.yj20258.top/gtxhbxvmqj.html

Java: String.join(",", items)
来源：http://hz.ybcxt.top/gtriaecbly.html

Go:   strings.Join(items, ",")
来源：http://hz.zhixingplan.top/gteqhpmebq.html

Ruby: items.join(",")
来源：http://hz.svipenyu.cn/gttnhneduz.html

C#:   string.Join(",", items)
来源：http://hz.xziqi.cn/gtrjrfuyhm.html

[E09] 去除所有空白字符
来源：http://hz.bjfxy.top/gtgafbkhyo.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.bjfxy.top/gtmezbcymr.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.guannengcc.top/gthofyzvlp.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.aibaodan.cn/gtszqbdhdq.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.havefunace.top/gthqzjikts.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.jqgfzy.top/gtsisqfkoh.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.sweek.top/gthikiydjj.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.cashguo.top/gtntsrlwsj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.cqqwz.cn/gtjlrzxjol.html

[E10] 左侧补零 / 定长填充
来源：http://hz.jinyuanbaomall.cn/gtiyoouzug.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.redwolf501.top/gttelpavtl.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.cqqwz.cn/gtnsksnhxv.html

JS:   "7".padStart(3, "0")
来源：http://hz.daxiang520.top/gtwhwmjcdj.html

TS:   "7".padStart(3, "0")
来源：http://hz.sysykeji.top/gteaukuasg.html

Java: String.format("%03d", 7)
来源：http://hz.haohaochexian.top/gtpdmkhyfj.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.iojbl.cn/gthcqwqoxt.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.fengsongda.top/gtwwsgkbxr.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.yvedp.cn/gtynymbolx.html

[E11] 反转字符串
来源：http://hz.aibaodan.cn/gtupbtczeq.html

Py:   s[::-1]
来源：http://hz.xylfe.cn/gtvbglrosg.html

PHP:  strrev($s);
来源：http://hz.zhaomingkeji.xyz/gtmnqbznyh.html

JS:   [...s].reverse().join("")
来源：http://hz.52xcode.cn/gtrsauuxnk.html

TS:   [...s].reverse().join("")
来源：http://hz.jinqigfzy.top/gtearrygsc.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.cheryme.top/gtgtaprkkz.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.yuxming.cn/gtpzjccqac.html

Ruby: s.reverse
来源：http://hz.jiagoushi.top/gtksfwtuao.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.cheryme.top/gtfoukaacb.html

[E12] 统计某字符出现次数
来源：http://hz.zhengqikj.top/gtuxumyolk.html

Py:   s.count("a")
来源：http://hz.bjfxy.top/gtjvzqagba.html

PHP:  substr_count($s, "a");
来源：http://hz.yj202588.top/gtjqykbmha.html

JS:   s.split("a").length - 1
来源：http://hz.cashguo.top/gtvtbttvba.html

TS:   s.split("a").length - 1
来源：http://hz.jqgfzy.top/gtuzeejjud.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.mhx1999.top/gtgqvedphx.html

Go:   strings.Count(s, "a")
来源：http://hz.ydzc1.top/gtqretcaxx.html

Ruby: s.count("a")
来源：http://hz.redwolf501.top/gtjhwdpsdq.html

C#:   s.Count(c => c == 'a')
来源：http://hz.iojbl.cn/gtrptaysms.html

[E13] 逐字符遍历
来源：http://hz.cdnleiting.top/gtydcurxma.html

Py:   for ch in s: print(ch)
来源：http://hz.yangfankeji.com/gtddjtasbc.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.zhoulong.xyz/gtroeihdxv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xingfuxueyuan.xyz/gttqmwrhii.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.shzxlz.cn/gtfpewghux.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.shzxlz.cn/gtbzzngzbq.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.ydjk.org.cn/gtacltvacm.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.yongpay.top/gtcpsrapfl.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.shuidangran.top/gtuyundowe.html

[E14] URL 编码与 Base64
来源：http://hz.nanxuanxn.top/gteushstbj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.hnqzz.top/gtzluhxocr.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.sysykeji.top/gtrlxwykge.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.iojbl.cn/gtwweepnev.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.yangfankeji.com/gtwlltcebf.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.haohaochexian.top/gtgrmwfoeu.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.jqgufenzy.top/gtrhqyuhwe.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.hysaishi.cn/gtprpsuobj.html


<!-- 参考信息 -->