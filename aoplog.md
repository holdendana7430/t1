代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://hz.pycfn.com/gtluevdrxf.html

JS:   (() => { console.log("run"); })();
来源：http://hz.yonumen.top/gtwobpdjub.html

TS:   (() => { console.log("run"); })();
来源：http://hz.havefunace.top/gtsnwbudpf.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.zhoulong.xyz/gtvhgafwop.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.zhiwuduotai.top/gtgtfyzlyu.html

Ruby: -> { puts "run" }.call
来源：http://hz.ivvv.top/gtfjpdjhpt.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.xylfe.cn/gtoilndvau.html

[C13] 类型声明 / 类型注解
来源：http://hz.316326.xyz/gtkucglata.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.zhengqikj.top/gtrvmfzghx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.xingfuxueyuan.xyz/gtpjxvhrqt.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.cqqwz.cn/gthaujmytu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.shanyushiyangtech.top/gtzrrjoggo.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.yvedp.cn/gtzihbwivb.html

Go:   func add(a, b int) int
来源：http://hz.tanke756.top/gtyeztkvxl.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.yonumen.top/gtbjbsqfwq.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.sxryk.cn/gttgffqujf.html

[C14] 泛型函数
来源：http://hz.nanxuanxn.top/gthujfnrmx.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.shzxlz.cn/gtxclqjkyn.html

PHP:  // 无泛型
来源：http://hz.daria6918.cn/gtmvmsddma.html

JS:   // 无泛型
来源：http://hz.shangyingyoupin.top/gtrexkybqo.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.ivvv.top/gtkwbnuajc.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.dianchejie.cn/gtftfquetv.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.bjfxy.top/gtvjwaiuel.html

Ruby: # 无泛型
来源：http://hz.tianlin.xyz/gtesnwivvf.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.zycfv.cn/gtewwoupfo.html

[C15] 解构 / 展开参数
来源：http://hz.zycfv.cn/gtjonhbhyk.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.xuanzx.com/gtjhfbxnet.html

PHP:  [$a, $b] = $pair;
来源：http://hz.andypj.xyz/gtssdkwqcn.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.yvedp.cn/gthcflcphd.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.jyoumei.cn/gtwbfiaayi.html

Java: // 无解构
来源：http://hz.zhixingplan.top/gttgmrykxd.html

Go:   // 无解构
来源：http://hz.yj20258.top/gtlpvftmbo.html

Ruby: a, b = pair
来源：http://hz.shanyushiyangtech.top/gtnlwzckkr.html

C#:   var (a, b) = pair;
来源：http://hz.ivvv.top/gtsooewedh.html

[C16] 函数 / 方法重载
来源：http://hz.c1oappe.top/gtakjgvoiu.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.cdnleiting.top/gtynlwwsro.html

PHP:  // 无重载
来源：http://hz.chenjidiqi.icu/gtamiwupyu.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.hnqzz.top/gtsqtwhmqe.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.yueranfly.top/gthxgweahf.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.ywan-chungtsiang.top/gtczupfxin.html

Go:   // 无重载：用不同函数名
来源：http://hz.gotoacloud.top/gtzfofzsmq.html

Ruby: # 无重载：靠动态参数
来源：http://hz.hnxiangtu.top/gtwvmgwxnx.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.quarkkingdee.top/gtkxdhbtel.html

================================================================================
来源：http://hz.dashuyun.cn/gtvsjdtwqi.html

D. 数组 / 列表 / 集合
来源：http://hz.ydzc1.top/gtyzjhlidt.html

================================================================================
来源：http://hz.hnxiangtu.top/gtokcqrkdv.html

[D01] 创建数组 / 列表
来源：http://hz.yuxming.cn/gtuhnavlhg.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.jlsjyb.cn/gtnoilsren.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.guannengcc.top/gtmsidvgsc.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.svipenyu.cn/gtsaaxpfnz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.jianghu66.top/gthfyanwbf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.hfpthk.cn/gtjzildnqs.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.sxryk.cn/gtbshqahzx.html

Ruby: arr = [1, 2, 3]
来源：http://hz.shzxlz.cn/gtrfhdlkqt.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.zdqjudy.top/gtjpaezwgw.html

[D02] 追加元素到末尾
来源：http://hz.pengpengdd.cyou/gtushegjfb.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.guowangkeji.top/gtxkrrbgzg.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.cucudq.cn/gtyfsrkljn.html

JS:   arr.push(4);
来源：http://hz.shanyushiyangkeji.top/gtemfvbbdz.html

TS:   arr.push(4);
来源：http://hz.guannengcc.top/gtafubhxiq.html

Java: list.add(4);
来源：http://hz.zhaomingkeji.xyz/gtlirseszg.html

Go:   arr = append(arr, 4)
来源：http://hz.cqqwz.cn/gtksmjuayi.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.redwolf501.top/gtcgbjiefd.html

C#:   list.Add(4);
来源：http://hz.chenlongwang.top/gttdaeghws.html

[D03] 在指定位置插入元素
来源：http://hz.dianchejie.cn/gtkhlpaqbv.html

Py:   arr.insert(0, 0)
来源：http://hz.shanyushiyangkeji.top/gtflcutzio.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.aibaodan.cn/gtpqwqdlgp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.guannengcc.top/gteqsgvbsu.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.shangyingyoupin.top/gtuttrflya.html

Java: list.add(0, 0);
来源：http://hz.cheryme.top/gtygfgmxtp.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.fzhhl.top/gtldlsuhft.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.fzhhl.top/gtrmptuudq.html

C#:   list.Insert(0, 0);
来源：http://hz.zhixingplan.top/gtwgrucbkn.html

[D04] 删除元素
来源：http://hz.hysaishi.cn/gtzsluzrwp.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.zhijiandao.cn/gtwaqlaecm.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.haohaochexian.top/gtgrjpcxpx.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.tanke756.top/gtiozveddp.html

TS:   arr.splice(0, 1);
来源：http://hz.jinqigfzy.top/gtdishstqr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.wangshuangyany.cn/gtmhaaviar.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.smart0.xyz/gtnkefjfwp.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.jinyuanbaomall.cn/gtlhtnzczq.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.c1oappe.top/gtxxvijhby.html

[D05] 访问与修改元素
来源：http://hz.shuidangran.top/gtwdwfrwbb.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.shanyushiyangkeji.top/gtfzghudtj.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.aibaodan.cn/gtxeegnyos.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.gotoacloud.top/gtztqaqhhn.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.nanxinkj.top/gtvysjbusz.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.xuanzx.com/gtfshojmcu.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.dashuyun.cn/gtafmczavw.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.shanyushiyangtech.top/gtyjqvfywg.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.jianghu66.top/gtufhydgfo.html

[D06] 数组长度
来源：http://hz.ppjwa.cn/gtybtlegiq.html

Py:   len(arr)
来源：http://hz.yj20258888.top/gtihydeenf.html

PHP:  count($arr);
来源：http://hz.jlsjyb.cn/gtjcfkwycn.html

JS:   arr.length
来源：http://hz.zdqjudy.top/gtukipevlf.html

TS:   arr.length
来源：http://hz.haohaochexian.top/gtjdzljatt.html

Java: list.size();
来源：http://hz.sxryk.cn/gtsgwtwwiz.html

Go:   len(arr)
来源：http://hz.52xcode.cn/gtygczsdzi.html

Ruby: arr.length; arr.size
来源：http://hz.ywan-chungtsiang.top/gtxsmgyefs.html

C#:   list.Count;
来源：http://hz.chenlongwang.top/gttwxkolmw.html

[D07] 切片 / 取子数组
来源：http://hz.haohaochexian.top/gtvymikfwa.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.xylfe.cn/gtqryodskh.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.ybcxt.top/gtzsxefvpd.html

JS:   arr.slice(1, 4);
来源：http://hz.tanke756.top/gtsbhvgzug.html

TS:   arr.slice(1, 4);
来源：http://hz.quarkkingdee.top/gtlaygcigb.html

Java: list.subList(1, 4);
来源：http://hz.birdmap.top/gtfdrnyuvi.html

Go:   arr[1:4]
来源：http://hz.fzhhl.top/gtjqpqvvak.html

Ruby: arr[1, 3]
来源：http://hz.cucudq.cn/gtmebpaefu.html

C#:   list.GetRange(1, 3);
来源：http://hz.xylfe.cn/gtqvmyabiz.html

[D08] 合并两个数组
来源：http://hz.snrcjt.cn/gtnnisyofa.html

Py:   a + b;  a.extend(b)
来源：http://hz.0kj1m.cn/gthxucoprn.html

PHP:  array_merge($a, $b);
来源：http://hz.daria6918.cn/gtwkjzfgmi.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.fengsongda.top/gtcxqvyqpu.html

TS:   [...a, ...b];
来源：http://hz.ywan-chungtsiang.top/gtockjhwxz.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.xingfuxueyuan.xyz/gtrdcgaqwx.html

Go:   append(a, b...)
来源：http://hz.jqgfzy.top/gtrszzncpj.html

Ruby: a + b;  a.concat(b)
来源：http://hz.hfpthk.cn/gtzrpwspye.html

C#:   a.Concat(b).ToList()
来源：http://hz.dianchejie.cn/gtwtcxlovn.html

[D09] 排序（升序）
来源：http://hz.hywenlv.cn/gtwqffthig.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.shangyingyoupin.top/gtkhfjdlkg.html

PHP:  sort($arr);
来源：http://hz.ydzc1.top/gtprdkhvgq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.cucudq.cn/gthogvaupa.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.nwbrower.top/gtxcabatej.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.havefunace.top/gtiulrclbr.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.shzxlz.cn/gtjdfgaeqx.html

Ruby: arr.sort
来源：http://hz.yanxiufei.cn/gtidfzujxq.html

C#:   list.Sort();
来源：http://hz.ywan-chungtsiang.top/gtzliivlhs.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.sufxvd.cn/gttirqpsfk.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.jlsjyb.cn/gtcgtlvlfc.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.sweek.top/gtgxffuovz.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.shzxlz.cn/gtzbjyihwu.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yongpay.top/gtrwroqnjo.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.c1oappe.top/gtikefcwtd.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.xingfuxueyuan.xyz/gtjloxoflr.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.xylfe.cn/gtxeloyvvt.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.jinyuanbaomall.cn/gtxfjvcigq.html

[D11] 反转数组
来源：http://hz.jinghuilouyu.cn/gtitptyggo.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.jiagoushi.top/gtxhicbiup.html

PHP:  array_reverse($arr);
来源：http://hz.yuanzhike.top/gtoyzuojux.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.fzhhl.top/gtjxgnsbgx.html

TS:   [...arr].reverse();
来源：http://hz.gzhubu.top/gtrhxbswlt.html

Java: Collections.reverse(list);
来源：http://hz.nwbrower.top/gtspgajeom.html

Go:   slices.Reverse(arr)
来源：http://hz.hongshengwenyu.top/gtbdzjlreq.html

Ruby: arr.reverse
来源：http://hz.shuidangran.top/gtutistgie.html

C#:   list.Reverse();
来源：http://hz.zhaomingkeji.xyz/gthscpmiom.html

[D12] 查找元素下标
来源：http://hz.zycfv.cn/gtdxkayqps.html

Py:   arr.index(x);  x in arr
来源：http://hz.shanyushiyangtech.top/gtlnzydgrr.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.shzxlz.cn/gtlhevdhjh.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.xylfe.cn/gtbzucjknf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.quarkkingdee.top/gtkvgmlaid.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.jinqigfzy.top/gtjvbiemqp.html

Go:   slices.Index(arr, x)
来源：http://hz.feifeiyinyue.top/gtpnfiyfss.html

Ruby: arr.index(x)
来源：http://hz.hnxiangtu.top/gthninvkla.html

C#:   list.IndexOf(x);
来源：http://hz.shanyushiyangtech.top/gtalcqqyim.html

[D13] 过滤（保留满足条件的）
来源：http://hz.tian-w.cn/gtdztfvfot.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.bjfxy.top/gtiqglmxyi.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.jinyuanbaomall.cn/gtwozzfath.html

JS:   arr.filter(x => x > 3)
来源：http://hz.jinghuilouyu.cn/gtoestqcyd.html

TS:   arr.filter(x => x > 3)
来源：http://hz.yuxming.cn/gthwlrkfjb.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.meibo888.top/gtrgwrivoi.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.cqqwz.cn/gtphirbmli.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.zhixingplan.top/gtjgvuzlut.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.yuxming.cn/gtezbpldcv.html

[D14] 映射转换（每个元素变形）
来源：http://hz.tianlin.xyz/gtglqiocmg.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.shuidangran.top/gtqzpqqunu.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.gaohongyu789.top/gtvbkpjcra.html

JS:   arr.map(x => x * 2)
来源：http://hz.jqgufenzy.top/gtuizvkvai.html

TS:   arr.map(x => x * 2)
来源：http://hz.xylfe.cn/gtfjljlnsq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.pycfn.com/gtcchmafha.html

Go:   // 手写循环
来源：http://hz.pengpengdd.cyou/gtizevvocx.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.zhongyouzk.top/gtipihuhns.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.hysaishi.cn/gtjazuftbq.html

[D15] 去重
来源：http://hz.sysykeji.top/gtfdodbqsn.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.yangfankeji.com/gtpyanshsx.html

PHP:  array_unique($arr);
来源：http://hz.aibaodan.cn/gtnftzbwyk.html

JS:   [...new Set(arr)]
来源：http://hz.cucudq.cn/gtxdvbctuc.html

TS:   [...new Set(arr)]
来源：http://hz.0kj1m.cn/gtpiwtfsrh.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.0kj1m.cn/gtvanshxbf.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.meibo888.top/gtmephjvac.html

Ruby: arr.uniq
来源：http://hz.xziqi.cn/gtpsgfyqgn.html

C#:   list.Distinct().ToList()
来源：http://hz.redwolf501.top/gtvaoaccep.html

[D16] 求和与平均值
来源：http://hz.chenjidiqi.icu/gtvapopdcx.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.sxryk.cn/gtsdzdyyow.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.shzxlz.cn/gtwiacflwy.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.svipenyu.cn/gtyfwmgozf.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hnxiangtu.top/gtslnmtutl.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.xuanzx.com/gtyzdudgjm.html

Go:   // 手写循环累加
来源：http://hz.pengpengdd.cyou/gtybxmbolm.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.ehwqpu.com/gtftsjznqz.html

C#:   list.Sum();  list.Average()
来源：http://hz.nanxuanxn.top/gtotcraodf.html

[D17] 最大值与最小值
来源：http://hz.yonumen.top/gtnagbbxol.html

Py:   max(arr);  min(arr)
来源：http://hz.feifeiyinyue.top/gthyeqvgdd.html

PHP:  max($arr);  min($arr);
来源：http://hz.zhoulong.xyz/gtovvzmnhq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.vqdsnc.cn/gtrqjdqnam.html

TS:   Math.max(...arr);
来源：http://hz.andypj.xyz/gtoxgusksd.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.shangyingyoupin.top/gtjfrjinws.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.xylfe.cn/gthmgizdqa.html

Ruby: arr.max;  arr.min
来源：http://hz.guannengcc.top/gtjhchdqpg.html

C#:   list.Max();  list.Min()
来源：http://hz.tian-w.cn/gtnmodiskw.html

[D18] 扁平化嵌套数组
来源：http://hz.shanyushiyangkeji.top/gtptmigvjn.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.zhoulong.xyz/gtnqjcnhvk.html

PHP:  array_merge(...$nested);
来源：http://hz.xinyue.icu/gtikgzgqwp.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.xinyue.icu/gtwiuhbcgf.html

TS:   nested.flat();
来源：http://hz.ppjwa.cn/gtavenxbqw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.chenlongwang.top/gtkqzwxlpv.html

Go:   // 手写双层循环
来源：http://hz.cheryme.top/gtvsmpaiqg.html

Ruby: nested.flatten
来源：http://hz.ydjk.org.cn/gtjqvpjclk.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.chenjidiqi.icu/gtbaztnevz.html

[D19] 按字段分组
来源：http://hz.jqgufenzy.top/gtkszhfvvx.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.0kj1m.cn/gthegjpbzt.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.jqgufenzy.top/gtvwpxbxgu.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.cucudq.cn/gtprrhsrbu.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.cqqwz.cn/gtwzcddmrh.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.feifeiyinyue.top/gtowkqfdaz.html

Go:   // 手写 map[string][]T
来源：http://hz.haohaochexian.top/gtzyibcqjc.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.xuanzx.com/gtefayoxyw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.xylfe.cn/gtvnpxucwl.html

[D20] 统计每个元素出现次数
来源：http://hz.nanxuanxn.top/gtezrximpm.html

Py:   Counter(arr)
来源：http://hz.ydjk.org.cn/gtqdudoapz.html

PHP:  array_count_values($arr);
来源：http://hz.jlsjyb.cn/gtaqwercsp.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zhoulong.xyz/gtwwubuzug.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.sufxvd.cn/gthztmgixh.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.haohaochexian.top/gtihclsjpr.html

Go:   // 手写 map[T]int
来源：http://hz.hnqzz.top/gtobewpjlv.html

Ruby: arr.tally
来源：http://hz.zhaomingkeji.xyz/gtagxiqwuk.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.aizwys.cn/gtrqcpwtpz.html

[D21] 判断是否包含某元素
来源：http://hz.gaohongyu789.top/gtfjcgbfhp.html

Py:   x in arr
来源：http://hz.zhongyouzk.top/gtonwmiuba.html

PHP:  in_array($x, $arr, true);
来源：http://hz.yuxming.cn/gtnjothhma.html

JS:   arr.includes(x)
来源：http://hz.hysaishi.cn/gtonyjxiuj.html

TS:   arr.includes(x)
来源：http://hz.kuanghao11.cn/gtfgoxxcdx.html

Java: list.contains(x)
来源：http://hz.yanxiufei.cn/gtcgyyzrcz.html

Go:   slices.Contains(arr, x)
来源：http://hz.bjfxy.top/gtffbntkol.html

Ruby: arr.include?(x)
来源：http://hz.chenzaomai.com/gtdoxxmauo.html

C#:   list.Contains(x)
来源：http://hz.aibaodan.cn/gtdygcmlsy.html

[D22] 复制数组（避免共享引用）
来源：http://hz.guowangkeji.top/gtppughdid.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.yonumen.top/gtgjqshyvr.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.yonumen.top/gtjtxbqxhj.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.xylfe.cn/gthpkaugcb.html

TS:   [...arr];
来源：http://hz.kuanghao11.cn/gtbzijaefj.html

Java: new ArrayList<>(list);
来源：http://hz.andypj.xyz/gtogfaxjbi.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.hammf.cn/gttfrgkxyl.html

Ruby: arr.dup;  arr.clone
来源：http://hz.yueranfly.top/gtpgknznnc.html

C#:   new List<int>(list);
来源：http://hz.cqqwz.cn/gtualhbjep.html

[D23] reduce 累积计算
来源：http://hz.zhijiandao.cn/gtgdchqjub.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.yuanzhike.top/gtwyfbxzto.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.chenlongwang.top/gtrjwzobdm.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.hywenlv.cn/gtpfudllqf.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.daria6918.cn/gtlgzfnhen.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.tian-w.cn/gtjyhjhdoi.html

Go:   // 手写循环
来源：http://hz.xinyue.icu/gtvdjynefm.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.meibo888.top/gtlzzsicvj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.jinqigufen.top/gtlhjzeyrd.html

[D24] 字典 / Map 基本操作
来源：http://hz.yongpay.top/gttbyrduap.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.mhx1999.top/gtwzjcidpq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.jlsjyb.cn/gtkwgumkym.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.316326.xyz/gtzqyxwjbb.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.jqgufenzy.top/gtznwpaqsl.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.chenjidiqi.icu/gtqobpudbz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.sufxvd.cn/gtnspiscly.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.jinyuanbaomall.cn/gtuoervkia.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.ybcxt.top/gtzzpydmns.html

[D25] Set 集合去重与交并差
来源：http://hz.jianghu66.top/gtyxirexuy.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.zdqjudy.top/gtofuwcdsj.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.mhx1999.top/gttxihavpw.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.yonumen.top/gthxnjortd.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.daria6918.cn/gtemwxlzaw.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.ywan-chungtsiang.top/gtgnsmalih.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.wangdashe.top/gtyfngpdyp.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.ybcxt.top/gtihrcpeoe.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.chenjidiqi.icu/gtemicsyki.html

[D26] 数组转字符串
来源：http://hz.jinghuilouyu.cn/gtmrvgzlsr.html

Py:   ", ".join(map(str, arr))
来源：http://hz.nwbrower.top/gtdkirakue.html

PHP:  implode(", ", $arr);
来源：http://hz.tian-w.cn/gtnaotinrv.html

JS:   arr.join(", ")
来源：http://hz.9152youxi.cn/gtjixdunsg.html

TS:   arr.join(", ")
来源：http://hz.hywenlv.cn/gtzcgrdkjq.html

Java: String.join(", ", list)
来源：http://hz.shanyushiyangtech.top/gtmuotcwoy.html

Go:   strings.Join(strs, ", ")
来源：http://hz.yuxming.cn/gtrprooexa.html

Ruby: arr.join(", ")
来源：http://hz.shanyushiyangkeji.top/gtyfgwrkrq.html

C#:   string.Join(", ", list)
来源：http://hz.daria6918.cn/gtkctjjqbi.html

================================================================================
来源：http://hz.svipenyu.cn/gtibcfwgze.html

E. 字符串处理
来源：http://hz.meibo888.top/gtvuwewbhv.html

================================================================================
来源：http://hz.cashguo.top/gtkdicuoox.html

[E01] 拼接字符串
来源：http://hz.shuidangran.top/gtzjgufwjn.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.ehwqpu.com/gtogmdmyqn.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.shangyingyoupin.top/gtxgeufajn.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.haohaochexian.top/gtgatjkmct.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yongpay.top/gtysakvfre.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.daxiang520.top/gtzzkzbrzf.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.tanke756.top/gthgzxixhc.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.jyoumei.cn/gtyboeelaw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.shangyingyoupin.top/gtqazheocx.html

[E02] 重复字符串
来源：http://hz.xuetiantiany.cn/gtvzdijwvw.html

Py:   "ab" * 3
来源：http://hz.guowangkeji.top/gtscpuwhww.html

PHP:  str_repeat("ab", 3);
来源：http://hz.xylfe.cn/gtlsfykqto.html

JS:   "ab".repeat(3)
来源：http://hz.xziqi.cn/gtgutynapp.html

TS:   "ab".repeat(3)
来源：http://hz.yuxming.cn/gtuweptmar.html

Java: "ab".repeat(3)
来源：http://hz.hnqzz.top/gtiemthfdp.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.birdmap.top/gtomyxstar.html

Ruby: "ab" * 3
来源：http://hz.gotoacloud.top/gtwxqhzrjf.html


<!-- 参考信息 -->