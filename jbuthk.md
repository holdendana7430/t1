代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.daxiang520.top/gtfzbhnumg.html

[C15] 解构 / 展开参数
来源：http://hz.birdmap.top/gtdwfwhchi.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.smart0.xyz/gtmjqlbaxq.html

PHP:  [$a, $b] = $pair;
来源：http://hz.xuanzx.com/gtnftgxyyn.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.svipenyu.cn/gtxkciencx.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.jinqigufen.top/gtkrsjnzut.html

Java: // 无解构
来源：http://hz.xinyue.icu/gtxjlapqxd.html

Go:   // 无解构
来源：http://hz.fzhhl.top/gtqeaiqopl.html

Ruby: a, b = pair
来源：http://hz.fzhhl.top/gtsssmgxej.html

C#:   var (a, b) = pair;
来源：http://hz.fzhhl.top/gtoqwoiojl.html

[C16] 函数 / 方法重载
来源：http://hz.cheryme.top/gtzxaidwan.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.0kj1m.cn/gtfjfyhosg.html

PHP:  // 无重载
来源：http://hz.ydjk.org.cn/gtnzgbiqiw.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.jinqigfzy.top/gtdwoydxdh.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.zycfv.cn/gtpwxpuhqb.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.birdmap.top/gtekxbdyzt.html

Go:   // 无重载：用不同函数名
来源：http://hz.andypj.xyz/gtokscupbc.html

Ruby: # 无重载：靠动态参数
来源：http://hz.zhijiandao.cn/gtaunzkyfv.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.tanke756.top/gtyscsqzij.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtcpnrsktv.html

D. 数组 / 列表 / 集合
来源：http://hz.yonumen.top/gtjeynuczx.html

================================================================================
来源：http://hz.zhengqikj.top/gtckuakplx.html

[D01] 创建数组 / 列表
来源：http://hz.hnxiangtu.top/gtwbfzyfyf.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.cdnleiting.top/gtsyhwegto.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.jiagoushi.top/gtpyfgwbpu.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.cucudq.cn/gtsmuxzekn.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.nanxuanxn.top/gtddhyooai.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.dashuyun.cn/gtgvmsubav.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.meibo888.top/gtyoitssnn.html

Ruby: arr = [1, 2, 3]
来源：http://hz.guowangkeji.top/gtuyuncycy.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.yongpay.top/gtazahiwzb.html

[D02] 追加元素到末尾
来源：http://hz.zhixingplan.top/gthjpottjs.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.yongpay.top/gtobwamnjc.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.xylfe.cn/gtesdlbume.html

JS:   arr.push(4);
来源：http://hz.kuanghao11.cn/gtehidbscr.html

TS:   arr.push(4);
来源：http://hz.xinyue.icu/gtzfmkjoqm.html

Java: list.add(4);
来源：http://hz.bjfxy.top/gtvfondcbw.html

Go:   arr = append(arr, 4)
来源：http://hz.xuetiantiany.cn/gtxvlvzpur.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.shuidangran.top/gtlbusnvif.html

C#:   list.Add(4);
来源：http://hz.dianchejie.cn/gtjikhkxwn.html

[D03] 在指定位置插入元素
来源：http://hz.ppjwa.cn/gtieblhjoj.html

Py:   arr.insert(0, 0)
来源：http://hz.hnqzz.top/gtumtswkwy.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.jlsjyb.cn/gtsugdbsef.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.havefunace.top/gtfdrvkvdk.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.fengsongda.top/gtfjuucmwj.html

Java: list.add(0, 0);
来源：http://hz.zhiwuduotai.top/gtzzdmiele.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.gotoacloud.top/gtjlauayko.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.ppjwa.cn/gtkjenfbkp.html

C#:   list.Insert(0, 0);
来源：http://hz.quarkkingdee.top/gtsapbkjeo.html

[D04] 删除元素
来源：http://hz.cashguo.top/gtrktgzhoz.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.zhixingplan.top/gtuqphnynb.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.feifeiyinyue.top/gtjzbqqytl.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.zhoulong.xyz/gtmjdbbwtz.html

TS:   arr.splice(0, 1);
来源：http://hz.sxryk.cn/gthypsftcw.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.pengpengdd.cyou/gtyzxqfcmm.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.0kj1m.cn/gtpuvzvkxr.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.yuxming.cn/gtwxtxpvxt.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.c1oappe.top/gtursxgsdh.html

[D05] 访问与修改元素
来源：http://hz.jlsjyb.cn/gttkbrokbf.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hysaishi.cn/gtpbhdrkpg.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.hywenlv.cn/gtbmopuito.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.ppjwa.cn/gtdowcbkns.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.zhengqikj.top/gtpwmydkyi.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.nwbrower.top/gtocizzwzq.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.zhengqikj.top/gtjuderqfl.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jqgfzy.top/gthfjpgvxg.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.havefunace.top/gtvoolfsht.html

[D06] 数组长度
来源：http://hz.tian-w.cn/gttllmylkj.html

Py:   len(arr)
来源：http://hz.zhengqikj.top/gtnlvryzgi.html

PHP:  count($arr);
来源：http://hz.hnxiangtu.top/gteezgflus.html

JS:   arr.length
来源：http://hz.yongpay.top/gtanlvjvrt.html

TS:   arr.length
来源：http://hz.tian-w.cn/gtcyxdzhmo.html

Java: list.size();
来源：http://hz.jinqigufen.top/gtqcaliqre.html

Go:   len(arr)
来源：http://hz.hammf.cn/gtzpoprqhf.html

Ruby: arr.length; arr.size
来源：http://hz.jinqigufen.top/gtmhshhlxv.html

C#:   list.Count;
来源：http://hz.jinyuanbaomall.cn/gtozgkvhpa.html

[D07] 切片 / 取子数组
来源：http://hz.gaohongyu789.top/gtyicewkoe.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.daxiang520.top/gthgwkesti.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.zhengqikj.top/gtablowqiq.html

JS:   arr.slice(1, 4);
来源：http://hz.jlsjyb.cn/gtkspxcrmy.html

TS:   arr.slice(1, 4);
来源：http://hz.jinghuilouyu.cn/gtmdhkvgvw.html

Java: list.subList(1, 4);
来源：http://hz.yanxiufei.cn/gtanshmhvb.html

Go:   arr[1:4]
来源：http://hz.shzxlz.cn/gtkceyilcq.html

Ruby: arr[1, 3]
来源：http://hz.jqgfzy.top/gtcgoeagjb.html

C#:   list.GetRange(1, 3);
来源：http://hz.snrcjt.cn/gtefyklfcc.html

[D08] 合并两个数组
来源：http://hz.zdqjudy.top/gtidmgcfpm.html

Py:   a + b;  a.extend(b)
来源：http://hz.jinqigfzy.top/gtanwiqrpm.html

PHP:  array_merge($a, $b);
来源：http://hz.wangshuangyany.cn/gtygqnpijr.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.ydjk.org.cn/gtsmyrvruu.html

TS:   [...a, ...b];
来源：http://hz.daxiang520.top/gtjthafnsz.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.jqgufenzy.top/gtbjhmzwxf.html

Go:   append(a, b...)
来源：http://hz.dashuyun.cn/gtdtizmrsi.html

Ruby: a + b;  a.concat(b)
来源：http://hz.hongshengwenyu.top/gtlmiwurdl.html

C#:   a.Concat(b).ToList()
来源：http://hz.snrcjt.cn/gtnaahppid.html

[D09] 排序（升序）
来源：http://hz.xylfe.cn/gtdiqdfqys.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.vqdsnc.cn/gtpdafsaoz.html

PHP:  sort($arr);
来源：http://hz.ppjwa.cn/gtccqsjgoq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.sysykeji.top/gtkwfwzpxy.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.zhixingplan.top/gtvxggscbn.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.xuanzx.com/gtjmbnlpnt.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.yueranfly.top/gtwxcfcwnd.html

Ruby: arr.sort
来源：http://hz.gogol.net.cn/gtxmigktve.html

C#:   list.Sort();
来源：http://hz.smart0.xyz/gtxpyqthty.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.ydzc1.top/gtjfoybnag.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.cashguo.top/gtfeufgrbb.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jianghu66.top/gtskunagew.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.snrcjt.cn/gtvjsycsmk.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.0kj1m.cn/gtyrbtctxo.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.yj20258.top/gtpfyrmdna.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.kuanghao11.cn/gtpymdqscm.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.cashguo.top/gtdlkzgapa.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.pycfn.com/gtmsitedhx.html

[D11] 反转数组
来源：http://hz.pengpengdd.cyou/gtggmdkjbn.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.zhiwuduotai.top/gtxkjlnevq.html

PHP:  array_reverse($arr);
来源：http://hz.jinyuanbaomall.cn/gtidflwqxi.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.hysaishi.cn/gtnqpkefhb.html

TS:   [...arr].reverse();
来源：http://hz.wangshuangyany.cn/gtnnzvljus.html

Java: Collections.reverse(list);
来源：http://hz.xinyue.icu/gtilvwajic.html

Go:   slices.Reverse(arr)
来源：http://hz.cucudq.cn/gtvvsiplpv.html

Ruby: arr.reverse
来源：http://hz.zdqjudy.top/gtwpbpzskh.html

C#:   list.Reverse();
来源：http://hz.xuetiantiany.cn/gtvsfxoupa.html

[D12] 查找元素下标
来源：http://hz.sufxvd.cn/gtgimeuwjb.html

Py:   arr.index(x);  x in arr
来源：http://hz.xinyue.icu/gtjhzeaamf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.daxiang520.top/gthnfqczfd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.ppjwa.cn/gtjfseicpb.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.xylfe.cn/gtrxiavvjp.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.haohaochexian.top/gtkhislwaz.html

Go:   slices.Index(arr, x)
来源：http://hz.cqqwz.cn/gtukuejvrt.html

Ruby: arr.index(x)
来源：http://hz.jlsjyb.cn/gthczucchz.html

C#:   list.IndexOf(x);
来源：http://hz.9152youxi.cn/gtgxhkxcpz.html

[D13] 过滤（保留满足条件的）
来源：http://hz.jlsjyb.cn/gthmwbcuep.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.jinqigufen.top/gttiupnofw.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.zhaomingkeji.xyz/gtzmuuckbf.html

JS:   arr.filter(x => x > 3)
来源：http://hz.xziqi.cn/gtvggeuwyq.html

TS:   arr.filter(x => x > 3)
来源：http://hz.yangfankeji.com/gtbcpukogt.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.jinghuilouyu.cn/gtisyeyijm.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.xuetiantiany.cn/gtytcvksjb.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.xuanzx.com/gtqepkhzde.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.zhengqikj.top/gtmgsyfklt.html

[D14] 映射转换（每个元素变形）
来源：http://hz.shangyingyoupin.top/gtzzubjubj.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.hammf.cn/gtqbfoyvgs.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.jinyuanbaomall.cn/gthdlgwavt.html

JS:   arr.map(x => x * 2)
来源：http://hz.kuanghao11.cn/gtxshcyhrx.html

TS:   arr.map(x => x * 2)
来源：http://hz.yueranfly.top/gtjqfjglrj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.nwbrower.top/gtfabewurk.html

Go:   // 手写循环
来源：http://hz.chenlongwang.top/gtfyygdcfz.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.wangshuangyany.cn/gtrjqojyiy.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.feifeiyinyue.top/gtmsfuhwrp.html

[D15] 去重
来源：http://hz.xuanzx.com/gtjwnzbbsi.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.shanyushiyangtech.top/gtusuflktb.html

PHP:  array_unique($arr);
来源：http://hz.shanyushiyangtech.top/gtuvkbsnyh.html

JS:   [...new Set(arr)]
来源：http://hz.jqgfzy.top/gtoslercax.html

TS:   [...new Set(arr)]
来源：http://hz.zhiwuduotai.top/gtwzdgcwpj.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.tianlin.xyz/gtoslyxhao.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.feifeiyinyue.top/gtpqnupnks.html

Ruby: arr.uniq
来源：http://hz.zhixingplan.top/gtkazhqkdq.html

C#:   list.Distinct().ToList()
来源：http://hz.shangyingyoupin.top/gtkhzulhaz.html

[D16] 求和与平均值
来源：http://hz.hywenlv.cn/gttzeetwhj.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.daxiang520.top/gtmoemyeiw.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.yueranfly.top/gtheckevjw.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jinghuilouyu.cn/gtnqsmvmbb.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yonumen.top/gtfbtossch.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.sxryk.cn/gtywnhxrzk.html

Go:   // 手写循环累加
来源：http://hz.hysaishi.cn/gtfqmuskll.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.zhengqikj.top/gtzfaxzntx.html

C#:   list.Sum();  list.Average()
来源：http://hz.cashguo.top/gtctylqkou.html

[D17] 最大值与最小值
来源：http://hz.hfpthk.cn/gtgvaizhrz.html

Py:   max(arr);  min(arr)
来源：http://hz.dianchejie.cn/gtmwmwhsre.html

PHP:  max($arr);  min($arr);
来源：http://hz.havefunace.top/gtwovladhe.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.cashguo.top/gtzdapgeka.html

TS:   Math.max(...arr);
来源：http://hz.yj20258888.top/gtmfpbeppi.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.snrcjt.cn/gtcbzvbyec.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.hfpthk.cn/gtliorrqzq.html

Ruby: arr.max;  arr.min
来源：http://hz.zdqjudy.top/gtwigueabj.html

C#:   list.Max();  list.Min()
来源：http://hz.gogol.net.cn/gtwsrbqudg.html

[D18] 扁平化嵌套数组
来源：http://hz.hnqzz.top/gttjktkxhl.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.tanke756.top/gtzfsegjrv.html

PHP:  array_merge(...$nested);
来源：http://hz.cqqwz.cn/gttogupyqg.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.yj20258.top/gtthehqlxj.html

TS:   nested.flat();
来源：http://hz.xuanzx.com/gtkumbhtjq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.svipenyu.cn/gtyirdnvbu.html

Go:   // 手写双层循环
来源：http://hz.svipenyu.cn/gteueoqxbz.html

Ruby: nested.flatten
来源：http://hz.yj20258888.top/gtnuyopovu.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.sweek.top/gtayprxogh.html

[D19] 按字段分组
来源：http://hz.hongshengwenyu.top/gtmyhjcqlm.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.jiagoushi.top/gtyeiqeycq.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.guowangkeji.top/gtmmyzxgcy.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.quarkkingdee.top/gtxhulyoxe.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.zhongyouzk.top/gtubhdrgeu.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.quarkkingdee.top/gtoifnbthp.html

Go:   // 手写 map[string][]T
来源：http://hz.gaohongyu789.top/gtickuddmf.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.ywan-chungtsiang.top/gtqkzvfqas.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.tianlin.xyz/gtisobjwly.html

[D20] 统计每个元素出现次数
来源：http://hz.zhijiandao.cn/gtfdfmbtpy.html

Py:   Counter(arr)
来源：http://hz.redwolf501.top/gtingfuyvh.html

PHP:  array_count_values($arr);
来源：http://hz.dianchejie.cn/gtxnlussmn.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.kuanghao11.cn/gtzxwnuuum.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zhengqikj.top/gtsbxjfmfy.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.daxiang520.top/gttimtofvg.html

Go:   // 手写 map[T]int
来源：http://hz.nanxuanxn.top/gtdofsncvx.html

Ruby: arr.tally
来源：http://hz.yuxming.cn/gtgtdhxwkr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.cashguo.top/gtmocrqnnr.html

[D21] 判断是否包含某元素
来源：http://hz.tianlin.xyz/gtiemehyys.html

Py:   x in arr
来源：http://hz.jinyuanbaomall.cn/gtwuadolde.html

PHP:  in_array($x, $arr, true);
来源：http://hz.hfpthk.cn/gtlrvicsew.html

JS:   arr.includes(x)
来源：http://hz.zycfv.cn/gtuyuyvlkh.html

TS:   arr.includes(x)
来源：http://hz.xingfuxueyuan.xyz/gtmswpgtli.html

Java: list.contains(x)
来源：http://hz.yvedp.cn/gtoptbszul.html

Go:   slices.Contains(arr, x)
来源：http://hz.tian-w.cn/gtdpqihygh.html

Ruby: arr.include?(x)
来源：http://hz.fengsongda.top/gtlxfenzes.html

C#:   list.Contains(x)
来源：http://hz.redwolf501.top/gttlldchqd.html

[D22] 复制数组（避免共享引用）
来源：http://hz.9152youxi.cn/gtscqrrepk.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.cheryme.top/gtttapcacc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.shanyushiyangkeji.top/gtkghwkkab.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.tanke756.top/gtzdcginoi.html

TS:   [...arr];
来源：http://hz.yvedp.cn/gtjaxuildj.html

Java: new ArrayList<>(list);
来源：http://hz.kuanghao11.cn/gtoeghsobx.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.jyoumei.cn/gtkccrmdip.html

Ruby: arr.dup;  arr.clone
来源：http://hz.vqdsnc.cn/gtcvmdaxuc.html

C#:   new List<int>(list);
来源：http://hz.jianghu66.top/gtripdmyde.html

[D23] reduce 累积计算
来源：http://hz.quarkkingdee.top/gtayowwwci.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.vqdsnc.cn/gteavxbirt.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.shuidangran.top/gtsjshfrov.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.gotoacloud.top/gtcemtyviz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.tian-w.cn/gtikubsbag.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.tanke756.top/gtzfnpncej.html

Go:   // 手写循环
来源：http://hz.jinghuilouyu.cn/gtwnvkfnvn.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.xingfuxueyuan.xyz/gtowjptlkh.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.quarkkingdee.top/gtcjgrlqoi.html

[D24] 字典 / Map 基本操作
来源：http://hz.vqdsnc.cn/gtgsgsywqg.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.chenjidiqi.icu/gtuieykeou.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.9152youxi.cn/gtryumpdwn.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.feifeiyinyue.top/gtrbmyapxs.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.quarkkingdee.top/gtfaqabiay.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.chenzaomai.com/gtbyyeovgm.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.hnxiangtu.top/gtxzqlqlfk.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.svipenyu.cn/gtfyzwlmzy.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.zycfv.cn/gtwkkwvvhp.html

[D25] Set 集合去重与交并差
来源：http://hz.yongpay.top/gtsuwhfynj.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.andypj.xyz/gtytxaxhqj.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.jinqigfzy.top/gtsywishgm.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.jianghu66.top/gtmipcbrdv.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.mhx1999.top/gtgixutpop.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.andypj.xyz/gtvakwltqf.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.zycfv.cn/gtvdtaqvlh.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.daxiang520.top/gtmyacawkd.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.zhengqikj.top/gtcrcbzybh.html

[D26] 数组转字符串
来源：http://hz.chenjidiqi.icu/gtpsvemtoo.html

Py:   ", ".join(map(str, arr))
来源：http://hz.cdnleiting.top/gtzwepcyyn.html

PHP:  implode(", ", $arr);
来源：http://hz.cheryme.top/gtnkbpxeer.html

JS:   arr.join(", ")
来源：http://hz.pengpengdd.cyou/gtgfvdgzsq.html

TS:   arr.join(", ")
来源：http://hz.zhijiandao.cn/gtqcpwnzzi.html

Java: String.join(", ", list)
来源：http://hz.yangfankeji.com/gtwmsirzoi.html

Go:   strings.Join(strs, ", ")
来源：http://hz.vqdsnc.cn/gtrjxtswml.html

Ruby: arr.join(", ")
来源：http://hz.shanyushiyangkeji.top/gtpbbhjiki.html

C#:   string.Join(", ", list)
来源：http://hz.wangshuangyany.cn/gtuztkmhiq.html

================================================================================
来源：http://hz.gaohongyu789.top/gtlavyspgl.html

E. 字符串处理
来源：http://hz.hnxiangtu.top/gthorvlqpb.html

================================================================================
来源：http://hz.yueranfly.top/gttpeerjtk.html

[E01] 拼接字符串
来源：http://hz.shuidangran.top/gtbpozwmpn.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.aibaodan.cn/gtqwvtwbgh.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.fengsongda.top/gttbyiioba.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.hongshengwenyu.top/gtyehrccuv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.xuanzx.com/gtvdxhshzg.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.redwolf501.top/gtphvhuhto.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.birdmap.top/gtthxmxygd.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.ywan-chungtsiang.top/gtovatzhfc.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.yj202588.top/gtrfxjtzja.html

[E02] 重复字符串
来源：http://hz.52xcode.cn/gtscocbbea.html

Py:   "ab" * 3
来源：http://hz.gotoacloud.top/gtmkidntys.html

PHP:  str_repeat("ab", 3);
来源：http://hz.ydjk.org.cn/gtwvlkguvf.html

JS:   "ab".repeat(3)
来源：http://hz.sysykeji.top/gtkdctvqfy.html

TS:   "ab".repeat(3)
来源：http://hz.jyoumei.cn/gtgkhqebpj.html

Java: "ab".repeat(3)
来源：http://hz.tian-w.cn/gtkeemcytl.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.pycfn.com/gtdxiucynb.html

Ruby: "ab" * 3
来源：http://hz.0kj1m.cn/gtdngpufwc.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.nanxuanxn.top/gtdeellnop.html

[E03] 截取子串
来源：http://hz.jinghuilouyu.cn/gtvnkjlnzb.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.pengpengdd.cyou/gtirkpawww.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.cheryme.top/gtjxjxsekn.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.kuanghao11.cn/gtmcmkfyrh.html

TS:   s.slice(1, 4)
来源：http://hz.yonumen.top/gtwctsvkmc.html

Java: s.substring(1, 4)
来源：http://hz.zhiwuduotai.top/gtgtcxuzdh.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.nwbrower.top/gtqwcfihdc.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.andypj.xyz/gtssjsihsx.html

C#:   s.Substring(1, 3)
来源：http://hz.iojbl.cn/gthuioeher.html

[E04] 查找子串位置
来源：http://hz.52xcode.cn/gthbxxpzfs.html

Py:   s.find("x");  s.index("x")
来源：http://hz.bjfxy.top/gthjakdybk.html

PHP:  strpos($s, "x");
来源：http://hz.shuidangran.top/gtzovjuvhg.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.cucudq.cn/gtqrmtjunb.html

TS:   s.indexOf("x")
来源：http://hz.gzhubu.top/gtcztyrygq.html

Java: s.indexOf("x")
来源：http://hz.quarkkingdee.top/gtlsjtagvz.html

Go:   strings.Index(s, "x")
来源：http://hz.guannengcc.top/gtapztcaft.html

Ruby: s.index("x")
来源：http://hz.cqqwz.cn/gtzjsjwdmm.html

C#:   s.IndexOf("x")
来源：http://hz.tian-w.cn/gttggnfgvz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.cheryme.top/gtvsrketdh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.yanxiufei.cn/gtvsnwgbyg.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.pengpengdd.cyou/gtoalkoyvn.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.shanyushiyangkeji.top/gtrkywgdus.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.hnxiangtu.top/gtywmoyjxv.html


<!-- 参考信息 -->