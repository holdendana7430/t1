代发 wailian999

Ruby: a, b = pair
来源：http://hz.yonumen.top/gtcdtzogmi.html

C#:   var (a, b) = pair;
来源：http://hz.dashuyun.cn/gtqqmbluph.html

[C16] 函数 / 方法重载
来源：http://hz.cucudq.cn/gtehspunwu.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.dashuyun.cn/gtztmjgyji.html

PHP:  // 无重载
来源：http://hz.pycfn.com/gtgaflniqa.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.gogol.net.cn/gtrsnynnyw.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.shangyingyoupin.top/gtwjfholmq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.sysykeji.top/gtaftghsqf.html

Go:   // 无重载：用不同函数名
来源：http://hz.ybcxt.top/gtbognwdvn.html

Ruby: # 无重载：靠动态参数
来源：http://hz.316326.xyz/gtxdqqgopd.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.yueranfly.top/gtrzxjwgud.html

================================================================================
来源：http://hz.hfpthk.cn/gtpvvkmjgt.html

D. 数组 / 列表 / 集合
来源：http://hz.smart0.xyz/gtwsczetac.html

================================================================================
来源：http://hz.birdmap.top/gtvcfqdhrc.html

[D01] 创建数组 / 列表
来源：http://hz.ydzc1.top/gthxvwjtax.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.jyoumei.cn/gtplkzvegb.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.jlsjyb.cn/gtmgiaausz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.hammf.cn/gtfyjtkbvm.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.sysykeji.top/gtqokpqvfa.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.ivvv.top/gtowkcgyam.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.birdmap.top/gtjpoxhpfa.html

Ruby: arr = [1, 2, 3]
来源：http://hz.daxiang520.top/gtxalnwvtj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.zhongyouzk.top/gtfplapdyk.html

[D02] 追加元素到末尾
来源：http://hz.guannengcc.top/gtujcqpwcu.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.xuanzx.com/gtsumpohrw.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.zdqjudy.top/gtjfcokhfy.html

JS:   arr.push(4);
来源：http://hz.zhengqikj.top/gtuhstiwlo.html

TS:   arr.push(4);
来源：http://hz.nanxuanxn.top/gtnurqjqnd.html

Java: list.add(4);
来源：http://hz.nanxinkj.top/gtuevpolgu.html

Go:   arr = append(arr, 4)
来源：http://hz.hnxiangtu.top/gthmbupezt.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.vqdsnc.cn/gtlqxynpkv.html

C#:   list.Add(4);
来源：http://hz.gaohongyu789.top/gtcriqdhwd.html

[D03] 在指定位置插入元素
来源：http://hz.pengpengdd.cyou/gtgugjnzki.html

Py:   arr.insert(0, 0)
来源：http://hz.xylfe.cn/gtjqnihggo.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.jyoumei.cn/gtqjbpgatb.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.cheryme.top/gtotgpyhrd.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.jinqigufen.top/gthlmusdaq.html

Java: list.add(0, 0);
来源：http://hz.meibo888.top/gtfpulpawv.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.xylfe.cn/gtaknkqfls.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.fengsongda.top/gtumqwnmhs.html

C#:   list.Insert(0, 0);
来源：http://hz.svipenyu.cn/gthjrqiwao.html

[D04] 删除元素
来源：http://hz.jyoumei.cn/gtnicwzbas.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.yonumen.top/gtpuxuhjyg.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.ywan-chungtsiang.top/gtsvpmesbk.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.zhongyouzk.top/gtyaaducgk.html

TS:   arr.splice(0, 1);
来源：http://hz.zhengqikj.top/gtzzskczmq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.9152youxi.cn/gtqthzkldc.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.xuanzx.com/gtvpwtdgtu.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.9152youxi.cn/gtdgunwujb.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.chenzaomai.com/gtevfymqyn.html

[D05] 访问与修改元素
来源：http://hz.ydjk.org.cn/gtkghiqegd.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.guannengcc.top/gteercokhq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.gzhubu.top/gtuqgaierz.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.zhaomingkeji.xyz/gtgocjptmo.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.mhx1999.top/gtxyaaunrm.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.jinghuilouyu.cn/gteqyqiuyp.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.smart0.xyz/gtmrgbkjlg.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jianghu66.top/gtdjgdlabs.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.feifeiyinyue.top/gttgonmqxq.html

[D06] 数组长度
来源：http://hz.yj20258.top/gtvsgujiqn.html

Py:   len(arr)
来源：http://hz.guowangkeji.top/gtycrlvltb.html

PHP:  count($arr);
来源：http://hz.ivvv.top/gtekkfpqpq.html

JS:   arr.length
来源：http://hz.ehwqpu.com/gtywmayvyl.html

TS:   arr.length
来源：http://hz.yonumen.top/gtijozhldf.html

Java: list.size();
来源：http://hz.yj202588.top/gtpuujuioa.html

Go:   len(arr)
来源：http://hz.sysykeji.top/gtvgvshwqo.html

Ruby: arr.length; arr.size
来源：http://hz.tianlin.xyz/gthlbzyohl.html

C#:   list.Count;
来源：http://hz.quarkkingdee.top/gtkqcqwecj.html

[D07] 切片 / 取子数组
来源：http://hz.jianghu66.top/gtqzdixyth.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.hnqzz.top/gtsaarvklp.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.pycfn.com/gtreqyvcwm.html

JS:   arr.slice(1, 4);
来源：http://hz.zhixingplan.top/gtrkfnxubn.html

TS:   arr.slice(1, 4);
来源：http://hz.zhaomingkeji.xyz/gtomfstnmj.html

Java: list.subList(1, 4);
来源：http://hz.quarkkingdee.top/gtfskzvgwe.html

Go:   arr[1:4]
来源：http://hz.ybcxt.top/gtkdogzgiq.html

Ruby: arr[1, 3]
来源：http://hz.zdqjudy.top/gtmvahrsuf.html

C#:   list.GetRange(1, 3);
来源：http://hz.aizwys.cn/gtbkxvudia.html

[D08] 合并两个数组
来源：http://hz.sweek.top/gtknfayszu.html

Py:   a + b;  a.extend(b)
来源：http://hz.sxryk.cn/gtssklaczc.html

PHP:  array_merge($a, $b);
来源：http://hz.guannengcc.top/gtpihhcfdw.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.jinqigfzy.top/gtymdhhsgj.html

TS:   [...a, ...b];
来源：http://hz.zhiwuduotai.top/gtadwpxjfc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.zhaomingkeji.xyz/gtbsdfjwrs.html

Go:   append(a, b...)
来源：http://hz.zycfv.cn/gtljadqdse.html

Ruby: a + b;  a.concat(b)
来源：http://hz.hammf.cn/gtjctfxsnf.html

C#:   a.Concat(b).ToList()
来源：http://hz.daxiang520.top/gtszivccul.html

[D09] 排序（升序）
来源：http://hz.redwolf501.top/gtazlkxjdt.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.fzhhl.top/gtxuqcrlpv.html

PHP:  sort($arr);
来源：http://hz.shanyushiyangtech.top/gttbmzkteb.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.vqdsnc.cn/gtxzuikktt.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.hnxiangtu.top/gtmyscfvmk.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.jianghu66.top/gthrkedngt.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.svipenyu.cn/gtyambhduo.html

Ruby: arr.sort
来源：http://hz.gaohongyu789.top/gtxdbawzsb.html

C#:   list.Sort();
来源：http://hz.jlsjyb.cn/gteepyivzy.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.dianchejie.cn/gtiutpzoau.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.nanxuanxn.top/gtbjnoblex.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.fzhhl.top/gtynwbejyw.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.pengpengdd.cyou/gtcwsiobkp.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.316326.xyz/gtwrankmax.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.jyoumei.cn/gtvmwbmmsl.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.xylfe.cn/gtmcndqblh.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.aibaodan.cn/gtusabkfgy.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.sxryk.cn/gtmelcterp.html

[D11] 反转数组
来源：http://hz.guowangkeji.top/gtptavjicv.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.yonumen.top/gtjnawgzyd.html

PHP:  array_reverse($arr);
来源：http://hz.zhijiandao.cn/gtzfozbeur.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.cashguo.top/gtyjvpjlcc.html

TS:   [...arr].reverse();
来源：http://hz.yuanzhike.top/gtokbpvuwr.html

Java: Collections.reverse(list);
来源：http://hz.fengsongda.top/gtzchupdmo.html

Go:   slices.Reverse(arr)
来源：http://hz.ybcxt.top/gtuhfwlmkd.html

Ruby: arr.reverse
来源：http://hz.feifeiyinyue.top/gtsyoactoh.html

C#:   list.Reverse();
来源：http://hz.aizwys.cn/gtcrkvzplo.html

[D12] 查找元素下标
来源：http://hz.cqqwz.cn/gtyqvapcqm.html

Py:   arr.index(x);  x in arr
来源：http://hz.daxiang520.top/gtowbtoofk.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.shanyushiyangkeji.top/gttstfhxej.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zhoulong.xyz/gtcspgniso.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zhixingplan.top/gtnoxiwokr.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.cheryme.top/gtnyijzydm.html

Go:   slices.Index(arr, x)
来源：http://hz.ybcxt.top/gthztxjeeh.html

Ruby: arr.index(x)
来源：http://hz.yangfankeji.com/gtthkolpkq.html

C#:   list.IndexOf(x);
来源：http://hz.dianchejie.cn/gtezrtwemd.html

[D13] 过滤（保留满足条件的）
来源：http://hz.birdmap.top/gtrxijhsjg.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.jinyuanbaomall.cn/gtbnbyuzsn.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.yvedp.cn/gtadstdmkw.html

JS:   arr.filter(x => x > 3)
来源：http://hz.zycfv.cn/gtfunwiobh.html

TS:   arr.filter(x => x > 3)
来源：http://hz.guowangkeji.top/gtersrnwik.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.shzxlz.cn/gtfacobpqt.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.gogol.net.cn/gtxxldworn.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.cheryme.top/gtnbuouajy.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.yonumen.top/gtfybahprf.html

[D14] 映射转换（每个元素变形）
来源：http://hz.gzhubu.top/gtcxbbpgha.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.svipenyu.cn/gttpvqadss.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.sweek.top/gtenqydehc.html

JS:   arr.map(x => x * 2)
来源：http://hz.bjfxy.top/gtwnjdrnrf.html

TS:   arr.map(x => x * 2)
来源：http://hz.zhijiandao.cn/gtorxebpxv.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.sysykeji.top/gtdvyovfgb.html

Go:   // 手写循环
来源：http://hz.jinghuilouyu.cn/gtjfybgncd.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.svipenyu.cn/gtaxrupjoj.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.ydzc1.top/gtdmvldziy.html

[D15] 去重
来源：http://hz.aibaodan.cn/gtisndrqoa.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.jianghu66.top/gtfptjgtjq.html

PHP:  array_unique($arr);
来源：http://hz.jinyuanbaomall.cn/gtrydnjjke.html

JS:   [...new Set(arr)]
来源：http://hz.chenzaomai.com/gtjlbpyhlr.html

TS:   [...new Set(arr)]
来源：http://hz.ydzc1.top/gtcywxlpbs.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.jianghu66.top/gtkrpibuuw.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.jiagoushi.top/gttpduklev.html

Ruby: arr.uniq
来源：http://hz.zhoulong.xyz/gtclkjethq.html

C#:   list.Distinct().ToList()
来源：http://hz.cheryme.top/gtrntphmqk.html

[D16] 求和与平均值
来源：http://hz.jyoumei.cn/gttvirgdpj.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.jianghu66.top/gtsoixbzac.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.ydzc1.top/gtpblecgib.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.wangshuangyany.cn/gtvmpazvkn.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.fengsongda.top/gtuqbizvpa.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.yvedp.cn/gtzwsovtee.html

Go:   // 手写循环累加
来源：http://hz.feifeiyinyue.top/gttzibxmvz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.chenlongwang.top/gtxmadkwuy.html

C#:   list.Sum();  list.Average()
来源：http://hz.birdmap.top/gtoykzcjwf.html

[D17] 最大值与最小值
来源：http://hz.feifeiyinyue.top/gtkbsnnhlz.html

Py:   max(arr);  min(arr)
来源：http://hz.zhixingplan.top/gtxcxqrdbs.html

PHP:  max($arr);  min($arr);
来源：http://hz.wangshuangyany.cn/gtryszsujb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.hywenlv.cn/gtuerzjwtw.html

TS:   Math.max(...arr);
来源：http://hz.0kj1m.cn/gtsmgzxvfn.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.dashuyun.cn/gtwuzlqhtl.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.guowangkeji.top/gtvugfowbi.html

Ruby: arr.max;  arr.min
来源：http://hz.sxryk.cn/gteedilytq.html

C#:   list.Max();  list.Min()
来源：http://hz.zycfv.cn/gtkvdndxma.html

[D18] 扁平化嵌套数组
来源：http://hz.yongpay.top/gtvkopuqok.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.aibaodan.cn/gtrgnyolhb.html

PHP:  array_merge(...$nested);
来源：http://hz.jinghuilouyu.cn/gtczqermwf.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.ydjk.org.cn/gtkehtiwck.html

TS:   nested.flat();
来源：http://hz.ywan-chungtsiang.top/gttlmljtro.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.cdnleiting.top/gtcpymytfr.html

Go:   // 手写双层循环
来源：http://hz.redwolf501.top/gtftytkfzy.html

Ruby: nested.flatten
来源：http://hz.tianlin.xyz/gtdsklspqr.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.cheryme.top/gtiysgflxk.html

[D19] 按字段分组
来源：http://hz.0kj1m.cn/gtdndzuxfa.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.tanke756.top/gtsivsmgdd.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.daria6918.cn/gttjpasqlr.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.hfpthk.cn/gtweygohqq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.shanyushiyangkeji.top/gtimerafza.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.316326.xyz/gthssxubfq.html

Go:   // 手写 map[string][]T
来源：http://hz.wangshuangyany.cn/gtqoiiwzip.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.iojbl.cn/gtgkurlmyq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.fzhhl.top/gtvoezteoo.html

[D20] 统计每个元素出现次数
来源：http://hz.jlsjyb.cn/gtozdevrma.html

Py:   Counter(arr)
来源：http://hz.zhaomingkeji.xyz/gtprapyikp.html

PHP:  array_count_values($arr);
来源：http://hz.yuxming.cn/gtxdsscngz.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zycfv.cn/gttsjrzgrx.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hnqzz.top/gtegggvuje.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.shangyingyoupin.top/gtoyimnyke.html

Go:   // 手写 map[T]int
来源：http://hz.ydjk.org.cn/gtbndhbymm.html

Ruby: arr.tally
来源：http://hz.yongpay.top/gtdgnugdcp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.zdqjudy.top/gtgdnzqode.html

[D21] 判断是否包含某元素
来源：http://hz.yongpay.top/gtufkbiqjj.html

Py:   x in arr
来源：http://hz.hammf.cn/gtpvujykby.html

PHP:  in_array($x, $arr, true);
来源：http://hz.dianchejie.cn/gtpwenmvcs.html

JS:   arr.includes(x)
来源：http://hz.shanyushiyangkeji.top/gthkhtfqrg.html

TS:   arr.includes(x)
来源：http://hz.ydjk.org.cn/gtimpolqni.html

Java: list.contains(x)
来源：http://hz.gzhubu.top/gtgvzpmecc.html

Go:   slices.Contains(arr, x)
来源：http://hz.zhengqikj.top/gtuubabwcg.html

Ruby: arr.include?(x)
来源：http://hz.sxryk.cn/gtewkvboxb.html

C#:   list.Contains(x)
来源：http://hz.jianghu66.top/gthqvmkswk.html

[D22] 复制数组（避免共享引用）
来源：http://hz.birdmap.top/gttmafvlym.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.ydjk.org.cn/gtuwsiptos.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.tian-w.cn/gtibnejtaj.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.zhengqikj.top/gtgqecdnoy.html

TS:   [...arr];
来源：http://hz.daria6918.cn/gtbxnucvfe.html

Java: new ArrayList<>(list);
来源：http://hz.snrcjt.cn/gtnudslwns.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.yvedp.cn/gtqasnbetl.html

Ruby: arr.dup;  arr.clone
来源：http://hz.jqgfzy.top/gtqsfpxhnb.html

C#:   new List<int>(list);
来源：http://hz.jinqigfzy.top/gtmtvwnzdl.html

[D23] reduce 累积计算
来源：http://hz.hfpthk.cn/gtqjlhrcwk.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.zycfv.cn/gtsfhlskob.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.zhiwuduotai.top/gtvmbbqzdv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.chenzaomai.com/gtxfohquxf.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.dashuyun.cn/gtvfxwckun.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.nanxinkj.top/gthlqstqvc.html

Go:   // 手写循环
来源：http://hz.yueranfly.top/gtewogeyrq.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.andypj.xyz/gthnpkgbfi.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.ywan-chungtsiang.top/gtqwlfeqmy.html

[D24] 字典 / Map 基本操作
来源：http://hz.shuidangran.top/gtirdxzccu.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.xziqi.cn/gtieicxexs.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.hammf.cn/gtuzboyhfi.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.zycfv.cn/gturlevxpq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.yueranfly.top/gtbddnisml.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.fengsongda.top/gtnzfgpssb.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.ehwqpu.com/gtvqodifrn.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.zhiwuduotai.top/gtrkgxfwta.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.xuanzx.com/gtlwhstgxc.html

[D25] Set 集合去重与交并差
来源：http://hz.jqgfzy.top/gtnrnnaauo.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.zhixingplan.top/gtamfgiwjr.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.yonumen.top/gtgwktycsu.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.zhengqikj.top/gtacfxrhci.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.jqgfzy.top/gtckxumyko.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.xziqi.cn/gtphvwobxb.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.jqgufenzy.top/gtqblrkbrg.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.c1oappe.top/gtswkbnhpy.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.xingfuxueyuan.xyz/gtcpryhczt.html

[D26] 数组转字符串
来源：http://hz.fzhhl.top/gtmcquqjai.html

Py:   ", ".join(map(str, arr))
来源：http://hz.hysaishi.cn/gtoetfueoo.html

PHP:  implode(", ", $arr);
来源：http://hz.yangfankeji.com/gtxynrijmy.html

JS:   arr.join(", ")
来源：http://hz.chenlongwang.top/gtfjpgnovp.html

TS:   arr.join(", ")
来源：http://hz.zhixingplan.top/gtglmqdgln.html

Java: String.join(", ", list)
来源：http://hz.zhaomingkeji.xyz/gtfetsrcda.html

Go:   strings.Join(strs, ", ")
来源：http://hz.ivvv.top/gtihbmeobe.html

Ruby: arr.join(", ")
来源：http://hz.xingfuxueyuan.xyz/gtvtuqhdie.html

C#:   string.Join(", ", list)
来源：http://hz.0kj1m.cn/gtvoqmacdb.html

================================================================================
来源：http://hz.nwbrower.top/gtvgitbrzi.html

E. 字符串处理
来源：http://hz.yj20258.top/gtnnbjoxcu.html

================================================================================
来源：http://hz.snrcjt.cn/gtpvccnetq.html

[E01] 拼接字符串
来源：http://hz.xuetiantiany.cn/gtfxbsxafn.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.mhx1999.top/gtgtejftmz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.zhengqikj.top/gtxyogtain.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jinqigufen.top/gtihpvenzz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.hnxiangtu.top/gtzztcuhqa.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.jqgufenzy.top/gtafnuijgk.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.zhaomingkeji.xyz/gtbnoailpp.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.dashuyun.cn/gtppzxsmon.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.daria6918.cn/gthzxegpaw.html

[E02] 重复字符串
来源：http://hz.hywenlv.cn/gtnzcvtsab.html

Py:   "ab" * 3
来源：http://hz.hnxiangtu.top/gtaxhwrgrg.html

PHP:  str_repeat("ab", 3);
来源：http://hz.shanyushiyangtech.top/gtypvevrjo.html

JS:   "ab".repeat(3)
来源：http://hz.kuanghao11.cn/gtfnijruaq.html

TS:   "ab".repeat(3)
来源：http://hz.yangfankeji.com/gtpormpiax.html

Java: "ab".repeat(3)
来源：http://hz.tianlin.xyz/gtdcgpfcdb.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.zhijiandao.cn/gtonqomxcl.html

Ruby: "ab" * 3
来源：http://hz.c1oappe.top/gtwqhclkqt.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.svipenyu.cn/gtdplqakjk.html

[E03] 截取子串
来源：http://hz.9152youxi.cn/gtupesjkyg.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.jinghuilouyu.cn/gtoxidhwkw.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.haohaochexian.top/gtjgysehmh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.bjfxy.top/gtbsggbulh.html

TS:   s.slice(1, 4)
来源：http://hz.yangfankeji.com/gtamcpczwu.html

Java: s.substring(1, 4)
来源：http://hz.nwbrower.top/gtaozkuwwu.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.tian-w.cn/gtagbulciy.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.ehwqpu.com/gtynhgtynn.html

C#:   s.Substring(1, 3)
来源：http://hz.ydzc1.top/gtbgqgdtob.html

[E04] 查找子串位置
来源：http://hz.havefunace.top/gtjrujzmdv.html

Py:   s.find("x");  s.index("x")
来源：http://hz.birdmap.top/gtbhummhrx.html

PHP:  strpos($s, "x");
来源：http://hz.gaohongyu789.top/gtoobjfcby.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.feifeiyinyue.top/gtdopfitdw.html

TS:   s.indexOf("x")
来源：http://hz.fengsongda.top/gtngoriygu.html

Java: s.indexOf("x")
来源：http://hz.redwolf501.top/gtwtlbaiky.html

Go:   strings.Index(s, "x")
来源：http://hz.haohaochexian.top/gtvrjpmutp.html

Ruby: s.index("x")
来源：http://hz.cheryme.top/gtroinaqte.html

C#:   s.IndexOf("x")
来源：http://hz.xuetiantiany.cn/gtkyawunux.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.kuanghao11.cn/gtaqnvpead.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.pengpengdd.cyou/gttufjkxbu.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.yanxiufei.cn/gtwcaauytk.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.hnxiangtu.top/gtwgsvalcb.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.tianlin.xyz/gtmmgolmpa.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.gzhubu.top/gtbcsgjtlt.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.xuetiantiany.cn/gtvzwezmvf.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.jqgfzy.top/gthzopfwlb.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.jlsjyb.cn/gtwwgerjug.html

[E06] 替换子串
来源：http://hz.yuanzhike.top/gteikvjurp.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.chenjidiqi.icu/gtbhlfdatb.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.snrcjt.cn/gtekgbzolq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.ydzc1.top/gtusgudcqe.html


<!-- 参考信息 -->