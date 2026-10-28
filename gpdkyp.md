代发 wailian999

C#:   list.Insert(0, 0);
来源：http://hz.chenzaomai.com/gtnujuvbhn.html

[D04] 删除元素
来源：http://hz.zhongyouzk.top/gtmrlwvtpo.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.mhx1999.top/gtcmgfdkjb.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.shanyushiyangkeji.top/gtjkimsxiv.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.hongshengwenyu.top/gttvxysknm.html

TS:   arr.splice(0, 1);
来源：http://hz.svipenyu.cn/gtvgcyuhfr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.yuanzhike.top/gthfvclgld.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.chenlongwang.top/gtovpavegq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.gogol.net.cn/gtjqtdqrxu.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.bjfxy.top/gtnuovenqy.html

[D05] 访问与修改元素
来源：http://hz.sysykeji.top/gteqyftyze.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.52xcode.cn/gtzwfqcuss.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.gaohongyu789.top/gtquwcxnyw.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.redwolf501.top/gtgwbwvbaq.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.52xcode.cn/gtfhmpcqat.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.0kj1m.cn/gtossdjtav.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.mhx1999.top/gtmtezbzew.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jqgufenzy.top/gtolbnpsuq.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.sufxvd.cn/gtnhbtwpfd.html

[D06] 数组长度
来源：http://hz.cheryme.top/gtyokekzul.html

Py:   len(arr)
来源：http://hz.quarkkingdee.top/gtjrgjkcub.html

PHP:  count($arr);
来源：http://hz.tian-w.cn/gtkomdnfgo.html

JS:   arr.length
来源：http://hz.svipenyu.cn/gtyuliqzsl.html

TS:   arr.length
来源：http://hz.hysaishi.cn/gthtowefgo.html

Java: list.size();
来源：http://hz.gaohongyu789.top/gtxzytnhoo.html

Go:   len(arr)
来源：http://hz.jqgfzy.top/gthedeqeya.html

Ruby: arr.length; arr.size
来源：http://hz.mhx1999.top/gthvyrbtba.html

C#:   list.Count;
来源：http://hz.quarkkingdee.top/gtqxxlydzz.html

[D07] 切片 / 取子数组
来源：http://hz.chenlongwang.top/gtmxizcxgh.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.gzhubu.top/gtqsurdjnv.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.xingfuxueyuan.xyz/gtesmcpaqg.html

JS:   arr.slice(1, 4);
来源：http://hz.xziqi.cn/gtsldadsnw.html

TS:   arr.slice(1, 4);
来源：http://hz.52xcode.cn/gtitrkjbgg.html

Java: list.subList(1, 4);
来源：http://hz.fzhhl.top/gtbdxqviwj.html

Go:   arr[1:4]
来源：http://hz.chenlongwang.top/gtxtlqaqls.html

Ruby: arr[1, 3]
来源：http://hz.andypj.xyz/gtxcpwjycm.html

C#:   list.GetRange(1, 3);
来源：http://hz.tian-w.cn/gtifpatlnu.html

[D08] 合并两个数组
来源：http://hz.xuetiantiany.cn/gtfhspxrgb.html

Py:   a + b;  a.extend(b)
来源：http://hz.chenlongwang.top/gtkpcvgonp.html

PHP:  array_merge($a, $b);
来源：http://hz.zhijiandao.cn/gtefigfplp.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.quarkkingdee.top/gtatasayzk.html

TS:   [...a, ...b];
来源：http://hz.meibo888.top/gtszoguxtm.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.yangfankeji.com/gtucsdcywf.html

Go:   append(a, b...)
来源：http://hz.birdmap.top/gtcrgcxvrt.html

Ruby: a + b;  a.concat(b)
来源：http://hz.sweek.top/gtxpcodiyu.html

C#:   a.Concat(b).ToList()
来源：http://hz.xziqi.cn/gtywjobvgx.html

[D09] 排序（升序）
来源：http://hz.xuanzx.com/gtpladshvc.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.daxiang520.top/gttwphgdws.html

PHP:  sort($arr);
来源：http://hz.ydzc1.top/gtxazwxwhy.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.ydjk.org.cn/gtkauudmie.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.ivvv.top/gtmhfbnfmy.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.bjfxy.top/gtuidhgjwu.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.jinghuilouyu.cn/gttmoxxwcw.html

Ruby: arr.sort
来源：http://hz.zhixingplan.top/gtzoatrtmz.html

C#:   list.Sort();
来源：http://hz.guannengcc.top/gtmrmreprr.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.ywan-chungtsiang.top/gtpstiikmv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.yueranfly.top/gtqfcrlhuc.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.316326.xyz/gtnicgolbc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jiagoushi.top/gttpcnsaxs.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xinyue.icu/gtzyxckegp.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.zhengqikj.top/gtyanfnrha.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.xylfe.cn/gtzfixgrpl.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.haohaochexian.top/gtnvhddohi.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.fengsongda.top/gtsvsbvkcu.html

[D11] 反转数组
来源：http://hz.zdqjudy.top/gtxfejukwc.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.ivvv.top/gtkodwwyqe.html

PHP:  array_reverse($arr);
来源：http://hz.zhiwuduotai.top/gtcdtjmqhj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.c1oappe.top/gtluoesyuj.html

TS:   [...arr].reverse();
来源：http://hz.0kj1m.cn/gtxpgkpele.html

Java: Collections.reverse(list);
来源：http://hz.hammf.cn/gtdcqcvmfb.html

Go:   slices.Reverse(arr)
来源：http://hz.chenlongwang.top/gtdpovutxp.html

Ruby: arr.reverse
来源：http://hz.tianlin.xyz/gtalfkuovg.html

C#:   list.Reverse();
来源：http://hz.quarkkingdee.top/gthviugsys.html

[D12] 查找元素下标
来源：http://hz.zhixingplan.top/gtalcwwxui.html

Py:   arr.index(x);  x in arr
来源：http://hz.cdnleiting.top/gtvpiluldf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.jinqigfzy.top/gtavksartl.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yj20258.top/gtwvwjtwed.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.tianlin.xyz/gtbazlsdnl.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.9152youxi.cn/gtadayfblj.html

Go:   slices.Index(arr, x)
来源：http://hz.gzhubu.top/gtisrqdfus.html

Ruby: arr.index(x)
来源：http://hz.kuanghao11.cn/gthuzgvkpu.html

C#:   list.IndexOf(x);
来源：http://hz.316326.xyz/gtcfurxjrh.html

[D13] 过滤（保留满足条件的）
来源：http://hz.yj20258888.top/gtehisdyqv.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.bjfxy.top/gtwdoxpaiu.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.svipenyu.cn/gtpdyrqfic.html

JS:   arr.filter(x => x > 3)
来源：http://hz.bjfxy.top/gtankyqhhj.html

TS:   arr.filter(x => x > 3)
来源：http://hz.jlsjyb.cn/gtpmkgeudb.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.zhiwuduotai.top/gtxievjmsj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.pengpengdd.cyou/gtlqjlutes.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.redwolf501.top/gtybgqlhth.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.shzxlz.cn/gtkluqnxjw.html

[D14] 映射转换（每个元素变形）
来源：http://hz.cucudq.cn/gtovxmevma.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.ywan-chungtsiang.top/gtmtewixsq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.iojbl.cn/gtsisieuvv.html

JS:   arr.map(x => x * 2)
来源：http://hz.svipenyu.cn/gtapuhlxwr.html

TS:   arr.map(x => x * 2)
来源：http://hz.shangyingyoupin.top/gtekrhltbs.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.tanke756.top/gtcpgxvyyo.html

Go:   // 手写循环
来源：http://hz.shanyushiyangkeji.top/gtwwszyadj.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.zhoulong.xyz/gtwkvfnnqh.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.nanxuanxn.top/gtpuxxkpsm.html

[D15] 去重
来源：http://hz.yonumen.top/gthhkcvtpv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.gotoacloud.top/gtacmnartk.html

PHP:  array_unique($arr);
来源：http://hz.0kj1m.cn/gttpvscnye.html

JS:   [...new Set(arr)]
来源：http://hz.yanxiufei.cn/gtizwzrchv.html

TS:   [...new Set(arr)]
来源：http://hz.52xcode.cn/gtqphwjujq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.daria6918.cn/gtkqqqagkd.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.hammf.cn/gtolsqwvza.html

Ruby: arr.uniq
来源：http://hz.snrcjt.cn/gtnnywfzft.html

C#:   list.Distinct().ToList()
来源：http://hz.zdqjudy.top/gtvqbuaumo.html

[D16] 求和与平均值
来源：http://hz.xingfuxueyuan.xyz/gtiuwyvgam.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.tanke756.top/gtbznanoet.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.guowangkeji.top/gtmrsqhrdn.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.gogol.net.cn/gtlbaypftj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.wangdashe.top/gtjplcmvjq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.cdnleiting.top/gtdqayjcls.html

Go:   // 手写循环累加
来源：http://hz.jinghuilouyu.cn/gthdhhaggz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.zycfv.cn/gtofoaxcbk.html

C#:   list.Sum();  list.Average()
来源：http://hz.cqqwz.cn/gtlvfeergu.html

[D17] 最大值与最小值
来源：http://hz.feifeiyinyue.top/gtheidntou.html

Py:   max(arr);  min(arr)
来源：http://hz.tanke756.top/gtxbyqsldf.html

PHP:  max($arr);  min($arr);
来源：http://hz.pycfn.com/gtdabiwbgp.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.snrcjt.cn/gtfibugflq.html

TS:   Math.max(...arr);
来源：http://hz.yongpay.top/gtganhkicv.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.jqgfzy.top/gtieiimlwk.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.pengpengdd.cyou/gthnlwkapb.html

Ruby: arr.max;  arr.min
来源：http://hz.kuanghao11.cn/gtwlysocnt.html

C#:   list.Max();  list.Min()
来源：http://hz.gogol.net.cn/gtlrwreckd.html

[D18] 扁平化嵌套数组
来源：http://hz.nwbrower.top/gtryfbertf.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.feifeiyinyue.top/gtksrrlbsm.html

PHP:  array_merge(...$nested);
来源：http://hz.yongpay.top/gtksozxnox.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.hywenlv.cn/gtmegopljd.html

TS:   nested.flat();
来源：http://hz.zycfv.cn/gthzueqamx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.andypj.xyz/gtbivotprp.html

Go:   // 手写双层循环
来源：http://hz.shzxlz.cn/gtfmscjpfl.html

Ruby: nested.flatten
来源：http://hz.hfpthk.cn/gtcqjdtqkk.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.shzxlz.cn/gtakagyiyj.html

[D19] 按字段分组
来源：http://hz.aizwys.cn/gtiqawtaoc.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.zhixingplan.top/gtozgmaxxx.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.cashguo.top/gtznnnbegd.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.zhongyouzk.top/gtcrevziln.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.ydzc1.top/gtyguwvfzs.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.hfpthk.cn/gtjibasgbh.html

Go:   // 手写 map[string][]T
来源：http://hz.jqgufenzy.top/gttgrzquct.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.yj202588.top/gtjqglbipa.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.hongshengwenyu.top/gtbfdpounn.html

[D20] 统计每个元素出现次数
来源：http://hz.feifeiyinyue.top/gtdkwghqne.html

Py:   Counter(arr)
来源：http://hz.tian-w.cn/gteicsomar.html

PHP:  array_count_values($arr);
来源：http://hz.aibaodan.cn/gtezfayrav.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hammf.cn/gthsucqymy.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.svipenyu.cn/gtgdwgvqum.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.shanyushiyangtech.top/gtsmtqmwou.html

Go:   // 手写 map[T]int
来源：http://hz.cdnleiting.top/gtxmjrkvwd.html

Ruby: arr.tally
来源：http://hz.kuanghao11.cn/gtmrwfxner.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.yj20258.top/gtzfzwxusf.html

[D21] 判断是否包含某元素
来源：http://hz.shanyushiyangkeji.top/gtmqiccxge.html

Py:   x in arr
来源：http://hz.chenlongwang.top/gtsragedyr.html

PHP:  in_array($x, $arr, true);
来源：http://hz.ydjk.org.cn/gtvrbdjitz.html

JS:   arr.includes(x)
来源：http://hz.jianghu66.top/gtsacqjjjs.html

TS:   arr.includes(x)
来源：http://hz.smart0.xyz/gtvocpnvdp.html

Java: list.contains(x)
来源：http://hz.hywenlv.cn/gtaapastbc.html

Go:   slices.Contains(arr, x)
来源：http://hz.cashguo.top/gtnwubngsw.html

Ruby: arr.include?(x)
来源：http://hz.tian-w.cn/gtdrrlyllv.html

C#:   list.Contains(x)
来源：http://hz.jyoumei.cn/gtcsmvhcec.html

[D22] 复制数组（避免共享引用）
来源：http://hz.jyoumei.cn/gtcecvdpcy.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.jinyuanbaomall.cn/gtdjcvhxhi.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.vqdsnc.cn/gtbhtorafa.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.daxiang520.top/gtierjzreu.html

TS:   [...arr];
来源：http://hz.kuanghao11.cn/gtuxqfgmpx.html

Java: new ArrayList<>(list);
来源：http://hz.jqgufenzy.top/gtxybwkbwu.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.cqqwz.cn/gtajxsxlzb.html

Ruby: arr.dup;  arr.clone
来源：http://hz.jqgfzy.top/gtediolqcn.html

C#:   new List<int>(list);
来源：http://hz.sweek.top/gtalhdlyol.html

[D23] reduce 累积计算
来源：http://hz.andypj.xyz/gtygjpwvwa.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.ybcxt.top/gtwiexqlsz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.vqdsnc.cn/gtmvupwnla.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.nanxinkj.top/gtvizxqoju.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.aizwys.cn/gtutxdybvn.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.ydjk.org.cn/gtqdnkutfw.html

Go:   // 手写循环
来源：http://hz.hywenlv.cn/gtihxemcsw.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.fzhhl.top/gtnadnkdbz.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.hongshengwenyu.top/gtjhkzgazq.html

[D24] 字典 / Map 基本操作
来源：http://hz.jianghu66.top/gtxclugvnv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.sysykeji.top/gtwbbocyue.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.jqgufenzy.top/gtneomskgu.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.ehwqpu.com/gtwxwcorjt.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.hfpthk.cn/gtvcowedhv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.yj20258888.top/gttanjjbtb.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.yuanzhike.top/gtsonhglxn.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.iojbl.cn/gtenlkrumr.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.snrcjt.cn/gtaczcbjqa.html

[D25] Set 集合去重与交并差
来源：http://hz.svipenyu.cn/gtflyaugwb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.zdqjudy.top/gtgtgeqkeu.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.zhaomingkeji.xyz/gtngohxxoz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.ivvv.top/gttbqhrvyz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.jinghuilouyu.cn/gtfsxlwjtm.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.guowangkeji.top/gtiukncvld.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.yuxming.cn/gtzfhoyykh.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.wangshuangyany.cn/gtistupbvd.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.yuanzhike.top/gthdfvqgyl.html

[D26] 数组转字符串
来源：http://hz.tanke756.top/gtyusvcqgr.html

Py:   ", ".join(map(str, arr))
来源：http://hz.xuetiantiany.cn/gtfiteoaql.html

PHP:  implode(", ", $arr);
来源：http://hz.yj202588.top/gtuznfyvrm.html

JS:   arr.join(", ")
来源：http://hz.jinqigfzy.top/gtpifqbqjg.html

TS:   arr.join(", ")
来源：http://hz.feifeiyinyue.top/gtbwyywlqa.html

Java: String.join(", ", list)
来源：http://hz.ywan-chungtsiang.top/gtwjcbdcuc.html

Go:   strings.Join(strs, ", ")
来源：http://hz.nanxinkj.top/gtdqrusbtv.html

Ruby: arr.join(", ")
来源：http://hz.ydjk.org.cn/gtixtqueaa.html

C#:   string.Join(", ", list)
来源：http://hz.jianghu66.top/gtzdzoptjj.html

================================================================================
来源：http://hz.pengpengdd.cyou/gttsfmgcvl.html

E. 字符串处理
来源：http://hz.zhixingplan.top/gtndtrcdrg.html

================================================================================
来源：http://hz.quarkkingdee.top/gtwioopohb.html

[E01] 拼接字符串
来源：http://hz.cheryme.top/gtemkeyqcs.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.xziqi.cn/gtgaockblx.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.redwolf501.top/gtrgjsfbwy.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.kuanghao11.cn/gtvbufkezv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.sufxvd.cn/gtrvvmgvrd.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.cqqwz.cn/gtzqnkwqry.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.mhx1999.top/gtblsqpitx.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.smart0.xyz/gtpqdubgkm.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.chenzaomai.com/gtpfujgyzx.html

[E02] 重复字符串
来源：http://hz.quarkkingdee.top/gtrevmjted.html

Py:   "ab" * 3
来源：http://hz.zdqjudy.top/gtgpaqfhpk.html

PHP:  str_repeat("ab", 3);
来源：http://hz.yvedp.cn/gtrogkfjfv.html

JS:   "ab".repeat(3)
来源：http://hz.dashuyun.cn/gtjlhhwsjn.html

TS:   "ab".repeat(3)
来源：http://hz.ywan-chungtsiang.top/gtrjocfmfy.html

Java: "ab".repeat(3)
来源：http://hz.birdmap.top/gtbioxbkps.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.tanke756.top/gtzqxjbieh.html

Ruby: "ab" * 3
来源：http://hz.xylfe.cn/gtamcvnqjw.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.jinyuanbaomall.cn/gtyfhwlvqn.html

[E03] 截取子串
来源：http://hz.andypj.xyz/gtxlwgynfj.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.tanke756.top/gtqqojafjn.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.yuxming.cn/gtyjyaeyyz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.feifeiyinyue.top/gtryetmrun.html

TS:   s.slice(1, 4)
来源：http://hz.316326.xyz/gtegwvagsg.html

Java: s.substring(1, 4)
来源：http://hz.jqgufenzy.top/gteoamcymv.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.xuetiantiany.cn/gtfolddpgm.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.316326.xyz/gtcruaajun.html

C#:   s.Substring(1, 3)
来源：http://hz.yj20258888.top/gttzzbweny.html

[E04] 查找子串位置
来源：http://hz.gzhubu.top/gtwhttnexg.html

Py:   s.find("x");  s.index("x")
来源：http://hz.gaohongyu789.top/gtnrlawtea.html

PHP:  strpos($s, "x");
来源：http://hz.hongshengwenyu.top/gthesiahwm.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.tanke756.top/gtiedieyjm.html

TS:   s.indexOf("x")
来源：http://hz.jqgfzy.top/gtchonaabl.html

Java: s.indexOf("x")
来源：http://hz.shanyushiyangkeji.top/gteuqmfuwx.html

Go:   strings.Index(s, "x")
来源：http://hz.daxiang520.top/gtyghrfkfp.html

Ruby: s.index("x")
来源：http://hz.cheryme.top/gtgclbtibs.html

C#:   s.IndexOf("x")
来源：http://hz.shzxlz.cn/gtjuqpkaqy.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.yuxming.cn/gtubsweslo.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.yj20258.top/gtnhuosrpt.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.cdnleiting.top/gtzporoaml.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.daxiang520.top/gttnvlnksv.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.redwolf501.top/gtnupazngi.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.iojbl.cn/gtymbcukeq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.52xcode.cn/gtrbeiaiwa.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.ybcxt.top/gtmzfzkzgt.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.iojbl.cn/gtaonjuvhd.html

[E06] 替换子串
来源：http://hz.yuanzhike.top/gtydgdwtff.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.yj202588.top/gtguaddyvl.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.cqqwz.cn/gtmmjsqgsu.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jlsjyb.cn/gtcjglmlks.html

TS:   s.replaceAll("a", "b")
来源：http://hz.9152youxi.cn/gtewxdsgzm.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.xinyue.icu/gtmygohete.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.chenzaomai.com/gtlhgykypj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.jqgufenzy.top/gtjtpidwhg.html

C#:   s.Replace("a", "b")
来源：http://hz.dianchejie.cn/gtnrrsvuvv.html

[E07] 按分隔符拆分
来源：http://hz.xinyue.icu/gtlipqcbsf.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.zhengqikj.top/gtvmnoalhp.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.wangdashe.top/gteuurnwwz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.nanxinkj.top/gteixacnoi.html

TS:   s.split(",")
来源：http://hz.guowangkeji.top/gtjkmmxizr.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.cqqwz.cn/gtrkjpbyta.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.cashguo.top/gtsriwdwvj.html

Ruby: s.split(",");  s.split
来源：http://hz.zycfv.cn/gtpmjyyapd.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.daxiang520.top/gtrttvyvud.html

[E08] 数组按分隔符合并
来源：http://hz.c1oappe.top/gtrgzrcxlo.html

Py:   ",".join(items)
来源：http://hz.feifeiyinyue.top/gtinivxzzj.html

PHP:  implode(",", $items);
来源：http://hz.quarkkingdee.top/gtawmwcrns.html

JS:   items.join(",")
来源：http://hz.wangshuangyany.cn/gtfyquxlwz.html

TS:   items.join(",")
来源：http://hz.guowangkeji.top/gtjojzufhq.html

Java: String.join(",", items)
来源：http://hz.xingfuxueyuan.xyz/gtekaurtma.html

Go:   strings.Join(items, ",")
来源：http://hz.jlsjyb.cn/gtfnesrsnv.html

Ruby: items.join(",")
来源：http://hz.jinqigfzy.top/gtzjvdrfjg.html

C#:   string.Join(",", items)
来源：http://hz.vqdsnc.cn/gtcqfdyebc.html

[E09] 去除所有空白字符
来源：http://hz.shzxlz.cn/gtfuhfacqy.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.hfpthk.cn/gtccwjpars.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.zhengqikj.top/gtljfmgqwg.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.yj20258.top/gtobkxhdxv.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.hfpthk.cn/gtzbwidlrt.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.yj20258.top/gtncmxbjco.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.xziqi.cn/gtxmatidqa.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.xuanzx.com/gtuddnvcsl.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.zdqjudy.top/gtrghtzgxk.html

[E10] 左侧补零 / 定长填充
来源：http://hz.xuanzx.com/gtobvzkuaf.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.tianlin.xyz/gtxrkeduam.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.jianghu66.top/gtwcdqckfv.html

JS:   "7".padStart(3, "0")
来源：http://hz.hnxiangtu.top/gtsmwmixes.html

TS:   "7".padStart(3, "0")
来源：http://hz.dashuyun.cn/gtmuqcnjwj.html

Java: String.format("%03d", 7)
来源：http://hz.tianlin.xyz/gtpzqkgyyk.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.yj20258888.top/gtspwhnsim.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.c1oappe.top/gtuifnhljj.html


<!-- 参考信息 -->