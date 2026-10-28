代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://hz.shanyushiyangtech.top/gttvgktvbj.html

Ruby: -> { puts "run" }.call
来源：http://hz.cqqwz.cn/gtybxksxse.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.yuxming.cn/gtgdpivbgl.html

[C13] 类型声明 / 类型注解
来源：http://hz.nanxinkj.top/gtjzmvtsof.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.jlsjyb.cn/gtrbriehne.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jqgfzy.top/gthuxnlncz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.tian-w.cn/gtifdqlxjj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.iojbl.cn/gthwlaeetm.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.zhongyouzk.top/gtsilmjnmp.html

Go:   func add(a, b int) int
来源：http://hz.sweek.top/gtiqwehrbl.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.chenlongwang.top/gtqpjrfrls.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.yueranfly.top/gtlnshtlmv.html

[C14] 泛型函数
来源：http://hz.316326.xyz/gtxzuexjut.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.birdmap.top/gtnrarqlgk.html

PHP:  // 无泛型
来源：http://hz.dashuyun.cn/gthcbwvsqp.html

JS:   // 无泛型
来源：http://hz.sweek.top/gtqhigyhbm.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.yj20258.top/gtteqkbzeo.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.jinqigufen.top/gtzinjnazf.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.zhongyouzk.top/gtrhmeisso.html

Ruby: # 无泛型
来源：http://hz.fzhhl.top/gtmsyyhzou.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.vqdsnc.cn/gtkdwpjjlr.html

[C15] 解构 / 展开参数
来源：http://hz.wangdashe.top/gtpqcimeen.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.zhijiandao.cn/gtublpguse.html

PHP:  [$a, $b] = $pair;
来源：http://hz.hongshengwenyu.top/gtvefaiyjo.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.yuanzhike.top/gtwdrwtyzl.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.gogol.net.cn/gtgbataqoh.html

Java: // 无解构
来源：http://hz.chenlongwang.top/gtetgiagwz.html

Go:   // 无解构
来源：http://hz.yj202588.top/gtswceapuy.html

Ruby: a, b = pair
来源：http://hz.tianlin.xyz/gtumhrnasw.html

C#:   var (a, b) = pair;
来源：http://hz.daria6918.cn/gtkblcpzyb.html

[C16] 函数 / 方法重载
来源：http://hz.cheryme.top/gtrckhszwe.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.guowangkeji.top/gtsduxqoct.html

PHP:  // 无重载
来源：http://hz.bjfxy.top/gtfrvuskkq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.ivvv.top/gtmgmtymrv.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.redwolf501.top/gtcjvkmksm.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.yanxiufei.cn/gtswiluaej.html

Go:   // 无重载：用不同函数名
来源：http://hz.shanyushiyangkeji.top/gthjxggsjn.html

Ruby: # 无重载：靠动态参数
来源：http://hz.hysaishi.cn/gtpkjmjelk.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.gogol.net.cn/gtjamtwabi.html

================================================================================
来源：http://hz.xylfe.cn/gtfnkuhuax.html

D. 数组 / 列表 / 集合
来源：http://hz.shangyingyoupin.top/gtdymknqhm.html

================================================================================
来源：http://hz.aizwys.cn/gtvipnhqrt.html

[D01] 创建数组 / 列表
来源：http://hz.yj20258888.top/gtsonxurbv.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.hammf.cn/gtykejbown.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.hongshengwenyu.top/gthicdqxgh.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.hnxiangtu.top/gtdoqpghrv.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.jlsjyb.cn/gtxxaetqnf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.xingfuxueyuan.xyz/gtxtslfihm.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.sxryk.cn/gtamghqgps.html

Ruby: arr = [1, 2, 3]
来源：http://hz.cdnleiting.top/gtxvkjinid.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.hammf.cn/gtflbnptbz.html

[D02] 追加元素到末尾
来源：http://hz.iojbl.cn/gtymugpimz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.9152youxi.cn/gtpqopyyxz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.zhaomingkeji.xyz/gtfyfoqafw.html

JS:   arr.push(4);
来源：http://hz.daria6918.cn/gtdxhqczcb.html

TS:   arr.push(4);
来源：http://hz.guowangkeji.top/gttjahtgjr.html

Java: list.add(4);
来源：http://hz.tian-w.cn/gttytsbfrz.html

Go:   arr = append(arr, 4)
来源：http://hz.aibaodan.cn/gtofpoeumb.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.nwbrower.top/gtszlgkwek.html

C#:   list.Add(4);
来源：http://hz.sweek.top/gtnhyztyrk.html

[D03] 在指定位置插入元素
来源：http://hz.nanxinkj.top/gtmdfmfcpz.html

Py:   arr.insert(0, 0)
来源：http://hz.feifeiyinyue.top/gtibxokotd.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.chenjidiqi.icu/gtzzzcvwfx.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.svipenyu.cn/gttwmrhjzv.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.xinyue.icu/gtgbrnyldn.html

Java: list.add(0, 0);
来源：http://hz.chenlongwang.top/gtunnhbzid.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.redwolf501.top/gtaejaxlfm.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.kuanghao11.cn/gtvzauumtp.html

C#:   list.Insert(0, 0);
来源：http://hz.0kj1m.cn/gtkhplsfkb.html

[D04] 删除元素
来源：http://hz.bjfxy.top/gtrznajezp.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.yuanzhike.top/gtrkqbpisi.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.jlsjyb.cn/gtvlxoiddq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.hfpthk.cn/gtxnohlfvw.html

TS:   arr.splice(0, 1);
来源：http://hz.smart0.xyz/gtokldncxv.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.shanyushiyangtech.top/gtqxzynqnq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.yongpay.top/gtixnpbcrh.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.yuxming.cn/gtqxkpakun.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.hywenlv.cn/gtkaghtovp.html

[D05] 访问与修改元素
来源：http://hz.zhixingplan.top/gtjndwyxah.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.tianlin.xyz/gtbihctdwo.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.cdnleiting.top/gtcowsjije.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.jqgfzy.top/gtcoxttrcr.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.xziqi.cn/gtxzbuktuc.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.zhongyouzk.top/gtvfbngfcl.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.zhiwuduotai.top/gtbpxgguxk.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.haohaochexian.top/gtvnwjepfg.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.gzhubu.top/gtgdoxnvqu.html

[D06] 数组长度
来源：http://hz.ydzc1.top/gtatdubriw.html

Py:   len(arr)
来源：http://hz.yanxiufei.cn/gtmceaijct.html

PHP:  count($arr);
来源：http://hz.jqgufenzy.top/gtppipqvgk.html

JS:   arr.length
来源：http://hz.cdnleiting.top/gtgmpeovzf.html

TS:   arr.length
来源：http://hz.yj202588.top/gtgrdcxmoi.html

Java: list.size();
来源：http://hz.jiagoushi.top/gtphswzljy.html

Go:   len(arr)
来源：http://hz.yanxiufei.cn/gtqohpghok.html

Ruby: arr.length; arr.size
来源：http://hz.sysykeji.top/gtdtianeph.html

C#:   list.Count;
来源：http://hz.hongshengwenyu.top/gtzkckzfda.html

[D07] 切片 / 取子数组
来源：http://hz.jinghuilouyu.cn/gtawrcmgid.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.jinqigfzy.top/gthycbeogh.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.gaohongyu789.top/gtaxsenven.html

JS:   arr.slice(1, 4);
来源：http://hz.fengsongda.top/gthkjcgdql.html

TS:   arr.slice(1, 4);
来源：http://hz.ywan-chungtsiang.top/gticfxcmgy.html

Java: list.subList(1, 4);
来源：http://hz.wangshuangyany.cn/gtzpujnyqt.html

Go:   arr[1:4]
来源：http://hz.cucudq.cn/gtwejycxvv.html

Ruby: arr[1, 3]
来源：http://hz.0kj1m.cn/gtawnkwkhr.html

C#:   list.GetRange(1, 3);
来源：http://hz.bjfxy.top/gtfvwdzpcu.html

[D08] 合并两个数组
来源：http://hz.ppjwa.cn/gtcpokrxum.html

Py:   a + b;  a.extend(b)
来源：http://hz.birdmap.top/gtvanwxwxv.html

PHP:  array_merge($a, $b);
来源：http://hz.xziqi.cn/gtxpoaopja.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.nanxinkj.top/gthylnlcbt.html

TS:   [...a, ...b];
来源：http://hz.ywan-chungtsiang.top/gtkjqafcau.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.havefunace.top/gtzkuorafg.html

Go:   append(a, b...)
来源：http://hz.xuanzx.com/gtqfcevrlm.html

Ruby: a + b;  a.concat(b)
来源：http://hz.jinyuanbaomall.cn/gtytdrrdjh.html

C#:   a.Concat(b).ToList()
来源：http://hz.shangyingyoupin.top/gtzsededpq.html

[D09] 排序（升序）
来源：http://hz.ydjk.org.cn/gtfzgsjstk.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.cashguo.top/gtqvwyiqvc.html

PHP:  sort($arr);
来源：http://hz.jyoumei.cn/gtslrhaqbk.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.zhiwuduotai.top/gtgjnnmnzv.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.hywenlv.cn/gttmeaeqws.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.chenjidiqi.icu/gtbkmeqmzt.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.fzhhl.top/gtuxriqtzl.html

Ruby: arr.sort
来源：http://hz.jqgfzy.top/gtifsjxnfw.html

C#:   list.Sort();
来源：http://hz.mhx1999.top/gtbxqwfdsi.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.sxryk.cn/gtviccefkk.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.bjfxy.top/gtwjjjzqpa.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zhengqikj.top/gtdacbzfot.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xziqi.cn/gtxadgqlya.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.nanxuanxn.top/gtgoquuyoi.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.guannengcc.top/gtfgmhqbxv.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.gzhubu.top/gtkefpxezf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.hysaishi.cn/gtzrobkryx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.yj20258888.top/gtidiziyjx.html

[D11] 反转数组
来源：http://hz.nanxuanxn.top/gtmfejvmma.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.ywan-chungtsiang.top/gtxrornpqk.html

PHP:  array_reverse($arr);
来源：http://hz.sweek.top/gtbehgwrba.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.zhoulong.xyz/gtrojydakc.html

TS:   [...arr].reverse();
来源：http://hz.zycfv.cn/gtufkrtxdn.html

Java: Collections.reverse(list);
来源：http://hz.yvedp.cn/gtllhuzdjt.html

Go:   slices.Reverse(arr)
来源：http://hz.pengpengdd.cyou/gtjqxqppqh.html

Ruby: arr.reverse
来源：http://hz.andypj.xyz/gtefptwapl.html

C#:   list.Reverse();
来源：http://hz.jinqigfzy.top/gtqomtxzll.html

[D12] 查找元素下标
来源：http://hz.feifeiyinyue.top/gtanvxntue.html

Py:   arr.index(x);  x in arr
来源：http://hz.chenjidiqi.icu/gttabmzfwe.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.ydjk.org.cn/gtgbktcesb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zdqjudy.top/gtxngdnden.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.havefunace.top/gtubdhlqdn.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.0kj1m.cn/gtalgtarej.html

Go:   slices.Index(arr, x)
来源：http://hz.bjfxy.top/gtvzaulvjm.html

Ruby: arr.index(x)
来源：http://hz.cqqwz.cn/gtzlzmkpxg.html

C#:   list.IndexOf(x);
来源：http://hz.birdmap.top/gtiqfyszmx.html

[D13] 过滤（保留满足条件的）
来源：http://hz.shuidangran.top/gtdzcutnkr.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.xuanzx.com/gtbgkirqpk.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.jinghuilouyu.cn/gtfpqamsyf.html

JS:   arr.filter(x => x > 3)
来源：http://hz.yanxiufei.cn/gtgejrhltt.html

TS:   arr.filter(x => x > 3)
来源：http://hz.shanyushiyangkeji.top/gtjyxyryet.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.dianchejie.cn/gtkmsnthsn.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.jqgufenzy.top/gtspibrird.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.vqdsnc.cn/gtndoziquk.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.yj202588.top/gtokgdqjfu.html

[D14] 映射转换（每个元素变形）
来源：http://hz.tian-w.cn/gtzospspaw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.jqgufenzy.top/gtgpvqlzqa.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.sxryk.cn/gtmqerxguh.html

JS:   arr.map(x => x * 2)
来源：http://hz.zhoulong.xyz/gtzmbzruqr.html

TS:   arr.map(x => x * 2)
来源：http://hz.aibaodan.cn/gtzjdxksqf.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.cheryme.top/gtbrqzupzd.html

Go:   // 手写循环
来源：http://hz.xuetiantiany.cn/gtsvukdhvi.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.yangfankeji.com/gtytnfmuhv.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.pengpengdd.cyou/gtugqocszq.html

[D15] 去重
来源：http://hz.wangdashe.top/gtsxtmsrvr.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.yj20258.top/gtvjttnpbp.html

PHP:  array_unique($arr);
来源：http://hz.sufxvd.cn/gthpkzysns.html

JS:   [...new Set(arr)]
来源：http://hz.zhijiandao.cn/gtveouedxz.html

TS:   [...new Set(arr)]
来源：http://hz.daria6918.cn/gtwzppdpwj.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.jyoumei.cn/gthzfwekds.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.iojbl.cn/gtrrdimcda.html

Ruby: arr.uniq
来源：http://hz.xingfuxueyuan.xyz/gtbmqmfmep.html

C#:   list.Distinct().ToList()
来源：http://hz.yuanzhike.top/gtrvuafptj.html

[D16] 求和与平均值
来源：http://hz.daxiang520.top/gtjdkylmss.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.sufxvd.cn/gtfeblnhba.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.mhx1999.top/gtlvbiluiy.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.aibaodan.cn/gtaaqorzsc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.shzxlz.cn/gttbelotwh.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.sysykeji.top/gtyjlavdsl.html

Go:   // 手写循环累加
来源：http://hz.andypj.xyz/gtmnihbtyn.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.jianghu66.top/gtiybhjfds.html

C#:   list.Sum();  list.Average()
来源：http://hz.yuanzhike.top/gttaqbmbis.html

[D17] 最大值与最小值
来源：http://hz.kuanghao11.cn/gtqfudioyf.html

Py:   max(arr);  min(arr)
来源：http://hz.fzhhl.top/gthhrdbwwc.html

PHP:  max($arr);  min($arr);
来源：http://hz.cqqwz.cn/gtddgwbszf.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.zhixingplan.top/gtgxpvewcv.html

TS:   Math.max(...arr);
来源：http://hz.chenjidiqi.icu/gtsyvgejmy.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.jinqigfzy.top/gtkizpdbiy.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.zhongyouzk.top/gthognzoko.html

Ruby: arr.max;  arr.min
来源：http://hz.shzxlz.cn/gtnjikgzgw.html

C#:   list.Max();  list.Min()
来源：http://hz.zycfv.cn/gtjufcvwta.html

[D18] 扁平化嵌套数组
来源：http://hz.shanyushiyangkeji.top/gtrzuhkltt.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.zhongyouzk.top/gtxzugrqxw.html

PHP:  array_merge(...$nested);
来源：http://hz.zdqjudy.top/gtkiljilnp.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.ehwqpu.com/gtdwehhfql.html

TS:   nested.flat();
来源：http://hz.chenzaomai.com/gtkunbatmj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.wangdashe.top/gtenafxtxg.html

Go:   // 手写双层循环
来源：http://hz.hammf.cn/gtdblvdowg.html

Ruby: nested.flatten
来源：http://hz.xuetiantiany.cn/gtsyoefonl.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.gotoacloud.top/gtjvlxsdls.html

[D19] 按字段分组
来源：http://hz.yonumen.top/gthdzuglvm.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.yangfankeji.com/gtpqtihutg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.wangdashe.top/gtjedobfea.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.yonumen.top/gtvohdhkbf.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.sxryk.cn/gtinsnlzlm.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.shzxlz.cn/gtcfvzdcrz.html

Go:   // 手写 map[string][]T
来源：http://hz.nanxuanxn.top/gteqgyirra.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.cdnleiting.top/gtakevwkiy.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.meibo888.top/gtkwziaaoj.html

[D20] 统计每个元素出现次数
来源：http://hz.yj202588.top/gtydpeectb.html

Py:   Counter(arr)
来源：http://hz.guannengcc.top/gtvwkqwjsh.html

PHP:  array_count_values($arr);
来源：http://hz.daxiang520.top/gttzrlbaax.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.shanyushiyangkeji.top/gtpscfvoge.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.shanyushiyangkeji.top/gtcsxcxnkj.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.iojbl.cn/gtukdfjhvj.html

Go:   // 手写 map[T]int
来源：http://hz.sysykeji.top/gthfglvelk.html

Ruby: arr.tally
来源：http://hz.yueranfly.top/gtxzqekikv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.sxryk.cn/gtmsiowggy.html

[D21] 判断是否包含某元素
来源：http://hz.chenjidiqi.icu/gtchiptfwr.html

Py:   x in arr
来源：http://hz.fengsongda.top/gtoghdpesl.html

PHP:  in_array($x, $arr, true);
来源：http://hz.cheryme.top/gtafbcfdkh.html

JS:   arr.includes(x)
来源：http://hz.shanyushiyangkeji.top/gtneiitxbr.html

TS:   arr.includes(x)
来源：http://hz.ydzc1.top/gtqkhpwfbb.html

Java: list.contains(x)
来源：http://hz.ehwqpu.com/gttiprfser.html

Go:   slices.Contains(arr, x)
来源：http://hz.aibaodan.cn/gtrigpfjdq.html

Ruby: arr.include?(x)
来源：http://hz.yongpay.top/gtxfuskyis.html

C#:   list.Contains(x)
来源：http://hz.cqqwz.cn/gtgjyeuvkp.html

[D22] 复制数组（避免共享引用）
来源：http://hz.jyoumei.cn/gtjetzmtha.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.jyoumei.cn/gtcwtritfs.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.xziqi.cn/gtywdxusiw.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.hysaishi.cn/gtbvmrlyjz.html

TS:   [...arr];
来源：http://hz.jlsjyb.cn/gtpsqutzif.html

Java: new ArrayList<>(list);
来源：http://hz.smart0.xyz/gtnsfuuyqw.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.xuetiantiany.cn/gtqbgiaydv.html

Ruby: arr.dup;  arr.clone
来源：http://hz.sxryk.cn/gtgvgebnzv.html

C#:   new List<int>(list);
来源：http://hz.hfpthk.cn/gtjwesrycw.html

[D23] reduce 累积计算
来源：http://hz.xziqi.cn/gtxpxvsdyv.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.jinyuanbaomall.cn/gtedvsaywd.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.guannengcc.top/gtcndlojus.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.pycfn.com/gteiswtdpq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ppjwa.cn/gtvyljmyac.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.0kj1m.cn/gtgohfpyvy.html

Go:   // 手写循环
来源：http://hz.ehwqpu.com/gtxetyqvye.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.zhaomingkeji.xyz/gtdmffznbf.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.fengsongda.top/gtkxtjjnye.html

[D24] 字典 / Map 基本操作
来源：http://hz.jianghu66.top/gtygwxvzfo.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.zycfv.cn/gtggesqopu.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.shanyushiyangtech.top/gtxlpornxw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.cheryme.top/gtonjdishj.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.0kj1m.cn/gthfazjxtx.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.xylfe.cn/gtdnduybbr.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.cheryme.top/gttuejmvff.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.chenjidiqi.icu/gtffcogomm.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.zhixingplan.top/gtbrkpwtue.html

[D25] Set 集合去重与交并差
来源：http://hz.jinghuilouyu.cn/gtypapcvzk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.quarkkingdee.top/gtpmqpyjqr.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.jlsjyb.cn/gtysxgcbml.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.jinyuanbaomall.cn/gttbuhdhzq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.yueranfly.top/gtuztfvxof.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.gzhubu.top/gtiuthtimc.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.nanxinkj.top/gtfzczuarv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.52xcode.cn/gtkpaxlsti.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.birdmap.top/gtnyvntngq.html

[D26] 数组转字符串
来源：http://hz.sweek.top/gthttkefcd.html

Py:   ", ".join(map(str, arr))
来源：http://hz.tanke756.top/gthuylogie.html

PHP:  implode(", ", $arr);
来源：http://hz.jianghu66.top/gtwuslmkpo.html

JS:   arr.join(", ")
来源：http://hz.9152youxi.cn/gtatyrforb.html

TS:   arr.join(", ")
来源：http://hz.xinyue.icu/gtwndcvvbp.html

Java: String.join(", ", list)
来源：http://hz.c1oappe.top/gtldxawfkq.html

Go:   strings.Join(strs, ", ")
来源：http://hz.fengsongda.top/gtrzznkvwq.html

Ruby: arr.join(", ")
来源：http://hz.jqgufenzy.top/gtwnftvcqb.html

C#:   string.Join(", ", list)
来源：http://hz.gzhubu.top/gtahmwndwm.html

================================================================================
来源：http://hz.bjfxy.top/gtavflozas.html

E. 字符串处理
来源：http://hz.nwbrower.top/gtumpkuuyw.html

================================================================================
来源：http://hz.vqdsnc.cn/gtbjqwnzlk.html

[E01] 拼接字符串
来源：http://hz.daria6918.cn/gtetqkpepx.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.dianchejie.cn/gtcnwvhxyl.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.zycfv.cn/gtpbomqhdg.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.vqdsnc.cn/gtdeqmvwrk.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.xziqi.cn/gtpjshjxdp.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.shanyushiyangkeji.top/gtjkfhqjgy.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.daria6918.cn/gtqmctocfv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.hnqzz.top/gtjmyemtsq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.jinqigufen.top/gtrqxmwrle.html

[E02] 重复字符串
来源：http://hz.jqgfzy.top/gtcwwivbun.html

Py:   "ab" * 3
来源：http://hz.jianghu66.top/gtazepzyco.html

PHP:  str_repeat("ab", 3);
来源：http://hz.aizwys.cn/gthumfqsjg.html

JS:   "ab".repeat(3)
来源：http://hz.aibaodan.cn/gtvxfwaxxr.html

TS:   "ab".repeat(3)
来源：http://hz.vqdsnc.cn/gtzogawsxp.html

Java: "ab".repeat(3)
来源：http://hz.yueranfly.top/gtdbegnqbh.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.bjfxy.top/gtvjjbwlmd.html

Ruby: "ab" * 3
来源：http://hz.ivvv.top/gtesiifskv.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.xuetiantiany.cn/gtjrjjemwf.html

[E03] 截取子串
来源：http://hz.pycfn.com/gtvnnveyit.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.c1oappe.top/gtnxryyhli.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.bjfxy.top/gtitbqwyrc.html


<!-- 参考信息 -->