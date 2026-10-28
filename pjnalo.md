代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.zdqjudy.top/gtetntybsy.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.zhaomingkeji.xyz/gtgemgjuut.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.xziqi.cn/gtsdkeizmr.html

Ruby: # 无泛型
来源：http://hz.hnqzz.top/gtfmnflqsr.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.316326.xyz/gteaenujjz.html

[C15] 解构 / 展开参数
来源：http://hz.jqgfzy.top/gtlaeiphzn.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.daxiang520.top/gtmkfiequh.html

PHP:  [$a, $b] = $pair;
来源：http://hz.tanke756.top/gtwaftjhcp.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.ywan-chungtsiang.top/gtgafgcmbf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.jinghuilouyu.cn/gtkhfxkeqm.html

Java: // 无解构
来源：http://hz.tian-w.cn/gtrxdmpniq.html

Go:   // 无解构
来源：http://hz.fzhhl.top/gtrdocmbew.html

Ruby: a, b = pair
来源：http://hz.haohaochexian.top/gtjbdsujyh.html

C#:   var (a, b) = pair;
来源：http://hz.haohaochexian.top/gtdtbsdfah.html

[C16] 函数 / 方法重载
来源：http://hz.jinyuanbaomall.cn/gtbwvqsnwr.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.zdqjudy.top/gtaxfqylat.html

PHP:  // 无重载
来源：http://hz.mhx1999.top/gtbspbttpq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.shzxlz.cn/gtorwpsuyu.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.hywenlv.cn/gtuaqsjzod.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.ywan-chungtsiang.top/gtjhiqnfuo.html

Go:   // 无重载：用不同函数名
来源：http://hz.316326.xyz/gtibeofylx.html

Ruby: # 无重载：靠动态参数
来源：http://hz.yj202588.top/gtazvkqhkm.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.jyoumei.cn/gtdpjxzurh.html

================================================================================
来源：http://hz.cashguo.top/gtlgpefhki.html

D. 数组 / 列表 / 集合
来源：http://hz.gaohongyu789.top/gtidggmmbr.html

================================================================================
来源：http://hz.yuxming.cn/gtbucgjtfm.html

[D01] 创建数组 / 列表
来源：http://hz.xylfe.cn/gtsscarzjf.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.vqdsnc.cn/gtuhglmtge.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.ydzc1.top/gtluzzrdjb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.pengpengdd.cyou/gtxonxphfs.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.hammf.cn/gtthuipnmn.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.xinyue.icu/gtpjifqzqm.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.tian-w.cn/gtuurlmtxo.html

Ruby: arr = [1, 2, 3]
来源：http://hz.hnqzz.top/gtdsugtwry.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.tian-w.cn/gtobfgwake.html

[D02] 追加元素到末尾
来源：http://hz.nanxuanxn.top/gtivphagdd.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.gotoacloud.top/gtnqukkieb.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.kuanghao11.cn/gtpmdmrmak.html

JS:   arr.push(4);
来源：http://hz.birdmap.top/gtlglkjyeb.html

TS:   arr.push(4);
来源：http://hz.0kj1m.cn/gtddhkqkba.html

Java: list.add(4);
来源：http://hz.hammf.cn/gtoqpmabol.html

Go:   arr = append(arr, 4)
来源：http://hz.hnqzz.top/gtpmftjmmw.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.tian-w.cn/gtvkbijlkm.html

C#:   list.Add(4);
来源：http://hz.sufxvd.cn/gtpcrktipv.html

[D03] 在指定位置插入元素
来源：http://hz.jiagoushi.top/gtmdilonoh.html

Py:   arr.insert(0, 0)
来源：http://hz.yvedp.cn/gtzyxgqcrm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.mhx1999.top/gtttxghozy.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.nanxinkj.top/gtshpehydn.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.aizwys.cn/gtqtpsqmvz.html

Java: list.add(0, 0);
来源：http://hz.shzxlz.cn/gtumnfgrta.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.yueranfly.top/gtraxgzxxz.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.redwolf501.top/gtlbauvpno.html

C#:   list.Insert(0, 0);
来源：http://hz.shanyushiyangkeji.top/gtxhlalyjx.html

[D04] 删除元素
来源：http://hz.hongshengwenyu.top/gtopaslcer.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.sufxvd.cn/gthqjpzmme.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.hammf.cn/gtjnktvvvr.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.daria6918.cn/gtbnxqnivj.html

TS:   arr.splice(0, 1);
来源：http://hz.xylfe.cn/gtqpjidpfz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.yueranfly.top/gtgedqyrvx.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.hongshengwenyu.top/gtfqtxelqj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.yueranfly.top/gtaqkgojbl.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.gotoacloud.top/gthikjdgbq.html

[D05] 访问与修改元素
来源：http://hz.shzxlz.cn/gtfhmqrrqh.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.sxryk.cn/gtuxzcgnvq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.kuanghao11.cn/gtupjhbfcr.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.pengpengdd.cyou/gtlllzhbjq.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.tian-w.cn/gtmgjhypbu.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.chenjidiqi.icu/gtgpjeapcv.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.sweek.top/gteynfnzrm.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.xinyue.icu/gtblmfarkx.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.sufxvd.cn/gtosflqdie.html

[D06] 数组长度
来源：http://hz.wangshuangyany.cn/gtoqpmyfpp.html

Py:   len(arr)
来源：http://hz.yj202588.top/gtvwgiwhxs.html

PHP:  count($arr);
来源：http://hz.chenlongwang.top/gtuhjzzxxz.html

JS:   arr.length
来源：http://hz.yj202588.top/gtjaabugyu.html

TS:   arr.length
来源：http://hz.cheryme.top/gthfqezmdu.html

Java: list.size();
来源：http://hz.cucudq.cn/gtvkrpofyg.html

Go:   len(arr)
来源：http://hz.yj20258.top/gtplvvjojo.html

Ruby: arr.length; arr.size
来源：http://hz.xinyue.icu/gtxkygczhf.html

C#:   list.Count;
来源：http://hz.hnqzz.top/gtatvzdjsh.html

[D07] 切片 / 取子数组
来源：http://hz.haohaochexian.top/gtsoedqlzr.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.yj202588.top/gttzxoefja.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.xuetiantiany.cn/gthgumkhbl.html

JS:   arr.slice(1, 4);
来源：http://hz.jqgfzy.top/gtjxfwpbqo.html

TS:   arr.slice(1, 4);
来源：http://hz.jqgfzy.top/gtbdcgmdcp.html

Java: list.subList(1, 4);
来源：http://hz.quarkkingdee.top/gtgjsrieqe.html

Go:   arr[1:4]
来源：http://hz.yongpay.top/gtlvzgtwxw.html

Ruby: arr[1, 3]
来源：http://hz.iojbl.cn/gtdfcixwuk.html

C#:   list.GetRange(1, 3);
来源：http://hz.yuxming.cn/gtkyhliynl.html

[D08] 合并两个数组
来源：http://hz.sufxvd.cn/gthfkzesqh.html

Py:   a + b;  a.extend(b)
来源：http://hz.bjfxy.top/gtysrxfftw.html

PHP:  array_merge($a, $b);
来源：http://hz.zhiwuduotai.top/gtsgzzppaf.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.xuanzx.com/gtkrpyneao.html

TS:   [...a, ...b];
来源：http://hz.hnxiangtu.top/gtqvdmkkri.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.xinyue.icu/gtvwaifgel.html

Go:   append(a, b...)
来源：http://hz.zhongyouzk.top/gtemsddsvw.html

Ruby: a + b;  a.concat(b)
来源：http://hz.yueranfly.top/gtixwyxnvo.html

C#:   a.Concat(b).ToList()
来源：http://hz.jqgufenzy.top/gtcjyamojh.html

[D09] 排序（升序）
来源：http://hz.jinqigfzy.top/gthwagcvin.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jlsjyb.cn/gtcdecupxv.html

PHP:  sort($arr);
来源：http://hz.c1oappe.top/gthyiidqwh.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.zhongyouzk.top/gtmzapypff.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.cashguo.top/gtilrvpcgs.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.cheryme.top/gtznbuococ.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.jianghu66.top/gteqvlajiq.html

Ruby: arr.sort
来源：http://hz.tianlin.xyz/gtpucirbhq.html

C#:   list.Sort();
来源：http://hz.316326.xyz/gtceixnlxm.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.cucudq.cn/gtyqpuwzbf.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.xziqi.cn/gtfyswcubx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.cucudq.cn/gtbboxolrq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.shuidangran.top/gteeyclmum.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yj20258888.top/gtiibgdapk.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.wangdashe.top/gtinbgoyvk.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.yueranfly.top/gthznbkjff.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.yuxming.cn/gtigrohtho.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.9152youxi.cn/gtmglpjkow.html

[D11] 反转数组
来源：http://hz.pycfn.com/gtvgfrinao.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.ivvv.top/gtqqlszcpw.html

PHP:  array_reverse($arr);
来源：http://hz.gzhubu.top/gtttbipvnj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.sweek.top/gtdybegcfa.html

TS:   [...arr].reverse();
来源：http://hz.ivvv.top/gtesskhnbh.html

Java: Collections.reverse(list);
来源：http://hz.haohaochexian.top/gtdshddhzq.html

Go:   slices.Reverse(arr)
来源：http://hz.shuidangran.top/gtmfeenouc.html

Ruby: arr.reverse
来源：http://hz.pengpengdd.cyou/gtfrabbhie.html

C#:   list.Reverse();
来源：http://hz.meibo888.top/gtosggznvp.html

[D12] 查找元素下标
来源：http://hz.fzhhl.top/gtrcfcopqa.html

Py:   arr.index(x);  x in arr
来源：http://hz.bjfxy.top/gtrgjsswib.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.meibo888.top/gtnmcybqop.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jqgfzy.top/gtyhtznqyq.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.shuidangran.top/gtyxykgklk.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.shangyingyoupin.top/gtvkahgtuu.html

Go:   slices.Index(arr, x)
来源：http://hz.ywan-chungtsiang.top/gtidnxffhv.html

Ruby: arr.index(x)
来源：http://hz.nanxinkj.top/gtamyxuhfw.html

C#:   list.IndexOf(x);
来源：http://hz.shanyushiyangtech.top/gtqybpauph.html

[D13] 过滤（保留满足条件的）
来源：http://hz.hysaishi.cn/gthdqjnmum.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.hongshengwenyu.top/gtkoxgygmc.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.mhx1999.top/gtmufndskk.html

JS:   arr.filter(x => x > 3)
来源：http://hz.cucudq.cn/gtocsjufjr.html

TS:   arr.filter(x => x > 3)
来源：http://hz.jinqigufen.top/gtpsmxyjmp.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.ydzc1.top/gtaidmytle.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.tanke756.top/gtpyvzwibn.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.zhoulong.xyz/gtixshhfso.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.ydzc1.top/gtgwngnjih.html

[D14] 映射转换（每个元素变形）
来源：http://hz.tianlin.xyz/gtmgvhcvxm.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.zhiwuduotai.top/gtnihpscse.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.ydjk.org.cn/gtgpqmdzkn.html

JS:   arr.map(x => x * 2)
来源：http://hz.shzxlz.cn/gtffbvwfxn.html

TS:   arr.map(x => x * 2)
来源：http://hz.jiagoushi.top/gtdnnjtgpn.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.jyoumei.cn/gtvxbhxfci.html

Go:   // 手写循环
来源：http://hz.jinyuanbaomall.cn/gtqijntesd.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.mhx1999.top/gtarxlmnst.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.zhixingplan.top/gtgaldnzyp.html

[D15] 去重
来源：http://hz.kuanghao11.cn/gtlabvrail.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.shangyingyoupin.top/gtkogrlkdx.html

PHP:  array_unique($arr);
来源：http://hz.hywenlv.cn/gtcneyvlmh.html

JS:   [...new Set(arr)]
来源：http://hz.dashuyun.cn/gtsshjxxwi.html

TS:   [...new Set(arr)]
来源：http://hz.gaohongyu789.top/gtkxcfnsmu.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.shangyingyoupin.top/gtukwvsczf.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.jiagoushi.top/gtypkyjntv.html

Ruby: arr.uniq
来源：http://hz.gaohongyu789.top/gtqettfzsx.html

C#:   list.Distinct().ToList()
来源：http://hz.kuanghao11.cn/gtmxtvnaob.html

[D16] 求和与平均值
来源：http://hz.pycfn.com/gtosnulztt.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.xuanzx.com/gtvcxvcpoc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.dianchejie.cn/gtdzgenvmj.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yanxiufei.cn/gtiiaxlreg.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zhijiandao.cn/gteozpsrnz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.52xcode.cn/gtueduxnss.html

Go:   // 手写循环累加
来源：http://hz.dianchejie.cn/gtyaispuxb.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.316326.xyz/gtijnkupsz.html

C#:   list.Sum();  list.Average()
来源：http://hz.smart0.xyz/gtrrggilca.html

[D17] 最大值与最小值
来源：http://hz.cucudq.cn/gtbnxmsmpy.html

Py:   max(arr);  min(arr)
来源：http://hz.shanyushiyangtech.top/gtcbjzollz.html

PHP:  max($arr);  min($arr);
来源：http://hz.havefunace.top/gtpqiemjxf.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.redwolf501.top/gtddcxxckp.html

TS:   Math.max(...arr);
来源：http://hz.xziqi.cn/gtcnmevppf.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.sxryk.cn/gtnvjryzkd.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.tian-w.cn/gthimviwxw.html

Ruby: arr.max;  arr.min
来源：http://hz.yanxiufei.cn/gtmfwiuolf.html

C#:   list.Max();  list.Min()
来源：http://hz.yongpay.top/gthgpuznch.html

[D18] 扁平化嵌套数组
来源：http://hz.gaohongyu789.top/gtcfgvzezv.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.chenjidiqi.icu/gtdbykbins.html

PHP:  array_merge(...$nested);
来源：http://hz.ydzc1.top/gtrwrvjyea.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.hammf.cn/gtsidegjbt.html

TS:   nested.flat();
来源：http://hz.chenlongwang.top/gtgmqkrndf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.ybcxt.top/gtkwyupihl.html

Go:   // 手写双层循环
来源：http://hz.jianghu66.top/gtvopdbinu.html

Ruby: nested.flatten
来源：http://hz.feifeiyinyue.top/gtihkbabpz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.mhx1999.top/gtyqvtquzg.html

[D19] 按字段分组
来源：http://hz.kuanghao11.cn/gtdhudtbdu.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.andypj.xyz/gtcscqsjog.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.ivvv.top/gtbjfonlcb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.ywan-chungtsiang.top/gtikixmyss.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.jqgufenzy.top/gtmqpyqxve.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.ywan-chungtsiang.top/gtnneltltc.html

Go:   // 手写 map[string][]T
来源：http://hz.c1oappe.top/gteoheepzq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.nanxuanxn.top/gtsmavwqng.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.ydjk.org.cn/gtceebvcpb.html

[D20] 统计每个元素出现次数
来源：http://hz.hfpthk.cn/gtvsubzexz.html

Py:   Counter(arr)
来源：http://hz.shanyushiyangkeji.top/gtyayhfoij.html

PHP:  array_count_values($arr);
来源：http://hz.shanyushiyangkeji.top/gtxtkqyskz.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.aibaodan.cn/gtzrnpiwhf.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.shangyingyoupin.top/gtdqjezowp.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.shzxlz.cn/gtnxcqzsrp.html

Go:   // 手写 map[T]int
来源：http://hz.vqdsnc.cn/gtwdjnrgip.html

Ruby: arr.tally
来源：http://hz.jqgfzy.top/gtjrqzmbvs.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.fengsongda.top/gtdcuktavf.html

[D21] 判断是否包含某元素
来源：http://hz.jyoumei.cn/gtbtaqchjm.html

Py:   x in arr
来源：http://hz.shanyushiyangtech.top/gtrkjmekqy.html

PHP:  in_array($x, $arr, true);
来源：http://hz.hongshengwenyu.top/gtbkprxxjt.html

JS:   arr.includes(x)
来源：http://hz.aibaodan.cn/gtkntdoobm.html

TS:   arr.includes(x)
来源：http://hz.shangyingyoupin.top/gtlvgdggbj.html

Java: list.contains(x)
来源：http://hz.yanxiufei.cn/gtbolspvfo.html

Go:   slices.Contains(arr, x)
来源：http://hz.gogol.net.cn/gtrnncoxym.html

Ruby: arr.include?(x)
来源：http://hz.smart0.xyz/gtvldmlthq.html

C#:   list.Contains(x)
来源：http://hz.jinghuilouyu.cn/gtmdcvelbp.html

[D22] 复制数组（避免共享引用）
来源：http://hz.smart0.xyz/gtosrybjgw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.aibaodan.cn/gttibppyeu.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.birdmap.top/gtmizmeujb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.sxryk.cn/gtlxybhbmx.html

TS:   [...arr];
来源：http://hz.hongshengwenyu.top/gtarnllfie.html

Java: new ArrayList<>(list);
来源：http://hz.jinqigufen.top/gtjghnwcbt.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.pycfn.com/gtlgotcjec.html

Ruby: arr.dup;  arr.clone
来源：http://hz.xuetiantiany.cn/gthvudoyny.html

C#:   new List<int>(list);
来源：http://hz.sxryk.cn/gtjprdqfwl.html

[D23] reduce 累积计算
来源：http://hz.xuanzx.com/gtkywfaicb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.yj20258.top/gtcwogbcrs.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.wangdashe.top/gtuwhgrakw.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yonumen.top/gtknqxeefp.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.shangyingyoupin.top/gtoaabwgoq.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.9152youxi.cn/gtdclbuzfq.html

Go:   // 手写循环
来源：http://hz.xziqi.cn/gtksdfpcbi.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.316326.xyz/gtzwqinnry.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.hammf.cn/gtrgccfroo.html

[D24] 字典 / Map 基本操作
来源：http://hz.jinqigfzy.top/gtxarjuinu.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.shzxlz.cn/gtbmrfydad.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.kuanghao11.cn/gtncxzgaul.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.smart0.xyz/gtcwphotyk.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.shzxlz.cn/gtijmuvuvj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.nanxuanxn.top/gtqhxtuwlq.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.cashguo.top/gtgidphebz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.nanxinkj.top/gtdjiunjvw.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.zhixingplan.top/gtbcsflmlh.html

[D25] Set 集合去重与交并差
来源：http://hz.bjfxy.top/gtnzxxxxop.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.pengpengdd.cyou/gtawulhles.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.gaohongyu789.top/gtozjafepx.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.xuetiantiany.cn/gtzlytzvzs.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.jiagoushi.top/gtqzzbdvhi.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.ydjk.org.cn/gtzaxmbhnw.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.hnqzz.top/gtzoxshrvl.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.birdmap.top/gtqggcfgch.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.zhongyouzk.top/gttekqmfxx.html

[D26] 数组转字符串
来源：http://hz.yanxiufei.cn/gtdkehcqqo.html

Py:   ", ".join(map(str, arr))
来源：http://hz.jinghuilouyu.cn/gtseargvsi.html

PHP:  implode(", ", $arr);
来源：http://hz.sweek.top/gtrvassjxq.html

JS:   arr.join(", ")
来源：http://hz.svipenyu.cn/gtjaqhxizx.html

TS:   arr.join(", ")
来源：http://hz.jqgfzy.top/gtxyqxlptg.html

Java: String.join(", ", list)
来源：http://hz.pycfn.com/gtuqxxeqbe.html

Go:   strings.Join(strs, ", ")
来源：http://hz.cheryme.top/gtwugsjrjp.html

Ruby: arr.join(", ")
来源：http://hz.cucudq.cn/gtpykzjugo.html

C#:   string.Join(", ", list)
来源：http://hz.gzhubu.top/gtckzgplup.html

================================================================================
来源：http://hz.yuxming.cn/gtqqvzyfpp.html

E. 字符串处理
来源：http://hz.daxiang520.top/gtsjdcsqvf.html

================================================================================
来源：http://hz.sweek.top/gtvzufwfqk.html

[E01] 拼接字符串
来源：http://hz.chenjidiqi.icu/gtwugvoqdz.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.dianchejie.cn/gtyhlvipns.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.yuxming.cn/gtxeihxylm.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zhijiandao.cn/gtabefixpy.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zhaomingkeji.xyz/gtvluyuamc.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.shangyingyoupin.top/gtgshqahfn.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.mhx1999.top/gthtqqiggj.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.9152youxi.cn/gthhmtzatz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.fzhhl.top/gtmbugiont.html

[E02] 重复字符串
来源：http://hz.zdqjudy.top/gtbedafhmg.html

Py:   "ab" * 3
来源：http://hz.aibaodan.cn/gtfaaspiyn.html

PHP:  str_repeat("ab", 3);
来源：http://hz.havefunace.top/gtvgsosoad.html

JS:   "ab".repeat(3)
来源：http://hz.hongshengwenyu.top/gtphjrrijg.html

TS:   "ab".repeat(3)
来源：http://hz.pycfn.com/gtvfwukqkf.html

Java: "ab".repeat(3)
来源：http://hz.52xcode.cn/gtipatlyuo.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.cashguo.top/gtzxjfiire.html

Ruby: "ab" * 3
来源：http://hz.jiagoushi.top/gtfzjddtmj.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.xuanzx.com/gtuhppmuvy.html

[E03] 截取子串
来源：http://hz.shzxlz.cn/gtshxlytbg.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.hfpthk.cn/gtuvucsefb.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.sxryk.cn/gtjhoyvqxz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.sysykeji.top/gtnxqwrwer.html

TS:   s.slice(1, 4)
来源：http://hz.jinghuilouyu.cn/gtqozvnuzi.html

Java: s.substring(1, 4)
来源：http://hz.xziqi.cn/gtffdjmuws.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.yanxiufei.cn/gtwzfhxvzw.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.gzhubu.top/gtjpjmlmwb.html

C#:   s.Substring(1, 3)
来源：http://hz.birdmap.top/gtjlbbkylh.html

[E04] 查找子串位置
来源：http://hz.chenzaomai.com/gtlcmndivk.html

Py:   s.find("x");  s.index("x")
来源：http://hz.shuidangran.top/gtoffikcwr.html

PHP:  strpos($s, "x");
来源：http://hz.ybcxt.top/gthsnvohgu.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.yangfankeji.com/gtwvyddwsa.html

TS:   s.indexOf("x")
来源：http://hz.chenlongwang.top/gtfqdqicko.html

Java: s.indexOf("x")
来源：http://hz.0kj1m.cn/gtemjyxhek.html

Go:   strings.Index(s, "x")
来源：http://hz.guowangkeji.top/gtgurdtkxt.html

Ruby: s.index("x")
来源：http://hz.hysaishi.cn/gtjqqmchod.html

C#:   s.IndexOf("x")
来源：http://hz.yj20258888.top/gtptembaug.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.yangfankeji.com/gtwebojzjf.html


<!-- 参考信息 -->