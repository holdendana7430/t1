代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.hysaishi.cn/gtrutycpnz.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.c1oappe.top/gtswowvgfo.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.shangyingyoupin.top/gteoscgydv.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.shanyushiyangkeji.top/gtbcphezox.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.guowangkeji.top/gtqortvgyj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhengqikj.top/gtgryklnca.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.cheryme.top/gtbayoukip.html

[D06] 数组长度
来源：http://hz.smart0.xyz/gtgwtphbwn.html

Py:   len(arr)
来源：http://hz.yj20258888.top/gtdnvbxqry.html

PHP:  count($arr);
来源：http://hz.jyoumei.cn/gtiisaqkyq.html

JS:   arr.length
来源：http://hz.yueranfly.top/gtndeaucix.html

TS:   arr.length
来源：http://hz.guowangkeji.top/gtqkgovrpl.html

Java: list.size();
来源：http://hz.jinghuilouyu.cn/gtmtocyrct.html

Go:   len(arr)
来源：http://hz.aibaodan.cn/gtanneloqo.html

Ruby: arr.length; arr.size
来源：http://hz.sxryk.cn/gtszjnljfy.html

C#:   list.Count;
来源：http://hz.gaohongyu789.top/gtlnggcmva.html

[D07] 切片 / 取子数组
来源：http://hz.haohaochexian.top/gtthuefero.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.yj202588.top/gtcwowrvih.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.hywenlv.cn/gtumdjtjlh.html

JS:   arr.slice(1, 4);
来源：http://hz.pycfn.com/gtawjhziwe.html

TS:   arr.slice(1, 4);
来源：http://hz.xinyue.icu/gtswjdfeiq.html

Java: list.subList(1, 4);
来源：http://hz.wangdashe.top/gtjfhfhhxu.html

Go:   arr[1:4]
来源：http://hz.shangyingyoupin.top/gtsabevbuc.html

Ruby: arr[1, 3]
来源：http://hz.wangshuangyany.cn/gtpsbhwbad.html

C#:   list.GetRange(1, 3);
来源：http://hz.zhengqikj.top/gttuzahhay.html

[D08] 合并两个数组
来源：http://hz.vqdsnc.cn/gtkpvipuqz.html

Py:   a + b;  a.extend(b)
来源：http://hz.pycfn.com/gtuqkfaugp.html

PHP:  array_merge($a, $b);
来源：http://hz.hfpthk.cn/gtfnmthafw.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.jyoumei.cn/gtcfijnaum.html

TS:   [...a, ...b];
来源：http://hz.yuxming.cn/gttvrkfgbv.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.quarkkingdee.top/gtmkpxmfso.html

Go:   append(a, b...)
来源：http://hz.pycfn.com/gtnwfcvplm.html

Ruby: a + b;  a.concat(b)
来源：http://hz.jinqigufen.top/gtclgebjft.html

C#:   a.Concat(b).ToList()
来源：http://hz.nanxinkj.top/gtgmgaafmy.html

[D09] 排序（升序）
来源：http://hz.zdqjudy.top/gtgpyfgaph.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.bjfxy.top/gtpslmdvdd.html

PHP:  sort($arr);
来源：http://hz.ydzc1.top/gtnnrbzscc.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.shanyushiyangtech.top/gtmipmkfbr.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.yanxiufei.cn/gtqapfoibs.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.jinyuanbaomall.cn/gtvhauiqlu.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.daxiang520.top/gtqlxjronx.html

Ruby: arr.sort
来源：http://hz.chenlongwang.top/gtuarrxoyy.html

C#:   list.Sort();
来源：http://hz.cdnleiting.top/gtvquotdnb.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.52xcode.cn/gtpkxzghct.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.smart0.xyz/gtfvlrpgqz.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.daxiang520.top/gtmodoocmo.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yj20258.top/gtxluegrsc.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yuxming.cn/gtpwphfuwo.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.zdqjudy.top/gtmuuppmys.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.shuidangran.top/gtkanjcxeq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.yangfankeji.com/gtyzkfysvs.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.jqgfzy.top/gtivkvlzpm.html

[D11] 反转数组
来源：http://hz.jianghu66.top/gtujegcrob.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.quarkkingdee.top/gtmlymlvpa.html

PHP:  array_reverse($arr);
来源：http://hz.nanxinkj.top/gtweiumrhn.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.aizwys.cn/gtxnguzlye.html

TS:   [...arr].reverse();
来源：http://hz.ydjk.org.cn/gtrqerpjmn.html

Java: Collections.reverse(list);
来源：http://hz.sweek.top/gtpwttkmef.html

Go:   slices.Reverse(arr)
来源：http://hz.hnxiangtu.top/gtgzkjuxjl.html

Ruby: arr.reverse
来源：http://hz.hysaishi.cn/gtvmdzlsbp.html

C#:   list.Reverse();
来源：http://hz.shzxlz.cn/gtiebvdwng.html

[D12] 查找元素下标
来源：http://hz.dashuyun.cn/gteevpimct.html

Py:   arr.index(x);  x in arr
来源：http://hz.daxiang520.top/gtwggcsuzw.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.ydjk.org.cn/gtieygbzir.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.hywenlv.cn/gtnnqfphdb.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.sxryk.cn/gttmrlpdjg.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.ppjwa.cn/gtlueqlqrb.html

Go:   slices.Index(arr, x)
来源：http://hz.sysykeji.top/gtjdttlith.html

Ruby: arr.index(x)
来源：http://hz.nwbrower.top/gtsjoexsvd.html

C#:   list.IndexOf(x);
来源：http://hz.jinqigfzy.top/gtaterlcgl.html

[D13] 过滤（保留满足条件的）
来源：http://hz.redwolf501.top/gtukxbtrpl.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.jinyuanbaomall.cn/gtwhxwdthm.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.quarkkingdee.top/gtezftyiux.html

JS:   arr.filter(x => x > 3)
来源：http://hz.yvedp.cn/gtyrovkkot.html

TS:   arr.filter(x => x > 3)
来源：http://hz.zhixingplan.top/gtqpcxjbqh.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.0kj1m.cn/gtyrewwjqb.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.zhiwuduotai.top/gtikdnuiyl.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.ivvv.top/gtqzudppey.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.shzxlz.cn/gtoprnohup.html

[D14] 映射转换（每个元素变形）
来源：http://hz.hywenlv.cn/gttoecdozb.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.tian-w.cn/gtqtuawlyi.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.ywan-chungtsiang.top/gtvwkxeuzk.html

JS:   arr.map(x => x * 2)
来源：http://hz.zycfv.cn/gtgppbvieq.html

TS:   arr.map(x => x * 2)
来源：http://hz.nwbrower.top/gtbfmgyfdr.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.aibaodan.cn/gtuibcarsg.html

Go:   // 手写循环
来源：http://hz.cheryme.top/gtdqlccxbd.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.xuanzx.com/gtexjovfmo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.ydzc1.top/gtryucbyej.html

[D15] 去重
来源：http://hz.yueranfly.top/gtftjewklo.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.andypj.xyz/gtlrmkwefu.html

PHP:  array_unique($arr);
来源：http://hz.fengsongda.top/gtuopnpjyf.html

JS:   [...new Set(arr)]
来源：http://hz.cheryme.top/gtlerzizgh.html

TS:   [...new Set(arr)]
来源：http://hz.jinqigfzy.top/gtmmakafkm.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.guannengcc.top/gtgftbphnp.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.shangyingyoupin.top/gtympbnxxg.html

Ruby: arr.uniq
来源：http://hz.jianghu66.top/gtebbyaujp.html

C#:   list.Distinct().ToList()
来源：http://hz.shanyushiyangtech.top/gthghdtzzf.html

[D16] 求和与平均值
来源：http://hz.ydzc1.top/gtddprlhvo.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.yuanzhike.top/gtummiezpg.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.shzxlz.cn/gtmtebmmzi.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hywenlv.cn/gtirmjzrin.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.9152youxi.cn/gtzrfitxtt.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.yanxiufei.cn/gttzacptsm.html

Go:   // 手写循环累加
来源：http://hz.guowangkeji.top/gtyzbjzcoz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.ehwqpu.com/gtuvvpgivl.html

C#:   list.Sum();  list.Average()
来源：http://hz.sweek.top/gtakafmhwq.html

[D17] 最大值与最小值
来源：http://hz.aizwys.cn/gtzgqxenxe.html

Py:   max(arr);  min(arr)
来源：http://hz.sufxvd.cn/gtnsjkuewl.html

PHP:  max($arr);  min($arr);
来源：http://hz.dianchejie.cn/gttqbtpgvq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.snrcjt.cn/gtsfbudlnh.html

TS:   Math.max(...arr);
来源：http://hz.fengsongda.top/gtsgvgntfl.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.dianchejie.cn/gtxrqzjiyc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.jianghu66.top/gtuelivgji.html

Ruby: arr.max;  arr.min
来源：http://hz.ydzc1.top/gtyesfmolb.html

C#:   list.Max();  list.Min()
来源：http://hz.jinyuanbaomall.cn/gtgvnqvpnj.html

[D18] 扁平化嵌套数组
来源：http://hz.tian-w.cn/gtdslbojzr.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.jlsjyb.cn/gtognmxwbd.html

PHP:  array_merge(...$nested);
来源：http://hz.haohaochexian.top/gtfxaabilp.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.xingfuxueyuan.xyz/gtvmsjuvjz.html

TS:   nested.flat();
来源：http://hz.wangdashe.top/gtmgfotwpc.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.sufxvd.cn/gtcofwfmhe.html

Go:   // 手写双层循环
来源：http://hz.ywan-chungtsiang.top/gtqopaulra.html

Ruby: nested.flatten
来源：http://hz.jinqigfzy.top/gtphwxrpms.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.daria6918.cn/gtanbhfvpq.html

[D19] 按字段分组
来源：http://hz.tianlin.xyz/gtpzodnfiw.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.shuidangran.top/gtihhkqijq.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.svipenyu.cn/gteorampfc.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.shuidangran.top/gtfmxrpikc.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.birdmap.top/gtsjrgxrxi.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.zycfv.cn/gttwkaokmq.html

Go:   // 手写 map[string][]T
来源：http://hz.chenzaomai.com/gtfdcnqeue.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.daria6918.cn/gtaaipsdjs.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.svipenyu.cn/gtxmerftac.html

[D20] 统计每个元素出现次数
来源：http://hz.sufxvd.cn/gtpeuupkpm.html

Py:   Counter(arr)
来源：http://hz.jinqigufen.top/gtieqwzqld.html

PHP:  array_count_values($arr);
来源：http://hz.yanxiufei.cn/gtmffynrrg.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.birdmap.top/gtbacypejy.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.meibo888.top/gthtytgzjy.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.yuanzhike.top/gtxmudxfgr.html

Go:   // 手写 map[T]int
来源：http://hz.9152youxi.cn/gtmofpvmjo.html

Ruby: arr.tally
来源：http://hz.yonumen.top/gtqpnskuxs.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.xingfuxueyuan.xyz/gtwwmaaczm.html

[D21] 判断是否包含某元素
来源：http://hz.hammf.cn/gtwlmqklpw.html

Py:   x in arr
来源：http://hz.zhongyouzk.top/gtajgexttq.html

PHP:  in_array($x, $arr, true);
来源：http://hz.cashguo.top/gtnxuzyqvv.html

JS:   arr.includes(x)
来源：http://hz.xylfe.cn/gtucolnwuk.html

TS:   arr.includes(x)
来源：http://hz.shzxlz.cn/gtxrivdqsl.html

Java: list.contains(x)
来源：http://hz.jqgfzy.top/gtsxjsnrlq.html

Go:   slices.Contains(arr, x)
来源：http://hz.hammf.cn/gtxybdthpg.html

Ruby: arr.include?(x)
来源：http://hz.wangshuangyany.cn/gtlszhjksm.html

C#:   list.Contains(x)
来源：http://hz.guowangkeji.top/gtorblhbdi.html

[D22] 复制数组（避免共享引用）
来源：http://hz.cdnleiting.top/gthmbcbfah.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.cashguo.top/gtmbvynxsp.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.cheryme.top/gtwmobxqnq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.yongpay.top/gtzrhhhxjl.html

TS:   [...arr];
来源：http://hz.yongpay.top/gtqsdnhpbm.html

Java: new ArrayList<>(list);
来源：http://hz.hfpthk.cn/gtnywynfpy.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.jqgufenzy.top/gtkhaurmvu.html

Ruby: arr.dup;  arr.clone
来源：http://hz.jinghuilouyu.cn/gtrcxldfyj.html

C#:   new List<int>(list);
来源：http://hz.jlsjyb.cn/gtmsnyjuya.html

[D23] reduce 累积计算
来源：http://hz.vqdsnc.cn/gtahmunqmr.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.fzhhl.top/gtkabexzhj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.daxiang520.top/gtsxsmzhte.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.iojbl.cn/gtlexnqixo.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.hongshengwenyu.top/gtvuwhdgdx.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.hnxiangtu.top/gtmsrdkdkx.html

Go:   // 手写循环
来源：http://hz.yongpay.top/gtgojbkofj.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.yonumen.top/gtpvssufqn.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.ydzc1.top/gtcatbfmgb.html

[D24] 字典 / Map 基本操作
来源：http://hz.ywan-chungtsiang.top/gtoifzanop.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.kuanghao11.cn/gtamluehde.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.jianghu66.top/gtbriviqcq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.cucudq.cn/gtuyvonlki.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.yangfankeji.com/gtkghkyeki.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.feifeiyinyue.top/gtsoklqded.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.hysaishi.cn/gtwdwhrzpc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.yj20258888.top/gtruyeevvu.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.jqgufenzy.top/gtclbzthfi.html

[D25] Set 集合去重与交并差
来源：http://hz.zhaomingkeji.xyz/gtqyalmitq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.yuxming.cn/gtdmcgjujh.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.aizwys.cn/gtllktspti.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.dashuyun.cn/gthsbcodlg.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.hammf.cn/gtbdxcdlxi.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.iojbl.cn/gtynlfypdu.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.yonumen.top/gtxxmvfomy.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.yonumen.top/gtfguvyfrz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.yj20258888.top/gtbehxpyce.html

[D26] 数组转字符串
来源：http://hz.vqdsnc.cn/gtditelbrn.html

Py:   ", ".join(map(str, arr))
来源：http://hz.kuanghao11.cn/gtrvogbuqk.html

PHP:  implode(", ", $arr);
来源：http://hz.yanxiufei.cn/gtezqxznvq.html

JS:   arr.join(", ")
来源：http://hz.hnxiangtu.top/gtrmfcjzad.html

TS:   arr.join(", ")
来源：http://hz.yangfankeji.com/gtjryruhbd.html

Java: String.join(", ", list)
来源：http://hz.nwbrower.top/gtxtonmqxc.html

Go:   strings.Join(strs, ", ")
来源：http://hz.daxiang520.top/gtrbpmrpom.html

Ruby: arr.join(", ")
来源：http://hz.wangshuangyany.cn/gtbfrcfwwv.html

C#:   string.Join(", ", list)
来源：http://hz.jqgfzy.top/gtslqlfpxx.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtelbabvtt.html

E. 字符串处理
来源：http://hz.quarkkingdee.top/gtkcpvfflv.html

================================================================================
来源：http://hz.yueranfly.top/gtjkrnmsrc.html

[E01] 拼接字符串
来源：http://hz.sweek.top/gtzafwitdu.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.xuetiantiany.cn/gtosuqrwkf.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.xylfe.cn/gtergradqu.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.cashguo.top/gtcgeffimx.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.gaohongyu789.top/gtiwtfbhsk.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.zdqjudy.top/gtljkxaack.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.guannengcc.top/gtzbgcwpgp.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.mhx1999.top/gtnqpxkbqk.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.yangfankeji.com/gtvlalhtxa.html

[E02] 重复字符串
来源：http://hz.jinyuanbaomall.cn/gtwurlqlvy.html

Py:   "ab" * 3
来源：http://hz.0kj1m.cn/gtxzclkifs.html

PHP:  str_repeat("ab", 3);
来源：http://hz.yuxming.cn/gtndikmobt.html

JS:   "ab".repeat(3)
来源：http://hz.gzhubu.top/gtrtauyoup.html

TS:   "ab".repeat(3)
来源：http://hz.haohaochexian.top/gtgffpxycc.html

Java: "ab".repeat(3)
来源：http://hz.fzhhl.top/gteozpcyat.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.sxryk.cn/gtyyacosws.html

Ruby: "ab" * 3
来源：http://hz.jyoumei.cn/gtvmujzahp.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.zhixingplan.top/gtsbiqqjos.html

[E03] 截取子串
来源：http://hz.fzhhl.top/gtqbuiiijp.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.xuetiantiany.cn/gtcgogzvbt.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.guowangkeji.top/gtzazyxyph.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.0kj1m.cn/gtxnikusma.html

TS:   s.slice(1, 4)
来源：http://hz.svipenyu.cn/gtbgyejdzd.html

Java: s.substring(1, 4)
来源：http://hz.xuetiantiany.cn/gtaqhkjuei.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.yuanzhike.top/gttgurpijh.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.cheryme.top/gtxkzjmiru.html

C#:   s.Substring(1, 3)
来源：http://hz.yanxiufei.cn/gtlwzmypmp.html

[E04] 查找子串位置
来源：http://hz.hongshengwenyu.top/gtgyqggcbh.html

Py:   s.find("x");  s.index("x")
来源：http://hz.jiagoushi.top/gtabxtlevk.html

PHP:  strpos($s, "x");
来源：http://hz.jyoumei.cn/gtqsofsojs.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.zycfv.cn/gtnrqgukxd.html

TS:   s.indexOf("x")
来源：http://hz.cqqwz.cn/gtuzlzkyio.html

Java: s.indexOf("x")
来源：http://hz.guannengcc.top/gtevyqrifz.html

Go:   strings.Index(s, "x")
来源：http://hz.hongshengwenyu.top/gtqpfflpyz.html

Ruby: s.index("x")
来源：http://hz.fzhhl.top/gtydkfinnw.html

C#:   s.IndexOf("x")
来源：http://hz.hysaishi.cn/gtwsanfkpk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.52xcode.cn/gtgpstvdbd.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.vqdsnc.cn/gtdkumonpt.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.yuanzhike.top/gtvfnvygvg.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.hywenlv.cn/gtllitnxie.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.jianghu66.top/gtfvdhhcdm.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.52xcode.cn/gtjwqwcnoe.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.nwbrower.top/gtfszddeah.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.xylfe.cn/gtvqocgbwe.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.hfpthk.cn/gtwgmzhskx.html

[E06] 替换子串
来源：http://hz.chenlongwang.top/gtfpjmkuzs.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.jinqigfzy.top/gtauvtcoqo.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.hysaishi.cn/gtjwlxtizn.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.cdnleiting.top/gtxgkmruqe.html

TS:   s.replaceAll("a", "b")
来源：http://hz.hammf.cn/gtulxntzow.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.meibo888.top/gtzlsvtdmr.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.xuanzx.com/gtmksxndbq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.hnqzz.top/gtgesmzgck.html

C#:   s.Replace("a", "b")
来源：http://hz.pycfn.com/gtyxiynlwa.html

[E07] 按分隔符拆分
来源：http://hz.feifeiyinyue.top/gtqygcpmtk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.quarkkingdee.top/gtajygjvus.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.mhx1999.top/gtcxpqaauz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.zhiwuduotai.top/gtrvhwgfvq.html

TS:   s.split(",")
来源：http://hz.gotoacloud.top/gtrawebvel.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.ehwqpu.com/gtnwyfdway.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.jinqigfzy.top/gtrenefwpa.html

Ruby: s.split(",");  s.split
来源：http://hz.tianlin.xyz/gtnipnwvwf.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.snrcjt.cn/gtzktjzkce.html

[E08] 数组按分隔符合并
来源：http://hz.jqgufenzy.top/gttwdyfomc.html

Py:   ",".join(items)
来源：http://hz.9152youxi.cn/gtwryijupk.html

PHP:  implode(",", $items);
来源：http://hz.gotoacloud.top/gtltwiqhkb.html

JS:   items.join(",")
来源：http://hz.fzhhl.top/gtqudmujsj.html

TS:   items.join(",")
来源：http://hz.zhiwuduotai.top/gtmdywqhpz.html

Java: String.join(",", items)
来源：http://hz.hammf.cn/gtvmybnugp.html

Go:   strings.Join(items, ",")
来源：http://hz.xuanzx.com/gttltuyytq.html

Ruby: items.join(",")
来源：http://hz.9152youxi.cn/gtgumozfho.html

C#:   string.Join(",", items)
来源：http://hz.ydzc1.top/gtoiiivtxg.html

[E09] 去除所有空白字符
来源：http://hz.cheryme.top/gtzogdipeb.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.zhaomingkeji.xyz/gtsrddnkon.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.jinqigufen.top/gtiirdfzpd.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.0kj1m.cn/gtyunuqyuc.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.shangyingyoupin.top/gthcjzagbs.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.hammf.cn/gtdgeouowj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.guowangkeji.top/gtznsqdbry.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.redwolf501.top/gtctaqjhyp.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.hywenlv.cn/gtxkomwmze.html

[E10] 左侧补零 / 定长填充
来源：http://hz.chenlongwang.top/gtchzhljcw.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.zdqjudy.top/gttdsxnqse.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.hnqzz.top/gtythvluks.html

JS:   "7".padStart(3, "0")
来源：http://hz.shanyushiyangkeji.top/gthxyxjgoy.html

TS:   "7".padStart(3, "0")
来源：http://hz.daxiang520.top/gtjqrunefz.html

Java: String.format("%03d", 7)
来源：http://hz.vqdsnc.cn/gtsgsfkifs.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.vqdsnc.cn/gtobszlskr.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.zhijiandao.cn/gthveuvekg.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.xziqi.cn/gtghypirco.html

[E11] 反转字符串
来源：http://hz.jqgfzy.top/gtpkilbbhy.html

Py:   s[::-1]
来源：http://hz.tian-w.cn/gtxbvaavsz.html

PHP:  strrev($s);
来源：http://hz.ydjk.org.cn/gtkrdzpmkj.html

JS:   [...s].reverse().join("")
来源：http://hz.aibaodan.cn/gtprwrgqqe.html

TS:   [...s].reverse().join("")
来源：http://hz.dashuyun.cn/gthqkqmsei.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.yvedp.cn/gtrmmuiphs.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.hammf.cn/gttusheybw.html

Ruby: s.reverse
来源：http://hz.yj20258888.top/gtdcsieren.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.jianghu66.top/gtmcbnrhpt.html

[E12] 统计某字符出现次数
来源：http://hz.zycfv.cn/gtgbejqshr.html

Py:   s.count("a")
来源：http://hz.gotoacloud.top/gthemmghlj.html


<!-- 参考信息 -->