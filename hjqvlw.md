代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.bjfxy.top/gtexncfvqt.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.ydjk.org.cn/gtykvubcha.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.gzhubu.top/gtdcribiec.html

Ruby: # 无泛型
来源：http://hz.wangdashe.top/gtyyoapeql.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.pycfn.com/gtjsbsqusv.html

[C15] 解构 / 展开参数
来源：http://hz.yanxiufei.cn/gtwsihcbqk.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.nanxuanxn.top/gtxgnnzxlf.html

PHP:  [$a, $b] = $pair;
来源：http://hz.nanxinkj.top/gtrtoeeiiq.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.yvedp.cn/gtryykrbag.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.daxiang520.top/gtoeiginpp.html

Java: // 无解构
来源：http://hz.wangdashe.top/gtvmpjaumn.html

Go:   // 无解构
来源：http://hz.mhx1999.top/gtyygrjmjf.html

Ruby: a, b = pair
来源：http://hz.gzhubu.top/gtadplcrfu.html

C#:   var (a, b) = pair;
来源：http://hz.tanke756.top/gtlpvlzsls.html

[C16] 函数 / 方法重载
来源：http://hz.dianchejie.cn/gtkamebxnr.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.yuanzhike.top/gturictlpq.html

PHP:  // 无重载
来源：http://hz.iojbl.cn/gteqcbklda.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.daxiang520.top/gtitnxsoeu.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.kuanghao11.cn/gtyxygrqbq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.shanyushiyangkeji.top/gtgqkzktqa.html

Go:   // 无重载：用不同函数名
来源：http://hz.yuxming.cn/gtnxvegkao.html

Ruby: # 无重载：靠动态参数
来源：http://hz.birdmap.top/gtnprgvkun.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.jqgfzy.top/gtmkzxpfnm.html

================================================================================
来源：http://hz.jqgfzy.top/gtdyeetods.html

D. 数组 / 列表 / 集合
来源：http://hz.zhengqikj.top/gtubrzzbos.html

================================================================================
来源：http://hz.gaohongyu789.top/gttdzmzbcf.html

[D01] 创建数组 / 列表
来源：http://hz.vqdsnc.cn/gthhvoyxdd.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.hammf.cn/gtzihpzria.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.shanyushiyangtech.top/gtmzfurecm.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.bjfxy.top/gtoqzuxqjk.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.hnqzz.top/gtlohshffc.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.kuanghao11.cn/gtswaybgxo.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.shuidangran.top/gtajptfdyr.html

Ruby: arr = [1, 2, 3]
来源：http://hz.iojbl.cn/gtmzgccavn.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.haohaochexian.top/gttrbjurpk.html

[D02] 追加元素到末尾
来源：http://hz.c1oappe.top/gttyheeamg.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.dashuyun.cn/gtreipvcyo.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.yangfankeji.com/gtmtiuzdfr.html

JS:   arr.push(4);
来源：http://hz.gogol.net.cn/gtgynfcygg.html

TS:   arr.push(4);
来源：http://hz.snrcjt.cn/gtildapgik.html

Java: list.add(4);
来源：http://hz.zhongyouzk.top/gtpnjdisqa.html

Go:   arr = append(arr, 4)
来源：http://hz.wangdashe.top/gtfwdysfnz.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.shanyushiyangkeji.top/gtdxknpkix.html

C#:   list.Add(4);
来源：http://hz.hongshengwenyu.top/gtejdrzlqc.html

[D03] 在指定位置插入元素
来源：http://hz.ivvv.top/gtyvzchqrj.html

Py:   arr.insert(0, 0)
来源：http://hz.xuanzx.com/gtxcdfzqky.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.9152youxi.cn/gtnkmvnppy.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.jinqigfzy.top/gtxyymcjcy.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.jiagoushi.top/gttvtgwcjy.html

Java: list.add(0, 0);
来源：http://hz.smart0.xyz/gtmdakvlwq.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.yuanzhike.top/gtgualtfvn.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.jinyuanbaomall.cn/gteijlfmec.html

C#:   list.Insert(0, 0);
来源：http://hz.nanxinkj.top/gtndblnrzj.html

[D04] 删除元素
来源：http://hz.9152youxi.cn/gtpeolfpuu.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.52xcode.cn/gtjolldryf.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.sysykeji.top/gtzfyhhngl.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.andypj.xyz/gttbskkbuy.html

TS:   arr.splice(0, 1);
来源：http://hz.pengpengdd.cyou/gtcbnkrwka.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.nanxinkj.top/gtgbvxcovz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.aizwys.cn/gtiiaprlqf.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.chenlongwang.top/gtwdusiifh.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.yuanzhike.top/gtwqsqjrvb.html

[D05] 访问与修改元素
来源：http://hz.hongshengwenyu.top/gtkmqtllcg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.gotoacloud.top/gtewvstprq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.iojbl.cn/gtsonqklwj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.quarkkingdee.top/gtspbcbvab.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.zhengqikj.top/gthiqctwfb.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.yj202588.top/gtecystdoe.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.jlsjyb.cn/gtrtqbjcpx.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.tanke756.top/gtuvvndsad.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.hfpthk.cn/gtqjfcprtm.html

[D06] 数组长度
来源：http://hz.shuidangran.top/gtmnjehbhv.html

Py:   len(arr)
来源：http://hz.zhongyouzk.top/gtjkqgueqp.html

PHP:  count($arr);
来源：http://hz.gaohongyu789.top/gtlfnwdxho.html

JS:   arr.length
来源：http://hz.jqgufenzy.top/gtmofjsxvb.html

TS:   arr.length
来源：http://hz.cheryme.top/gtaptagdme.html

Java: list.size();
来源：http://hz.redwolf501.top/gtueyjabbq.html

Go:   len(arr)
来源：http://hz.daria6918.cn/gtxtdijtce.html

Ruby: arr.length; arr.size
来源：http://hz.yueranfly.top/gtglczjvcl.html

C#:   list.Count;
来源：http://hz.dianchejie.cn/gtzttswupe.html

[D07] 切片 / 取子数组
来源：http://hz.hywenlv.cn/gtlmayrdpa.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.zycfv.cn/gtzbvrvwkf.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.aizwys.cn/gtgefwzqhm.html

JS:   arr.slice(1, 4);
来源：http://hz.svipenyu.cn/gtkepzqcoj.html

TS:   arr.slice(1, 4);
来源：http://hz.yj20258.top/gtfinmguau.html

Java: list.subList(1, 4);
来源：http://hz.chenzaomai.com/gtybfvaahe.html

Go:   arr[1:4]
来源：http://hz.xinyue.icu/gtttvycbqo.html

Ruby: arr[1, 3]
来源：http://hz.tanke756.top/gtccfjvqfk.html

C#:   list.GetRange(1, 3);
来源：http://hz.xuetiantiany.cn/gtecfqwpum.html

[D08] 合并两个数组
来源：http://hz.dianchejie.cn/gtqwmwuynk.html

Py:   a + b;  a.extend(b)
来源：http://hz.yuxming.cn/gtheigvlrw.html

PHP:  array_merge($a, $b);
来源：http://hz.kuanghao11.cn/gtcahizjze.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.andypj.xyz/gtqjjeftgr.html

TS:   [...a, ...b];
来源：http://hz.0kj1m.cn/gteblsfiil.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.chenlongwang.top/gtkickkkut.html

Go:   append(a, b...)
来源：http://hz.bjfxy.top/gtehpyehee.html

Ruby: a + b;  a.concat(b)
来源：http://hz.zhixingplan.top/gtxpmpbicl.html

C#:   a.Concat(b).ToList()
来源：http://hz.zhongyouzk.top/gtifdejsxw.html

[D09] 排序（升序）
来源：http://hz.9152youxi.cn/gtnzxwctmi.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.meibo888.top/gtwaxerdcj.html

PHP:  sort($arr);
来源：http://hz.yongpay.top/gtvuthxdfs.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.jqgufenzy.top/gtrmamklhx.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.nanxuanxn.top/gtodemxand.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.guannengcc.top/gtjvaylrok.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.gotoacloud.top/gtvhhaapjz.html

Ruby: arr.sort
来源：http://hz.gogol.net.cn/gtmggjobnn.html

C#:   list.Sort();
来源：http://hz.xuanzx.com/gtbrazvsmq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.9152youxi.cn/gtvpuoulek.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.hfpthk.cn/gtdmacsycb.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yvedp.cn/gtmtsxwltk.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.chenjidiqi.icu/gteskobwix.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hysaishi.cn/gtynjcuvde.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.cheryme.top/gtnmqfxmqh.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.316326.xyz/gtmllacdfo.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.jyoumei.cn/gtmyjwlldp.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.jianghu66.top/gtxxttstkj.html

[D11] 反转数组
来源：http://hz.sufxvd.cn/gtjmohsddt.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.c1oappe.top/gttyiyimvv.html

PHP:  array_reverse($arr);
来源：http://hz.ivvv.top/gthztcjbdt.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.ivvv.top/gtdpvzumxp.html

TS:   [...arr].reverse();
来源：http://hz.zhongyouzk.top/gtvlwigvso.html

Java: Collections.reverse(list);
来源：http://hz.aizwys.cn/gtkrhgfufh.html

Go:   slices.Reverse(arr)
来源：http://hz.haohaochexian.top/gtjewkwhwo.html

Ruby: arr.reverse
来源：http://hz.jyoumei.cn/gtyhxithrk.html

C#:   list.Reverse();
来源：http://hz.sufxvd.cn/gtzmyavgbm.html

[D12] 查找元素下标
来源：http://hz.9152youxi.cn/gtmufgiaey.html

Py:   arr.index(x);  x in arr
来源：http://hz.yanxiufei.cn/gturkqvuij.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.chenzaomai.com/gtcrjxtrch.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yj20258.top/gttihcmmqx.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yongpay.top/gtekoeetev.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.hywenlv.cn/gtmgruguqx.html

Go:   slices.Index(arr, x)
来源：http://hz.ppjwa.cn/gtneudqxcn.html

Ruby: arr.index(x)
来源：http://hz.9152youxi.cn/gtnavlrxqz.html

C#:   list.IndexOf(x);
来源：http://hz.jianghu66.top/gtbdqmdrqc.html

[D13] 过滤（保留满足条件的）
来源：http://hz.chenlongwang.top/gtqlzfzmwl.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.shanyushiyangkeji.top/gtppxgveux.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.yj202588.top/gtyybhmmnw.html

JS:   arr.filter(x => x > 3)
来源：http://hz.chenjidiqi.icu/gtubkisghc.html

TS:   arr.filter(x => x > 3)
来源：http://hz.tianlin.xyz/gthwxbmmzv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.yj202588.top/gtglqgdopk.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.yj202588.top/gtjdzqsbbe.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.guowangkeji.top/gthzkomcel.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.zhijiandao.cn/gtgjnvxufo.html

[D14] 映射转换（每个元素变形）
来源：http://hz.yvedp.cn/gtwymikhtm.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.zhijiandao.cn/gtdmhjvalx.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.havefunace.top/gtslenonwn.html

JS:   arr.map(x => x * 2)
来源：http://hz.svipenyu.cn/gtkdcyytks.html

TS:   arr.map(x => x * 2)
来源：http://hz.zhongyouzk.top/gtojqqstrl.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.tian-w.cn/gtibwqqahn.html

Go:   // 手写循环
来源：http://hz.sufxvd.cn/gtbfaclyin.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.yuanzhike.top/gtgmduvior.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.ydzc1.top/gtahntiuol.html

[D15] 去重
来源：http://hz.xuetiantiany.cn/gtdwrrshvt.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.0kj1m.cn/gtigojsbli.html

PHP:  array_unique($arr);
来源：http://hz.zhongyouzk.top/gtnjjfnbkg.html

JS:   [...new Set(arr)]
来源：http://hz.shangyingyoupin.top/gtngjimdtb.html

TS:   [...new Set(arr)]
来源：http://hz.shangyingyoupin.top/gtvdphiryi.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.pycfn.com/gthhjslzks.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.iojbl.cn/gtyntqkerj.html

Ruby: arr.uniq
来源：http://hz.sysykeji.top/gtcxbspilu.html

C#:   list.Distinct().ToList()
来源：http://hz.yvedp.cn/gtbvltitmb.html

[D16] 求和与平均值
来源：http://hz.cqqwz.cn/gtxmrzettu.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.sxryk.cn/gtvpduxuku.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.wangdashe.top/gtktecahfv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.tian-w.cn/gtzrqcdmcw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yj202588.top/gttydgnbrs.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.yanxiufei.cn/gtglinulcf.html

Go:   // 手写循环累加
来源：http://hz.cdnleiting.top/gtooioxgoo.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.sxryk.cn/gtpsdsnqeg.html

C#:   list.Sum();  list.Average()
来源：http://hz.zycfv.cn/gtxhvfspjg.html

[D17] 最大值与最小值
来源：http://hz.jinqigufen.top/gtryopkmsh.html

Py:   max(arr);  min(arr)
来源：http://hz.ywan-chungtsiang.top/gtlgwjgulb.html

PHP:  max($arr);  min($arr);
来源：http://hz.9152youxi.cn/gtlnkvvkrs.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.fengsongda.top/gtqwhazgko.html

TS:   Math.max(...arr);
来源：http://hz.yj202588.top/gtgmcbrtci.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.jiagoushi.top/gtanuabvhm.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.cashguo.top/gtrucjsguw.html

Ruby: arr.max;  arr.min
来源：http://hz.zhoulong.xyz/gtfzyjkukd.html

C#:   list.Max();  list.Min()
来源：http://hz.yangfankeji.com/gtsihlogai.html

[D18] 扁平化嵌套数组
来源：http://hz.zhoulong.xyz/gtxgoctelo.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.yuanzhike.top/gtzcshrqtn.html

PHP:  array_merge(...$nested);
来源：http://hz.snrcjt.cn/gtyhweaqvu.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.nwbrower.top/gtawhvswqn.html

TS:   nested.flat();
来源：http://hz.xuanzx.com/gtzyrwkvdn.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.jinqigfzy.top/gtifbjggkn.html

Go:   // 手写双层循环
来源：http://hz.nwbrower.top/gthrcxmkfb.html

Ruby: nested.flatten
来源：http://hz.wangdashe.top/gtaetvlxwt.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.zdqjudy.top/gtxkwccbzb.html

[D19] 按字段分组
来源：http://hz.zhijiandao.cn/gtnsiuupxe.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.zycfv.cn/gtdrqxuuss.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.zhixingplan.top/gtvtzhckcm.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.nanxinkj.top/gtmfjstybp.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.c1oappe.top/gtusfjeekb.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.yongpay.top/gttsgwlmzq.html

Go:   // 手写 map[string][]T
来源：http://hz.ppjwa.cn/gtuanhkbjl.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.yueranfly.top/gthobwitvu.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.wangdashe.top/gtxnunplil.html

[D20] 统计每个元素出现次数
来源：http://hz.wangshuangyany.cn/gtyqbdgmlh.html

Py:   Counter(arr)
来源：http://hz.haohaochexian.top/gtnmdntwkc.html

PHP:  array_count_values($arr);
来源：http://hz.daxiang520.top/gtjbemxixw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.svipenyu.cn/gtruufrmnt.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.wangdashe.top/gtdgmpjdnn.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.cucudq.cn/gtrapnwklc.html

Go:   // 手写 map[T]int
来源：http://hz.shanyushiyangkeji.top/gtovznrzti.html

Ruby: arr.tally
来源：http://hz.shzxlz.cn/gtxbvldsfo.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.jqgfzy.top/gtyasxqeic.html

[D21] 判断是否包含某元素
来源：http://hz.fzhhl.top/gtntcustrm.html

Py:   x in arr
来源：http://hz.zhongyouzk.top/gttqrbngxk.html

PHP:  in_array($x, $arr, true);
来源：http://hz.hysaishi.cn/gtscuraeek.html

JS:   arr.includes(x)
来源：http://hz.guowangkeji.top/gtvnbdtayz.html

TS:   arr.includes(x)
来源：http://hz.aizwys.cn/gtloxsavju.html

Java: list.contains(x)
来源：http://hz.fengsongda.top/gtwyoogpit.html

Go:   slices.Contains(arr, x)
来源：http://hz.zhiwuduotai.top/gteaeowzbr.html

Ruby: arr.include?(x)
来源：http://hz.nanxuanxn.top/gtblwchltt.html

C#:   list.Contains(x)
来源：http://hz.gzhubu.top/gtdjjdvwif.html

[D22] 复制数组（避免共享引用）
来源：http://hz.zhoulong.xyz/gtnsxtalzg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.jqgufenzy.top/gtzwzezajf.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.hongshengwenyu.top/gtnaoojtdl.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.tanke756.top/gtejjbirwt.html

TS:   [...arr];
来源：http://hz.cucudq.cn/gtzjxyplmb.html

Java: new ArrayList<>(list);
来源：http://hz.cashguo.top/gtrvtkqbuq.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.tianlin.xyz/gtlosawjyy.html

Ruby: arr.dup;  arr.clone
来源：http://hz.yj20258.top/gtfqwxhvcv.html

C#:   new List<int>(list);
来源：http://hz.gaohongyu789.top/gtqhffmefc.html

[D23] reduce 累积计算
来源：http://hz.nanxuanxn.top/gtszonkzzd.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.zhaomingkeji.xyz/gtmrglanjh.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.xuetiantiany.cn/gtiqathrec.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.smart0.xyz/gtwzhslkcj.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yangfankeji.com/gtexjahlcw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.sweek.top/gtatlassql.html

Go:   // 手写循环
来源：http://hz.feifeiyinyue.top/gtaijtnlob.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.chenjidiqi.icu/gtajzpqjnm.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.chenzaomai.com/gtsubatfpq.html

[D24] 字典 / Map 基本操作
来源：http://hz.jqgfzy.top/gtroyjjzde.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.fzhhl.top/gtplvnqqrn.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.bjfxy.top/gtyoropjsl.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.hfpthk.cn/gtwlewuucc.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.yuxming.cn/gtnclbsbhl.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.zycfv.cn/gtncnxbouc.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.nwbrower.top/gtvzrildtt.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.redwolf501.top/gtpunjntmn.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.cheryme.top/gtqlxquhof.html

[D25] Set 集合去重与交并差
来源：http://hz.ydzc1.top/gttrlrdjtg.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.iojbl.cn/gtzvsnecca.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.ppjwa.cn/gtpebhqwzy.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.hammf.cn/gtqwctbbub.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.ehwqpu.com/gtbgoznsdo.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.wangdashe.top/gtsknlwqgl.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.jqgfzy.top/gteelqszvc.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.jqgufenzy.top/gtbmllguve.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.hywenlv.cn/gtpdowbust.html

[D26] 数组转字符串
来源：http://hz.dashuyun.cn/gtxvaiyjow.html

Py:   ", ".join(map(str, arr))
来源：http://hz.shanyushiyangtech.top/gtmechnoul.html

PHP:  implode(", ", $arr);
来源：http://hz.jyoumei.cn/gtrzprowpa.html

JS:   arr.join(", ")
来源：http://hz.andypj.xyz/gtwfxamvmz.html

TS:   arr.join(", ")
来源：http://hz.gogol.net.cn/gtrqdvnsyb.html

Java: String.join(", ", list)
来源：http://hz.zycfv.cn/gtwmygcdrb.html

Go:   strings.Join(strs, ", ")
来源：http://hz.yj20258888.top/gtbkrteadm.html

Ruby: arr.join(", ")
来源：http://hz.c1oappe.top/gtchshkbaq.html

C#:   string.Join(", ", list)
来源：http://hz.yangfankeji.com/gtpyqtczea.html

================================================================================
来源：http://hz.sweek.top/gtsfeghtpa.html

E. 字符串处理
来源：http://hz.yj20258888.top/gtrbzvzbzg.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtgtadfimf.html

[E01] 拼接字符串
来源：http://hz.0kj1m.cn/gtzewpltfp.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.zhiwuduotai.top/gtoodyyivm.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.zhengqikj.top/gtetqeasxs.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.guannengcc.top/gtogqlhxzq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.0kj1m.cn/gthaeafpul.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.xinyue.icu/gtmwubjvpr.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.pengpengdd.cyou/gtnxjkyjtr.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.cdnleiting.top/gtxsfpefiy.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.smart0.xyz/gtmegydpfo.html

[E02] 重复字符串
来源：http://hz.sysykeji.top/gtwzihpbop.html

Py:   "ab" * 3
来源：http://hz.zhongyouzk.top/gtvgnzdxda.html

PHP:  str_repeat("ab", 3);
来源：http://hz.jqgufenzy.top/gtccvmfyma.html

JS:   "ab".repeat(3)
来源：http://hz.zhixingplan.top/gttrvsvmsc.html

TS:   "ab".repeat(3)
来源：http://hz.gaohongyu789.top/gteericxrb.html

Java: "ab".repeat(3)
来源：http://hz.iojbl.cn/gtinooyqsc.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.daria6918.cn/gtmmxtcdyb.html

Ruby: "ab" * 3
来源：http://hz.zhaomingkeji.xyz/gtpmatnnkk.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.quarkkingdee.top/gtfohsxhhc.html

[E03] 截取子串
来源：http://hz.hfpthk.cn/gtumgosqom.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.shuidangran.top/gttzzsgnzv.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.tianlin.xyz/gtmcejkzvt.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.iojbl.cn/gttrzlcdwl.html

TS:   s.slice(1, 4)
来源：http://hz.zhoulong.xyz/gtmmyweorp.html

Java: s.substring(1, 4)
来源：http://hz.sufxvd.cn/gtpcrpmwmm.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.hywenlv.cn/gtevoidsdy.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.nanxuanxn.top/gthbbkokji.html

C#:   s.Substring(1, 3)
来源：http://hz.wangdashe.top/gtenmgymuw.html

[E04] 查找子串位置
来源：http://hz.hfpthk.cn/gtsvlemnav.html

Py:   s.find("x");  s.index("x")
来源：http://hz.hysaishi.cn/gteunuuxqd.html

PHP:  strpos($s, "x");
来源：http://hz.52xcode.cn/gtxptojiec.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.jlsjyb.cn/gtckitxamo.html

TS:   s.indexOf("x")
来源：http://hz.zdqjudy.top/gtfiylbdhk.html

Java: s.indexOf("x")
来源：http://hz.xylfe.cn/gtywljtklg.html

Go:   strings.Index(s, "x")
来源：http://hz.ywan-chungtsiang.top/gtwradizhv.html

Ruby: s.index("x")
来源：http://hz.yvedp.cn/gtxgwmekwc.html

C#:   s.IndexOf("x")
来源：http://hz.birdmap.top/gtnkdrhplf.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.hongshengwenyu.top/gtxhkdinmk.html


<!-- 参考信息 -->