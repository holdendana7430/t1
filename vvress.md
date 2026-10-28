代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.jinyuanbaomall.cn/gtusliodmk.html

[C15] 解构 / 展开参数
来源：http://hz.birdmap.top/gtsixvnzxa.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.yanxiufei.cn/gthcguvfdp.html

PHP:  [$a, $b] = $pair;
来源：http://hz.andypj.xyz/gtnjyeqeze.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.sweek.top/gtnbukionm.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.gogol.net.cn/gtzfsvyafq.html

Java: // 无解构
来源：http://hz.daria6918.cn/gtpqwnuxgt.html

Go:   // 无解构
来源：http://hz.zhiwuduotai.top/gtfwgojwnw.html

Ruby: a, b = pair
来源：http://hz.nanxuanxn.top/gtnvugpwgs.html

C#:   var (a, b) = pair;
来源：http://hz.shzxlz.cn/gtodzevmbu.html

[C16] 函数 / 方法重载
来源：http://hz.zhongyouzk.top/gtpjdskgmb.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.zhiwuduotai.top/gtsxmtugdv.html

PHP:  // 无重载
来源：http://hz.xinyue.icu/gtvuunxteg.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.zycfv.cn/gtjhvdxkqp.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.guowangkeji.top/gtjiesikkc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.zhixingplan.top/gtinnwxtrn.html

Go:   // 无重载：用不同函数名
来源：http://hz.hammf.cn/gtetuxkupl.html

Ruby: # 无重载：靠动态参数
来源：http://hz.guannengcc.top/gtxdrfbkgn.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.hammf.cn/gtgpmnvrkp.html

================================================================================
来源：http://hz.cheryme.top/gtmgrdtbeo.html

D. 数组 / 列表 / 集合
来源：http://hz.zhijiandao.cn/gtlhnfoqvk.html

================================================================================
来源：http://hz.jinqigufen.top/gtigtmrfgo.html

[D01] 创建数组 / 列表
来源：http://hz.sysykeji.top/gtebotuuyn.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.redwolf501.top/gtfjeeinnz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.zycfv.cn/gtbloqomem.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.zhoulong.xyz/gtvdhjpxgy.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.iojbl.cn/gtjemozurm.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.sxryk.cn/gtvhmechyw.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.snrcjt.cn/gtggsxuenv.html

Ruby: arr = [1, 2, 3]
来源：http://hz.redwolf501.top/gtvzctvgtf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.shanyushiyangkeji.top/gtesuizqch.html

[D02] 追加元素到末尾
来源：http://hz.redwolf501.top/gtffptctez.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.svipenyu.cn/gtbzuotrej.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.jinyuanbaomall.cn/gtbyjjrgcp.html

JS:   arr.push(4);
来源：http://hz.aizwys.cn/gtarkhuops.html

TS:   arr.push(4);
来源：http://hz.andypj.xyz/gtpocsqujq.html

Java: list.add(4);
来源：http://hz.ehwqpu.com/gtdzsgwcre.html

Go:   arr = append(arr, 4)
来源：http://hz.jqgufenzy.top/gtxplocjyu.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.tianlin.xyz/gtzgudrzes.html

C#:   list.Add(4);
来源：http://hz.gogol.net.cn/gtaxfrvgru.html

[D03] 在指定位置插入元素
来源：http://hz.daria6918.cn/gtgnzfaagb.html

Py:   arr.insert(0, 0)
来源：http://hz.cashguo.top/gtetnylljr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.gotoacloud.top/gtthjbotyz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.jinqigfzy.top/gtrkvhjfdh.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.xinyue.icu/gtvrngbztx.html

Java: list.add(0, 0);
来源：http://hz.fengsongda.top/gtccsdtztn.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.shanyushiyangtech.top/gtkleradtl.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.nwbrower.top/gttfwsfrzk.html

C#:   list.Insert(0, 0);
来源：http://hz.hfpthk.cn/gtpqxtpspd.html

[D04] 删除元素
来源：http://hz.pycfn.com/gtjvdoccul.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.yonumen.top/gtluswengm.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.nanxinkj.top/gtkdvloonc.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.vqdsnc.cn/gthukkbypk.html

TS:   arr.splice(0, 1);
来源：http://hz.chenjidiqi.icu/gttiqllqgo.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.jinqigfzy.top/gtukcujexu.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.yuxming.cn/gtrjilkoju.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.shanyushiyangkeji.top/gtkgjzpcmh.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.smart0.xyz/gtgrguhzem.html

[D05] 访问与修改元素
来源：http://hz.xuetiantiany.cn/gtfkunksrb.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zycfv.cn/gtotxalhni.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.nanxinkj.top/gtavhdupkr.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.vqdsnc.cn/gtgzaxhjqf.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.kuanghao11.cn/gtpctpwkhh.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.hysaishi.cn/gtntvjiasn.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.gotoacloud.top/gttikljsje.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hammf.cn/gtqlhhidrk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.sufxvd.cn/gtemwgpnva.html

[D06] 数组长度
来源：http://hz.ywan-chungtsiang.top/gtalxtaajc.html

Py:   len(arr)
来源：http://hz.nanxuanxn.top/gtrztrkylb.html

PHP:  count($arr);
来源：http://hz.aizwys.cn/gtfspayoaj.html

JS:   arr.length
来源：http://hz.0kj1m.cn/gtvpatygbe.html

TS:   arr.length
来源：http://hz.ydjk.org.cn/gttqfcetfj.html

Java: list.size();
来源：http://hz.tianlin.xyz/gthqlbypri.html

Go:   len(arr)
来源：http://hz.cdnleiting.top/gtojbjajfp.html

Ruby: arr.length; arr.size
来源：http://hz.shanyushiyangtech.top/gtmgwwrioq.html

C#:   list.Count;
来源：http://hz.vqdsnc.cn/gtudlkcgrr.html

[D07] 切片 / 取子数组
来源：http://hz.xuanzx.com/gtawsfkebt.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.shangyingyoupin.top/gtdbwmtvxg.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.ivvv.top/gteiwplibp.html

JS:   arr.slice(1, 4);
来源：http://hz.hysaishi.cn/gtwcbutwak.html

TS:   arr.slice(1, 4);
来源：http://hz.yj202588.top/gtyaubzlch.html

Java: list.subList(1, 4);
来源：http://hz.c1oappe.top/gtmykjhllh.html

Go:   arr[1:4]
来源：http://hz.nanxinkj.top/gtrcarrltk.html

Ruby: arr[1, 3]
来源：http://hz.chenzaomai.com/gtnlyzmdmo.html

C#:   list.GetRange(1, 3);
来源：http://hz.wangshuangyany.cn/gtwthiwniw.html

[D08] 合并两个数组
来源：http://hz.gogol.net.cn/gtxzmnnccx.html

Py:   a + b;  a.extend(b)
来源：http://hz.haohaochexian.top/gtzfqnvhjp.html

PHP:  array_merge($a, $b);
来源：http://hz.zhaomingkeji.xyz/gteucjhwkb.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.9152youxi.cn/gtqhpmwzlt.html

TS:   [...a, ...b];
来源：http://hz.dashuyun.cn/gtxzdeiijs.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.zhixingplan.top/gtbrvgycfa.html

Go:   append(a, b...)
来源：http://hz.c1oappe.top/gtaijxigih.html

Ruby: a + b;  a.concat(b)
来源：http://hz.shanyushiyangkeji.top/gtchlhgvyw.html

C#:   a.Concat(b).ToList()
来源：http://hz.zhongyouzk.top/gtjhococbz.html

[D09] 排序（升序）
来源：http://hz.hammf.cn/gtjykyfozs.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ehwqpu.com/gtpmfckhrd.html

PHP:  sort($arr);
来源：http://hz.jqgfzy.top/gtsxjfanpj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.guannengcc.top/gtubzsyhaa.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.zhaomingkeji.xyz/gtprptnjyx.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.hongshengwenyu.top/gtwhnksiop.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.dashuyun.cn/gtrvxdwsos.html

Ruby: arr.sort
来源：http://hz.zhiwuduotai.top/gtaueoylhd.html

C#:   list.Sort();
来源：http://hz.quarkkingdee.top/gtsxdhcfgw.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.snrcjt.cn/gttbjkqcfl.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.chenlongwang.top/gtplexnntg.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yj20258888.top/gtukdfqzje.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.ybcxt.top/gtzpdhkezt.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.chenjidiqi.icu/gthxbdlkqg.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.jinghuilouyu.cn/gticezgvrw.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.havefunace.top/gtwpbownhs.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.jinyuanbaomall.cn/gtsqkcrvah.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.jqgufenzy.top/gtelurhvez.html

[D11] 反转数组
来源：http://hz.yuxming.cn/gtptakphoj.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.aizwys.cn/gtpcwcxjya.html

PHP:  array_reverse($arr);
来源：http://hz.jlsjyb.cn/gtmkjjgtgr.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.yj20258888.top/gtkrpmloaq.html

TS:   [...arr].reverse();
来源：http://hz.kuanghao11.cn/gtfkjxxlta.html

Java: Collections.reverse(list);
来源：http://hz.daxiang520.top/gtyvkanpgl.html

Go:   slices.Reverse(arr)
来源：http://hz.ivvv.top/gtgtlgrimo.html

Ruby: arr.reverse
来源：http://hz.yueranfly.top/gttwjgjnuu.html

C#:   list.Reverse();
来源：http://hz.daria6918.cn/gtlsrilibm.html

[D12] 查找元素下标
来源：http://hz.jlsjyb.cn/gthcypcyhi.html

Py:   arr.index(x);  x in arr
来源：http://hz.hammf.cn/gtozbqdror.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.xingfuxueyuan.xyz/gtkjeeadnn.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jinghuilouyu.cn/gtegkcvtnj.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yueranfly.top/gtcuavyxsf.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.sxryk.cn/gtdsvhnuyq.html

Go:   slices.Index(arr, x)
来源：http://hz.snrcjt.cn/gtuazebsjc.html

Ruby: arr.index(x)
来源：http://hz.kuanghao11.cn/gtwhuvcpgp.html

C#:   list.IndexOf(x);
来源：http://hz.pycfn.com/gtllvpcshu.html

[D13] 过滤（保留满足条件的）
来源：http://hz.hammf.cn/gtuwqeiwqf.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.cqqwz.cn/gtcfvrfayl.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.mhx1999.top/gtywgdnfns.html

JS:   arr.filter(x => x > 3)
来源：http://hz.xuetiantiany.cn/gtgkzljtbw.html

TS:   arr.filter(x => x > 3)
来源：http://hz.jiagoushi.top/gtvrgahppn.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.shanyushiyangkeji.top/gtsvayplom.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.jlsjyb.cn/gtywrtmfuy.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.nanxuanxn.top/gtfagcxrae.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.yuanzhike.top/gtivohrmtz.html

[D14] 映射转换（每个元素变形）
来源：http://hz.aizwys.cn/gttowgfltx.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.cheryme.top/gtpqnnzmwn.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.pycfn.com/gtygdbtsox.html

JS:   arr.map(x => x * 2)
来源：http://hz.shangyingyoupin.top/gtgfuqslrp.html

TS:   arr.map(x => x * 2)
来源：http://hz.sxryk.cn/gtthabsjnc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.aibaodan.cn/gtuycqvhta.html

Go:   // 手写循环
来源：http://hz.hammf.cn/gtssrfptfl.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.jlsjyb.cn/gtqpvpimzy.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.jqgfzy.top/gtzmqqmffa.html

[D15] 去重
来源：http://hz.quarkkingdee.top/gtlkstggpo.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.wangdashe.top/gtolchtcbk.html

PHP:  array_unique($arr);
来源：http://hz.zycfv.cn/gtormrposs.html

JS:   [...new Set(arr)]
来源：http://hz.ydjk.org.cn/gtovpboyvo.html

TS:   [...new Set(arr)]
来源：http://hz.dashuyun.cn/gtftfwegyx.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.cqqwz.cn/gteadgfmdr.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.snrcjt.cn/gtvidvylpj.html

Ruby: arr.uniq
来源：http://hz.pengpengdd.cyou/gtgzvetwqe.html

C#:   list.Distinct().ToList()
来源：http://hz.xylfe.cn/gtahbukkmg.html

[D16] 求和与平均值
来源：http://hz.vqdsnc.cn/gtnicymzty.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.daxiang520.top/gtwrgtzmbf.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.vqdsnc.cn/gtytyiipas.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hammf.cn/gthyefwtki.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.aizwys.cn/gtwhtlqpcq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.hammf.cn/gtoivojamb.html

Go:   // 手写循环累加
来源：http://hz.jinyuanbaomall.cn/gticeyxizi.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.kuanghao11.cn/gtdapktkqo.html

C#:   list.Sum();  list.Average()
来源：http://hz.wangdashe.top/gtralzutuk.html

[D17] 最大值与最小值
来源：http://hz.pycfn.com/gtzotznmsk.html

Py:   max(arr);  min(arr)
来源：http://hz.tianlin.xyz/gtbcnbdxtb.html

PHP:  max($arr);  min($arr);
来源：http://hz.cqqwz.cn/gtfaxwyacb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.nwbrower.top/gtovjegozy.html

TS:   Math.max(...arr);
来源：http://hz.zhengqikj.top/gtjvmsnjfn.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.chenlongwang.top/gtmslzdapr.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.shuidangran.top/gtabjazurb.html

Ruby: arr.max;  arr.min
来源：http://hz.hfpthk.cn/gtihesvjdy.html

C#:   list.Max();  list.Min()
来源：http://hz.cheryme.top/gtpvvmhqtt.html

[D18] 扁平化嵌套数组
来源：http://hz.ybcxt.top/gtszxcgomb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.cdnleiting.top/gtqfdacmmc.html

PHP:  array_merge(...$nested);
来源：http://hz.yuanzhike.top/gtikcatvug.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.chenjidiqi.icu/gtlwuwuidj.html

TS:   nested.flat();
来源：http://hz.iojbl.cn/gtkqrompup.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.ydzc1.top/gtyujrsueh.html

Go:   // 手写双层循环
来源：http://hz.andypj.xyz/gtsramebxn.html

Ruby: nested.flatten
来源：http://hz.yuxming.cn/gtolgcikoo.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.andypj.xyz/gtsrcpnuwe.html

[D19] 按字段分组
来源：http://hz.yonumen.top/gtpmmpdgjp.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.xziqi.cn/gtijdzsaqy.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.cashguo.top/gtktzuidvx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.gzhubu.top/gtfyusyvas.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.mhx1999.top/gtcarztgql.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.yuanzhike.top/gtvqfeoesk.html

Go:   // 手写 map[string][]T
来源：http://hz.jinghuilouyu.cn/gtbfbwjwgo.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.nwbrower.top/gtvhwcovsw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.havefunace.top/gtlzggqxlq.html

[D20] 统计每个元素出现次数
来源：http://hz.gotoacloud.top/gtuawfvvpv.html

Py:   Counter(arr)
来源：http://hz.ydjk.org.cn/gtmgzwtvel.html

PHP:  array_count_values($arr);
来源：http://hz.hongshengwenyu.top/gtgliflacw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.xingfuxueyuan.xyz/gtmccqwabs.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.haohaochexian.top/gtthfdwmgj.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.kuanghao11.cn/gtmygdvush.html

Go:   // 手写 map[T]int
来源：http://hz.yuxming.cn/gtxzhvnvcw.html

Ruby: arr.tally
来源：http://hz.smart0.xyz/gtyullwmck.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.hnxiangtu.top/gtldmhhwea.html

[D21] 判断是否包含某元素
来源：http://hz.dashuyun.cn/gtmrupoipx.html

Py:   x in arr
来源：http://hz.snrcjt.cn/gtnornzshm.html

PHP:  in_array($x, $arr, true);
来源：http://hz.yuxming.cn/gtkwphbwtr.html

JS:   arr.includes(x)
来源：http://hz.yongpay.top/gtnatwjvew.html

TS:   arr.includes(x)
来源：http://hz.shuidangran.top/gtbifyrcwy.html

Java: list.contains(x)
来源：http://hz.yj20258.top/gtzuoculzd.html

Go:   slices.Contains(arr, x)
来源：http://hz.pengpengdd.cyou/gtugdebeot.html

Ruby: arr.include?(x)
来源：http://hz.yuanzhike.top/gtunbrnjdf.html

C#:   list.Contains(x)
来源：http://hz.haohaochexian.top/gtzdcgtvnv.html

[D22] 复制数组（避免共享引用）
来源：http://hz.xuanzx.com/gtvitpsnli.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.aizwys.cn/gtgfmubptn.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.yj202588.top/gtnhbgcmdk.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.nanxinkj.top/gtrqogvfnn.html

TS:   [...arr];
来源：http://hz.vqdsnc.cn/gtkinhtasm.html

Java: new ArrayList<>(list);
来源：http://hz.yuxming.cn/gtshflzjmn.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.sxryk.cn/gtctvnwveq.html

Ruby: arr.dup;  arr.clone
来源：http://hz.redwolf501.top/gtquevpcwp.html

C#:   new List<int>(list);
来源：http://hz.yueranfly.top/gtwkcbyjjd.html

[D23] reduce 累积计算
来源：http://hz.jinyuanbaomall.cn/gtiayqskjz.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.jinyuanbaomall.cn/gtkzfocuid.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.jqgfzy.top/gtlbemcaav.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.havefunace.top/gtvvgynwez.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.hammf.cn/gtpltwevci.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.wangshuangyany.cn/gtjfjljlnk.html

Go:   // 手写循环
来源：http://hz.ywan-chungtsiang.top/gtunbuwfyx.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.cucudq.cn/gtrpglwjem.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.xingfuxueyuan.xyz/gtyjkhxwxv.html

[D24] 字典 / Map 基本操作
来源：http://hz.chenjidiqi.icu/gtfyvcheic.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.ybcxt.top/gtrdrzdnxe.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.zhoulong.xyz/gtqsgrdlpe.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.wangdashe.top/gtjzoqmvdu.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.yangfankeji.com/gtfyuwrbkj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.redwolf501.top/gtptdgzxyz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.cheryme.top/gtzncuqave.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.bjfxy.top/gttbuzfhhz.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.chenlongwang.top/gtqaymdlin.html

[D25] Set 集合去重与交并差
来源：http://hz.pycfn.com/gtwdguygci.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.ybcxt.top/gtflkprsnk.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.meibo888.top/gtkevgeipn.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.ydjk.org.cn/gtwaahjega.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.gzhubu.top/gtkfhkdere.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.sxryk.cn/gtlvejrmim.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.hfpthk.cn/gtxzqdxotc.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.xuetiantiany.cn/gtufrgrudv.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.wangshuangyany.cn/gtvrnkdxnv.html

[D26] 数组转字符串
来源：http://hz.guannengcc.top/gtmfrsltrv.html

Py:   ", ".join(map(str, arr))
来源：http://hz.gogol.net.cn/gtclydpgjo.html

PHP:  implode(", ", $arr);
来源：http://hz.daria6918.cn/gtdmdrydbk.html

JS:   arr.join(", ")
来源：http://hz.jinqigufen.top/gtmglbdimp.html

TS:   arr.join(", ")
来源：http://hz.9152youxi.cn/gtyjnpggfc.html

Java: String.join(", ", list)
来源：http://hz.yj202588.top/gtlnghvhik.html

Go:   strings.Join(strs, ", ")
来源：http://hz.ybcxt.top/gtvxohhpuh.html

Ruby: arr.join(", ")
来源：http://hz.ehwqpu.com/gtiyjjdcho.html

C#:   string.Join(", ", list)
来源：http://hz.yuxming.cn/gtbsueeibt.html

================================================================================
来源：http://hz.zdqjudy.top/gttajpmtxe.html

E. 字符串处理
来源：http://hz.c1oappe.top/gtiqqhiftj.html

================================================================================
来源：http://hz.0kj1m.cn/gtdqgxrthv.html

[E01] 拼接字符串
来源：http://hz.cdnleiting.top/gtuvjqupte.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.yangfankeji.com/gtcyjjhazk.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.ydjk.org.cn/gtuuujxwby.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jinghuilouyu.cn/gtlbvvgnnm.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ydjk.org.cn/gtsuqtqtkl.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.cdnleiting.top/gtqyzompjf.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.chenlongwang.top/gtmlurzzlc.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.cucudq.cn/gtednfhmjv.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.gogol.net.cn/gtqpwoqypl.html

[E02] 重复字符串
来源：http://hz.aibaodan.cn/gtbgbvwdbg.html

Py:   "ab" * 3
来源：http://hz.shuidangran.top/gtfkeikmjq.html

PHP:  str_repeat("ab", 3);
来源：http://hz.sufxvd.cn/gtgbjpmicb.html

JS:   "ab".repeat(3)
来源：http://hz.shangyingyoupin.top/gtosxuzzfd.html

TS:   "ab".repeat(3)
来源：http://hz.hywenlv.cn/gtdetgnlrb.html

Java: "ab".repeat(3)
来源：http://hz.cdnleiting.top/gttxqmvmqj.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.hfpthk.cn/gtbmhkqvek.html

Ruby: "ab" * 3
来源：http://hz.yonumen.top/gtbrkewutp.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.sxryk.cn/gtfnirhfqp.html

[E03] 截取子串
来源：http://hz.zhijiandao.cn/gthxvhkuwx.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.zhongyouzk.top/gturihxlhq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.chenzaomai.com/gtodsebeys.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.hammf.cn/gtwnousrjk.html

TS:   s.slice(1, 4)
来源：http://hz.andypj.xyz/gtygdggnrv.html

Java: s.substring(1, 4)
来源：http://hz.ydjk.org.cn/gtahyykamf.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.jyoumei.cn/gtyeyumerb.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.daxiang520.top/gteusibwax.html

C#:   s.Substring(1, 3)
来源：http://hz.yanxiufei.cn/gtbduglhhl.html

[E04] 查找子串位置
来源：http://hz.jqgufenzy.top/gtcgmcvkgi.html

Py:   s.find("x");  s.index("x")
来源：http://hz.yueranfly.top/gtbljqpfvv.html

PHP:  strpos($s, "x");
来源：http://hz.svipenyu.cn/gtdzjqkbue.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.xuetiantiany.cn/gtmpgdfgyt.html

TS:   s.indexOf("x")
来源：http://hz.guowangkeji.top/gthbcevfda.html

Java: s.indexOf("x")
来源：http://hz.gotoacloud.top/gtddeoplwb.html

Go:   strings.Index(s, "x")
来源：http://hz.nanxinkj.top/gtegxyyvpv.html

Ruby: s.index("x")
来源：http://hz.yj202588.top/gtuawgxuhm.html

C#:   s.IndexOf("x")
来源：http://hz.ybcxt.top/gtcimcpvyn.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.cdnleiting.top/gtsvceebim.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.gzhubu.top/gtbphktohi.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.sufxvd.cn/gtjbvgcllb.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.hysaishi.cn/gtsjjnmhql.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.jinyuanbaomall.cn/gtshpaxqsp.html


<!-- 参考信息 -->