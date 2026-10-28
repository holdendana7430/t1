代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.xinyue.icu/gtsrevhufz.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.xylfe.cn/gthqbbzhog.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.dianchejie.cn/gtwnpqrjpv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zhijiandao.cn/gtwqrgfexq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.tanke756.top/gtqkropsdb.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.yueranfly.top/gttfdaxqsx.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.yuanzhike.top/gtyvmgzzud.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.feifeiyinyue.top/gtstyzlale.html

[D11] 反转数组
来源：http://hz.c1oappe.top/gtchdreqqf.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.iojbl.cn/gtcyzwzyel.html

PHP:  array_reverse($arr);
来源：http://hz.dianchejie.cn/gtlpwjwcwf.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.ydjk.org.cn/gtlxqzadql.html

TS:   [...arr].reverse();
来源：http://hz.wangdashe.top/gthyoizygk.html

Java: Collections.reverse(list);
来源：http://hz.hnxiangtu.top/gtylywdkby.html

Go:   slices.Reverse(arr)
来源：http://hz.xuetiantiany.cn/gtplwngjxj.html

Ruby: arr.reverse
来源：http://hz.jinqigufen.top/gtxlyokkpt.html

C#:   list.Reverse();
来源：http://hz.52xcode.cn/gtohptynwx.html

[D12] 查找元素下标
来源：http://hz.zhixingplan.top/gtdzbucsnt.html

Py:   arr.index(x);  x in arr
来源：http://hz.yj202588.top/gtplprcnzg.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.sweek.top/gtouxcdrdi.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.0kj1m.cn/gtdxynkabb.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.feifeiyinyue.top/gtawiqkczv.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.yj20258888.top/gtolxuidzd.html

Go:   slices.Index(arr, x)
来源：http://hz.yanxiufei.cn/gtxbtsglgg.html

Ruby: arr.index(x)
来源：http://hz.chenjidiqi.icu/gtvwdntmpr.html

C#:   list.IndexOf(x);
来源：http://hz.zhaomingkeji.xyz/gtafiaxanb.html

[D13] 过滤（保留满足条件的）
来源：http://hz.gogol.net.cn/gtwlguzrkb.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.hnqzz.top/gtdimsidjo.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.jqgufenzy.top/gtvymyovjz.html

JS:   arr.filter(x => x > 3)
来源：http://hz.guowangkeji.top/gtlkedfxzx.html

TS:   arr.filter(x => x > 3)
来源：http://hz.daria6918.cn/gtrjwgciba.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.yangfankeji.com/gtnacbxngt.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.ydjk.org.cn/gtnvhsynxn.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.quarkkingdee.top/gtcamlwhex.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.0kj1m.cn/gtnrrvzqub.html

[D14] 映射转换（每个元素变形）
来源：http://hz.bjfxy.top/gtbnntpvum.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.iojbl.cn/gtvlcvhdnb.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.0kj1m.cn/gthpnrfylq.html

JS:   arr.map(x => x * 2)
来源：http://hz.shzxlz.cn/gtsthvyodr.html

TS:   arr.map(x => x * 2)
来源：http://hz.andypj.xyz/gtimkgfjwu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.gzhubu.top/gtwjrlndmw.html

Go:   // 手写循环
来源：http://hz.zhixingplan.top/gtogtpybtq.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.chenlongwang.top/gtjxzpxxuy.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.jiagoushi.top/gtpfuohxrj.html

[D15] 去重
来源：http://hz.gaohongyu789.top/gtrypnzigc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.sufxvd.cn/gtgwiuwkow.html

PHP:  array_unique($arr);
来源：http://hz.yongpay.top/gtidlvdkss.html

JS:   [...new Set(arr)]
来源：http://hz.aibaodan.cn/gtlmfnophz.html

TS:   [...new Set(arr)]
来源：http://hz.jlsjyb.cn/gtddhsmcfs.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.cashguo.top/gtekxwmdzg.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.yj20258.top/gtiunghmaj.html

Ruby: arr.uniq
来源：http://hz.zhoulong.xyz/gtusnuwsdc.html

C#:   list.Distinct().ToList()
来源：http://hz.birdmap.top/gtejppyyvj.html

[D16] 求和与平均值
来源：http://hz.gotoacloud.top/gtjmfresvy.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.cashguo.top/gtnhivrgfi.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.316326.xyz/gtygupuesj.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hysaishi.cn/gtmjkeuagp.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zhengqikj.top/gttcpneomc.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.haohaochexian.top/gtmbrhxtsu.html

Go:   // 手写循环累加
来源：http://hz.jqgfzy.top/gtudslabyw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.hfpthk.cn/gttylafrrz.html

C#:   list.Sum();  list.Average()
来源：http://hz.yuxming.cn/gtqiuaqldy.html

[D17] 最大值与最小值
来源：http://hz.cdnleiting.top/gteaaihqyj.html

Py:   max(arr);  min(arr)
来源：http://hz.sysykeji.top/gtlwegmcsn.html

PHP:  max($arr);  min($arr);
来源：http://hz.quarkkingdee.top/gtgdikbrfv.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.tian-w.cn/gtlhfzamlw.html

TS:   Math.max(...arr);
来源：http://hz.redwolf501.top/gtzkrfxhjo.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.tianlin.xyz/gtfuimlrza.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.smart0.xyz/gtdeiwjzhh.html

Ruby: arr.max;  arr.min
来源：http://hz.ywan-chungtsiang.top/gtrceyedfp.html

C#:   list.Max();  list.Min()
来源：http://hz.ppjwa.cn/gtqnnpcjbj.html

[D18] 扁平化嵌套数组
来源：http://hz.iojbl.cn/gtywmxscnt.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.zhiwuduotai.top/gtmpwttrdw.html

PHP:  array_merge(...$nested);
来源：http://hz.yongpay.top/gtxnppibmu.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.yanxiufei.cn/gtaqgysmuu.html

TS:   nested.flat();
来源：http://hz.yonumen.top/gtclbygykp.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.daxiang520.top/gtbsnwnlld.html

Go:   // 手写双层循环
来源：http://hz.gotoacloud.top/gtiofmjkvk.html

Ruby: nested.flatten
来源：http://hz.hammf.cn/gtajbwtdgg.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.zhongyouzk.top/gthdbdxngu.html

[D19] 按字段分组
来源：http://hz.ydzc1.top/gtwvzoiyff.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.zhoulong.xyz/gthnujjnrv.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.wangdashe.top/gtdiuttmvg.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.jianghu66.top/gtnxxtvzyx.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.snrcjt.cn/gttaenuhyn.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.hywenlv.cn/gtqspjvfuk.html

Go:   // 手写 map[string][]T
来源：http://hz.cucudq.cn/gtwospahnh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.yanxiufei.cn/gtzkbrcygx.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.snrcjt.cn/gtpccdaugg.html

[D20] 统计每个元素出现次数
来源：http://hz.jinghuilouyu.cn/gtxpvxgsis.html

Py:   Counter(arr)
来源：http://hz.tianlin.xyz/gtexldigse.html

PHP:  array_count_values($arr);
来源：http://hz.hongshengwenyu.top/gtbozatnme.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.shangyingyoupin.top/gtnqaojltm.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jinqigufen.top/gtzawrmdul.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.yj202588.top/gtacdiyitn.html

Go:   // 手写 map[T]int
来源：http://hz.52xcode.cn/gthsclfpgb.html

Ruby: arr.tally
来源：http://hz.shzxlz.cn/gtmpziqmea.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.guowangkeji.top/gtrgtdnlok.html

[D21] 判断是否包含某元素
来源：http://hz.nanxuanxn.top/gtwtkitqhv.html

Py:   x in arr
来源：http://hz.chenzaomai.com/gtnswimnvr.html

PHP:  in_array($x, $arr, true);
来源：http://hz.jqgfzy.top/gtjnqcsupc.html

JS:   arr.includes(x)
来源：http://hz.gaohongyu789.top/gtuqrkbuxb.html

TS:   arr.includes(x)
来源：http://hz.zhiwuduotai.top/gtfhxizzft.html

Java: list.contains(x)
来源：http://hz.zhijiandao.cn/gtrblhjgrw.html

Go:   slices.Contains(arr, x)
来源：http://hz.yvedp.cn/gtrybuivak.html

Ruby: arr.include?(x)
来源：http://hz.gzhubu.top/gtiqxxnymb.html

C#:   list.Contains(x)
来源：http://hz.yongpay.top/gtjnfnkkkc.html

[D22] 复制数组（避免共享引用）
来源：http://hz.cqqwz.cn/gtpfjyhbam.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.sxryk.cn/gtwlmxqcfq.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.aibaodan.cn/gthzkghrkd.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.ppjwa.cn/gtoxkpgexs.html

TS:   [...arr];
来源：http://hz.daxiang520.top/gtjnzrjamf.html

Java: new ArrayList<>(list);
来源：http://hz.guowangkeji.top/gtijxwhcdp.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.yanxiufei.cn/gtbbhymdcp.html

Ruby: arr.dup;  arr.clone
来源：http://hz.smart0.xyz/gtixfjsbgn.html

C#:   new List<int>(list);
来源：http://hz.jlsjyb.cn/gtmfxooibg.html

[D23] reduce 累积计算
来源：http://hz.yj202588.top/gtpipwqscq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.hnqzz.top/gtksvzjujs.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.yvedp.cn/gtltmxhvce.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jiagoushi.top/gtmmfjpdnv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.haohaochexian.top/gtgntokyez.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.xingfuxueyuan.xyz/gtibpuwhqb.html

Go:   // 手写循环
来源：http://hz.gaohongyu789.top/gtzdbigdmt.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.kuanghao11.cn/gtyqygsaap.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.tianlin.xyz/gtvhmibqqn.html

[D24] 字典 / Map 基本操作
来源：http://hz.pengpengdd.cyou/gtkggouuer.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.jiagoushi.top/gtmjyofdyo.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.yangfankeji.com/gtvfvyxuaw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.dianchejie.cn/gtefmsutdi.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.cqqwz.cn/gtfpdortmg.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.xingfuxueyuan.xyz/gtjkluqpqi.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.hysaishi.cn/gtrclqcvgu.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.zhiwuduotai.top/gthqghdfon.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.sufxvd.cn/gtppfyccyz.html

[D25] Set 集合去重与交并差
来源：http://hz.cdnleiting.top/gtpfkdfcve.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.hysaishi.cn/gtfxhqnuee.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.gaohongyu789.top/gtdqcrkuqo.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.pycfn.com/gtzxrlgupv.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.smart0.xyz/gtwmqjqtmu.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.redwolf501.top/gtivaovoph.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.zdqjudy.top/gtvxpwdehp.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.shanyushiyangkeji.top/gtvkgvesve.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.feifeiyinyue.top/gtirlwbzwd.html

[D26] 数组转字符串
来源：http://hz.jinyuanbaomall.cn/gtahrtxhef.html

Py:   ", ".join(map(str, arr))
来源：http://hz.hammf.cn/gtokrflirx.html

PHP:  implode(", ", $arr);
来源：http://hz.ehwqpu.com/gtbkaxownd.html

JS:   arr.join(", ")
来源：http://hz.hfpthk.cn/gtfntjwbtp.html

TS:   arr.join(", ")
来源：http://hz.jinqigfzy.top/gtwyigzrgf.html

Java: String.join(", ", list)
来源：http://hz.iojbl.cn/gtwvsmcyqq.html

Go:   strings.Join(strs, ", ")
来源：http://hz.smart0.xyz/gtuongmpgj.html

Ruby: arr.join(", ")
来源：http://hz.dashuyun.cn/gtrrqycize.html

C#:   string.Join(", ", list)
来源：http://hz.zhengqikj.top/gtfgdnvnog.html

================================================================================
来源：http://hz.xinyue.icu/gtzzzigadp.html

E. 字符串处理
来源：http://hz.yvedp.cn/gtbwxrrcgn.html

================================================================================
来源：http://hz.yj20258.top/gttmbcnafv.html

[E01] 拼接字符串
来源：http://hz.quarkkingdee.top/gthrnyezpt.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.jqgufenzy.top/gtzxmrdftr.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.daxiang520.top/gtxenotfaf.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.wangshuangyany.cn/gtystlcoiz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jqgufenzy.top/gtxldffjuw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.hysaishi.cn/gtowlnclbz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.jinqigufen.top/gtcuyuxbvr.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.sysykeji.top/gtztpczaiv.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.jlsjyb.cn/gtdcnxbwsz.html

[E02] 重复字符串
来源：http://hz.feifeiyinyue.top/gtfpmackbt.html

Py:   "ab" * 3
来源：http://hz.yuanzhike.top/gtjwkuqzbc.html

PHP:  str_repeat("ab", 3);
来源：http://hz.sysykeji.top/gtdwpfxlnd.html

JS:   "ab".repeat(3)
来源：http://hz.nanxuanxn.top/gtziakhdgi.html

TS:   "ab".repeat(3)
来源：http://hz.cucudq.cn/gthlddechn.html

Java: "ab".repeat(3)
来源：http://hz.jyoumei.cn/gtffmdoevw.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.andypj.xyz/gtxxkrajcp.html

Ruby: "ab" * 3
来源：http://hz.snrcjt.cn/gtempbbxua.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.ybcxt.top/gtsldnjbvc.html

[E03] 截取子串
来源：http://hz.pycfn.com/gtqacvdksd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.ehwqpu.com/gttblepqfu.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.wangdashe.top/gtlfmhsbnr.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.vqdsnc.cn/gtzcmhqvwe.html

TS:   s.slice(1, 4)
来源：http://hz.zycfv.cn/gtmpqgjxvs.html

Java: s.substring(1, 4)
来源：http://hz.xylfe.cn/gtmbbsfuhx.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.nwbrower.top/gtmrqgmkob.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.jinyuanbaomall.cn/gthtuowslv.html

C#:   s.Substring(1, 3)
来源：http://hz.yueranfly.top/gtzjksbgss.html

[E04] 查找子串位置
来源：http://hz.yangfankeji.com/gtopzvwsln.html

Py:   s.find("x");  s.index("x")
来源：http://hz.cdnleiting.top/gtvgnujnwe.html

PHP:  strpos($s, "x");
来源：http://hz.yvedp.cn/gtujwjxtbl.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.fzhhl.top/gtsfpxqjat.html

TS:   s.indexOf("x")
来源：http://hz.ywan-chungtsiang.top/gtiosqeyjr.html

Java: s.indexOf("x")
来源：http://hz.tanke756.top/gthtoitjts.html

Go:   strings.Index(s, "x")
来源：http://hz.ydzc1.top/gtfaxtclum.html

Ruby: s.index("x")
来源：http://hz.feifeiyinyue.top/gtjxawzbal.html

C#:   s.IndexOf("x")
来源：http://hz.yj202588.top/gtkibbxtgk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.sysykeji.top/gtzfxywqvs.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.shuidangran.top/gtufvuvrmc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.cucudq.cn/gttzwdbzyb.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jinqigufen.top/gtbqlkscde.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.xylfe.cn/gtphxdaftk.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.nwbrower.top/gtiztddpea.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.xuetiantiany.cn/gtdhonjtjf.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.shanyushiyangkeji.top/gtblpnclhp.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.yongpay.top/gtklwerhmg.html

[E06] 替换子串
来源：http://hz.iojbl.cn/gtgpcfybjn.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.jqgufenzy.top/gtvylecpju.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.shzxlz.cn/gtuzjudsdn.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jiagoushi.top/gthuxdcxwp.html

TS:   s.replaceAll("a", "b")
来源：http://hz.yonumen.top/gtlqkuaupb.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.vqdsnc.cn/gtqofhwviu.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.316326.xyz/gtoxbtzpdn.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.jinqigufen.top/gtlwvggctp.html

C#:   s.Replace("a", "b")
来源：http://hz.0kj1m.cn/gtmyxnvjfb.html

[E07] 按分隔符拆分
来源：http://hz.jlsjyb.cn/gtvwkuwhdv.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.shzxlz.cn/gtjnczesic.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.jyoumei.cn/gtliflpbeg.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.zhongyouzk.top/gtpevqjdcj.html

TS:   s.split(",")
来源：http://hz.kuanghao11.cn/gtdxqarigq.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.smart0.xyz/gtaitstgct.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.ehwqpu.com/gtycrcmemv.html

Ruby: s.split(",");  s.split
来源：http://hz.gaohongyu789.top/gtjbczfjte.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.jiagoushi.top/gtzvutpstf.html

[E08] 数组按分隔符合并
来源：http://hz.guowangkeji.top/gteojakjfh.html

Py:   ",".join(items)
来源：http://hz.nanxinkj.top/gtsvwbqabj.html

PHP:  implode(",", $items);
来源：http://hz.tanke756.top/gtcvgpxrqa.html

JS:   items.join(",")
来源：http://hz.snrcjt.cn/gtwyfhzqwp.html

TS:   items.join(",")
来源：http://hz.yj202588.top/gtibytwdog.html

Java: String.join(",", items)
来源：http://hz.hongshengwenyu.top/gtnblemnlo.html

Go:   strings.Join(items, ",")
来源：http://hz.shanyushiyangtech.top/gtgczsehsi.html

Ruby: items.join(",")
来源：http://hz.hnqzz.top/gtdrxknyuv.html

C#:   string.Join(",", items)
来源：http://hz.52xcode.cn/gtlxdfxicv.html

[E09] 去除所有空白字符
来源：http://hz.nwbrower.top/gtyleprdyk.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.ydzc1.top/gtekjqmbxa.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.pengpengdd.cyou/gtyrohnkuv.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.quarkkingdee.top/gtthpjstzt.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.yangfankeji.com/gtytjtjlzc.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.yueranfly.top/gtwtysiifs.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.yj20258.top/gtaynodjll.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.chenlongwang.top/gtauuadhsf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.nanxinkj.top/gtaihijhtz.html

[E10] 左侧补零 / 定长填充
来源：http://hz.ivvv.top/gtrajmvhts.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.jqgfzy.top/gtvkxksulm.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.shangyingyoupin.top/gtjydmbbms.html

JS:   "7".padStart(3, "0")
来源：http://hz.mhx1999.top/gtkbwnfpht.html

TS:   "7".padStart(3, "0")
来源：http://hz.pengpengdd.cyou/gthvcwkqby.html

Java: String.format("%03d", 7)
来源：http://hz.aizwys.cn/gthwnggvni.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.vqdsnc.cn/gtewpfyohp.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.fzhhl.top/gthabqhfhu.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.yuanzhike.top/gtvkkvnsde.html

[E11] 反转字符串
来源：http://hz.fzhhl.top/gtxukafbos.html

Py:   s[::-1]
来源：http://hz.ydjk.org.cn/gttxbwixwa.html

PHP:  strrev($s);
来源：http://hz.yvedp.cn/gtzwrcxxnw.html

JS:   [...s].reverse().join("")
来源：http://hz.shangyingyoupin.top/gtxwyakdqo.html

TS:   [...s].reverse().join("")
来源：http://hz.9152youxi.cn/gtwcnfggxl.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.svipenyu.cn/gtpfqkwmjd.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.ydjk.org.cn/gtnxfknqpf.html

Ruby: s.reverse
来源：http://hz.guowangkeji.top/gtmuvdpplj.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.dianchejie.cn/gtmnjratre.html

[E12] 统计某字符出现次数
来源：http://hz.chenjidiqi.icu/gtgtifmxds.html

Py:   s.count("a")
来源：http://hz.jinyuanbaomall.cn/gteqclamvz.html

PHP:  substr_count($s, "a");
来源：http://hz.tianlin.xyz/gtwxjbuhbf.html

JS:   s.split("a").length - 1
来源：http://hz.nwbrower.top/gttzagplwf.html

TS:   s.split("a").length - 1
来源：http://hz.tianlin.xyz/gtayzzgayr.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.zhongyouzk.top/gtekbqflqh.html

Go:   strings.Count(s, "a")
来源：http://hz.yanxiufei.cn/gtsbokucap.html

Ruby: s.count("a")
来源：http://hz.yangfankeji.com/gtthdggaoq.html

C#:   s.Count(c => c == 'a')
来源：http://hz.pycfn.com/gtxxsviboc.html

[E13] 逐字符遍历
来源：http://hz.hfpthk.cn/gtvkvghlzg.html

Py:   for ch in s: print(ch)
来源：http://hz.cdnleiting.top/gtulqzzebc.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.cheryme.top/gtnpmmkhlo.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xingfuxueyuan.xyz/gtkctmydnh.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.9152youxi.cn/gtxqsuymcm.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.ydjk.org.cn/gtjpknwbgi.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.guowangkeji.top/gtpkyyzblq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.ydzc1.top/gtvnqvamlu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.xingfuxueyuan.xyz/gtuibzxlwx.html

[E14] URL 编码与 Base64
来源：http://hz.jinqigfzy.top/gtkshmwxwr.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.dianchejie.cn/gthzrenuoq.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.aizwys.cn/gtnhkooxss.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.fzhhl.top/gtzlsmbpsa.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.hywenlv.cn/gtmrzcwvzx.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.haohaochexian.top/gtzuwgvecn.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.yuxming.cn/gtewmczkqy.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.shuidangran.top/gtksrbeddm.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.tianlin.xyz/gtrjschobo.html

[E15] HTML 转义 / 反转义
来源：http://hz.hfpthk.cn/gtltnouwpm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.cdnleiting.top/gtpztijhlj.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.xylfe.cn/gtowhkowvt.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.mhx1999.top/gtzgivjisq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.xuanzx.com/gtygwggzkl.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.hongshengwenyu.top/gtiaglnteu.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.chenzaomai.com/gtbrczqenl.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.jianghu66.top/gtybdvjnmf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.dashuyun.cn/gtcipysxbb.html

[E16] 数字千分位
来源：http://hz.0kj1m.cn/gtjuhasmuz.html

Py:   f"{1234567:,}"
来源：http://hz.yj202588.top/gtidwijhtd.html

PHP:  number_format(1234567);
来源：http://hz.jinghuilouyu.cn/gtvaktorbb.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.0kj1m.cn/gtoaeaxflo.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.zhixingplan.top/gtwtjpreyp.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.quarkkingdee.top/gtwzrtjjgn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.jianghu66.top/gteriodgse.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.chenjidiqi.icu/gtbdseqqua.html

C#:   1234567.ToString("N0")
来源：http://hz.dashuyun.cn/gtudwycjxf.html

[E17] 首字母大写
来源：http://hz.yj20258888.top/gtpangslbf.html


<!-- 参考信息 -->