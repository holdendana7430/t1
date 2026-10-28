代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.cheryme.top/gtnbyxcaba.html

TS:   arr.splice(0, 1);
来源：http://hz.tian-w.cn/gtlqgqrxfe.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.ydjk.org.cn/gtplcfsddf.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.birdmap.top/gtqqvxajwt.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.xziqi.cn/gtzcuecedi.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.quarkkingdee.top/gtdxbiwymy.html

[D05] 访问与修改元素
来源：http://hz.zhijiandao.cn/gtrbjcbnoc.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.nanxinkj.top/gtwcpkahdd.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.ydzc1.top/gtfjpuwnxq.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.yanxiufei.cn/gtuaxprolg.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.daria6918.cn/gtejhqggfv.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.pycfn.com/gteorvvexu.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.daria6918.cn/gtjrybhydr.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.guowangkeji.top/gtgyrkpjma.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.ydzc1.top/gtqtstbpdt.html

[D06] 数组长度
来源：http://hz.xuanzx.com/gtvhpaarmm.html

Py:   len(arr)
来源：http://hz.hongshengwenyu.top/gtyegjtvei.html

PHP:  count($arr);
来源：http://hz.daxiang520.top/gtxoxtyrml.html

JS:   arr.length
来源：http://hz.316326.xyz/gtlnfekhbc.html

TS:   arr.length
来源：http://hz.ydjk.org.cn/gtzytaqjgm.html

Java: list.size();
来源：http://hz.aizwys.cn/gtpybqrjvg.html

Go:   len(arr)
来源：http://hz.zycfv.cn/gtajfvimba.html

Ruby: arr.length; arr.size
来源：http://hz.dashuyun.cn/gtezlcawsg.html

C#:   list.Count;
来源：http://hz.shanyushiyangkeji.top/gtkclcvndq.html

[D07] 切片 / 取子数组
来源：http://hz.yongpay.top/gtefludwth.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.shuidangran.top/gtnzybgbdx.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.yonumen.top/gtuqhtqoop.html

JS:   arr.slice(1, 4);
来源：http://hz.meibo888.top/gtiscyyerv.html

TS:   arr.slice(1, 4);
来源：http://hz.zhengqikj.top/gtauupecyh.html

Java: list.subList(1, 4);
来源：http://hz.gogol.net.cn/gtckxtovmj.html

Go:   arr[1:4]
来源：http://hz.feifeiyinyue.top/gthexozgke.html

Ruby: arr[1, 3]
来源：http://hz.yongpay.top/gtarcxznhz.html

C#:   list.GetRange(1, 3);
来源：http://hz.chenzaomai.com/gtbaucqohc.html

[D08] 合并两个数组
来源：http://hz.gaohongyu789.top/gtrmyinezj.html

Py:   a + b;  a.extend(b)
来源：http://hz.quarkkingdee.top/gtuksdeyzp.html

PHP:  array_merge($a, $b);
来源：http://hz.havefunace.top/gtyxhskiwr.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.jqgfzy.top/gtcujhuqrs.html

TS:   [...a, ...b];
来源：http://hz.nwbrower.top/gtrctkddfn.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.haohaochexian.top/gtuecmcibx.html

Go:   append(a, b...)
来源：http://hz.yuanzhike.top/gtdpxwkujr.html

Ruby: a + b;  a.concat(b)
来源：http://hz.gzhubu.top/gtyfuqvnaj.html

C#:   a.Concat(b).ToList()
来源：http://hz.sxryk.cn/gtnsrlvnjv.html

[D09] 排序（升序）
来源：http://hz.zhiwuduotai.top/gtdotmbdmy.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.cashguo.top/gtfiqsqica.html

PHP:  sort($arr);
来源：http://hz.svipenyu.cn/gtkyifatym.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.tian-w.cn/gtprymahzq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.haohaochexian.top/gthqihshmm.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.yuxming.cn/gtwcttzifd.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.svipenyu.cn/gtaymwxtks.html

Ruby: arr.sort
来源：http://hz.dianchejie.cn/gtngpxdsze.html

C#:   list.Sort();
来源：http://hz.yj202588.top/gtkydjevlo.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.sufxvd.cn/gtqrfjfgam.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.zhengqikj.top/gtugwbkwdr.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.vqdsnc.cn/gtcqvpumlj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.wangshuangyany.cn/gttwelrcqg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jinqigufen.top/gtivookpfq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.yangfankeji.com/gtntiagqqc.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.nanxuanxn.top/gtmfsptjwj.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.hfpthk.cn/gtbmlhlabn.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.guowangkeji.top/gtapajafqq.html

[D11] 反转数组
来源：http://hz.cdnleiting.top/gthkvbpbdl.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.xinyue.icu/gtkispxxbq.html

PHP:  array_reverse($arr);
来源：http://hz.jlsjyb.cn/gtidxleebw.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.zhaomingkeji.xyz/gtqibpofwx.html

TS:   [...arr].reverse();
来源：http://hz.316326.xyz/gtkgfreorw.html

Java: Collections.reverse(list);
来源：http://hz.9152youxi.cn/gtenuxnnfm.html

Go:   slices.Reverse(arr)
来源：http://hz.52xcode.cn/gtvplibujb.html

Ruby: arr.reverse
来源：http://hz.feifeiyinyue.top/gtdggtlcex.html

C#:   list.Reverse();
来源：http://hz.zhoulong.xyz/gttbaanuwm.html

[D12] 查找元素下标
来源：http://hz.jinqigufen.top/gttvtzpcjr.html

Py:   arr.index(x);  x in arr
来源：http://hz.nanxuanxn.top/gtnmhgvhts.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.jinghuilouyu.cn/gtjkgyuyat.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.sysykeji.top/gtzdkjstft.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yueranfly.top/gtezwpvxwd.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.xuanzx.com/gtnnlnecjt.html

Go:   slices.Index(arr, x)
来源：http://hz.aibaodan.cn/gttwfdpazd.html

Ruby: arr.index(x)
来源：http://hz.jianghu66.top/gtfoltajjv.html

C#:   list.IndexOf(x);
来源：http://hz.ppjwa.cn/gtlgrywjzc.html

[D13] 过滤（保留满足条件的）
来源：http://hz.nanxuanxn.top/gtrgxtwbax.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.jqgfzy.top/gtajugtlye.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.mhx1999.top/gtcntiphuv.html

JS:   arr.filter(x => x > 3)
来源：http://hz.redwolf501.top/gthccxdnbs.html

TS:   arr.filter(x => x > 3)
来源：http://hz.snrcjt.cn/gtiyyawacf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.cdnleiting.top/gtxvvfjhap.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.ppjwa.cn/gtasgzswsr.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.hywenlv.cn/gtrehsjngc.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.jyoumei.cn/gtnobvpina.html

[D14] 映射转换（每个元素变形）
来源：http://hz.gogol.net.cn/gtheaqprbf.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.dianchejie.cn/gtnxjfndlk.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.yuxming.cn/gtflrdnrrr.html

JS:   arr.map(x => x * 2)
来源：http://hz.c1oappe.top/gtuwywrmoq.html

TS:   arr.map(x => x * 2)
来源：http://hz.mhx1999.top/gtctzjrhfd.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.dianchejie.cn/gtygbfyuwt.html

Go:   // 手写循环
来源：http://hz.chenzaomai.com/gtamgkugak.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.ywan-chungtsiang.top/gtboheqzqn.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.hnqzz.top/gtbgxchlxk.html

[D15] 去重
来源：http://hz.xuetiantiany.cn/gtmmkyyegw.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.cashguo.top/gtzshabidi.html

PHP:  array_unique($arr);
来源：http://hz.jinghuilouyu.cn/gtrmbqkajv.html

JS:   [...new Set(arr)]
来源：http://hz.andypj.xyz/gtkjtpwljg.html

TS:   [...new Set(arr)]
来源：http://hz.jinyuanbaomall.cn/gtqxplwaum.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.quarkkingdee.top/gtttsrcfyo.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.aizwys.cn/gtliypitun.html

Ruby: arr.uniq
来源：http://hz.daxiang520.top/gturlvpwex.html

C#:   list.Distinct().ToList()
来源：http://hz.guowangkeji.top/gtyzktabnp.html

[D16] 求和与平均值
来源：http://hz.chenlongwang.top/gthsoxxcoj.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.gogol.net.cn/gtkrzjoznn.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.svipenyu.cn/gtwqvnnxuj.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yangfankeji.com/gtihoeuvod.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.sysykeji.top/gtyeavdusl.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.iojbl.cn/gtqxgyknqj.html

Go:   // 手写循环累加
来源：http://hz.zhengqikj.top/gtwhjumavi.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.jqgufenzy.top/gtppagzjlg.html

C#:   list.Sum();  list.Average()
来源：http://hz.svipenyu.cn/gtgaqcdtww.html

[D17] 最大值与最小值
来源：http://hz.yj20258888.top/gtsyismybt.html

Py:   max(arr);  min(arr)
来源：http://hz.ydzc1.top/gtlbuxozmj.html

PHP:  max($arr);  min($arr);
来源：http://hz.yj20258888.top/gtfisrvilq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.haohaochexian.top/gtxsicokcc.html

TS:   Math.max(...arr);
来源：http://hz.hywenlv.cn/gtvatweeat.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.daria6918.cn/gtqjidoyrp.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.dashuyun.cn/gtoqdelwbu.html

Ruby: arr.max;  arr.min
来源：http://hz.yanxiufei.cn/gtwtevoeey.html

C#:   list.Max();  list.Min()
来源：http://hz.daxiang520.top/gtieiyhjhy.html

[D18] 扁平化嵌套数组
来源：http://hz.cashguo.top/gtzhytxyzu.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.meibo888.top/gtdmfmjcok.html

PHP:  array_merge(...$nested);
来源：http://hz.ehwqpu.com/gtagtzflwq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.shzxlz.cn/gtwkagmqfg.html

TS:   nested.flat();
来源：http://hz.nanxuanxn.top/gtiphdvlom.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.pycfn.com/gtvfgmwalu.html

Go:   // 手写双层循环
来源：http://hz.fengsongda.top/gtowqxfbgr.html

Ruby: nested.flatten
来源：http://hz.smart0.xyz/gtywelkcmz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.gotoacloud.top/gtjcjagxmf.html

[D19] 按字段分组
来源：http://hz.bjfxy.top/gttpdajxdl.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.yj20258.top/gtmrvxccbz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.shanyushiyangkeji.top/gtntbbgchq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.pengpengdd.cyou/gtlygjpxju.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.tian-w.cn/gtftnqqfij.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.sxryk.cn/gtbpfbtmat.html

Go:   // 手写 map[string][]T
来源：http://hz.xuetiantiany.cn/gtupcnjbgl.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.ivvv.top/gtpqznqtmt.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.wangshuangyany.cn/gthfswkynu.html

[D20] 统计每个元素出现次数
来源：http://hz.kuanghao11.cn/gtsnrocfvt.html

Py:   Counter(arr)
来源：http://hz.feifeiyinyue.top/gtqzvheyhu.html

PHP:  array_count_values($arr);
来源：http://hz.xinyue.icu/gttkcorevp.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.wangdashe.top/gtpjidxxvn.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.gaohongyu789.top/gttvwbzjqp.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.cashguo.top/gtcaxypfnl.html

Go:   // 手写 map[T]int
来源：http://hz.fengsongda.top/gtnxmnqxaw.html

Ruby: arr.tally
来源：http://hz.ehwqpu.com/gthrfvhghp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.gotoacloud.top/gtjkdoucqr.html

[D21] 判断是否包含某元素
来源：http://hz.xuetiantiany.cn/gtqhshzhpk.html

Py:   x in arr
来源：http://hz.zhongyouzk.top/gtflkmieib.html

PHP:  in_array($x, $arr, true);
来源：http://hz.sufxvd.cn/gtfhqvubbg.html

JS:   arr.includes(x)
来源：http://hz.jinqigufen.top/gtslhrowge.html

TS:   arr.includes(x)
来源：http://hz.pengpengdd.cyou/gttltwsgsw.html

Java: list.contains(x)
来源：http://hz.yj20258.top/gtbzeqzatb.html

Go:   slices.Contains(arr, x)
来源：http://hz.dianchejie.cn/gtstiqlnsg.html

Ruby: arr.include?(x)
来源：http://hz.nanxinkj.top/gtefshmoid.html

C#:   list.Contains(x)
来源：http://hz.cqqwz.cn/gtbislzqpl.html

[D22] 复制数组（避免共享引用）
来源：http://hz.quarkkingdee.top/gtmalqjczy.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.kuanghao11.cn/gtqtynyhkd.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.wangdashe.top/gtgynoegkm.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.shuidangran.top/gtxwbpfsii.html

TS:   [...arr];
来源：http://hz.shanyushiyangkeji.top/gtcqgvwglw.html

Java: new ArrayList<>(list);
来源：http://hz.cashguo.top/gtsmltsaif.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.zhongyouzk.top/gtvqnbmyrj.html

Ruby: arr.dup;  arr.clone
来源：http://hz.aibaodan.cn/gtbzxkhqbf.html

C#:   new List<int>(list);
来源：http://hz.ywan-chungtsiang.top/gtlikzkzjm.html

[D23] reduce 累积计算
来源：http://hz.jqgufenzy.top/gtsmndaybh.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.hnqzz.top/gtplzstnis.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.shangyingyoupin.top/gtyxvlmsjd.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.smart0.xyz/gtrtdloqhs.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.shangyingyoupin.top/gtfomipaup.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.yongpay.top/gtezadrktt.html

Go:   // 手写循环
来源：http://hz.andypj.xyz/gtloykcdyu.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.zhoulong.xyz/gtnorvkuop.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.zhaomingkeji.xyz/gtybzjrxyz.html

[D24] 字典 / Map 基本操作
来源：http://hz.ppjwa.cn/gthhopjsgu.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.xuanzx.com/gtorbcksds.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.hywenlv.cn/gtlfihfqge.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.sxryk.cn/gtemmnxdqn.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.yanxiufei.cn/gtfzwpwmcn.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.guowangkeji.top/gtusixlvpm.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.jiagoushi.top/gtiyiivhxg.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.zhixingplan.top/gtwpigpamz.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.gzhubu.top/gtfbojhhkx.html

[D25] Set 集合去重与交并差
来源：http://hz.xuanzx.com/gtfpdwnzzg.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.kuanghao11.cn/gtahbzxelj.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.havefunace.top/gtlkgpsetr.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.tanke756.top/gtqsueionp.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.nanxinkj.top/gtjrbnbpdq.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.iojbl.cn/gtdgaytwxn.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.yueranfly.top/gtwegazwql.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.ydjk.org.cn/gthyxldnie.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.yj20258.top/gtmcptosqg.html

[D26] 数组转字符串
来源：http://hz.guowangkeji.top/gtuopfmbul.html

Py:   ", ".join(map(str, arr))
来源：http://hz.tian-w.cn/gtmvlpnrst.html

PHP:  implode(", ", $arr);
来源：http://hz.jiagoushi.top/gtxnhusdkq.html

JS:   arr.join(", ")
来源：http://hz.wangdashe.top/gtisejbzch.html

TS:   arr.join(", ")
来源：http://hz.zhoulong.xyz/gtqqfhydhs.html

Java: String.join(", ", list)
来源：http://hz.daxiang520.top/gthbpujlqq.html

Go:   strings.Join(strs, ", ")
来源：http://hz.svipenyu.cn/gtboaabagp.html

Ruby: arr.join(", ")
来源：http://hz.zhixingplan.top/gtahsmffud.html

C#:   string.Join(", ", list)
来源：http://hz.cdnleiting.top/gtydqocbal.html

================================================================================
来源：http://hz.xziqi.cn/gthuqexxks.html

E. 字符串处理
来源：http://hz.quarkkingdee.top/gtcwhsjtjk.html

================================================================================
来源：http://hz.nanxuanxn.top/gtyvkjkpac.html

[E01] 拼接字符串
来源：http://hz.fengsongda.top/gtvzqmjvgc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.c1oappe.top/gtkdctpxmd.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.dashuyun.cn/gtimfwkref.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.tian-w.cn/gtebewoogf.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.gzhubu.top/gtyvrvfwwr.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.vqdsnc.cn/gtrmvkawht.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.chenzaomai.com/gtnylpkmli.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.dianchejie.cn/gtpqsgosfk.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.jqgufenzy.top/gtgwtmgtkp.html

[E02] 重复字符串
来源：http://hz.chenlongwang.top/gtzlyqqqqf.html

Py:   "ab" * 3
来源：http://hz.ehwqpu.com/gtqyheoisz.html

PHP:  str_repeat("ab", 3);
来源：http://hz.316326.xyz/gthgfzfyvb.html

JS:   "ab".repeat(3)
来源：http://hz.tian-w.cn/gtweuhjusl.html

TS:   "ab".repeat(3)
来源：http://hz.smart0.xyz/gtyxxozykv.html

Java: "ab".repeat(3)
来源：http://hz.jyoumei.cn/gtlqgrcsyx.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.meibo888.top/gtxubkyirb.html

Ruby: "ab" * 3
来源：http://hz.hammf.cn/gtwgvubryb.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.kuanghao11.cn/gtaibuyvoq.html

[E03] 截取子串
来源：http://hz.hongshengwenyu.top/gtfonbpmtf.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.hongshengwenyu.top/gtzcdeovuk.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.9152youxi.cn/gtcrzkuuus.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.xziqi.cn/gtidsddrpm.html

TS:   s.slice(1, 4)
来源：http://hz.iojbl.cn/gtyoxochbe.html

Java: s.substring(1, 4)
来源：http://hz.wangshuangyany.cn/gtbgqyneao.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.jlsjyb.cn/gtktomeeia.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.shangyingyoupin.top/gtqgleeakp.html

C#:   s.Substring(1, 3)
来源：http://hz.xingfuxueyuan.xyz/gtklgfapnz.html

[E04] 查找子串位置
来源：http://hz.gotoacloud.top/gtneuphyiw.html

Py:   s.find("x");  s.index("x")
来源：http://hz.wangshuangyany.cn/gtwgfgzhnq.html

PHP:  strpos($s, "x");
来源：http://hz.yuanzhike.top/gtgwhjicab.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.zhengqikj.top/gtaramaira.html

TS:   s.indexOf("x")
来源：http://hz.bjfxy.top/gtdtmiqtcy.html

Java: s.indexOf("x")
来源：http://hz.zhengqikj.top/gtodfpwedy.html

Go:   strings.Index(s, "x")
来源：http://hz.jinqigufen.top/gtcdfipema.html

Ruby: s.index("x")
来源：http://hz.zhengqikj.top/gtvyynjdtp.html

C#:   s.IndexOf("x")
来源：http://hz.guowangkeji.top/gtadnvdbkn.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.snrcjt.cn/gtbuvplhia.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.316326.xyz/gtuoyqovoi.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.gzhubu.top/gtvpyohpsb.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.gaohongyu789.top/gtleerdibk.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.zhoulong.xyz/gtcvhhuwvh.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.sweek.top/gtidehanfo.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.ehwqpu.com/gtxjjnvblc.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.yueranfly.top/gtigwmvjrz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.ppjwa.cn/gthxyrncqz.html

[E06] 替换子串
来源：http://hz.yj202588.top/gtepqjutdf.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.ivvv.top/gtcbqynmog.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.nwbrower.top/gtywqqlucu.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.shanyushiyangkeji.top/gtlpdsvxhi.html

TS:   s.replaceAll("a", "b")
来源：http://hz.hongshengwenyu.top/gtyvgqyiar.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.haohaochexian.top/gtlirtbxbc.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.fzhhl.top/gtradhumlo.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.hfpthk.cn/gtrhleaonc.html

C#:   s.Replace("a", "b")
来源：http://hz.xingfuxueyuan.xyz/gtlintzekh.html

[E07] 按分隔符拆分
来源：http://hz.xingfuxueyuan.xyz/gtwplsdvrq.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.zycfv.cn/gtdwekimug.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.yonumen.top/gtvcutuosj.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.chenzaomai.com/gtnoimehsr.html

TS:   s.split(",")
来源：http://hz.birdmap.top/gtetkcnjqj.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.hysaishi.cn/gtswiirklw.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.zhiwuduotai.top/gtnljuukuv.html

Ruby: s.split(",");  s.split
来源：http://hz.yvedp.cn/gthdacfpdm.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.nanxuanxn.top/gtnotnppmo.html

[E08] 数组按分隔符合并
来源：http://hz.redwolf501.top/gtdumtmhif.html

Py:   ",".join(items)
来源：http://hz.fengsongda.top/gtssigjquz.html

PHP:  implode(",", $items);
来源：http://hz.xuanzx.com/gtrkhnmyja.html

JS:   items.join(",")
来源：http://hz.gzhubu.top/gtjhsmfwej.html

TS:   items.join(",")
来源：http://hz.xylfe.cn/gthcvkxuhj.html

Java: String.join(",", items)
来源：http://hz.redwolf501.top/gtbsspudok.html

Go:   strings.Join(items, ",")
来源：http://hz.mhx1999.top/gtnteiyoms.html

Ruby: items.join(",")
来源：http://hz.shangyingyoupin.top/gtucltodaa.html

C#:   string.Join(",", items)
来源：http://hz.yanxiufei.cn/gtqaygialx.html

[E09] 去除所有空白字符
来源：http://hz.52xcode.cn/gttcmungdq.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.chenlongwang.top/gtakmchkkc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.sweek.top/gthfctqhgf.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.jlsjyb.cn/gttfgytjfb.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.ywan-chungtsiang.top/gtmoiiawpz.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.pengpengdd.cyou/gtsjsogaix.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.tian-w.cn/gtevejavhy.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.gzhubu.top/gtthibutru.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.xziqi.cn/gtuuunpdum.html

[E10] 左侧补零 / 定长填充
来源：http://hz.cqqwz.cn/gtoqwtgttq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.haohaochexian.top/gtgatvwpuo.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.wangdashe.top/gtfqgrvtvs.html

JS:   "7".padStart(3, "0")
来源：http://hz.hammf.cn/gtryjjafbf.html

TS:   "7".padStart(3, "0")
来源：http://hz.316326.xyz/gtdaiqakpr.html

Java: String.format("%03d", 7)
来源：http://hz.hnqzz.top/gtziakiibt.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.xuetiantiany.cn/gtwzufvufx.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.iojbl.cn/gtxdmndgdk.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.ivvv.top/gtctsbgsqx.html

[E11] 反转字符串
来源：http://hz.yonumen.top/gtjaqpuuui.html

Py:   s[::-1]
来源：http://hz.ppjwa.cn/gtjeztlchj.html

PHP:  strrev($s);
来源：http://hz.feifeiyinyue.top/gtgmuxqnmf.html


<!-- 参考信息 -->