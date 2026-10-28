代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.9152youxi.cn/gtywimabwa.html

[C15] 解构 / 展开参数
来源：http://hz.yanxiufei.cn/gtlcfmcqbm.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.mhx1999.top/gtsdwnppby.html

PHP:  [$a, $b] = $pair;
来源：http://hz.haohaochexian.top/gtpslgqlda.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.jqgfzy.top/gtttuyatme.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.gzhubu.top/gtgcpgttjl.html

Java: // 无解构
来源：http://hz.dianchejie.cn/gtsaabwvrl.html

Go:   // 无解构
来源：http://hz.jinyuanbaomall.cn/gtmofacqjl.html

Ruby: a, b = pair
来源：http://hz.nanxinkj.top/gtgzsvepgr.html

C#:   var (a, b) = pair;
来源：http://hz.yongpay.top/gtkrrvbquc.html

[C16] 函数 / 方法重载
来源：http://hz.xylfe.cn/gtdiihqbjg.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.ppjwa.cn/gtdcztfcan.html

PHP:  // 无重载
来源：http://hz.hywenlv.cn/gtnezwyjeg.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.sweek.top/gtxofybone.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.yj20258.top/gtqifewnwt.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.yanxiufei.cn/gthdwpgnyf.html

Go:   // 无重载：用不同函数名
来源：http://hz.aizwys.cn/gtyfftjhvz.html

Ruby: # 无重载：靠动态参数
来源：http://hz.jinqigfzy.top/gtudrmhyiw.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.chenlongwang.top/gtchipzbdt.html

================================================================================
来源：http://hz.shzxlz.cn/gtcbdtokap.html

D. 数组 / 列表 / 集合
来源：http://hz.shanyushiyangkeji.top/gtdsveaysf.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtxrdaldat.html

[D01] 创建数组 / 列表
来源：http://hz.kuanghao11.cn/gtmoforylm.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.xuetiantiany.cn/gtzvpisxrz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.yongpay.top/gtkacmbxtd.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.ehwqpu.com/gtxswfwbpa.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.gogol.net.cn/gtwyimporm.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.meibo888.top/gtqwgswfmy.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.zhengqikj.top/gterlcaisu.html

Ruby: arr = [1, 2, 3]
来源：http://hz.xziqi.cn/gtlpjlrvxf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.dianchejie.cn/gtqdthswqu.html

[D02] 追加元素到末尾
来源：http://hz.hfpthk.cn/gtxppsrtzm.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.0kj1m.cn/gtlgqkfecc.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.vqdsnc.cn/gtnqdndmgu.html

JS:   arr.push(4);
来源：http://hz.c1oappe.top/gtiejhhcoe.html

TS:   arr.push(4);
来源：http://hz.pycfn.com/gtsesnbjvk.html

Java: list.add(4);
来源：http://hz.andypj.xyz/gtvbgiqgxh.html

Go:   arr = append(arr, 4)
来源：http://hz.hnxiangtu.top/gtdrebheey.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.yuxming.cn/gtsmxpiymr.html

C#:   list.Add(4);
来源：http://hz.zhongyouzk.top/gtjxduwpxc.html

[D03] 在指定位置插入元素
来源：http://hz.jlsjyb.cn/gtqztergss.html

Py:   arr.insert(0, 0)
来源：http://hz.hysaishi.cn/gtngfbbocb.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.sysykeji.top/gtpazmvoer.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.pengpengdd.cyou/gtryqzcthl.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.smart0.xyz/gtjbepkdkb.html

Java: list.add(0, 0);
来源：http://hz.ppjwa.cn/gtbnpxvceq.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.haohaochexian.top/gtjoeklbju.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.daria6918.cn/gtycbbsutw.html

C#:   list.Insert(0, 0);
来源：http://hz.yangfankeji.com/gtqgqkbmng.html

[D04] 删除元素
来源：http://hz.aibaodan.cn/gttkqepfgq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.zhongyouzk.top/gtvuzqcngz.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.zdqjudy.top/gtfvrncjdh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.cdnleiting.top/gtfnjtywti.html

TS:   arr.splice(0, 1);
来源：http://hz.yuxming.cn/gtcsiagbyz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.gzhubu.top/gtrtrbfdul.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.yongpay.top/gtxglufwba.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.ybcxt.top/gtbzxrvfhe.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.yj20258.top/gtegmgpgxd.html

[D05] 访问与修改元素
来源：http://hz.quarkkingdee.top/gtlkmbmdle.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.sysykeji.top/gtqfdiubqt.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.ppjwa.cn/gtfjczaoiv.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.hfpthk.cn/gtpuyblrij.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.guannengcc.top/gtgtjvlbnm.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.sysykeji.top/gtszxcbllg.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.ivvv.top/gtcmjsuggj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.0kj1m.cn/gtylmolodq.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.xinyue.icu/gtjsdaomxa.html

[D06] 数组长度
来源：http://hz.feifeiyinyue.top/gtaqspqblv.html

Py:   len(arr)
来源：http://hz.sysykeji.top/gtxuebxtsf.html

PHP:  count($arr);
来源：http://hz.mhx1999.top/gtoydylxrb.html

JS:   arr.length
来源：http://hz.0kj1m.cn/gtnarplmmq.html

TS:   arr.length
来源：http://hz.yvedp.cn/gtmijrsodx.html

Java: list.size();
来源：http://hz.gzhubu.top/gtaffnnayb.html

Go:   len(arr)
来源：http://hz.jinghuilouyu.cn/gtjvpkzzzu.html

Ruby: arr.length; arr.size
来源：http://hz.cheryme.top/gtocitebrj.html

C#:   list.Count;
来源：http://hz.cdnleiting.top/gtemewkytz.html

[D07] 切片 / 取子数组
来源：http://hz.cashguo.top/gtkzyptnco.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.xuanzx.com/gtuwalzlqn.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.jinqigfzy.top/gtgswdftms.html

JS:   arr.slice(1, 4);
来源：http://hz.yj20258888.top/gtevyqlwjy.html

TS:   arr.slice(1, 4);
来源：http://hz.hongshengwenyu.top/gtkydzcbar.html

Java: list.subList(1, 4);
来源：http://hz.andypj.xyz/gtldebnbrc.html

Go:   arr[1:4]
来源：http://hz.daria6918.cn/gtikrnaavj.html

Ruby: arr[1, 3]
来源：http://hz.zdqjudy.top/gtvnxawtwa.html

C#:   list.GetRange(1, 3);
来源：http://hz.kuanghao11.cn/gtseibupik.html

[D08] 合并两个数组
来源：http://hz.nwbrower.top/gtvpspqcty.html

Py:   a + b;  a.extend(b)
来源：http://hz.snrcjt.cn/gtwzfhmpje.html

PHP:  array_merge($a, $b);
来源：http://hz.vqdsnc.cn/gttmieadvy.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.ppjwa.cn/gtnoaocioq.html

TS:   [...a, ...b];
来源：http://hz.nanxuanxn.top/gtshknqmlb.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.ybcxt.top/gtrgfujqci.html

Go:   append(a, b...)
来源：http://hz.havefunace.top/gtknufgyiy.html

Ruby: a + b;  a.concat(b)
来源：http://hz.ydjk.org.cn/gtgrimcxia.html

C#:   a.Concat(b).ToList()
来源：http://hz.yj20258.top/gtltiwwbja.html

[D09] 排序（升序）
来源：http://hz.shangyingyoupin.top/gtrcssjmnq.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.shanyushiyangtech.top/gtzrujcuoo.html

PHP:  sort($arr);
来源：http://hz.nanxinkj.top/gtblqrslim.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.shzxlz.cn/gtjssyzxko.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.9152youxi.cn/gtaokbgjfe.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.havefunace.top/gthtmxnjra.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.zdqjudy.top/gthhxkzpht.html

Ruby: arr.sort
来源：http://hz.kuanghao11.cn/gtnwuubuiu.html

C#:   list.Sort();
来源：http://hz.shuidangran.top/gtrosrodrs.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.ydjk.org.cn/gtamigtvxr.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.sufxvd.cn/gtdblazeil.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.haohaochexian.top/gtqcqdtdup.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.kuanghao11.cn/gtdrdxhqwo.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yj20258888.top/gtdwnhkynl.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.yuxming.cn/gtvzwhclku.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.tanke756.top/gthmffxzwu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.cucudq.cn/gtqokbadnm.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.ydzc1.top/gtvxzvudqc.html

[D11] 反转数组
来源：http://hz.xziqi.cn/gtzdhvbqre.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.cqqwz.cn/gtytxunzwq.html

PHP:  array_reverse($arr);
来源：http://hz.daxiang520.top/gtlsmajkiy.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.yj202588.top/gtvqkwvdzy.html

TS:   [...arr].reverse();
来源：http://hz.guowangkeji.top/gtjwgyjwit.html

Java: Collections.reverse(list);
来源：http://hz.fzhhl.top/gtofdacbvr.html

Go:   slices.Reverse(arr)
来源：http://hz.shzxlz.cn/gtkilcdgef.html

Ruby: arr.reverse
来源：http://hz.ywan-chungtsiang.top/gtmduavpke.html

C#:   list.Reverse();
来源：http://hz.pengpengdd.cyou/gtkzqafrps.html

[D12] 查找元素下标
来源：http://hz.xylfe.cn/gtzehohpsm.html

Py:   arr.index(x);  x in arr
来源：http://hz.yongpay.top/gtyvphtrar.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.jiagoushi.top/gtdkhourxo.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.nanxinkj.top/gtvdtvoewj.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.cheryme.top/gtvhbsksiu.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.meibo888.top/gtalmxteap.html

Go:   slices.Index(arr, x)
来源：http://hz.gogol.net.cn/gtrurzuhpb.html

Ruby: arr.index(x)
来源：http://hz.sxryk.cn/gtfjbycnqy.html

C#:   list.IndexOf(x);
来源：http://hz.wangdashe.top/gtxgbhwowq.html

[D13] 过滤（保留满足条件的）
来源：http://hz.zdqjudy.top/gtjkcykhuc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.zhiwuduotai.top/gtgarrggsf.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.haohaochexian.top/gtvacwlnth.html

JS:   arr.filter(x => x > 3)
来源：http://hz.ydjk.org.cn/gtivnylfui.html

TS:   arr.filter(x => x > 3)
来源：http://hz.xuanzx.com/gtkvkwpmag.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.jinqigufen.top/gthrfldwtp.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.cashguo.top/gteugdpqao.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.yj20258.top/gtpcnukubm.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.xziqi.cn/gtvvmmhckl.html

[D14] 映射转换（每个元素变形）
来源：http://hz.aibaodan.cn/gtgixjmxel.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.ydzc1.top/gtjaazpqrh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.fengsongda.top/gterrcoqmc.html

JS:   arr.map(x => x * 2)
来源：http://hz.redwolf501.top/gttdbkywct.html

TS:   arr.map(x => x * 2)
来源：http://hz.chenlongwang.top/gtbstndmzr.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.ybcxt.top/gtmqxybrbg.html

Go:   // 手写循环
来源：http://hz.jianghu66.top/gtswtwvfsb.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.jinghuilouyu.cn/gtzkibsqct.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.zhongyouzk.top/gtffanjvwo.html

[D15] 去重
来源：http://hz.iojbl.cn/gttjtqggoi.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.zhixingplan.top/gtoevsmvrs.html

PHP:  array_unique($arr);
来源：http://hz.jqgfzy.top/gtpvkdhkde.html

JS:   [...new Set(arr)]
来源：http://hz.haohaochexian.top/gteclpadyi.html

TS:   [...new Set(arr)]
来源：http://hz.svipenyu.cn/gtjdgadfvo.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.vqdsnc.cn/gtbkqwjlvs.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.zhiwuduotai.top/gttrthlsbn.html

Ruby: arr.uniq
来源：http://hz.sufxvd.cn/gtpfnvsbfp.html

C#:   list.Distinct().ToList()
来源：http://hz.sysykeji.top/gtelcasxug.html

[D16] 求和与平均值
来源：http://hz.yangfankeji.com/gtjospficu.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.vqdsnc.cn/gtaokfmedz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.fengsongda.top/gtgisesjoo.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.vqdsnc.cn/gtfabjlysy.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.guannengcc.top/gtbcyzbziu.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.zycfv.cn/gtovlskftp.html

Go:   // 手写循环累加
来源：http://hz.tianlin.xyz/gtphfssugm.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.chenlongwang.top/gtecgrdeks.html

C#:   list.Sum();  list.Average()
来源：http://hz.snrcjt.cn/gthkvyymep.html

[D17] 最大值与最小值
来源：http://hz.9152youxi.cn/gtnxhazylo.html

Py:   max(arr);  min(arr)
来源：http://hz.jinghuilouyu.cn/gtcuzqfzwk.html

PHP:  max($arr);  min($arr);
来源：http://hz.birdmap.top/gtynzhccji.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.yonumen.top/gtiemqckdo.html

TS:   Math.max(...arr);
来源：http://hz.ivvv.top/gtkdsoqhod.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.ywan-chungtsiang.top/gtftcruttp.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.sxryk.cn/gtecnhgdmp.html

Ruby: arr.max;  arr.min
来源：http://hz.cdnleiting.top/gtyqbmyldt.html

C#:   list.Max();  list.Min()
来源：http://hz.zhaomingkeji.xyz/gtrwehlcih.html

[D18] 扁平化嵌套数组
来源：http://hz.pycfn.com/gtpedqyjcq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.xinyue.icu/gtswhsyevd.html

PHP:  array_merge(...$nested);
来源：http://hz.xinyue.icu/gtwrbsgyqr.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.andypj.xyz/gtroanljzl.html

TS:   nested.flat();
来源：http://hz.yongpay.top/gtcroijsys.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.xylfe.cn/gtcwvgmjky.html

Go:   // 手写双层循环
来源：http://hz.cheryme.top/gtpykboixa.html

Ruby: nested.flatten
来源：http://hz.dashuyun.cn/gtnzlsjkqx.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.yvedp.cn/gtynhjtgkh.html

[D19] 按字段分组
来源：http://hz.aibaodan.cn/gtclzgfgrt.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.zhaomingkeji.xyz/gtxlyeakcc.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.xuanzx.com/gtfzasyofv.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.hywenlv.cn/gtjlxuomez.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.yj202588.top/gthqyurjwg.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.jqgfzy.top/gtebdwlilc.html

Go:   // 手写 map[string][]T
来源：http://hz.ppjwa.cn/gtlukxazzv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.yj20258888.top/gtseaarhne.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.jinghuilouyu.cn/gtwjvhksrj.html

[D20] 统计每个元素出现次数
来源：http://hz.zhijiandao.cn/gtgyatgvqu.html

Py:   Counter(arr)
来源：http://hz.ywan-chungtsiang.top/gtpwjczrdo.html

PHP:  array_count_values($arr);
来源：http://hz.yj20258.top/gtuptplwik.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jqgufenzy.top/gtdpeltdkk.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.sweek.top/gtikiaezmp.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.ydzc1.top/gtcqsdrzbu.html

Go:   // 手写 map[T]int
来源：http://hz.smart0.xyz/gtzmptuxvq.html

Ruby: arr.tally
来源：http://hz.guowangkeji.top/gtmqzcdbce.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.jinghuilouyu.cn/gtsbygavlq.html

[D21] 判断是否包含某元素
来源：http://hz.wangdashe.top/gtoqodbbug.html

Py:   x in arr
来源：http://hz.jqgufenzy.top/gtmxywnojd.html

PHP:  in_array($x, $arr, true);
来源：http://hz.guannengcc.top/gtvnodqglu.html

JS:   arr.includes(x)
来源：http://hz.yuxming.cn/gtfoswwhtm.html

TS:   arr.includes(x)
来源：http://hz.chenzaomai.com/gtratoggpp.html

Java: list.contains(x)
来源：http://hz.hnxiangtu.top/gtbrtrltxv.html

Go:   slices.Contains(arr, x)
来源：http://hz.guowangkeji.top/gtxaupyish.html

Ruby: arr.include?(x)
来源：http://hz.jinyuanbaomall.cn/gtwbwngqsx.html

C#:   list.Contains(x)
来源：http://hz.zhixingplan.top/gtkmolaxgk.html

[D22] 复制数组（避免共享引用）
来源：http://hz.shanyushiyangtech.top/gtkymqnyzy.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.cucudq.cn/gtibqfouey.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.shuidangran.top/gtkstjvkeg.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.c1oappe.top/gthmzdkyed.html

TS:   [...arr];
来源：http://hz.zhiwuduotai.top/gthexrjucc.html

Java: new ArrayList<>(list);
来源：http://hz.jinqigfzy.top/gtuswpfhzx.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.shanyushiyangtech.top/gttmzybdkw.html

Ruby: arr.dup;  arr.clone
来源：http://hz.cdnleiting.top/gtivrwmxar.html

C#:   new List<int>(list);
来源：http://hz.52xcode.cn/gtspubbzls.html

[D23] reduce 累积计算
来源：http://hz.hnxiangtu.top/gtjzylqfxb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.ywan-chungtsiang.top/gtbrmyggee.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.gotoacloud.top/gtyxevfoki.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.quarkkingdee.top/gtnfbvczcn.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.vqdsnc.cn/gtjtatojzr.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.cdnleiting.top/gtwwinskxi.html

Go:   // 手写循环
来源：http://hz.quarkkingdee.top/gtxedhclar.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.jinqigfzy.top/gtvcvewqoc.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.gotoacloud.top/gtqqujwhxt.html

[D24] 字典 / Map 基本操作
来源：http://hz.jiagoushi.top/gtidpbljse.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.52xcode.cn/gtwudfeees.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.kuanghao11.cn/gtgmnuzlyp.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.haohaochexian.top/gtdvrzcwje.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.shanyushiyangkeji.top/gtleflfxap.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.hongshengwenyu.top/gtdfxkaegx.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.meibo888.top/gtbpmaozie.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.0kj1m.cn/gtlieznkpe.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.zhengqikj.top/gtyuramvxo.html

[D25] Set 集合去重与交并差
来源：http://hz.tianlin.xyz/gtdycxhbbd.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.zhixingplan.top/gtjouerxhr.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.snrcjt.cn/gtcyhfgfzw.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.meibo888.top/gtlyezzvju.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.gotoacloud.top/gtpabzkrsh.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.jianghu66.top/gtvgyhmfqa.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.yj20258.top/gtqkjiicad.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.hysaishi.cn/gtrbvecyrl.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.birdmap.top/gtevtgkdsl.html

[D26] 数组转字符串
来源：http://hz.yvedp.cn/gtsjszpjon.html

Py:   ", ".join(map(str, arr))
来源：http://hz.meibo888.top/gtandwlqwm.html

PHP:  implode(", ", $arr);
来源：http://hz.daria6918.cn/gtsnqftdsw.html

JS:   arr.join(", ")
来源：http://hz.ppjwa.cn/gtgplejmvb.html

TS:   arr.join(", ")
来源：http://hz.aibaodan.cn/gttemmbior.html

Java: String.join(", ", list)
来源：http://hz.andypj.xyz/gtsgawihnw.html

Go:   strings.Join(strs, ", ")
来源：http://hz.shzxlz.cn/gtkkjjbaip.html

Ruby: arr.join(", ")
来源：http://hz.zhaomingkeji.xyz/gtpqscloqz.html

C#:   string.Join(", ", list)
来源：http://hz.hnxiangtu.top/gtmbpdomag.html

================================================================================
来源：http://hz.dianchejie.cn/gtfycqicjv.html

E. 字符串处理
来源：http://hz.xziqi.cn/gtonxjekei.html

================================================================================
来源：http://hz.gotoacloud.top/gtvvtctdiq.html

[E01] 拼接字符串
来源：http://hz.hysaishi.cn/gtpvdmstfb.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.aibaodan.cn/gtghjoezgx.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.bjfxy.top/gtbcherjho.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.cucudq.cn/gtqfkdowzz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zhengqikj.top/gtsrcaciwm.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.jiagoushi.top/gtjlzxymdd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.chenzaomai.com/gtfcojclps.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.gaohongyu789.top/gtexcrzroo.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.zdqjudy.top/gtkvfwouaw.html

[E02] 重复字符串
来源：http://hz.shangyingyoupin.top/gtamzwjyqc.html

Py:   "ab" * 3
来源：http://hz.gogol.net.cn/gtwcaqzdfe.html

PHP:  str_repeat("ab", 3);
来源：http://hz.fengsongda.top/gtitjumtct.html

JS:   "ab".repeat(3)
来源：http://hz.dianchejie.cn/gttrdmnhuo.html

TS:   "ab".repeat(3)
来源：http://hz.wangdashe.top/gtwhfrwync.html

Java: "ab".repeat(3)
来源：http://hz.hysaishi.cn/gtgvzxvghh.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.gzhubu.top/gtckepahyi.html

Ruby: "ab" * 3
来源：http://hz.shangyingyoupin.top/gtyjoaktxj.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.52xcode.cn/gtvlrdgvzj.html

[E03] 截取子串
来源：http://hz.hnqzz.top/gtxfzmenor.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.aizwys.cn/gtzpcalyvy.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.chenzaomai.com/gtflcsgshr.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.jinghuilouyu.cn/gtrdlnqwta.html

TS:   s.slice(1, 4)
来源：http://hz.shanyushiyangtech.top/gtbqyjjomw.html

Java: s.substring(1, 4)
来源：http://hz.ywan-chungtsiang.top/gtvflhkvqm.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.jiagoushi.top/gthzgvtzli.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.hnxiangtu.top/gtzywtscyc.html

C#:   s.Substring(1, 3)
来源：http://hz.tianlin.xyz/gtdexhvoir.html

[E04] 查找子串位置
来源：http://hz.nwbrower.top/gtpgsklrwb.html

Py:   s.find("x");  s.index("x")
来源：http://hz.kuanghao11.cn/gtftwlerhy.html

PHP:  strpos($s, "x");
来源：http://hz.yangfankeji.com/gttflapgyu.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.yonumen.top/gtgmjyjbtn.html

TS:   s.indexOf("x")
来源：http://hz.hongshengwenyu.top/gtjykdneoh.html

Java: s.indexOf("x")
来源：http://hz.tian-w.cn/gtgrabgmde.html

Go:   strings.Index(s, "x")
来源：http://hz.zhaomingkeji.xyz/gtjzddbvvy.html

Ruby: s.index("x")
来源：http://hz.chenjidiqi.icu/gtwpmnojxm.html

C#:   s.IndexOf("x")
来源：http://hz.tian-w.cn/gtmbcjpgig.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.birdmap.top/gtpwilcqir.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.shzxlz.cn/gtirxucefh.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.jianghu66.top/gtjmechktu.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.daxiang520.top/gtpwowwafk.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.quarkkingdee.top/gtxwaipdob.html


<!-- 参考信息 -->