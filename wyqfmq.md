代发 wailian999

[C14] 泛型函数
来源：http://hz.c1oappe.top/gtmxiatloo.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.zdqjudy.top/gtwwpvpbzx.html

PHP:  // 无泛型
来源：http://hz.sweek.top/gtcbkjgeqp.html

JS:   // 无泛型
来源：http://hz.sysykeji.top/gthvewvvef.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.tian-w.cn/gtvnfhilor.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.ybcxt.top/gtggmzcjei.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.fzhhl.top/gtacuipppt.html

Ruby: # 无泛型
来源：http://hz.chenjidiqi.icu/gtzyjqhdpk.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.pengpengdd.cyou/gtpbofqgyg.html

[C15] 解构 / 展开参数
来源：http://hz.sxryk.cn/gtysakalwc.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.zdqjudy.top/gtkxaaoopb.html

PHP:  [$a, $b] = $pair;
来源：http://hz.yonumen.top/gtzajoauts.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.c1oappe.top/gtnjctdwcx.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.chenlongwang.top/gtbinjnhhd.html

Java: // 无解构
来源：http://hz.ehwqpu.com/gtisfjyknr.html

Go:   // 无解构
来源：http://hz.hfpthk.cn/gtlaqjucbz.html

Ruby: a, b = pair
来源：http://hz.yonumen.top/gtuaqwpamf.html

C#:   var (a, b) = pair;
来源：http://hz.birdmap.top/gtyfpdvyfj.html

[C16] 函数 / 方法重载
来源：http://hz.jinqigufen.top/gtuujobtbc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.ywan-chungtsiang.top/gtjjxiclsl.html

PHP:  // 无重载
来源：http://hz.yj20258.top/gtguoowedj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.yanxiufei.cn/gtwvcrnoag.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.pengpengdd.cyou/gtkjzspznp.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.zhixingplan.top/gtiuupciod.html

Go:   // 无重载：用不同函数名
来源：http://hz.cheryme.top/gtlxwlajki.html

Ruby: # 无重载：靠动态参数
来源：http://hz.ywan-chungtsiang.top/gtjhotrmhq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.meibo888.top/gtvmstkmya.html

================================================================================
来源：http://hz.yuxming.cn/gtaqidyxyq.html

D. 数组 / 列表 / 集合
来源：http://hz.chenjidiqi.icu/gtkqqkgknj.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtvgteruhn.html

[D01] 创建数组 / 列表
来源：http://hz.yj20258.top/gtsbucoapw.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.hongshengwenyu.top/gtypxrtzjh.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.xziqi.cn/gtatiirkxe.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.9152youxi.cn/gtmnqtvxjm.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.52xcode.cn/gthexrxhkn.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.0kj1m.cn/gtllgecrdp.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.ybcxt.top/gtzyndeypf.html

Ruby: arr = [1, 2, 3]
来源：http://hz.jiagoushi.top/gtbokgzprg.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.wangshuangyany.cn/gtfgntxmrl.html

[D02] 追加元素到末尾
来源：http://hz.jqgfzy.top/gtuvdaprre.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.yuxming.cn/gtwblzrvpr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.xuanzx.com/gtiudelgld.html

JS:   arr.push(4);
来源：http://hz.yongpay.top/gtdnelqcgn.html

TS:   arr.push(4);
来源：http://hz.hnxiangtu.top/gteiaqjelj.html

Java: list.add(4);
来源：http://hz.aizwys.cn/gtfbvldltn.html

Go:   arr = append(arr, 4)
来源：http://hz.jianghu66.top/gtiyakiobx.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.jlsjyb.cn/gtrbdvdlll.html

C#:   list.Add(4);
来源：http://hz.xylfe.cn/gtrkqbvaoa.html

[D03] 在指定位置插入元素
来源：http://hz.cqqwz.cn/gtdfthofkv.html

Py:   arr.insert(0, 0)
来源：http://hz.sysykeji.top/gtjceauros.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.jinyuanbaomall.cn/gtvzjzzzxo.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.ydzc1.top/gtbwhcfwze.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.gogol.net.cn/gtmviiksbe.html

Java: list.add(0, 0);
来源：http://hz.fengsongda.top/gttyvfjred.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.gotoacloud.top/gtowkkyetz.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.jinyuanbaomall.cn/gtbwccvbbd.html

C#:   list.Insert(0, 0);
来源：http://hz.havefunace.top/gtmysewgwl.html

[D04] 删除元素
来源：http://hz.chenlongwang.top/gtrbjbtuwa.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.zycfv.cn/gtnquveqtk.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.cashguo.top/gtteynwblv.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.yueranfly.top/gtyyhqglye.html

TS:   arr.splice(0, 1);
来源：http://hz.xinyue.icu/gtlxnydgxw.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.zycfv.cn/gtonsptnqs.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.yuanzhike.top/gtksqmxuhe.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.yuanzhike.top/gttqdyvivu.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.zhoulong.xyz/gtxxchgomg.html

[D05] 访问与修改元素
来源：http://hz.yj20258.top/gtkytazeow.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.meibo888.top/gtaxpnwbzq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.0kj1m.cn/gtzkxvnepr.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.sweek.top/gtltmwbfpn.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.zdqjudy.top/gtbceaxtyq.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.sufxvd.cn/gtchueuwna.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.pycfn.com/gtljcvqnfe.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.ywan-chungtsiang.top/gtyrnjvwpi.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.chenlongwang.top/gtlrstevpd.html

[D06] 数组长度
来源：http://hz.daxiang520.top/gtacrvjhvu.html

Py:   len(arr)
来源：http://hz.haohaochexian.top/gtstxegule.html

PHP:  count($arr);
来源：http://hz.sysykeji.top/gtkraufdfb.html

JS:   arr.length
来源：http://hz.pycfn.com/gtzlqkrxuk.html

TS:   arr.length
来源：http://hz.dashuyun.cn/gtqgejxogg.html

Java: list.size();
来源：http://hz.birdmap.top/gtcbzwbxdg.html

Go:   len(arr)
来源：http://hz.pycfn.com/gtuhqjqzmv.html

Ruby: arr.length; arr.size
来源：http://hz.chenlongwang.top/gtmsfegvmi.html

C#:   list.Count;
来源：http://hz.aizwys.cn/gtndjifipd.html

[D07] 切片 / 取子数组
来源：http://hz.cqqwz.cn/gtvzkfktcn.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.zhiwuduotai.top/gtexnwvllc.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.aibaodan.cn/gtgykagmyl.html

JS:   arr.slice(1, 4);
来源：http://hz.jqgfzy.top/gtbidvcnav.html

TS:   arr.slice(1, 4);
来源：http://hz.ivvv.top/gtxqgzgcxt.html

Java: list.subList(1, 4);
来源：http://hz.jqgufenzy.top/gtsxcvjejl.html

Go:   arr[1:4]
来源：http://hz.hongshengwenyu.top/gtzjpsflby.html

Ruby: arr[1, 3]
来源：http://hz.cheryme.top/gtfauphomn.html

C#:   list.GetRange(1, 3);
来源：http://hz.ywan-chungtsiang.top/gtvbkuwuwj.html

[D08] 合并两个数组
来源：http://hz.tanke756.top/gtcewwcvak.html

Py:   a + b;  a.extend(b)
来源：http://hz.ivvv.top/gtnijrpndb.html

PHP:  array_merge($a, $b);
来源：http://hz.hammf.cn/gtnvtiuund.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.yueranfly.top/gttgaiewkt.html

TS:   [...a, ...b];
来源：http://hz.hammf.cn/gtnqvliptn.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.aibaodan.cn/gtsonxuqql.html

Go:   append(a, b...)
来源：http://hz.yangfankeji.com/gtpjbznqpd.html

Ruby: a + b;  a.concat(b)
来源：http://hz.hnqzz.top/gtcndprdea.html

C#:   a.Concat(b).ToList()
来源：http://hz.guannengcc.top/gtyvrbaour.html

[D09] 排序（升序）
来源：http://hz.cheryme.top/gtjqjqgadq.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhengqikj.top/gtfzmitpfk.html

PHP:  sort($arr);
来源：http://hz.xziqi.cn/gtqetrbuni.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.zycfv.cn/gtmylnecqh.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.hammf.cn/gtswqfbxco.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.zhiwuduotai.top/gtfzfbuoav.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.hnxiangtu.top/gtticiabew.html

Ruby: arr.sort
来源：http://hz.hongshengwenyu.top/gtxuujrtra.html

C#:   list.Sort();
来源：http://hz.gzhubu.top/gthqfjkqmb.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.cashguo.top/gtiejetjkc.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.xingfuxueyuan.xyz/gtrsspukep.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jinqigfzy.top/gtdgqznhfl.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jianghu66.top/gtmppyvyad.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.chenzaomai.com/gtjqvofexn.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.daxiang520.top/gteatkpjes.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.chenzaomai.com/gtmpqyhpjj.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.xuetiantiany.cn/gthzacigeo.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.ehwqpu.com/gtdiddhxkj.html

[D11] 反转数组
来源：http://hz.jyoumei.cn/gthptpcwxc.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.ivvv.top/gtixjzahlo.html

PHP:  array_reverse($arr);
来源：http://hz.yj202588.top/gtcojkkpov.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.feifeiyinyue.top/gtnrbriamw.html

TS:   [...arr].reverse();
来源：http://hz.jyoumei.cn/gtdbaoches.html

Java: Collections.reverse(list);
来源：http://hz.xylfe.cn/gtwcvzvzne.html

Go:   slices.Reverse(arr)
来源：http://hz.yangfankeji.com/gttisocrfa.html

Ruby: arr.reverse
来源：http://hz.tianlin.xyz/gtkehoulao.html

C#:   list.Reverse();
来源：http://hz.xuanzx.com/gtdzaydcpl.html

[D12] 查找元素下标
来源：http://hz.zhoulong.xyz/gtqzvqztma.html

Py:   arr.index(x);  x in arr
来源：http://hz.birdmap.top/gtlwdodzll.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.yongpay.top/gtjjfqfbvu.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yangfankeji.com/gtwaxoecee.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.cucudq.cn/gtahlzbgty.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.sysykeji.top/gtwkjyvpou.html

Go:   slices.Index(arr, x)
来源：http://hz.hnqzz.top/gtezybjlwl.html

Ruby: arr.index(x)
来源：http://hz.hysaishi.cn/gtsiizkplp.html

C#:   list.IndexOf(x);
来源：http://hz.redwolf501.top/gtvuirzsht.html

[D13] 过滤（保留满足条件的）
来源：http://hz.jianghu66.top/gtzoeqzlij.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.chenzaomai.com/gtstqvjkip.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.shanyushiyangtech.top/gtogxkuoyu.html

JS:   arr.filter(x => x > 3)
来源：http://hz.daxiang520.top/gtpwxefeky.html

TS:   arr.filter(x => x > 3)
来源：http://hz.gogol.net.cn/gtdgkezrxc.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.havefunace.top/gtrowpcakb.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.gaohongyu789.top/gthptrxmba.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.havefunace.top/gthmoeywdz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.iojbl.cn/gtozoqzlvz.html

[D14] 映射转换（每个元素变形）
来源：http://hz.gzhubu.top/gtjvwoylye.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.jlsjyb.cn/gtnecaolmi.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.fzhhl.top/gtavefjbyh.html

JS:   arr.map(x => x * 2)
来源：http://hz.jlsjyb.cn/gtdsgqkjvv.html

TS:   arr.map(x => x * 2)
来源：http://hz.shangyingyoupin.top/gtesnfpgju.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.cashguo.top/gtncnrkatf.html

Go:   // 手写循环
来源：http://hz.nanxuanxn.top/gtztcjcqyu.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.gaohongyu789.top/gteftryyjx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.dashuyun.cn/gtklvnvnvx.html

[D15] 去重
来源：http://hz.quarkkingdee.top/gtexltbymj.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.guowangkeji.top/gtmwfcfydt.html

PHP:  array_unique($arr);
来源：http://hz.aizwys.cn/gtvbeunuqv.html

JS:   [...new Set(arr)]
来源：http://hz.yuanzhike.top/gtctkdrbqt.html

TS:   [...new Set(arr)]
来源：http://hz.vqdsnc.cn/gtxvcpjodu.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.jinghuilouyu.cn/gtphuzcini.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.52xcode.cn/gtmndaebtf.html

Ruby: arr.uniq
来源：http://hz.zhiwuduotai.top/gtljahkwxc.html

C#:   list.Distinct().ToList()
来源：http://hz.zycfv.cn/gtmgvnnjlk.html

[D16] 求和与平均值
来源：http://hz.zhijiandao.cn/gtpszqrzxw.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.dashuyun.cn/gtnnfhpfvq.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.zdqjudy.top/gtejgvhwgd.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zhaomingkeji.xyz/gtvsrqaiie.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.andypj.xyz/gterxqjply.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.sysykeji.top/gtmrkjufby.html

Go:   // 手写循环累加
来源：http://hz.shanyushiyangkeji.top/gtyxgjivpf.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.snrcjt.cn/gtdgirehtb.html

C#:   list.Sum();  list.Average()
来源：http://hz.nanxuanxn.top/gtwypaiupk.html

[D17] 最大值与最小值
来源：http://hz.jqgfzy.top/gthiunqwvw.html

Py:   max(arr);  min(arr)
来源：http://hz.bjfxy.top/gtzyuziplq.html

PHP:  max($arr);  min($arr);
来源：http://hz.guowangkeji.top/gtnmllrbcv.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.yuanzhike.top/gtuhucrazg.html

TS:   Math.max(...arr);
来源：http://hz.jinyuanbaomall.cn/gtaynfxysk.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.dianchejie.cn/gtuoztghjd.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.ehwqpu.com/gtoaxervyr.html

Ruby: arr.max;  arr.min
来源：http://hz.vqdsnc.cn/gtmnxbkhkc.html

C#:   list.Max();  list.Min()
来源：http://hz.svipenyu.cn/gthpdxwrnw.html

[D18] 扁平化嵌套数组
来源：http://hz.yanxiufei.cn/gtjypoabys.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.jianghu66.top/gtdamagnhe.html

PHP:  array_merge(...$nested);
来源：http://hz.haohaochexian.top/gtotzjjogt.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.nwbrower.top/gtmcstvuwj.html

TS:   nested.flat();
来源：http://hz.iojbl.cn/gtttgschpv.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.nanxinkj.top/gtferndpen.html

Go:   // 手写双层循环
来源：http://hz.jqgfzy.top/gthzlymkzu.html

Ruby: nested.flatten
来源：http://hz.kuanghao11.cn/gtshecwlke.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.chenjidiqi.icu/gtoikxaegt.html

[D19] 按字段分组
来源：http://hz.jiagoushi.top/gtvakxxtnq.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.chenjidiqi.icu/gtjiwlxndg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.jyoumei.cn/gtlcywbsec.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.jyoumei.cn/gtquojwucm.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.nwbrower.top/gtkiijnsco.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.aibaodan.cn/gtnxnmzanh.html

Go:   // 手写 map[string][]T
来源：http://hz.zhengqikj.top/gtzbudlsim.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.tianlin.xyz/gtaozbtrwc.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.ivvv.top/gtlbljllxi.html

[D20] 统计每个元素出现次数
来源：http://hz.jqgfzy.top/gtjszihbnt.html

Py:   Counter(arr)
来源：http://hz.gaohongyu789.top/gtsqqpkwre.html

PHP:  array_count_values($arr);
来源：http://hz.jlsjyb.cn/gtmvubqypc.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.xingfuxueyuan.xyz/gtjuuxpjkz.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.quarkkingdee.top/gtzyrgalam.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.yueranfly.top/gtyddctlfm.html

Go:   // 手写 map[T]int
来源：http://hz.shanyushiyangkeji.top/gtorxtrtne.html

Ruby: arr.tally
来源：http://hz.jqgufenzy.top/gttnwfsbvz.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.jqgufenzy.top/gtvzmlnywd.html

[D21] 判断是否包含某元素
来源：http://hz.xuanzx.com/gtzcdzmprk.html

Py:   x in arr
来源：http://hz.ydzc1.top/gtglvwcdvf.html

PHP:  in_array($x, $arr, true);
来源：http://hz.sweek.top/gtlujsydhl.html

JS:   arr.includes(x)
来源：http://hz.jiagoushi.top/gtafjjtqjo.html

TS:   arr.includes(x)
来源：http://hz.nanxinkj.top/gtmbalciaz.html

Java: list.contains(x)
来源：http://hz.gogol.net.cn/gtqlbljcpo.html

Go:   slices.Contains(arr, x)
来源：http://hz.0kj1m.cn/gtuqghnzjt.html

Ruby: arr.include?(x)
来源：http://hz.pycfn.com/gtxmikciqf.html

C#:   list.Contains(x)
来源：http://hz.yj20258888.top/gtxtckjzky.html

[D22] 复制数组（避免共享引用）
来源：http://hz.ivvv.top/gtkshyqiyc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.birdmap.top/gtavfmkuay.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.tanke756.top/gtyfoskiem.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.jqgufenzy.top/gtowblwpva.html

TS:   [...arr];
来源：http://hz.jiagoushi.top/gtrpuvuytx.html

Java: new ArrayList<>(list);
来源：http://hz.xinyue.icu/gthsfereki.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.zhongyouzk.top/gtzuswnadb.html

Ruby: arr.dup;  arr.clone
来源：http://hz.zhaomingkeji.xyz/gtiwfjfuwy.html

C#:   new List<int>(list);
来源：http://hz.zhengqikj.top/gtinxhlall.html

[D23] reduce 累积计算
来源：http://hz.tanke756.top/gtxwmofdca.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.xuetiantiany.cn/gttycekhhs.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.sufxvd.cn/gtlsgfcoyn.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.sysykeji.top/gtuerbbyts.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.chenlongwang.top/gtgwfjgeqy.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.hammf.cn/gtuaiqrtuz.html

Go:   // 手写循环
来源：http://hz.mhx1999.top/gtoxapcwow.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.jinyuanbaomall.cn/gtkonjqdev.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.quarkkingdee.top/gtifibxhqg.html

[D24] 字典 / Map 基本操作
来源：http://hz.tianlin.xyz/gtodakykwb.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.nanxuanxn.top/gtpqdtloef.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.dianchejie.cn/gtnnlwqsrl.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.0kj1m.cn/gtowwnjlxq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.gaohongyu789.top/gtnpjpsvlu.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.daxiang520.top/gtyxltrtbv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.quarkkingdee.top/gtsxyalhbq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.smart0.xyz/gtzyyochnm.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.xingfuxueyuan.xyz/gtvrteydtq.html

[D25] Set 集合去重与交并差
来源：http://hz.tanke756.top/gtfeafkimp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.ydjk.org.cn/gtygtmpllu.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.birdmap.top/gtimrhmjir.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.hfpthk.cn/gtvukibayo.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.xziqi.cn/gtuobczghd.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.cqqwz.cn/gtpnaijlac.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.hnxiangtu.top/gtjijiitlo.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.yueranfly.top/gtohwqypqa.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.nwbrower.top/gtbhlorunw.html

[D26] 数组转字符串
来源：http://hz.pengpengdd.cyou/gtfjctqevy.html

Py:   ", ".join(map(str, arr))
来源：http://hz.ydzc1.top/gtovqscybx.html

PHP:  implode(", ", $arr);
来源：http://hz.fengsongda.top/gtolyvvoel.html

JS:   arr.join(", ")
来源：http://hz.dianchejie.cn/gtwqupyoiz.html

TS:   arr.join(", ")
来源：http://hz.iojbl.cn/gtvawvadiu.html

Java: String.join(", ", list)
来源：http://hz.zhaomingkeji.xyz/gtxljowhxl.html

Go:   strings.Join(strs, ", ")
来源：http://hz.iojbl.cn/gtonayqhsk.html

Ruby: arr.join(", ")
来源：http://hz.havefunace.top/gtroxuimcy.html

C#:   string.Join(", ", list)
来源：http://hz.nanxinkj.top/gttkrclhge.html

================================================================================
来源：http://hz.chenzaomai.com/gtqrusoaac.html

E. 字符串处理
来源：http://hz.jqgufenzy.top/gtwavfzsta.html

================================================================================
来源：http://hz.c1oappe.top/gtoxdqzvhj.html

[E01] 拼接字符串
来源：http://hz.jyoumei.cn/gtxbahmqpm.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.shanyushiyangkeji.top/gtrkzwdddj.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.quarkkingdee.top/gtdfvvwbza.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ybcxt.top/gtwnjizeem.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yvedp.cn/gtkjvdcgny.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.havefunace.top/gtqawbezbk.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.redwolf501.top/gtjkopotmg.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.cheryme.top/gtpiweledt.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.andypj.xyz/gtiyukbflu.html

[E02] 重复字符串
来源：http://hz.shangyingyoupin.top/gtspclmlfs.html

Py:   "ab" * 3
来源：http://hz.wangshuangyany.cn/gtmhzpgghu.html

PHP:  str_repeat("ab", 3);
来源：http://hz.ppjwa.cn/gthhjpkfiz.html

JS:   "ab".repeat(3)
来源：http://hz.yj202588.top/gtenphqrzg.html

TS:   "ab".repeat(3)
来源：http://hz.aibaodan.cn/gthjozwvst.html

Java: "ab".repeat(3)
来源：http://hz.tianlin.xyz/gtjhqtmkzp.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.svipenyu.cn/gtvtockbxf.html

Ruby: "ab" * 3
来源：http://hz.cucudq.cn/gtgtwfukpf.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.haohaochexian.top/gtvgwnwvyz.html

[E03] 截取子串
来源：http://hz.ywan-chungtsiang.top/gtqmdxasep.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.jyoumei.cn/gtphqjhsdh.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.jinghuilouyu.cn/gtkncyegxn.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.cheryme.top/gtdzkkeyuu.html

TS:   s.slice(1, 4)
来源：http://hz.guannengcc.top/gtljbygtce.html

Java: s.substring(1, 4)
来源：http://hz.zhongyouzk.top/gtuighzatq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.quarkkingdee.top/gtyxxfkbvc.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.yangfankeji.com/gtzqqhoimk.html

C#:   s.Substring(1, 3)
来源：http://hz.zhoulong.xyz/gtjpdhinwd.html

[E04] 查找子串位置
来源：http://hz.meibo888.top/gtcwqzrjjf.html

Py:   s.find("x");  s.index("x")
来源：http://hz.jyoumei.cn/gtcbnsqzqz.html

PHP:  strpos($s, "x");
来源：http://hz.xuetiantiany.cn/gtovhgbaok.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.hysaishi.cn/gtoqwtbqct.html

TS:   s.indexOf("x")
来源：http://hz.tanke756.top/gthpfflxvl.html

Java: s.indexOf("x")
来源：http://hz.hnxiangtu.top/gtevrphqkb.html


<!-- 参考信息 -->