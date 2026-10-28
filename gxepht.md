代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.jiagoushi.top/gtmklluowe.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.ydzc1.top/gtproherzp.html

[D05] 访问与修改元素
来源：http://hz.0kj1m.cn/gtcavhzjct.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hysaishi.cn/gttmsrqoja.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.zhengqikj.top/gtxyrotmba.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.aibaodan.cn/gtjxhreazv.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.redwolf501.top/gtuelmovfe.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.hfpthk.cn/gtuylfjyxa.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.sweek.top/gthkqpetgr.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.xziqi.cn/gtkewdlmpt.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.jinyuanbaomall.cn/gttbjcvljs.html

[D06] 数组长度
来源：http://hz.jianghu66.top/gtrapzouli.html

Py:   len(arr)
来源：http://hz.aibaodan.cn/gtguzjjfzo.html

PHP:  count($arr);
来源：http://hz.52xcode.cn/gtahvizusq.html

JS:   arr.length
来源：http://hz.tanke756.top/gtwufdkbxf.html

TS:   arr.length
来源：http://hz.xziqi.cn/gtmhvlcwyh.html

Java: list.size();
来源：http://hz.yueranfly.top/gtsjiqsqmr.html

Go:   len(arr)
来源：http://hz.jqgfzy.top/gtfxinukod.html

Ruby: arr.length; arr.size
来源：http://hz.yj20258.top/gtrqttsyky.html

C#:   list.Count;
来源：http://hz.yongpay.top/gtwhcvjoca.html

[D07] 切片 / 取子数组
来源：http://hz.guowangkeji.top/gtfosvjuzc.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.ybcxt.top/gtsvywwzsu.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.zhaomingkeji.xyz/gtsakyjgoc.html

JS:   arr.slice(1, 4);
来源：http://hz.cqqwz.cn/gtmfuvjjiy.html

TS:   arr.slice(1, 4);
来源：http://hz.dashuyun.cn/gttnjbupxz.html

Java: list.subList(1, 4);
来源：http://hz.shuidangran.top/gtfzqidfrc.html

Go:   arr[1:4]
来源：http://hz.zhiwuduotai.top/gtbtufkrmn.html

Ruby: arr[1, 3]
来源：http://hz.316326.xyz/gtfjgznjky.html

C#:   list.GetRange(1, 3);
来源：http://hz.zdqjudy.top/gtshplsnfy.html

[D08] 合并两个数组
来源：http://hz.cucudq.cn/gtclrdihlk.html

Py:   a + b;  a.extend(b)
来源：http://hz.snrcjt.cn/gtpiklnjnb.html

PHP:  array_merge($a, $b);
来源：http://hz.sxryk.cn/gteveeevww.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.shuidangran.top/gtysparuri.html

TS:   [...a, ...b];
来源：http://hz.jqgufenzy.top/gtygrvtupd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.yuanzhike.top/gtjlrgqtgp.html

Go:   append(a, b...)
来源：http://hz.smart0.xyz/gtjoyybmdx.html

Ruby: a + b;  a.concat(b)
来源：http://hz.sysykeji.top/gtfiaqxrwc.html

C#:   a.Concat(b).ToList()
来源：http://hz.sweek.top/gtwigknpxl.html

[D09] 排序（升序）
来源：http://hz.cashguo.top/gtpccsvxcq.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.andypj.xyz/gtzvmoeume.html

PHP:  sort($arr);
来源：http://hz.feifeiyinyue.top/gtecpciiqc.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.wangdashe.top/gtikvweqhq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.tanke756.top/gtwmhurzoa.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.nanxuanxn.top/gtoaodyytj.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.daxiang520.top/gtmhomprwq.html

Ruby: arr.sort
来源：http://hz.fzhhl.top/gtedlrgjeq.html

C#:   list.Sort();
来源：http://hz.zhixingplan.top/gtcaypxyfn.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.wangdashe.top/gtfrbwxicj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.ybcxt.top/gttmysyord.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.birdmap.top/gtvzsgnhmk.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jinqigufen.top/gtvrfnvtvh.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zycfv.cn/gtrocmxlpj.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.zhijiandao.cn/gtekxemnhn.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.jinqigfzy.top/gteiaekywq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.aibaodan.cn/gtoddgdiaa.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.chenlongwang.top/gtyspfozet.html

[D11] 反转数组
来源：http://hz.shanyushiyangtech.top/gtlrpqsnzo.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.snrcjt.cn/gtzwdzstqr.html

PHP:  array_reverse($arr);
来源：http://hz.cqqwz.cn/gttwcgwose.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.havefunace.top/gtrltozgch.html

TS:   [...arr].reverse();
来源：http://hz.jiagoushi.top/gtnpazokad.html

Java: Collections.reverse(list);
来源：http://hz.quarkkingdee.top/gtunmaofba.html

Go:   slices.Reverse(arr)
来源：http://hz.ydzc1.top/gtxymepphz.html

Ruby: arr.reverse
来源：http://hz.xuetiantiany.cn/gtjstqmbzd.html

C#:   list.Reverse();
来源：http://hz.yueranfly.top/gtsmcqlbuc.html

[D12] 查找元素下标
来源：http://hz.jqgufenzy.top/gtvfkesrja.html

Py:   arr.index(x);  x in arr
来源：http://hz.zhijiandao.cn/gtjqyzhgie.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.gzhubu.top/gtovkxsobk.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.dianchejie.cn/gtdmbqcqpc.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.daria6918.cn/gtrjeiqpzv.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.yanxiufei.cn/gtqbsysjvx.html

Go:   slices.Index(arr, x)
来源：http://hz.cucudq.cn/gtqrqarwlo.html

Ruby: arr.index(x)
来源：http://hz.bjfxy.top/gtycelmiru.html

C#:   list.IndexOf(x);
来源：http://hz.guannengcc.top/gtefkmgppc.html

[D13] 过滤（保留满足条件的）
来源：http://hz.dianchejie.cn/gtyagleygu.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.mhx1999.top/gtnuckgejr.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.andypj.xyz/gtilnvftzm.html

JS:   arr.filter(x => x > 3)
来源：http://hz.haohaochexian.top/gttsacdbyd.html

TS:   arr.filter(x => x > 3)
来源：http://hz.aizwys.cn/gtqsynfzgj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.wangdashe.top/gtdqyqrxzv.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.shangyingyoupin.top/gtopqystfr.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.gotoacloud.top/gtwultfkrk.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.kuanghao11.cn/gtaloskwzb.html

[D14] 映射转换（每个元素变形）
来源：http://hz.sweek.top/gtnaatmjmk.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.gzhubu.top/gtsjnujszq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.jinqigufen.top/gtoythlnbq.html

JS:   arr.map(x => x * 2)
来源：http://hz.guannengcc.top/gtqtcybknc.html

TS:   arr.map(x => x * 2)
来源：http://hz.jyoumei.cn/gteaboenmz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.cashguo.top/gtxwqfjmdy.html

Go:   // 手写循环
来源：http://hz.smart0.xyz/gtgcvxvgwt.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.kuanghao11.cn/gtidznyvsv.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.jinghuilouyu.cn/gtycooipii.html

[D15] 去重
来源：http://hz.yanxiufei.cn/gtrtnmjoac.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.xylfe.cn/gtiuxqqruh.html

PHP:  array_unique($arr);
来源：http://hz.ivvv.top/gtlbdxhomt.html

JS:   [...new Set(arr)]
来源：http://hz.jiagoushi.top/gtqsjawsbj.html

TS:   [...new Set(arr)]
来源：http://hz.feifeiyinyue.top/gtucbfklld.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.tian-w.cn/gtseaxphbe.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.svipenyu.cn/gtacjtqzqy.html

Ruby: arr.uniq
来源：http://hz.shanyushiyangkeji.top/gtziudfalu.html

C#:   list.Distinct().ToList()
来源：http://hz.tanke756.top/gtbxvfvtqh.html

[D16] 求和与平均值
来源：http://hz.mhx1999.top/gtnviogofs.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.redwolf501.top/gtzazwetpp.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.jinyuanbaomall.cn/gtsbplpbym.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jinyuanbaomall.cn/gtglhcqcel.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.tanke756.top/gtwbexxfqw.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.shangyingyoupin.top/gtjdswnnya.html

Go:   // 手写循环累加
来源：http://hz.dashuyun.cn/gtnqsmnpfm.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.feifeiyinyue.top/gtvcljqsux.html

C#:   list.Sum();  list.Average()
来源：http://hz.52xcode.cn/gtnmcqytyv.html

[D17] 最大值与最小值
来源：http://hz.gzhubu.top/gtrftdvyqv.html

Py:   max(arr);  min(arr)
来源：http://hz.snrcjt.cn/gttovionst.html

PHP:  max($arr);  min($arr);
来源：http://hz.yj20258888.top/gtqcxbifei.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.meibo888.top/gtysqvrake.html

TS:   Math.max(...arr);
来源：http://hz.chenlongwang.top/gttbgyfaoq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.gogol.net.cn/gtvurswdcd.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.jlsjyb.cn/gtwubcyggi.html

Ruby: arr.max;  arr.min
来源：http://hz.gzhubu.top/gtpfiarwvz.html

C#:   list.Max();  list.Min()
来源：http://hz.fengsongda.top/gtelpvexiw.html

[D18] 扁平化嵌套数组
来源：http://hz.jinyuanbaomall.cn/gtnhejwxcx.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.jianghu66.top/gtyxpqxvxl.html

PHP:  array_merge(...$nested);
来源：http://hz.chenzaomai.com/gtwauxouul.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.yuxming.cn/gtzehmlwjy.html

TS:   nested.flat();
来源：http://hz.tianlin.xyz/gtugefxfhg.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.gotoacloud.top/gtfshwixwa.html

Go:   // 手写双层循环
来源：http://hz.bjfxy.top/gtdbvwrwtv.html

Ruby: nested.flatten
来源：http://hz.nwbrower.top/gtyscuwtxt.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.sufxvd.cn/gtujwxvfui.html

[D19] 按字段分组
来源：http://hz.fzhhl.top/gtwsxnlfmn.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.yvedp.cn/gtxlknksuc.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.gotoacloud.top/gtalseewnf.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.birdmap.top/gttnkoclci.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.yj20258888.top/gtxxxewjvh.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.chenzaomai.com/gtqgkepfnt.html

Go:   // 手写 map[string][]T
来源：http://hz.jianghu66.top/gtzpptkklz.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.xuanzx.com/gtncdcmlty.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.sweek.top/gtmdgvzlun.html

[D20] 统计每个元素出现次数
来源：http://hz.jlsjyb.cn/gtqfnqhpbc.html

Py:   Counter(arr)
来源：http://hz.yanxiufei.cn/gthosyites.html

PHP:  array_count_values($arr);
来源：http://hz.jinyuanbaomall.cn/gtzzsoseaq.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hysaishi.cn/gtssgmmaef.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yuxming.cn/gtuxuuiwej.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.xinyue.icu/gtblocdghu.html

Go:   // 手写 map[T]int
来源：http://hz.fzhhl.top/gtdxagqxjl.html

Ruby: arr.tally
来源：http://hz.9152youxi.cn/gtvlaqcoam.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.shanyushiyangtech.top/gtsifuowqw.html

[D21] 判断是否包含某元素
来源：http://hz.jlsjyb.cn/gtbdfkuugm.html

Py:   x in arr
来源：http://hz.pycfn.com/gtobecgvbz.html

PHP:  in_array($x, $arr, true);
来源：http://hz.yueranfly.top/gtxqqryaki.html

JS:   arr.includes(x)
来源：http://hz.zhiwuduotai.top/gtrcgcagcl.html

TS:   arr.includes(x)
来源：http://hz.chenjidiqi.icu/gtcljpujil.html

Java: list.contains(x)
来源：http://hz.jinqigufen.top/gtjsluzdok.html

Go:   slices.Contains(arr, x)
来源：http://hz.chenjidiqi.icu/gtvicttexi.html

Ruby: arr.include?(x)
来源：http://hz.svipenyu.cn/gtrdvuuxhb.html

C#:   list.Contains(x)
来源：http://hz.gogol.net.cn/gththxedry.html

[D22] 复制数组（避免共享引用）
来源：http://hz.haohaochexian.top/gtrepjjpeo.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.iojbl.cn/gtzsaldadm.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.ydjk.org.cn/gtvgnudgts.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.havefunace.top/gtxftiisdi.html

TS:   [...arr];
来源：http://hz.wangdashe.top/gtaikvusjs.html

Java: new ArrayList<>(list);
来源：http://hz.smart0.xyz/gttsqctjdc.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.havefunace.top/gtqwttmjiy.html

Ruby: arr.dup;  arr.clone
来源：http://hz.hongshengwenyu.top/gtmcvufgjm.html

C#:   new List<int>(list);
来源：http://hz.zycfv.cn/gtmujjyect.html

[D23] reduce 累积计算
来源：http://hz.vqdsnc.cn/gtrkjhpbup.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.guowangkeji.top/gttjjftxfj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.birdmap.top/gtyfblfzos.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.xylfe.cn/gtesbtdbiy.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jlsjyb.cn/gterpkcimu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.zhijiandao.cn/gttecoemaz.html

Go:   // 手写循环
来源：http://hz.shanyushiyangkeji.top/gtwzvcginh.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.yangfankeji.com/gtpjvaetlm.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.yangfankeji.com/gtllvnordr.html

[D24] 字典 / Map 基本操作
来源：http://hz.chenzaomai.com/gtmuknvylo.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.smart0.xyz/gtorwbnupt.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.quarkkingdee.top/gtxpcmpyks.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.vqdsnc.cn/gtwxsvfbdx.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.sysykeji.top/gtmvulxinq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.shzxlz.cn/gthfbzkurh.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.jianghu66.top/gtvmaaktvw.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.daxiang520.top/gttskruheg.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.hnqzz.top/gtlbkgbqxt.html

[D25] Set 集合去重与交并差
来源：http://hz.havefunace.top/gtswhkyyyl.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.yuanzhike.top/gtblvpeapz.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.0kj1m.cn/gtfxdfnivb.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.tanke756.top/gtyvdbdlaq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.cucudq.cn/gtyeztbdtb.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.guannengcc.top/gtevrbqpen.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.wangshuangyany.cn/gtexzuwfcz.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.ppjwa.cn/gtzbtcyqmw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.redwolf501.top/gtjpchyigc.html

[D26] 数组转字符串
来源：http://hz.kuanghao11.cn/gtstckjwke.html

Py:   ", ".join(map(str, arr))
来源：http://hz.jqgfzy.top/gtzayawdrm.html

PHP:  implode(", ", $arr);
来源：http://hz.daria6918.cn/gtuyfsdfbb.html

JS:   arr.join(", ")
来源：http://hz.dianchejie.cn/gtdrdqoedy.html

TS:   arr.join(", ")
来源：http://hz.shuidangran.top/gtskxulssi.html

Java: String.join(", ", list)
来源：http://hz.yangfankeji.com/gtdrbgxstn.html

Go:   strings.Join(strs, ", ")
来源：http://hz.c1oappe.top/gtwkfmzsrs.html

Ruby: arr.join(", ")
来源：http://hz.redwolf501.top/gtgrmyalcc.html

C#:   string.Join(", ", list)
来源：http://hz.gaohongyu789.top/gtadjhjcmg.html

================================================================================
来源：http://hz.yangfankeji.com/gtisdhwcsv.html

E. 字符串处理
来源：http://hz.yj202588.top/gtheuyjnsw.html

================================================================================
来源：http://hz.jinqigfzy.top/gtegambbnm.html

[E01] 拼接字符串
来源：http://hz.zhiwuduotai.top/gtlcupaqnl.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.cheryme.top/gtejofstez.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.gaohongyu789.top/gtdnddwbfa.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.kuanghao11.cn/gtfuuieans.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.gaohongyu789.top/gtscimlurj.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.shangyingyoupin.top/gtjmmawwbu.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.yj20258888.top/gtwhvyntsj.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.tanke756.top/gtebxtaigy.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.chenlongwang.top/gtuakgagzt.html

[E02] 重复字符串
来源：http://hz.xziqi.cn/gtkplujqkg.html

Py:   "ab" * 3
来源：http://hz.dashuyun.cn/gtaazszevw.html

PHP:  str_repeat("ab", 3);
来源：http://hz.yuxming.cn/gtpjohpgsi.html

JS:   "ab".repeat(3)
来源：http://hz.hywenlv.cn/gtkhomtgma.html

TS:   "ab".repeat(3)
来源：http://hz.nanxuanxn.top/gtpyocatgs.html

Java: "ab".repeat(3)
来源：http://hz.gaohongyu789.top/gtuwlotrhb.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.yj20258.top/gtfocupvln.html

Ruby: "ab" * 3
来源：http://hz.jianghu66.top/gtxtnqroks.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.daria6918.cn/gtkaxhzlvk.html

[E03] 截取子串
来源：http://hz.yangfankeji.com/gtrthyytlj.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.nanxinkj.top/gtkctzfqgw.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.ivvv.top/gtcxwifghh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.guowangkeji.top/gtbzvwwrlb.html

TS:   s.slice(1, 4)
来源：http://hz.vqdsnc.cn/gtahmqjfpw.html

Java: s.substring(1, 4)
来源：http://hz.shzxlz.cn/gtstrivaro.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.hysaishi.cn/gtaoyzsqwe.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.pycfn.com/gtfxzhwryv.html

C#:   s.Substring(1, 3)
来源：http://hz.chenlongwang.top/gtqsgxcncd.html

[E04] 查找子串位置
来源：http://hz.cucudq.cn/gtrqasjxqa.html

Py:   s.find("x");  s.index("x")
来源：http://hz.yueranfly.top/gtkleuibmd.html

PHP:  strpos($s, "x");
来源：http://hz.meibo888.top/gtzrplnmlu.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.cdnleiting.top/gtnzrxpqlj.html

TS:   s.indexOf("x")
来源：http://hz.shuidangran.top/gtvbcmlgxl.html

Java: s.indexOf("x")
来源：http://hz.ehwqpu.com/gtfdtfrtfa.html

Go:   strings.Index(s, "x")
来源：http://hz.svipenyu.cn/gteirgevmv.html

Ruby: s.index("x")
来源：http://hz.xuetiantiany.cn/gtbbdwyvej.html

C#:   s.IndexOf("x")
来源：http://hz.andypj.xyz/gtmgshakps.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.cheryme.top/gtfvptbomd.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.tanke756.top/gtuufdhjkb.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.gaohongyu789.top/gtnoqohlwe.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.birdmap.top/gtfotensma.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.cheryme.top/gtxfvmsfqb.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.sysykeji.top/gtfzjokcbg.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.chenlongwang.top/gtusigkufr.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.havefunace.top/gtptmmmgwi.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.zhijiandao.cn/gttxdinuyx.html

[E06] 替换子串
来源：http://hz.xziqi.cn/gtsashjgce.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.xinyue.icu/gtrjshgmcn.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.ydjk.org.cn/gtmzuihuil.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.9152youxi.cn/gtxzhuzmkh.html

TS:   s.replaceAll("a", "b")
来源：http://hz.shangyingyoupin.top/gtxaofnfdr.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.chenlongwang.top/gtbwmuuhxg.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.chenlongwang.top/gtrpxjgcea.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.yuanzhike.top/gtfuhcxkrx.html

C#:   s.Replace("a", "b")
来源：http://hz.hongshengwenyu.top/gtlamttdyu.html

[E07] 按分隔符拆分
来源：http://hz.yueranfly.top/gtpvupiuew.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.zhijiandao.cn/gtjbnorlzv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.jlsjyb.cn/gtzadhmgpj.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.jinqigfzy.top/gthembyigf.html

TS:   s.split(",")
来源：http://hz.sufxvd.cn/gtlvgytnew.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.ivvv.top/gtneudkkyk.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.yangfankeji.com/gtbmtczlzx.html

Ruby: s.split(",");  s.split
来源：http://hz.snrcjt.cn/gtvemynini.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.ywan-chungtsiang.top/gtjnohqdaz.html

[E08] 数组按分隔符合并
来源：http://hz.yongpay.top/gtvcbzwvbw.html

Py:   ",".join(items)
来源：http://hz.jinqigfzy.top/gtimlmquty.html

PHP:  implode(",", $items);
来源：http://hz.mhx1999.top/gtqicfseqi.html

JS:   items.join(",")
来源：http://hz.52xcode.cn/gtogdvvtls.html

TS:   items.join(",")
来源：http://hz.meibo888.top/gtdqxrdhbd.html

Java: String.join(",", items)
来源：http://hz.vqdsnc.cn/gthdmmcaot.html

Go:   strings.Join(items, ",")
来源：http://hz.ivvv.top/gtefjtryql.html

Ruby: items.join(",")
来源：http://hz.daxiang520.top/gtjadmpupr.html

C#:   string.Join(",", items)
来源：http://hz.chenjidiqi.icu/gtolsjcdwt.html

[E09] 去除所有空白字符
来源：http://hz.gzhubu.top/gtwgugyins.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.chenlongwang.top/gtemrvlvhl.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.shanyushiyangkeji.top/gtggwfdomc.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.ivvv.top/gtinrsxxlv.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.snrcjt.cn/gtaiuyxuky.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.sweek.top/gtfygwlpyt.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.dashuyun.cn/gtsszplhaf.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.cashguo.top/gtpcgqzjbn.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.meibo888.top/gtkahrxsle.html

[E10] 左侧补零 / 定长填充
来源：http://hz.ivvv.top/gtdkmfkgdd.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.sweek.top/gtzjpyqdnl.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.hnqzz.top/gtqrwhmvam.html

JS:   "7".padStart(3, "0")
来源：http://hz.smart0.xyz/gtylwranqd.html

TS:   "7".padStart(3, "0")
来源：http://hz.sufxvd.cn/gtadnauyqp.html

Java: String.format("%03d", 7)
来源：http://hz.316326.xyz/gtosrbsewf.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.shuidangran.top/gtpeixjlzw.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.zhengqikj.top/gtzypnzypx.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.0kj1m.cn/gtueletczk.html

[E11] 反转字符串
来源：http://hz.shanyushiyangkeji.top/gtrwtkeoay.html

Py:   s[::-1]
来源：http://hz.zhiwuduotai.top/gtgzccypqx.html

PHP:  strrev($s);
来源：http://hz.nwbrower.top/gtqkhxznyi.html

JS:   [...s].reverse().join("")
来源：http://hz.jlsjyb.cn/gtlbgfqicj.html

TS:   [...s].reverse().join("")
来源：http://hz.bjfxy.top/gtloywstjh.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.feifeiyinyue.top/gtemvoniwt.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.gotoacloud.top/gtabwhvabx.html


<!-- 参考信息 -->