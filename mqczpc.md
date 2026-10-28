代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.sxryk.cn/gtxexwaqqi.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.daria6918.cn/gtgsmhgrze.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.svipenyu.cn/gtfyxrcbuw.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.aizwys.cn/gtjedcutqk.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.gaohongyu789.top/gtathdhbuz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.dianchejie.cn/gtsuduxwdm.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.shangyingyoupin.top/gtsbpowzxy.html

[D06] 数组长度
来源：http://hz.jyoumei.cn/gtsevygecz.html

Py:   len(arr)
来源：http://hz.yj20258888.top/gtmbuhiuom.html

PHP:  count($arr);
来源：http://hz.ywan-chungtsiang.top/gtceimgbbf.html

JS:   arr.length
来源：http://hz.jinqigufen.top/gtjexiuygu.html

TS:   arr.length
来源：http://hz.zhengqikj.top/gthxoyxxzd.html

Java: list.size();
来源：http://hz.hnqzz.top/gteaxvqtfz.html

Go:   len(arr)
来源：http://hz.hysaishi.cn/gtmuqocrwo.html

Ruby: arr.length; arr.size
来源：http://hz.52xcode.cn/gtwxxbayrs.html

C#:   list.Count;
来源：http://hz.jlsjyb.cn/gtboqkhrbo.html

[D07] 切片 / 取子数组
来源：http://hz.chenjidiqi.icu/gtlcrtkadb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.tanke756.top/gtrhjnzmmz.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.hammf.cn/gtrzmezitp.html

JS:   arr.slice(1, 4);
来源：http://hz.shangyingyoupin.top/gtxkfcomnw.html

TS:   arr.slice(1, 4);
来源：http://hz.cdnleiting.top/gtbcprfslt.html

Java: list.subList(1, 4);
来源：http://hz.xylfe.cn/gtsoojowtm.html

Go:   arr[1:4]
来源：http://hz.zhongyouzk.top/gtoppdycbq.html

Ruby: arr[1, 3]
来源：http://hz.feifeiyinyue.top/gtjvjghegv.html

C#:   list.GetRange(1, 3);
来源：http://hz.zhoulong.xyz/gtnovpgmrk.html

[D08] 合并两个数组
来源：http://hz.guowangkeji.top/gtidwvpscp.html

Py:   a + b;  a.extend(b)
来源：http://hz.quarkkingdee.top/gttcjpoaxr.html

PHP:  array_merge($a, $b);
来源：http://hz.wangshuangyany.cn/gtjdzkrfgk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.haohaochexian.top/gtdkffoywg.html

TS:   [...a, ...b];
来源：http://hz.tian-w.cn/gtsxmhnigi.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.sufxvd.cn/gtskpcpaju.html

Go:   append(a, b...)
来源：http://hz.hysaishi.cn/gtpwuulpaj.html

Ruby: a + b;  a.concat(b)
来源：http://hz.feifeiyinyue.top/gtcrjdqmxd.html

C#:   a.Concat(b).ToList()
来源：http://hz.gogol.net.cn/gtxrqnhwrm.html

[D09] 排序（升序）
来源：http://hz.wangshuangyany.cn/gtkfqgocyh.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ehwqpu.com/gtcornukkk.html

PHP:  sort($arr);
来源：http://hz.zhoulong.xyz/gtmyqspisa.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.hongshengwenyu.top/gtacoxmdoy.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.fengsongda.top/gtckgsuhhk.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.hysaishi.cn/gtrctnaiaz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.havefunace.top/gtjuwlaxfo.html

Ruby: arr.sort
来源：http://hz.hnxiangtu.top/gtyiedgehu.html

C#:   list.Sort();
来源：http://hz.sweek.top/gtwxcessks.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.shanyushiyangtech.top/gtotdyfgys.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.cucudq.cn/gtehrhcvef.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yuxming.cn/gtkhrlakyk.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hongshengwenyu.top/gtefbkwhft.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.havefunace.top/gtuargiegt.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.zhongyouzk.top/gtpdsrymgr.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.jlsjyb.cn/gtklauveqj.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.xinyue.icu/gthkcaahsu.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.ywan-chungtsiang.top/gtbhdekyfp.html

[D11] 反转数组
来源：http://hz.xinyue.icu/gtbpoiwgmx.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.jyoumei.cn/gtyfsbvxrb.html

PHP:  array_reverse($arr);
来源：http://hz.nwbrower.top/gteqxvdnhq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.xuetiantiany.cn/gtolaqrtkw.html

TS:   [...arr].reverse();
来源：http://hz.yj20258.top/gtbskuefrt.html

Java: Collections.reverse(list);
来源：http://hz.snrcjt.cn/gtnqxexwde.html

Go:   slices.Reverse(arr)
来源：http://hz.havefunace.top/gtbgfaeyfb.html

Ruby: arr.reverse
来源：http://hz.yvedp.cn/gtznvcvihv.html

C#:   list.Reverse();
来源：http://hz.sysykeji.top/gtwjypsuwc.html

[D12] 查找元素下标
来源：http://hz.xuanzx.com/gtigaxoosy.html

Py:   arr.index(x);  x in arr
来源：http://hz.xinyue.icu/gtrkgqdshh.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.zhiwuduotai.top/gtvkpicbpr.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yvedp.cn/gtiwayghfj.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.ppjwa.cn/gtnmyighcn.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.9152youxi.cn/gtcpbqucaw.html

Go:   slices.Index(arr, x)
来源：http://hz.shzxlz.cn/gtlnkqodvv.html

Ruby: arr.index(x)
来源：http://hz.yangfankeji.com/gtgvhrjvqt.html

C#:   list.IndexOf(x);
来源：http://hz.shuidangran.top/gtvnqqwcnf.html

[D13] 过滤（保留满足条件的）
来源：http://hz.dianchejie.cn/gtbrufynke.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.hywenlv.cn/gtclipanhs.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.mhx1999.top/gtqhqehzec.html

JS:   arr.filter(x => x > 3)
来源：http://hz.gzhubu.top/gtbikiaprs.html

TS:   arr.filter(x => x > 3)
来源：http://hz.xuetiantiany.cn/gtgleojpuc.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.hysaishi.cn/gtqgehultt.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.gzhubu.top/gtktwwnrem.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.shanyushiyangtech.top/gtyblilmqp.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.fzhhl.top/gtvazrcuad.html

[D14] 映射转换（每个元素变形）
来源：http://hz.birdmap.top/gtjtfufqxt.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.zhengqikj.top/gtmpzedwcb.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.guowangkeji.top/gtnmthrckl.html

JS:   arr.map(x => x * 2)
来源：http://hz.gotoacloud.top/gtziblenmq.html

TS:   arr.map(x => x * 2)
来源：http://hz.zhongyouzk.top/gtwxbwhukt.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.chenzaomai.com/gtasudpemx.html

Go:   // 手写循环
来源：http://hz.jiagoushi.top/gtypwrhxyi.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.quarkkingdee.top/gtcsupsiwd.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.sufxvd.cn/gtefkqsdfi.html

[D15] 去重
来源：http://hz.hywenlv.cn/gtmulfafkm.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.shangyingyoupin.top/gtlufdpztx.html

PHP:  array_unique($arr);
来源：http://hz.meibo888.top/gtyrlynwiv.html

JS:   [...new Set(arr)]
来源：http://hz.gogol.net.cn/gtlvusdlpw.html

TS:   [...new Set(arr)]
来源：http://hz.ydjk.org.cn/gtovisdvsr.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.dashuyun.cn/gthyetjtxm.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.yonumen.top/gtyqbgngdx.html

Ruby: arr.uniq
来源：http://hz.hfpthk.cn/gtgrcapqwn.html

C#:   list.Distinct().ToList()
来源：http://hz.ehwqpu.com/gtyrguxnzn.html

[D16] 求和与平均值
来源：http://hz.aizwys.cn/gtelanqxrt.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.hfpthk.cn/gtxnaisyxs.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.snrcjt.cn/gtqtxivfxt.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.bjfxy.top/gtoxskxfjr.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yanxiufei.cn/gtpjpctwnq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.jinyuanbaomall.cn/gtrauxxwqv.html

Go:   // 手写循环累加
来源：http://hz.nanxinkj.top/gtoqirvqez.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.xuanzx.com/gtctdxvzjt.html

C#:   list.Sum();  list.Average()
来源：http://hz.fzhhl.top/gttzxwqyqc.html

[D17] 最大值与最小值
来源：http://hz.cdnleiting.top/gtetwuiyvj.html

Py:   max(arr);  min(arr)
来源：http://hz.zhengqikj.top/gtjvyozgei.html

PHP:  max($arr);  min($arr);
来源：http://hz.shanyushiyangkeji.top/gtspliopul.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.gotoacloud.top/gtrxnkuuld.html

TS:   Math.max(...arr);
来源：http://hz.hnxiangtu.top/gtzwhdusev.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.jlsjyb.cn/gtwwjagbau.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.xinyue.icu/gtzuuljnov.html

Ruby: arr.max;  arr.min
来源：http://hz.jyoumei.cn/gtmsotkfir.html

C#:   list.Max();  list.Min()
来源：http://hz.ydzc1.top/gtukqizkij.html

[D18] 扁平化嵌套数组
来源：http://hz.shzxlz.cn/gtshjdixlb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.jyoumei.cn/gtvprqsrmm.html

PHP:  array_merge(...$nested);
来源：http://hz.shangyingyoupin.top/gtxtwumyym.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.bjfxy.top/gtkkvdisnn.html

TS:   nested.flat();
来源：http://hz.nanxinkj.top/gtilwfncdl.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.yj202588.top/gtyweduvjl.html

Go:   // 手写双层循环
来源：http://hz.wangdashe.top/gtmzirsmxn.html

Ruby: nested.flatten
来源：http://hz.hywenlv.cn/gtyocieoix.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.zhijiandao.cn/gtmkaucrhw.html

[D19] 按字段分组
来源：http://hz.zhoulong.xyz/gtvhjsloan.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.vqdsnc.cn/gtgkhmxsmr.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.yanxiufei.cn/gtctbcmnyt.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.cqqwz.cn/gtvdwqfcek.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.jqgufenzy.top/gtbgqzivht.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.ehwqpu.com/gtpqvzxikb.html

Go:   // 手写 map[string][]T
来源：http://hz.tian-w.cn/gtujopsqlh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.dianchejie.cn/gtnugyzicc.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.birdmap.top/gtnhtaxuvf.html

[D20] 统计每个元素出现次数
来源：http://hz.redwolf501.top/gtxhhuruid.html

Py:   Counter(arr)
来源：http://hz.svipenyu.cn/gtwakpyjrk.html

PHP:  array_count_values($arr);
来源：http://hz.xuetiantiany.cn/gtzabgnstb.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.havefunace.top/gtrdaxokyb.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.tianlin.xyz/gtjvuelqgd.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.jinghuilouyu.cn/gtqcmsehpx.html

Go:   // 手写 map[T]int
来源：http://hz.zycfv.cn/gtlgejqczp.html

Ruby: arr.tally
来源：http://hz.ehwqpu.com/gtvnnnqaya.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.shanyushiyangkeji.top/gtlcascptz.html

[D21] 判断是否包含某元素
来源：http://hz.zhengqikj.top/gtbyzhgenq.html

Py:   x in arr
来源：http://hz.ydjk.org.cn/gtbbvmlgtf.html

PHP:  in_array($x, $arr, true);
来源：http://hz.hnxiangtu.top/gttkjewkvk.html

JS:   arr.includes(x)
来源：http://hz.jianghu66.top/gtqpzjelvp.html

TS:   arr.includes(x)
来源：http://hz.xuanzx.com/gtnvqqlgeq.html

Java: list.contains(x)
来源：http://hz.quarkkingdee.top/gtxscxkgej.html

Go:   slices.Contains(arr, x)
来源：http://hz.0kj1m.cn/gtfcygrolz.html

Ruby: arr.include?(x)
来源：http://hz.hammf.cn/gtgnvritkr.html

C#:   list.Contains(x)
来源：http://hz.zhixingplan.top/gtmafshwxl.html

[D22] 复制数组（避免共享引用）
来源：http://hz.gaohongyu789.top/gtcxwziiok.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.shuidangran.top/gtwlehsvjj.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.gzhubu.top/gtmjftgeti.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.xinyue.icu/gtxxapjpue.html

TS:   [...arr];
来源：http://hz.jinqigufen.top/gtnqzsxsac.html

Java: new ArrayList<>(list);
来源：http://hz.aibaodan.cn/gteldbnwxe.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.hnqzz.top/gtqpyvihqi.html

Ruby: arr.dup;  arr.clone
来源：http://hz.yueranfly.top/gtfwavhwft.html

C#:   new List<int>(list);
来源：http://hz.hywenlv.cn/gtrmbrrvta.html

[D23] reduce 累积计算
来源：http://hz.nanxinkj.top/gtkjrawtui.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.haohaochexian.top/gtbkiybrhw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.jinqigfzy.top/gtdlxaecsp.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.snrcjt.cn/gtdntvpbnv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.wangdashe.top/gtneschrgt.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.52xcode.cn/gtqaewbpef.html

Go:   // 手写循环
来源：http://hz.haohaochexian.top/gtjkuhlhgq.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.gogol.net.cn/gtdscfpnbj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.tian-w.cn/gtskzbslfv.html

[D24] 字典 / Map 基本操作
来源：http://hz.zhijiandao.cn/gtiuzaxusv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.guowangkeji.top/gtqoojciws.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.shanyushiyangkeji.top/gtzklvljbd.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.chenzaomai.com/gtwnokpjoc.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.zycfv.cn/gtlrahfjmx.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.0kj1m.cn/gtfhijmtwv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.xziqi.cn/gtldxtbleh.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.zhongyouzk.top/gtcxfleejw.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.shangyingyoupin.top/gtelapeovc.html

[D25] Set 集合去重与交并差
来源：http://hz.jqgufenzy.top/gtdbabzyjv.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.ehwqpu.com/gtsmqlkhgi.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.yangfankeji.com/gtwhfsashw.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.dianchejie.cn/gtbsgabtkw.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.jiagoushi.top/gtrqavjcth.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.chenzaomai.com/gtfsjpwnob.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.zhengqikj.top/gtwuqdxvaa.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.ydzc1.top/gtwdivfxkw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.gotoacloud.top/gtrhbsjwav.html

[D26] 数组转字符串
来源：http://hz.havefunace.top/gtlrhuczhf.html

Py:   ", ".join(map(str, arr))
来源：http://hz.jinyuanbaomall.cn/gtnjayrill.html

PHP:  implode(", ", $arr);
来源：http://hz.jianghu66.top/gtyukuopsg.html

JS:   arr.join(", ")
来源：http://hz.gaohongyu789.top/gtupgscoqb.html

TS:   arr.join(", ")
来源：http://hz.gogol.net.cn/gtrbqprvrs.html

Java: String.join(", ", list)
来源：http://hz.gaohongyu789.top/gtedesheti.html

Go:   strings.Join(strs, ", ")
来源：http://hz.pycfn.com/gtowfdljgn.html

Ruby: arr.join(", ")
来源：http://hz.pycfn.com/gtsvtlznki.html

C#:   string.Join(", ", list)
来源：http://hz.cheryme.top/gtjeaaunff.html

================================================================================
来源：http://hz.wangdashe.top/gtvkttreja.html

E. 字符串处理
来源：http://hz.316326.xyz/gtrgyrwvfl.html

================================================================================
来源：http://hz.andypj.xyz/gtvxlrcxka.html

[E01] 拼接字符串
来源：http://hz.andypj.xyz/gtxgkmxjme.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.aizwys.cn/gtnwyuvfbu.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.aibaodan.cn/gtjhqorgkg.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jinqigufen.top/gtrdeihaoj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.xuanzx.com/gtcwfyzlat.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.shanyushiyangtech.top/gtntdfijtn.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.shangyingyoupin.top/gtdmfjqxif.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.ehwqpu.com/gtkdhxhpjd.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.yangfankeji.com/gtgqrcecrp.html

[E02] 重复字符串
来源：http://hz.yongpay.top/gtmdruhzgm.html

Py:   "ab" * 3
来源：http://hz.xylfe.cn/gtfbxutfbc.html

PHP:  str_repeat("ab", 3);
来源：http://hz.andypj.xyz/gtpdvjqjlr.html

JS:   "ab".repeat(3)
来源：http://hz.sweek.top/gtfhthotra.html

TS:   "ab".repeat(3)
来源：http://hz.hywenlv.cn/gtznqncqtm.html

Java: "ab".repeat(3)
来源：http://hz.smart0.xyz/gtcuqfcmse.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.nanxuanxn.top/gtenjjxafx.html

Ruby: "ab" * 3
来源：http://hz.hongshengwenyu.top/gthwcfxehm.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.zhijiandao.cn/gtueynbuiy.html

[E03] 截取子串
来源：http://hz.yvedp.cn/gtivwnawkr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.feifeiyinyue.top/gtilgtxuxr.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.hnxiangtu.top/gtsojtrrym.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.xziqi.cn/gttgilmdix.html

TS:   s.slice(1, 4)
来源：http://hz.dianchejie.cn/gtjdjejlrp.html

Java: s.substring(1, 4)
来源：http://hz.mhx1999.top/gtebxemmtr.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.shuidangran.top/gtxtyamjyd.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.havefunace.top/gtorznnvbv.html

C#:   s.Substring(1, 3)
来源：http://hz.quarkkingdee.top/gticohbgmh.html

[E04] 查找子串位置
来源：http://hz.ivvv.top/gtcfolmgry.html

Py:   s.find("x");  s.index("x")
来源：http://hz.birdmap.top/gtkdyqrbnr.html

PHP:  strpos($s, "x");
来源：http://hz.guannengcc.top/gtkxukxsli.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.zhiwuduotai.top/gtvfdngyhk.html

TS:   s.indexOf("x")
来源：http://hz.nwbrower.top/gtxkjiriln.html

Java: s.indexOf("x")
来源：http://hz.aizwys.cn/gtfzwebzgr.html

Go:   strings.Index(s, "x")
来源：http://hz.yanxiufei.cn/gtpcgyqgni.html

Ruby: s.index("x")
来源：http://hz.nanxinkj.top/gtiycjluas.html

C#:   s.IndexOf("x")
来源：http://hz.shanyushiyangkeji.top/gtaifauwdb.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.pengpengdd.cyou/gtczskrhea.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.guowangkeji.top/gtktixfxjt.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.jinqigfzy.top/gttomyyitq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.xingfuxueyuan.xyz/gtrionismu.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.xingfuxueyuan.xyz/gtyhwwzaqm.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.shanyushiyangtech.top/gtquttbuyv.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.ywan-chungtsiang.top/gtnhjbeszv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.andypj.xyz/gtbdtshpme.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.zhaomingkeji.xyz/gthmvewjhz.html

[E06] 替换子串
来源：http://hz.birdmap.top/gtjxuoeamh.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.jinyuanbaomall.cn/gtvldqnkrk.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.dashuyun.cn/gtbprlljmm.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.hnxiangtu.top/gtrtvzrrdr.html

TS:   s.replaceAll("a", "b")
来源：http://hz.tianlin.xyz/gtluczbuua.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.tian-w.cn/gtaujtubie.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.sxryk.cn/gtkhwmdakr.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.hywenlv.cn/gtaucudqqb.html

C#:   s.Replace("a", "b")
来源：http://hz.tianlin.xyz/gtywowrbix.html

[E07] 按分隔符拆分
来源：http://hz.ivvv.top/gtjzevoeqq.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.nanxuanxn.top/gtidhkdgtt.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.zycfv.cn/gtfrnqbvpv.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.cdnleiting.top/gtptnjrbxr.html

TS:   s.split(",")
来源：http://hz.xziqi.cn/gtvuwxbvde.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.aibaodan.cn/gttmnglgdx.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.sufxvd.cn/gtskdnywjz.html

Ruby: s.split(",");  s.split
来源：http://hz.meibo888.top/gtdrwrnkja.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.shzxlz.cn/gtboxeaysr.html

[E08] 数组按分隔符合并
来源：http://hz.zhixingplan.top/gtofdoqmqb.html

Py:   ",".join(items)
来源：http://hz.guannengcc.top/gtmsaltfdl.html

PHP:  implode(",", $items);
来源：http://hz.havefunace.top/gtgwwpkigh.html

JS:   items.join(",")
来源：http://hz.shanyushiyangtech.top/gtwtlrttzb.html

TS:   items.join(",")
来源：http://hz.pengpengdd.cyou/gtwtzaivau.html

Java: String.join(",", items)
来源：http://hz.cashguo.top/gthherfbmb.html

Go:   strings.Join(items, ",")
来源：http://hz.shuidangran.top/gtqlxjyrcr.html

Ruby: items.join(",")
来源：http://hz.shzxlz.cn/gtmgnbsscg.html

C#:   string.Join(",", items)
来源：http://hz.andypj.xyz/gtqiuxxyqq.html

[E09] 去除所有空白字符
来源：http://hz.ivvv.top/gtbtxbtyly.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.fengsongda.top/gtxdssjmkt.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.daria6918.cn/gtvjgdtayy.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.zdqjudy.top/gteivvgkhb.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.jlsjyb.cn/gtezfgxztc.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.sxryk.cn/gttwazpuuh.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.shanyushiyangkeji.top/gtlyawjajf.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.52xcode.cn/gtxolyyfyj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.daria6918.cn/gtqkvqlyer.html

[E10] 左侧补零 / 定长填充
来源：http://hz.dashuyun.cn/gtmgmtlnav.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.cdnleiting.top/gtdpjjlpag.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.wangshuangyany.cn/gtlmzbbzmz.html

JS:   "7".padStart(3, "0")
来源：http://hz.jianghu66.top/gttrugsqwq.html

TS:   "7".padStart(3, "0")
来源：http://hz.nanxuanxn.top/gtnrszshow.html

Java: String.format("%03d", 7)
来源：http://hz.zhiwuduotai.top/gtbimneula.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.hongshengwenyu.top/gtoaxsyxdp.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.hfpthk.cn/gtprenoemx.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.sufxvd.cn/gtqhwvokjs.html

[E11] 反转字符串
来源：http://hz.chenlongwang.top/gtbmnmbnjk.html

Py:   s[::-1]
来源：http://hz.vqdsnc.cn/gtfiwlzdht.html

PHP:  strrev($s);
来源：http://hz.redwolf501.top/gthlcgfeud.html

JS:   [...s].reverse().join("")
来源：http://hz.nanxuanxn.top/gtmairmqyu.html

TS:   [...s].reverse().join("")
来源：http://hz.chenlongwang.top/gtouteswpk.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.jyoumei.cn/gtutewiuit.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.xinyue.icu/gtlxkfyiew.html

Ruby: s.reverse
来源：http://hz.jlsjyb.cn/gtgdqqpxir.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.shanyushiyangtech.top/gtughhdudw.html

[E12] 统计某字符出现次数
来源：http://hz.jiagoushi.top/gtxahjuixj.html

Py:   s.count("a")
来源：http://hz.ivvv.top/gtcfgdpoml.html


<!-- 参考信息 -->