代发 wailian999

[C14] 泛型函数
来源：http://hz.snrcjt.cn/gttifayyso.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.fengsongda.top/gtevbecjez.html

PHP:  // 无泛型
来源：http://hz.shanyushiyangtech.top/gtgmioidft.html

JS:   // 无泛型
来源：http://hz.vqdsnc.cn/gtnxstpwlf.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.nanxuanxn.top/gtaogbzybb.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.quarkkingdee.top/gtokxacwru.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.ehwqpu.com/gtwdpqaqft.html

Ruby: # 无泛型
来源：http://hz.dashuyun.cn/gtmsnfpgod.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.xuanzx.com/gtlqzqguez.html

[C15] 解构 / 展开参数
来源：http://hz.cheryme.top/gtmezoxmsl.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.zhengqikj.top/gtubsofzzo.html

PHP:  [$a, $b] = $pair;
来源：http://hz.ehwqpu.com/gtjwftvuqo.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.haohaochexian.top/gtnuthyect.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.chenlongwang.top/gtedlznarp.html

Java: // 无解构
来源：http://hz.ydjk.org.cn/gtweqcjtnh.html

Go:   // 无解构
来源：http://hz.hnqzz.top/gtuaqnnkmm.html

Ruby: a, b = pair
来源：http://hz.fzhhl.top/gtelspkpht.html

C#:   var (a, b) = pair;
来源：http://hz.yueranfly.top/gthecmfcng.html

[C16] 函数 / 方法重载
来源：http://hz.tian-w.cn/gtonapbiom.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.guowangkeji.top/gtynymsmzz.html

PHP:  // 无重载
来源：http://hz.guannengcc.top/gtgjqgjvjl.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.guowangkeji.top/gtgcvprtzc.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.ywan-chungtsiang.top/gtjbyqlhfo.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.shanyushiyangtech.top/gtognagfkm.html

Go:   // 无重载：用不同函数名
来源：http://hz.jinyuanbaomall.cn/gtkecliceh.html

Ruby: # 无重载：靠动态参数
来源：http://hz.ivvv.top/gtfwkgczlc.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.chenzaomai.com/gtpvxxsind.html

================================================================================
来源：http://hz.kuanghao11.cn/gtisiksjgf.html

D. 数组 / 列表 / 集合
来源：http://hz.ivvv.top/gtpjnihnar.html

================================================================================
来源：http://hz.bjfxy.top/gtqxbmmcxq.html

[D01] 创建数组 / 列表
来源：http://hz.zhijiandao.cn/gtdngfzeen.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.ywan-chungtsiang.top/gtokbnkxfn.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.quarkkingdee.top/gtosmjlftq.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.sysykeji.top/gtuegjcyio.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.yanxiufei.cn/gtgeixnegr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.redwolf501.top/gtpkxxyoym.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.c1oappe.top/gtuvuabfqi.html

Ruby: arr = [1, 2, 3]
来源：http://hz.gaohongyu789.top/gteeyelvtk.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.hysaishi.cn/gthtipaqql.html

[D02] 追加元素到末尾
来源：http://hz.jiagoushi.top/gtjpbqgori.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.svipenyu.cn/gtrbadqtwz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.jinqigufen.top/gtetavgyuk.html

JS:   arr.push(4);
来源：http://hz.hfpthk.cn/gteqdaqfdq.html

TS:   arr.push(4);
来源：http://hz.redwolf501.top/gtnciboauy.html

Java: list.add(4);
来源：http://hz.hysaishi.cn/gtrcbzxnaf.html

Go:   arr = append(arr, 4)
来源：http://hz.jinqigufen.top/gtdflllnud.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.pycfn.com/gtmqohxyfv.html

C#:   list.Add(4);
来源：http://hz.daxiang520.top/gtauwngsfk.html

[D03] 在指定位置插入元素
来源：http://hz.svipenyu.cn/gtkllxzsnv.html

Py:   arr.insert(0, 0)
来源：http://hz.yonumen.top/gtpbqhvmni.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.kuanghao11.cn/gthxaxusjf.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.zhiwuduotai.top/gtkgerilic.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.tianlin.xyz/gtbtjmmopo.html

Java: list.add(0, 0);
来源：http://hz.fzhhl.top/gtcxiedxrz.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.yangfankeji.com/gtivkmlbms.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.tianlin.xyz/gtxwdizidw.html

C#:   list.Insert(0, 0);
来源：http://hz.nanxinkj.top/gtymmwuyas.html

[D04] 删除元素
来源：http://hz.xuetiantiany.cn/gtulzzsdio.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.shzxlz.cn/gtsqndyosk.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.yj20258888.top/gttsudfqlo.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.tian-w.cn/gtddhlygfu.html

TS:   arr.splice(0, 1);
来源：http://hz.ybcxt.top/gtyrtznxdn.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.chenjidiqi.icu/gtvekiesuv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.zycfv.cn/gtqtggjuwf.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.guannengcc.top/gtrjwcrkae.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.zhiwuduotai.top/gtevtiqckf.html

[D05] 访问与修改元素
来源：http://hz.hfpthk.cn/gtuaagkkqg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.ppjwa.cn/gtyjoylgko.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.birdmap.top/gtwrjehuty.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.feifeiyinyue.top/gtfjavgjri.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.hammf.cn/gtdijbtihg.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.cucudq.cn/gtmnhurnlv.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.316326.xyz/gtncwmszcn.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yj20258.top/gtsovfinkj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.yueranfly.top/gtwznocrsd.html

[D06] 数组长度
来源：http://hz.gotoacloud.top/gtxpxokchq.html

Py:   len(arr)
来源：http://hz.shanyushiyangkeji.top/gtbkviwptj.html

PHP:  count($arr);
来源：http://hz.0kj1m.cn/gtymnplzbp.html

JS:   arr.length
来源：http://hz.sufxvd.cn/gtplebowna.html

TS:   arr.length
来源：http://hz.ehwqpu.com/gtlbnurgfq.html

Java: list.size();
来源：http://hz.gotoacloud.top/gtfcfdgqwo.html

Go:   len(arr)
来源：http://hz.smart0.xyz/gtfapgfyya.html

Ruby: arr.length; arr.size
来源：http://hz.jinyuanbaomall.cn/gtgskcydjk.html

C#:   list.Count;
来源：http://hz.nanxuanxn.top/gttnhppryi.html

[D07] 切片 / 取子数组
来源：http://hz.52xcode.cn/gtqgiqaoty.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.jyoumei.cn/gtzxalwzoa.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.feifeiyinyue.top/gtsfsbrakj.html

JS:   arr.slice(1, 4);
来源：http://hz.cdnleiting.top/gtrqophqzj.html

TS:   arr.slice(1, 4);
来源：http://hz.zhixingplan.top/gtgwdqtrii.html

Java: list.subList(1, 4);
来源：http://hz.feifeiyinyue.top/gtswlyfylt.html

Go:   arr[1:4]
来源：http://hz.daria6918.cn/gtqvfvjozp.html

Ruby: arr[1, 3]
来源：http://hz.yuanzhike.top/gtqlfvpqfl.html

C#:   list.GetRange(1, 3);
来源：http://hz.cheryme.top/gtsktykhvc.html

[D08] 合并两个数组
来源：http://hz.nwbrower.top/gtbefhohri.html

Py:   a + b;  a.extend(b)
来源：http://hz.yanxiufei.cn/gtgzkhlnsf.html

PHP:  array_merge($a, $b);
来源：http://hz.jqgufenzy.top/gttoxxvyww.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.sysykeji.top/gtegfstdnr.html

TS:   [...a, ...b];
来源：http://hz.52xcode.cn/gtrvztpmtf.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.gogol.net.cn/gtzixmlpkh.html

Go:   append(a, b...)
来源：http://hz.52xcode.cn/gtzpwbixdk.html

Ruby: a + b;  a.concat(b)
来源：http://hz.svipenyu.cn/gtvyadkibh.html

C#:   a.Concat(b).ToList()
来源：http://hz.hnxiangtu.top/gtodstomfb.html

[D09] 排序（升序）
来源：http://hz.shanyushiyangtech.top/gtdfbzgspi.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.guowangkeji.top/gtvgjobbwq.html

PHP:  sort($arr);
来源：http://hz.ywan-chungtsiang.top/gtpyejfcyv.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.snrcjt.cn/gtffsvbryy.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.ivvv.top/gtmjbcgnmj.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.c1oappe.top/gtikgcuevu.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.hnxiangtu.top/gtujlylwpx.html

Ruby: arr.sort
来源：http://hz.cqqwz.cn/gtaageshth.html

C#:   list.Sort();
来源：http://hz.tianlin.xyz/gttuxbgmpn.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.52xcode.cn/gtxvhhsgac.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.sysykeji.top/gtrnktvcyg.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.smart0.xyz/gtbtucxtem.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.gaohongyu789.top/gtrerqofsc.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.gzhubu.top/gtnadihsyx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.havefunace.top/gtgatogbnz.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.yvedp.cn/gteyyafxlj.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.jinghuilouyu.cn/gtzpqgewos.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.yanxiufei.cn/gtkmfxrrsc.html

[D11] 反转数组
来源：http://hz.jinyuanbaomall.cn/gthooxqecf.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.zhiwuduotai.top/gtrakiilco.html

PHP:  array_reverse($arr);
来源：http://hz.dashuyun.cn/gtbsikhovu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.cashguo.top/gtdulzoqiq.html

TS:   [...arr].reverse();
来源：http://hz.52xcode.cn/gtjgnrjgly.html

Java: Collections.reverse(list);
来源：http://hz.guowangkeji.top/gtmcuzogba.html

Go:   slices.Reverse(arr)
来源：http://hz.haohaochexian.top/gttsrnhoqv.html

Ruby: arr.reverse
来源：http://hz.zhongyouzk.top/gtqmqbkpqj.html

C#:   list.Reverse();
来源：http://hz.jiagoushi.top/gtsgmyganp.html

[D12] 查找元素下标
来源：http://hz.hnxiangtu.top/gtojoigfvb.html

Py:   arr.index(x);  x in arr
来源：http://hz.wangdashe.top/gtobcqowso.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.sxryk.cn/gtzvmgkthg.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.hammf.cn/gtxmytuwrm.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.guowangkeji.top/gtchmfhida.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.snrcjt.cn/gtavbueqsu.html

Go:   slices.Index(arr, x)
来源：http://hz.nanxuanxn.top/gtpfhdsdow.html

Ruby: arr.index(x)
来源：http://hz.jiagoushi.top/gtgtfnnvvv.html

C#:   list.IndexOf(x);
来源：http://hz.smart0.xyz/gthzkvkhoj.html

[D13] 过滤（保留满足条件的）
来源：http://hz.cheryme.top/gtjkowdkmg.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.chenjidiqi.icu/gtewaklsva.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.birdmap.top/gtktnbfexe.html

JS:   arr.filter(x => x > 3)
来源：http://hz.fzhhl.top/gtwvbwvupm.html

TS:   arr.filter(x => x > 3)
来源：http://hz.hongshengwenyu.top/gtdcuifpfl.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.zhoulong.xyz/gtfmocklpd.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.quarkkingdee.top/gtfqshcrfx.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.chenlongwang.top/gtcvjbsgnd.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.chenzaomai.com/gtyktkuxaa.html

[D14] 映射转换（每个元素变形）
来源：http://hz.zhixingplan.top/gtegmubrbo.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.wangshuangyany.cn/gtbwlsgabi.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.yuxming.cn/gttyrwiioz.html

JS:   arr.map(x => x * 2)
来源：http://hz.zhixingplan.top/gtqljmfpub.html

TS:   arr.map(x => x * 2)
来源：http://hz.tanke756.top/gtnraodhtk.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.zhaomingkeji.xyz/gttzpqpndl.html

Go:   // 手写循环
来源：http://hz.52xcode.cn/gtrsgjwtfo.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.jianghu66.top/gtzcyzfysu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.tanke756.top/gtsctdkcbh.html

[D15] 去重
来源：http://hz.svipenyu.cn/gtdidszlyk.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.aizwys.cn/gtwzfoympb.html

PHP:  array_unique($arr);
来源：http://hz.hnqzz.top/gtchtweewh.html

JS:   [...new Set(arr)]
来源：http://hz.jlsjyb.cn/gtehpmeqdn.html

TS:   [...new Set(arr)]
来源：http://hz.feifeiyinyue.top/gtqpiimpmx.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.iojbl.cn/gtwxyqdudw.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.zhixingplan.top/gtcyghrztu.html

Ruby: arr.uniq
来源：http://hz.dashuyun.cn/gtdlkkueub.html

C#:   list.Distinct().ToList()
来源：http://hz.yangfankeji.com/gtsrcsmuez.html

[D16] 求和与平均值
来源：http://hz.aizwys.cn/gtmqdvsckt.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.xinyue.icu/gtwyyitpcc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.316326.xyz/gtmetyxskj.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.birdmap.top/gtcioycagr.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.fzhhl.top/gtvhzufuhr.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.gogol.net.cn/gtkiqtklfn.html

Go:   // 手写循环累加
来源：http://hz.hongshengwenyu.top/gtjoprofde.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.xylfe.cn/gtynrxgayt.html

C#:   list.Sum();  list.Average()
来源：http://hz.xylfe.cn/gtglejsqef.html

[D17] 最大值与最小值
来源：http://hz.yanxiufei.cn/gtshjilfls.html

Py:   max(arr);  min(arr)
来源：http://hz.shanyushiyangtech.top/gtuxldvntt.html

PHP:  max($arr);  min($arr);
来源：http://hz.yj20258888.top/gtbeohzesx.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.guowangkeji.top/gtbazyyhbp.html

TS:   Math.max(...arr);
来源：http://hz.hfpthk.cn/gtiitntgnv.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.fengsongda.top/gtxfizbqom.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.ivvv.top/gtaplgyruq.html

Ruby: arr.max;  arr.min
来源：http://hz.mhx1999.top/gtrtfbjrwa.html

C#:   list.Max();  list.Min()
来源：http://hz.sxryk.cn/gtglpniiei.html

[D18] 扁平化嵌套数组
来源：http://hz.guowangkeji.top/gtbgbltdib.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.smart0.xyz/gtaotmklht.html

PHP:  array_merge(...$nested);
来源：http://hz.shanyushiyangtech.top/gtayzgmypa.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.haohaochexian.top/gtociwfnxh.html

TS:   nested.flat();
来源：http://hz.sxryk.cn/gtnazegkjy.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.hfpthk.cn/gtcnggxnaj.html

Go:   // 手写双层循环
来源：http://hz.hywenlv.cn/gtaievdseu.html

Ruby: nested.flatten
来源：http://hz.hammf.cn/gtlxlfjgti.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.yangfankeji.com/gttnmobloa.html

[D19] 按字段分组
来源：http://hz.meibo888.top/gtjejsmshm.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.guowangkeji.top/gtpdibpipy.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.zhixingplan.top/gtnnlzxayr.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.chenlongwang.top/gtgxkfzaml.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.cashguo.top/gthidqsdvl.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.zhengqikj.top/gtmhiqmujk.html

Go:   // 手写 map[string][]T
来源：http://hz.sweek.top/gtamhfkrrz.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.andypj.xyz/gtdmrjvlno.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.zhaomingkeji.xyz/gtdwxtjdzt.html

[D20] 统计每个元素出现次数
来源：http://hz.daria6918.cn/gtkxnafqne.html

Py:   Counter(arr)
来源：http://hz.tian-w.cn/gtyjxayuqc.html

PHP:  array_count_values($arr);
来源：http://hz.jinghuilouyu.cn/gtrahyepsg.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.ehwqpu.com/gtwxzfubhe.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.gogol.net.cn/gtvuaifkcd.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.svipenyu.cn/gtyvplojuo.html

Go:   // 手写 map[T]int
来源：http://hz.wangshuangyany.cn/gtjclmwgyw.html

Ruby: arr.tally
来源：http://hz.ybcxt.top/gtmytohcdn.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.chenjidiqi.icu/gtseoetqrb.html

[D21] 判断是否包含某元素
来源：http://hz.chenlongwang.top/gtljhwcswz.html

Py:   x in arr
来源：http://hz.wangshuangyany.cn/gtnegwqmze.html

PHP:  in_array($x, $arr, true);
来源：http://hz.xylfe.cn/gtxtpjzkzf.html

JS:   arr.includes(x)
来源：http://hz.yj20258888.top/gtagtfjbws.html

TS:   arr.includes(x)
来源：http://hz.nanxinkj.top/gtjdggbdyz.html

Java: list.contains(x)
来源：http://hz.hongshengwenyu.top/gtbjouiztw.html

Go:   slices.Contains(arr, x)
来源：http://hz.svipenyu.cn/gtmowuxktg.html

Ruby: arr.include?(x)
来源：http://hz.ydzc1.top/gtwvwihrod.html

C#:   list.Contains(x)
来源：http://hz.shzxlz.cn/gtimxudmfv.html

[D22] 复制数组（避免共享引用）
来源：http://hz.yuxming.cn/gtlvhuiqfh.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.havefunace.top/gtxynjljqq.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.feifeiyinyue.top/gtwlzcwuih.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.mhx1999.top/gtvmpryrol.html

TS:   [...arr];
来源：http://hz.jqgufenzy.top/gtijcirkpu.html

Java: new ArrayList<>(list);
来源：http://hz.meibo888.top/gtctrwaxdd.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.0kj1m.cn/gtzouleprm.html

Ruby: arr.dup;  arr.clone
来源：http://hz.shanyushiyangtech.top/gtsyksihiw.html

C#:   new List<int>(list);
来源：http://hz.fzhhl.top/gtasglipyl.html

[D23] reduce 累积计算
来源：http://hz.cashguo.top/gtemokoyrr.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.snrcjt.cn/gtstfdqpwv.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.ydzc1.top/gtquvgeghp.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ivvv.top/gtdpmofxjv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.iojbl.cn/gtsyadkcsp.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.yj20258.top/gtbmodidon.html

Go:   // 手写循环
来源：http://hz.nwbrower.top/gtbzdcvvph.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.jyoumei.cn/gtuknirqga.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.birdmap.top/gtbvkujkgi.html

[D24] 字典 / Map 基本操作
来源：http://hz.yanxiufei.cn/gtfxnyiebx.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.xylfe.cn/gtuqswcyaw.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.gzhubu.top/gtbgifqnuf.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.pengpengdd.cyou/gtrmahmvgu.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.yj20258888.top/gtxfihdfiu.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.chenlongwang.top/gtktarrodv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.yuxming.cn/gttnwpejhk.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.gogol.net.cn/gtqaidlave.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.cdnleiting.top/gtfchjuhcx.html

[D25] Set 集合去重与交并差
来源：http://hz.shuidangran.top/gtvyofjpvb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.cashguo.top/gtiyrbnuhk.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.jinqigfzy.top/gtvxcwetuk.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.yvedp.cn/gtsnosjhjf.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.ybcxt.top/gtawasngmq.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.jinyuanbaomall.cn/gtmydxjaze.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.tanke756.top/gtqdisbfbk.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.quarkkingdee.top/gtcotsxyzd.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.zhaomingkeji.xyz/gtgtvxtpit.html

[D26] 数组转字符串
来源：http://hz.ehwqpu.com/gtadmrsvgg.html

Py:   ", ".join(map(str, arr))
来源：http://hz.hnxiangtu.top/gtjcgjcieg.html

PHP:  implode(", ", $arr);
来源：http://hz.xziqi.cn/gttowduzyp.html

JS:   arr.join(", ")
来源：http://hz.hnqzz.top/gtiaitcvdv.html

TS:   arr.join(", ")
来源：http://hz.yueranfly.top/gtakmfshea.html

Java: String.join(", ", list)
来源：http://hz.hywenlv.cn/gtpvnckgzn.html

Go:   strings.Join(strs, ", ")
来源：http://hz.yanxiufei.cn/gtisvvoxbq.html

Ruby: arr.join(", ")
来源：http://hz.yanxiufei.cn/gtojnayuqa.html

C#:   string.Join(", ", list)
来源：http://hz.shanyushiyangkeji.top/gtjqjqgpoa.html

================================================================================
来源：http://hz.ydjk.org.cn/gtyrkzxzyv.html

E. 字符串处理
来源：http://hz.jinghuilouyu.cn/gtoxdpemft.html

================================================================================
来源：http://hz.yongpay.top/gtxjcuxsva.html

[E01] 拼接字符串
来源：http://hz.hnqzz.top/gtiggbkhhw.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.shangyingyoupin.top/gttlajncmn.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.nanxuanxn.top/gtmemzryiv.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.gogol.net.cn/gtgyzfskpp.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ehwqpu.com/gtqslxftkb.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.hammf.cn/gtaswxfudj.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.yj20258888.top/gtnsxpdqyp.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.ywan-chungtsiang.top/gtyngzgail.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.pengpengdd.cyou/gtjldedioy.html

[E02] 重复字符串
来源：http://hz.mhx1999.top/gtqzqcenna.html

Py:   "ab" * 3
来源：http://hz.tianlin.xyz/gtlxxmyvgc.html

PHP:  str_repeat("ab", 3);
来源：http://hz.hnxiangtu.top/gtygzfwjxy.html

JS:   "ab".repeat(3)
来源：http://hz.0kj1m.cn/gtkuzhvsxw.html

TS:   "ab".repeat(3)
来源：http://hz.snrcjt.cn/gtqvulmviz.html

Java: "ab".repeat(3)
来源：http://hz.ppjwa.cn/gtminhravu.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.yangfankeji.com/gthjxembao.html

Ruby: "ab" * 3
来源：http://hz.pengpengdd.cyou/gtfezsthni.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.hnxiangtu.top/gtdjipxtfc.html

[E03] 截取子串
来源：http://hz.zhijiandao.cn/gthgdvbpsu.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.snrcjt.cn/gtvqthmwzc.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.vqdsnc.cn/gtxewbqxxb.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.pycfn.com/gtzkisqlyk.html

TS:   s.slice(1, 4)
来源：http://hz.mhx1999.top/gtkxiivpyq.html

Java: s.substring(1, 4)
来源：http://hz.nanxuanxn.top/gtcomfpbot.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.zhoulong.xyz/gtvcfzvtaw.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.jyoumei.cn/gtcgjmxyeo.html

C#:   s.Substring(1, 3)
来源：http://hz.jinqigfzy.top/gtzjzzefjb.html

[E04] 查找子串位置
来源：http://hz.haohaochexian.top/gtsmwjqxmo.html

Py:   s.find("x");  s.index("x")
来源：http://hz.pengpengdd.cyou/gtmwnhyjve.html

PHP:  strpos($s, "x");
来源：http://hz.wangdashe.top/gtjqoxqmuf.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.zhiwuduotai.top/gtphxhlqip.html

TS:   s.indexOf("x")
来源：http://hz.redwolf501.top/gtdhlzlzur.html

Java: s.indexOf("x")
来源：http://hz.yangfankeji.com/gtnmkkmrnl.html


<!-- 参考信息 -->