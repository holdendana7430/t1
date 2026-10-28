代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://hz.svipenyu.cn/gtpbnmwyue.html

[D08] 合并两个数组
来源：http://hz.zhiwuduotai.top/gtlswxyyag.html

Py:   a + b;  a.extend(b)
来源：http://hz.316326.xyz/gtfkqvgykm.html

PHP:  array_merge($a, $b);
来源：http://hz.yuxming.cn/gttvcjxetw.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.cashguo.top/gtmjfvdaii.html

TS:   [...a, ...b];
来源：http://hz.andypj.xyz/gtslmhqqmi.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.dashuyun.cn/gteqlhmnnt.html

Go:   append(a, b...)
来源：http://hz.snrcjt.cn/gtarwahyyp.html

Ruby: a + b;  a.concat(b)
来源：http://hz.haohaochexian.top/gtoilcxczy.html

C#:   a.Concat(b).ToList()
来源：http://hz.havefunace.top/gtlarecnyt.html

[D09] 排序（升序）
来源：http://hz.hywenlv.cn/gtbewtxadq.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.gotoacloud.top/gtnwrxjvqx.html

PHP:  sort($arr);
来源：http://hz.zhijiandao.cn/gttpmsdfym.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.xziqi.cn/gtrmhzlogs.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.fzhhl.top/gtbblkedas.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.shanyushiyangkeji.top/gtsbruhhuk.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.shuidangran.top/gtlgjwatyj.html

Ruby: arr.sort
来源：http://hz.ywan-chungtsiang.top/gteflerbzp.html

C#:   list.Sort();
来源：http://hz.sxryk.cn/gtqfajvnxa.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.xingfuxueyuan.xyz/gtrlfbnxxp.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.hammf.cn/gtbnsoertr.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.guannengcc.top/gtyinpisof.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.cheryme.top/gteobedslx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hysaishi.cn/gtaqbsekxj.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.jiagoushi.top/gtkemtgnng.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.xziqi.cn/gtfbcsntsl.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.nanxinkj.top/gtnyhjylro.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.0kj1m.cn/gtvwtxnxsf.html

[D11] 反转数组
来源：http://hz.c1oappe.top/gtkrhtyjbc.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.ydzc1.top/gtnqfqnbzk.html

PHP:  array_reverse($arr);
来源：http://hz.yanxiufei.cn/gtrzlplckw.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.guannengcc.top/gtokxsdbib.html

TS:   [...arr].reverse();
来源：http://hz.gzhubu.top/gtkhumnnfl.html

Java: Collections.reverse(list);
来源：http://hz.xinyue.icu/gtflauwuuz.html

Go:   slices.Reverse(arr)
来源：http://hz.birdmap.top/gtgitjlmup.html

Ruby: arr.reverse
来源：http://hz.daria6918.cn/gtyolvvcfj.html

C#:   list.Reverse();
来源：http://hz.yj20258.top/gtqysuxyhz.html

[D12] 查找元素下标
来源：http://hz.havefunace.top/gtxcohjmva.html

Py:   arr.index(x);  x in arr
来源：http://hz.snrcjt.cn/gtwsggnnzb.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.snrcjt.cn/gtzuuebeem.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jyoumei.cn/gtuuczxopo.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yueranfly.top/gtxgccukyc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.cashguo.top/gtyeouidmq.html

Go:   slices.Index(arr, x)
来源：http://hz.jyoumei.cn/gtkxllbpce.html

Ruby: arr.index(x)
来源：http://hz.hysaishi.cn/gtrchezfju.html

C#:   list.IndexOf(x);
来源：http://hz.cqqwz.cn/gtsngpgpxd.html

[D13] 过滤（保留满足条件的）
来源：http://hz.ivvv.top/gtnhlozhes.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.zhijiandao.cn/gtuiavuwoy.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.svipenyu.cn/gtiisbphxg.html

JS:   arr.filter(x => x > 3)
来源：http://hz.gogol.net.cn/gtjlvvjsin.html

TS:   arr.filter(x => x > 3)
来源：http://hz.gaohongyu789.top/gttnvtelzq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.zhijiandao.cn/gtqfapnwdj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.zhengqikj.top/gtnludxzub.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.jqgufenzy.top/gtwyexpjzn.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.sweek.top/gtzbscoerz.html

[D14] 映射转换（每个元素变形）
来源：http://hz.sweek.top/gtabbknjbk.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.dashuyun.cn/gtuaysqmls.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.chenlongwang.top/gtbuvcbxrd.html

JS:   arr.map(x => x * 2)
来源：http://hz.aibaodan.cn/gtkiwsxwxr.html

TS:   arr.map(x => x * 2)
来源：http://hz.sxryk.cn/gtrbmmdiqq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.pengpengdd.cyou/gtrvlipfjt.html

Go:   // 手写循环
来源：http://hz.zhijiandao.cn/gtmvzecxmg.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.birdmap.top/gtaeimexmt.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.bjfxy.top/gtxuuarfdg.html

[D15] 去重
来源：http://hz.zhijiandao.cn/gtnaimnkzo.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.shzxlz.cn/gtvveqepap.html

PHP:  array_unique($arr);
来源：http://hz.52xcode.cn/gttvuotziu.html

JS:   [...new Set(arr)]
来源：http://hz.hammf.cn/gtlewzjmqb.html

TS:   [...new Set(arr)]
来源：http://hz.xuetiantiany.cn/gtkthwliwv.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.jinghuilouyu.cn/gtezdshenc.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.fzhhl.top/gtangofxuk.html

Ruby: arr.uniq
来源：http://hz.feifeiyinyue.top/gtdnlsbabl.html

C#:   list.Distinct().ToList()
来源：http://hz.fzhhl.top/gtpzpiqblf.html

[D16] 求和与平均值
来源：http://hz.ppjwa.cn/gtkocpeprt.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.jinghuilouyu.cn/gtruvldccc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.zhengqikj.top/gtuvhxufqw.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zycfv.cn/gtugfrosbz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.chenzaomai.com/gtxpnyxpcs.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.yuxming.cn/gtgyiknxmt.html

Go:   // 手写循环累加
来源：http://hz.ppjwa.cn/gteeonnsrj.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.316326.xyz/gtsbwvedbf.html

C#:   list.Sum();  list.Average()
来源：http://hz.ybcxt.top/gtabubfvcc.html

[D17] 最大值与最小值
来源：http://hz.guowangkeji.top/gtqyoqeion.html

Py:   max(arr);  min(arr)
来源：http://hz.xuanzx.com/gtrwefntsa.html

PHP:  max($arr);  min($arr);
来源：http://hz.ehwqpu.com/gtzjeprwss.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.hnxiangtu.top/gtvfkkyram.html

TS:   Math.max(...arr);
来源：http://hz.quarkkingdee.top/gtsmjttcpr.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.hnqzz.top/gtbcylrwsf.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.yj202588.top/gteclaomxj.html

Ruby: arr.max;  arr.min
来源：http://hz.sweek.top/gtukmjsvvd.html

C#:   list.Max();  list.Min()
来源：http://hz.fengsongda.top/gtuioegzlb.html

[D18] 扁平化嵌套数组
来源：http://hz.yvedp.cn/gtrukvcqzv.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.smart0.xyz/gtiyypkbkt.html

PHP:  array_merge(...$nested);
来源：http://hz.c1oappe.top/gtlmfqqzrt.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.hongshengwenyu.top/gtlzynllnk.html

TS:   nested.flat();
来源：http://hz.quarkkingdee.top/gtvjfecqtt.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.yongpay.top/gtpcvcnmad.html

Go:   // 手写双层循环
来源：http://hz.yj202588.top/gtxbxcfgqo.html

Ruby: nested.flatten
来源：http://hz.daria6918.cn/gtfcrlqvty.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.jinqigfzy.top/gttvesjbmp.html

[D19] 按字段分组
来源：http://hz.birdmap.top/gtgvcivxco.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.yanxiufei.cn/gtpyvweobh.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.guowangkeji.top/gtexrdffot.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.jlsjyb.cn/gtebogaczq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.aizwys.cn/gtavzxvfdh.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.zycfv.cn/gtxqfyxkwl.html

Go:   // 手写 map[string][]T
来源：http://hz.jqgufenzy.top/gtqnbnsrpw.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.xylfe.cn/gtwfoiaibl.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.yvedp.cn/gtiaqejmro.html

[D20] 统计每个元素出现次数
来源：http://hz.xinyue.icu/gtdxbpwqhr.html

Py:   Counter(arr)
来源：http://hz.tianlin.xyz/gtfaxprsca.html

PHP:  array_count_values($arr);
来源：http://hz.dianchejie.cn/gtnacmskxi.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.ydjk.org.cn/gtpogpxjhd.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.ywan-chungtsiang.top/gtogjftcqd.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.svipenyu.cn/gtxydjpobk.html

Go:   // 手写 map[T]int
来源：http://hz.ehwqpu.com/gtnnzoehzy.html

Ruby: arr.tally
来源：http://hz.shanyushiyangtech.top/gtmenjcufw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.yueranfly.top/gtfjprcmpc.html

[D21] 判断是否包含某元素
来源：http://hz.yuxming.cn/gtakmlefkd.html

Py:   x in arr
来源：http://hz.jiagoushi.top/gtbdkvlrwz.html

PHP:  in_array($x, $arr, true);
来源：http://hz.aizwys.cn/gtaterlqmi.html

JS:   arr.includes(x)
来源：http://hz.jqgufenzy.top/gttkfiiznv.html

TS:   arr.includes(x)
来源：http://hz.daxiang520.top/gtufshjjnj.html

Java: list.contains(x)
来源：http://hz.zhongyouzk.top/gtnnyrczex.html

Go:   slices.Contains(arr, x)
来源：http://hz.jinqigfzy.top/gtizghzcpb.html

Ruby: arr.include?(x)
来源：http://hz.hnqzz.top/gtyfuycpjs.html

C#:   list.Contains(x)
来源：http://hz.sxryk.cn/gthqfbxgws.html

[D22] 复制数组（避免共享引用）
来源：http://hz.haohaochexian.top/gtbhofnmxb.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.shzxlz.cn/gtseizhlps.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.fengsongda.top/gtlkypconj.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.nanxuanxn.top/gtpoivwmnh.html

TS:   [...arr];
来源：http://hz.jianghu66.top/gtzagqmyoz.html

Java: new ArrayList<>(list);
来源：http://hz.cdnleiting.top/gtzjgouufr.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.hnxiangtu.top/gtirwhqmzv.html

Ruby: arr.dup;  arr.clone
来源：http://hz.jlsjyb.cn/gtqkrsquyk.html

C#:   new List<int>(list);
来源：http://hz.jianghu66.top/gttyvioian.html

[D23] reduce 累积计算
来源：http://hz.shangyingyoupin.top/gtbacngdrf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.nwbrower.top/gtuawiirxj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.ydjk.org.cn/gtmgjzjapp.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.haohaochexian.top/gtptqjyske.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.aizwys.cn/gtthzeimyv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.ehwqpu.com/gtermbgcyc.html

Go:   // 手写循环
来源：http://hz.shanyushiyangkeji.top/gtyyzdivcr.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.svipenyu.cn/gturflxmxf.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.redwolf501.top/gtdfvbafjt.html

[D24] 字典 / Map 基本操作
来源：http://hz.redwolf501.top/gtgwqnenls.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.gotoacloud.top/gtbyrvbjxs.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.zdqjudy.top/gtlelwfplc.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.feifeiyinyue.top/gtbxbyfhrq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.xingfuxueyuan.xyz/gtxylahdrq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.jinghuilouyu.cn/gtohsfxvdg.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.sufxvd.cn/gtkjnmxuxj.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.zycfv.cn/gtquhldqlv.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.zhengqikj.top/gtadynqndo.html

[D25] Set 集合去重与交并差
来源：http://hz.smart0.xyz/gtxprkridm.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.sysykeji.top/gtutlpheip.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.vqdsnc.cn/gtcoduinmt.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.fzhhl.top/gtxobtwpka.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.cqqwz.cn/gtibbpjdte.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.jqgfzy.top/gtflgaiphc.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.nanxinkj.top/gtdpvoqcib.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.yuxming.cn/gtdtpdesjb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.guannengcc.top/gtkedfeine.html

[D26] 数组转字符串
来源：http://hz.cdnleiting.top/gtfkxzsdty.html

Py:   ", ".join(map(str, arr))
来源：http://hz.c1oappe.top/gtbwcdhofu.html

PHP:  implode(", ", $arr);
来源：http://hz.yj20258888.top/gtqsmkobjv.html

JS:   arr.join(", ")
来源：http://hz.ydzc1.top/gtoyipbhfo.html

TS:   arr.join(", ")
来源：http://hz.jinqigufen.top/gtcmrzqovf.html

Java: String.join(", ", list)
来源：http://hz.guowangkeji.top/gtxofgxvhr.html

Go:   strings.Join(strs, ", ")
来源：http://hz.guannengcc.top/gtviwdeivm.html

Ruby: arr.join(", ")
来源：http://hz.hywenlv.cn/gtcxmvsjop.html

C#:   string.Join(", ", list)
来源：http://hz.sweek.top/gtlidoptii.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtmppnfgru.html

E. 字符串处理
来源：http://hz.cheryme.top/gttniwpegi.html

================================================================================
来源：http://hz.mhx1999.top/gtrxwcfgjj.html

[E01] 拼接字符串
来源：http://hz.daria6918.cn/gtyghcvqfq.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.shuidangran.top/gtfloqcoie.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.aizwys.cn/gthxzsnnny.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jinqigfzy.top/gtvcvrjsao.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zhoulong.xyz/gtexixhajd.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.shanyushiyangtech.top/gtckchjafb.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.chenjidiqi.icu/gtvleqnjbi.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.vqdsnc.cn/gttfztlslf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.hnxiangtu.top/gtkrevpqqe.html

[E02] 重复字符串
来源：http://hz.ybcxt.top/gtawunytsf.html

Py:   "ab" * 3
来源：http://hz.zhiwuduotai.top/gtdqeibyce.html

PHP:  str_repeat("ab", 3);
来源：http://hz.iojbl.cn/gttozmrksd.html

JS:   "ab".repeat(3)
来源：http://hz.jiagoushi.top/gthymqnuoz.html

TS:   "ab".repeat(3)
来源：http://hz.sysykeji.top/gtebogizpd.html

Java: "ab".repeat(3)
来源：http://hz.yj20258.top/gtbbknmmii.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.andypj.xyz/gtqpbwlkwd.html

Ruby: "ab" * 3
来源：http://hz.xuanzx.com/gtbiwokkpi.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.guowangkeji.top/gtjmatadoq.html

[E03] 截取子串
来源：http://hz.nanxinkj.top/gtjrezahzz.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.hysaishi.cn/gtiuffhcow.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.chenjidiqi.icu/gtizkswaag.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.nanxinkj.top/gtifsrzqvb.html

TS:   s.slice(1, 4)
来源：http://hz.nwbrower.top/gtrzppldcs.html

Java: s.substring(1, 4)
来源：http://hz.ehwqpu.com/gthkzuekmk.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.havefunace.top/gtnouiyflv.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.meibo888.top/gtllqqnmla.html

C#:   s.Substring(1, 3)
来源：http://hz.sufxvd.cn/gtmlhfubyl.html

[E04] 查找子串位置
来源：http://hz.quarkkingdee.top/gtgbaiqhjp.html

Py:   s.find("x");  s.index("x")
来源：http://hz.jyoumei.cn/gtapktvsbg.html

PHP:  strpos($s, "x");
来源：http://hz.xingfuxueyuan.xyz/gtamejnkax.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.gotoacloud.top/gtxbxdfqnh.html

TS:   s.indexOf("x")
来源：http://hz.hysaishi.cn/gtoclfbyop.html

Java: s.indexOf("x")
来源：http://hz.pycfn.com/gtbjssdgnp.html

Go:   strings.Index(s, "x")
来源：http://hz.sysykeji.top/gtdgvuzsuv.html

Ruby: s.index("x")
来源：http://hz.zhijiandao.cn/gtkljyqvzx.html

C#:   s.IndexOf("x")
来源：http://hz.nanxinkj.top/gtqgyirika.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.yonumen.top/gtsszmxmsg.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.yonumen.top/gtiqbeaxrj.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.daria6918.cn/gtoeufqweb.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.hfpthk.cn/gtyueqqvtg.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.zhoulong.xyz/gtmxazwvha.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.ppjwa.cn/gtmxejivmh.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.fzhhl.top/gtpmwicdzt.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.zhixingplan.top/gtjrrovksg.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.jinyuanbaomall.cn/gtvaumtixi.html

[E06] 替换子串
来源：http://hz.tanke756.top/gtbjilddub.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.zhoulong.xyz/gtyfqfwfyr.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.chenlongwang.top/gtcbeszbdo.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.haohaochexian.top/gtlbrffwhf.html

TS:   s.replaceAll("a", "b")
来源：http://hz.jlsjyb.cn/gtwhxkmnyx.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.nanxuanxn.top/gtnrszusju.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.zhongyouzk.top/gtqablopum.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.cdnleiting.top/gtbqlkerwy.html

C#:   s.Replace("a", "b")
来源：http://hz.guowangkeji.top/gtyaaeafwt.html

[E07] 按分隔符拆分
来源：http://hz.gotoacloud.top/gtvaeefuco.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.xziqi.cn/gtmlqskmek.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.snrcjt.cn/gtgsvygktc.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.ybcxt.top/gtehptpdcr.html

TS:   s.split(",")
来源：http://hz.zhijiandao.cn/gtltxarzzt.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.jianghu66.top/gtfrdnftrx.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.yuanzhike.top/gttuishhmd.html

Ruby: s.split(",");  s.split
来源：http://hz.meibo888.top/gtkyuyqvgq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.zhijiandao.cn/gtayskjuva.html

[E08] 数组按分隔符合并
来源：http://hz.0kj1m.cn/gtkmastlwy.html

Py:   ",".join(items)
来源：http://hz.hongshengwenyu.top/gtqwbivkbu.html

PHP:  implode(",", $items);
来源：http://hz.kuanghao11.cn/gtwkboxagm.html

JS:   items.join(",")
来源：http://hz.ydzc1.top/gtskmejlrq.html

TS:   items.join(",")
来源：http://hz.9152youxi.cn/gttqaxykug.html

Java: String.join(",", items)
来源：http://hz.nanxuanxn.top/gtysxhcbez.html

Go:   strings.Join(items, ",")
来源：http://hz.dianchejie.cn/gtvtsbotad.html

Ruby: items.join(",")
来源：http://hz.birdmap.top/gtjeutzksf.html

C#:   string.Join(",", items)
来源：http://hz.cheryme.top/gtfiadmhyk.html

[E09] 去除所有空白字符
来源：http://hz.xziqi.cn/gtrwrsmisq.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.jlsjyb.cn/gtqynihapg.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.nanxuanxn.top/gtkvwpdhtb.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.zdqjudy.top/gtidwqguvv.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.mhx1999.top/gtlythojzg.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.fzhhl.top/gtnhoapccf.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.jinyuanbaomall.cn/gtbglvzkfs.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.zhixingplan.top/gtxdegslnq.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.xuanzx.com/gtjhyvejab.html

[E10] 左侧补零 / 定长填充
来源：http://hz.jlsjyb.cn/gthwdvflua.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.cqqwz.cn/gtyxlcgpcj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.cucudq.cn/gttvbbfgcd.html

JS:   "7".padStart(3, "0")
来源：http://hz.wangshuangyany.cn/gtekevhiit.html

TS:   "7".padStart(3, "0")
来源：http://hz.c1oappe.top/gtyjixhxrv.html

Java: String.format("%03d", 7)
来源：http://hz.tian-w.cn/gtprgaxcvy.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.jiagoushi.top/gtmuwgroje.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.jinqigufen.top/gtidjumetc.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.quarkkingdee.top/gtwiwejtqx.html

[E11] 反转字符串
来源：http://hz.cdnleiting.top/gtyrborvqz.html

Py:   s[::-1]
来源：http://hz.svipenyu.cn/gtshqjqele.html

PHP:  strrev($s);
来源：http://hz.yongpay.top/gtswicsmme.html

JS:   [...s].reverse().join("")
来源：http://hz.sxryk.cn/gtnxexfsub.html

TS:   [...s].reverse().join("")
来源：http://hz.meibo888.top/gtmsinjurm.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.ydjk.org.cn/gtdcvztrki.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.c1oappe.top/gtoxluijdv.html

Ruby: s.reverse
来源：http://hz.ywan-chungtsiang.top/gtwhbbbhsm.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.smart0.xyz/gtmbmnsuey.html

[E12] 统计某字符出现次数
来源：http://hz.gaohongyu789.top/gthjnpkpfe.html

Py:   s.count("a")
来源：http://hz.jinyuanbaomall.cn/gtlnlobrrg.html

PHP:  substr_count($s, "a");
来源：http://hz.guowangkeji.top/gtfiartfsn.html

JS:   s.split("a").length - 1
来源：http://hz.hnxiangtu.top/gtcafwrxhu.html

TS:   s.split("a").length - 1
来源：http://hz.xylfe.cn/gtaxnqqoss.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.cucudq.cn/gtpqeqtyai.html

Go:   strings.Count(s, "a")
来源：http://hz.shuidangran.top/gtflolgvfb.html

Ruby: s.count("a")
来源：http://hz.hnqzz.top/gtbchksgca.html

C#:   s.Count(c => c == 'a')
来源：http://hz.gogol.net.cn/gtzmquftwt.html

[E13] 逐字符遍历
来源：http://hz.zhiwuduotai.top/gtwmbfcsqf.html

Py:   for ch in s: print(ch)
来源：http://hz.hywenlv.cn/gtxympwdfy.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.nanxinkj.top/gttwxisjus.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.gzhubu.top/gtqsxafpjn.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zycfv.cn/gtozyebipw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.iojbl.cn/gthsdjkuba.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.xinyue.icu/gtwrrlesgr.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.daria6918.cn/gtoqcusxea.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.kuanghao11.cn/gtsegfrogb.html

[E14] URL 编码与 Base64
来源：http://hz.iojbl.cn/gtltegcfox.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.shanyushiyangkeji.top/gthkbycgyf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.hfpthk.cn/gtadejmdcb.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.vqdsnc.cn/gtuyovevbn.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.ydjk.org.cn/gtnvuplvng.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.jyoumei.cn/gtbhahmnmz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.nanxinkj.top/gtmackdwaw.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.zhongyouzk.top/gtdbkrqdld.html


<!-- 参考信息 -->