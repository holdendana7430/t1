代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://hz.dashuyun.cn/gtikrlmtny.html

C#:   using System.Text;
来源：http://hz.wangdashe.top/gtxvqsyogg.html

[C12] 立即执行函数 IIFE
来源：http://hz.0kj1m.cn/gtcqxdpogp.html

Py:   (lambda: print("run"))()
来源：http://hz.hfpthk.cn/gtnqdwptvf.html

PHP:  (function () { echo "run"; })();
来源：http://hz.sufxvd.cn/gtaotzqicu.html

JS:   (() => { console.log("run"); })();
来源：http://hz.tianlin.xyz/gtnndxjvig.html

TS:   (() => { console.log("run"); })();
来源：http://hz.jinghuilouyu.cn/gtbdoocvut.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.xuetiantiany.cn/gttzoyvumv.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.hnqzz.top/gtopkvmgew.html

Ruby: -> { puts "run" }.call
来源：http://hz.jinghuilouyu.cn/gtiaggvmod.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.dianchejie.cn/gthkpmccqn.html

[C13] 类型声明 / 类型注解
来源：http://hz.gzhubu.top/gtnemyluie.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.aibaodan.cn/gtafiinczd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.feifeiyinyue.top/gtybzdiuid.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.zhijiandao.cn/gtwglfjsfx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhixingplan.top/gtbrjamvdj.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.cdnleiting.top/gturfvqxts.html

Go:   func add(a, b int) int
来源：http://hz.birdmap.top/gtafefsqpf.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.cheryme.top/gtwerkzatc.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.zdqjudy.top/gtnolalfap.html

[C14] 泛型函数
来源：http://hz.9152youxi.cn/gtipirryuw.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.nanxuanxn.top/gtnzmxpoii.html

PHP:  // 无泛型
来源：http://hz.sxryk.cn/gtndgzanun.html

JS:   // 无泛型
来源：http://hz.hywenlv.cn/gtueussmno.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.zhengqikj.top/gtrhrbodjl.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.vqdsnc.cn/gtdthlmfle.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.chenzaomai.com/gtnubrnogw.html

Ruby: # 无泛型
来源：http://hz.nanxuanxn.top/gthjmwnpel.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.hysaishi.cn/gtlhxklhjv.html

[C15] 解构 / 展开参数
来源：http://hz.chenzaomai.com/gtxlmvnpze.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.zycfv.cn/gtljzztozr.html

PHP:  [$a, $b] = $pair;
来源：http://hz.ydjk.org.cn/gthxgulnry.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.wangshuangyany.cn/gthyrnpwvj.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.nanxuanxn.top/gtovlhlodq.html

Java: // 无解构
来源：http://hz.sysykeji.top/gtkbtvotcm.html

Go:   // 无解构
来源：http://hz.zhoulong.xyz/gtnhyykyew.html

Ruby: a, b = pair
来源：http://hz.c1oappe.top/gtrmkxojwg.html

C#:   var (a, b) = pair;
来源：http://hz.zhengqikj.top/gtmvikjohb.html

[C16] 函数 / 方法重载
来源：http://hz.yueranfly.top/gtroicaqaw.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.birdmap.top/gtisttcukk.html

PHP:  // 无重载
来源：http://hz.ybcxt.top/gtmnlbszze.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.jinyuanbaomall.cn/gtndapsaza.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.chenlongwang.top/gtajsgibmx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.sysykeji.top/gtfsryvmkk.html

Go:   // 无重载：用不同函数名
来源：http://hz.mhx1999.top/gtpvlkuffc.html

Ruby: # 无重载：靠动态参数
来源：http://hz.andypj.xyz/gtonkyhety.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.shuidangran.top/gthieidlxe.html

================================================================================
来源：http://hz.nwbrower.top/gtaphcyqlr.html

D. 数组 / 列表 / 集合
来源：http://hz.zycfv.cn/gtsoilqeti.html

================================================================================
来源：http://hz.havefunace.top/gtpwasrcuo.html

[D01] 创建数组 / 列表
来源：http://hz.iojbl.cn/gtjrvqgmvb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.tanke756.top/gtajvqkrxj.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.dianchejie.cn/gtjdpnkkns.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.yanxiufei.cn/gtuuyhtgso.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.guannengcc.top/gtihkyxweq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.hongshengwenyu.top/gtjkiutpua.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.snrcjt.cn/gtcpmzgysu.html

Ruby: arr = [1, 2, 3]
来源：http://hz.yvedp.cn/gtxjirlfjh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.pengpengdd.cyou/gtkehnwszz.html

[D02] 追加元素到末尾
来源：http://hz.pengpengdd.cyou/gtlryktcsi.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.zhiwuduotai.top/gtwbeybswy.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.redwolf501.top/gtpoquovys.html

JS:   arr.push(4);
来源：http://hz.chenjidiqi.icu/gtlflynavc.html

TS:   arr.push(4);
来源：http://hz.sweek.top/gtvgaeqoas.html

Java: list.add(4);
来源：http://hz.gaohongyu789.top/gtovinggit.html

Go:   arr = append(arr, 4)
来源：http://hz.cqqwz.cn/gtyslegzne.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.0kj1m.cn/gtfuzgygtf.html

C#:   list.Add(4);
来源：http://hz.sysykeji.top/gtdnarisqh.html

[D03] 在指定位置插入元素
来源：http://hz.kuanghao11.cn/gtguetyywe.html

Py:   arr.insert(0, 0)
来源：http://hz.jinqigufen.top/gtmcnygxvc.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.jianghu66.top/gtklgamncn.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.guowangkeji.top/gtdgounzvm.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.zhoulong.xyz/gtxtskljjq.html

Java: list.add(0, 0);
来源：http://hz.gaohongyu789.top/gtjvnpbddy.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.xuanzx.com/gtvjukztmp.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.c1oappe.top/gtkasbmsdh.html

C#:   list.Insert(0, 0);
来源：http://hz.hnxiangtu.top/gtdmalxcqh.html

[D04] 删除元素
来源：http://hz.52xcode.cn/gtkmfivuzx.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.hongshengwenyu.top/gtmktgrtcn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.shzxlz.cn/gtoljnmtqn.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.ydjk.org.cn/gtsucvgscm.html

TS:   arr.splice(0, 1);
来源：http://hz.yonumen.top/gtsnqtxirl.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.ppjwa.cn/gtlukfbyct.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.yonumen.top/gtxxezplar.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.dashuyun.cn/gtovibmknr.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.ywan-chungtsiang.top/gtwpoqaarm.html

[D05] 访问与修改元素
来源：http://hz.xziqi.cn/gtndrrkqcr.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.ehwqpu.com/gtqwwwqrfv.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.andypj.xyz/gtjpridqlh.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.shanyushiyangtech.top/gtrtqdtbey.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.ybcxt.top/gtmfjijtcb.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.xingfuxueyuan.xyz/gtelawqmnr.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.shangyingyoupin.top/gtolgebgei.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.cqqwz.cn/gtiwchtozl.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.gaohongyu789.top/gtghwbhcdk.html

[D06] 数组长度
来源：http://hz.yueranfly.top/gtlrftyhik.html

Py:   len(arr)
来源：http://hz.xinyue.icu/gtovtajgoc.html

PHP:  count($arr);
来源：http://hz.nanxinkj.top/gtsnokatxq.html

JS:   arr.length
来源：http://hz.hammf.cn/gtzutfuptx.html

TS:   arr.length
来源：http://hz.fzhhl.top/gtmfhprqli.html

Java: list.size();
来源：http://hz.hnxiangtu.top/gtloimscnw.html

Go:   len(arr)
来源：http://hz.vqdsnc.cn/gtresvykfd.html

Ruby: arr.length; arr.size
来源：http://hz.cqqwz.cn/gtfmjksuov.html

C#:   list.Count;
来源：http://hz.ybcxt.top/gtdgptucix.html

[D07] 切片 / 取子数组
来源：http://hz.yangfankeji.com/gtrpgvxnep.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.chenlongwang.top/gtsaicvikt.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.fzhhl.top/gttmhoxxdy.html

JS:   arr.slice(1, 4);
来源：http://hz.daxiang520.top/gtgmedupxr.html

TS:   arr.slice(1, 4);
来源：http://hz.fengsongda.top/gtbtpuqolo.html

Java: list.subList(1, 4);
来源：http://hz.yuxming.cn/gtoybkmoab.html

Go:   arr[1:4]
来源：http://hz.yongpay.top/gtcddhxbgx.html

Ruby: arr[1, 3]
来源：http://hz.xuanzx.com/gtobdwzrdx.html

C#:   list.GetRange(1, 3);
来源：http://hz.shzxlz.cn/gthkgrgody.html

[D08] 合并两个数组
来源：http://hz.hongshengwenyu.top/gtynzehebu.html

Py:   a + b;  a.extend(b)
来源：http://hz.52xcode.cn/gtbsdzpghj.html

PHP:  array_merge($a, $b);
来源：http://hz.xziqi.cn/gthxgshwmg.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.yongpay.top/gtpbtypsfv.html

TS:   [...a, ...b];
来源：http://hz.chenzaomai.com/gtpzmcxpps.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.yanxiufei.cn/gtpptdlsoc.html

Go:   append(a, b...)
来源：http://hz.gzhubu.top/gtnvqshiih.html

Ruby: a + b;  a.concat(b)
来源：http://hz.jinqigufen.top/gtqqtjyrru.html

C#:   a.Concat(b).ToList()
来源：http://hz.svipenyu.cn/gtjxqonmiv.html

[D09] 排序（升序）
来源：http://hz.nanxinkj.top/gtrbrstomm.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.xinyue.icu/gtxufnyhjc.html

PHP:  sort($arr);
来源：http://hz.yj20258888.top/gtcvogukvr.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.jinqigfzy.top/gtmtzvyepk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.sweek.top/gtkqndsqsb.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.shanyushiyangtech.top/gtyvieacpp.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.snrcjt.cn/gtyfoxychm.html

Ruby: arr.sort
来源：http://hz.daxiang520.top/gtqtqrvakc.html

C#:   list.Sort();
来源：http://hz.hnqzz.top/gtxsafhuix.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.cashguo.top/gtpmhkjivx.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.ydzc1.top/gtldgwohli.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.chenlongwang.top/gtrqkxbanz.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zhiwuduotai.top/gtlqlqsdin.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xylfe.cn/gtgkjqsflm.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.dashuyun.cn/gtjqtcthnm.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.meibo888.top/gtygyjzlzz.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.jinghuilouyu.cn/gtbewimbnl.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.kuanghao11.cn/gtudzflieu.html

[D11] 反转数组
来源：http://hz.aizwys.cn/gtcwazzpuw.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.sufxvd.cn/gtrckiwpsp.html

PHP:  array_reverse($arr);
来源：http://hz.xingfuxueyuan.xyz/gteqcyzpzj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.hnxiangtu.top/gtpllaswcf.html

TS:   [...arr].reverse();
来源：http://hz.aibaodan.cn/gtixzkfxmv.html

Java: Collections.reverse(list);
来源：http://hz.shzxlz.cn/gtqbykfzss.html

Go:   slices.Reverse(arr)
来源：http://hz.quarkkingdee.top/gtosncoasm.html

Ruby: arr.reverse
来源：http://hz.daria6918.cn/gtppknpqyt.html

C#:   list.Reverse();
来源：http://hz.xinyue.icu/gtxonzdfma.html

[D12] 查找元素下标
来源：http://hz.zhijiandao.cn/gtxfslgugt.html

Py:   arr.index(x);  x in arr
来源：http://hz.meibo888.top/gtlmeaxggy.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.9152youxi.cn/gtfbkkhraj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yueranfly.top/gtmhwyiula.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yj20258.top/gtliuduyjj.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.xuanzx.com/gtighjawxo.html

Go:   slices.Index(arr, x)
来源：http://hz.gotoacloud.top/gtvvcunrzq.html

Ruby: arr.index(x)
来源：http://hz.jiagoushi.top/gtszgkaprb.html

C#:   list.IndexOf(x);
来源：http://hz.snrcjt.cn/gtmzadzbbr.html

[D13] 过滤（保留满足条件的）
来源：http://hz.pycfn.com/gtvdkhbnrc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.yueranfly.top/gtqbzdtoli.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.hfpthk.cn/gtfaywizbj.html

JS:   arr.filter(x => x > 3)
来源：http://hz.hnqzz.top/gtsqlnyqyq.html

TS:   arr.filter(x => x > 3)
来源：http://hz.hysaishi.cn/gtptzdvfbl.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.nwbrower.top/gtokjfzoqb.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.sysykeji.top/gtbnvayjic.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.sweek.top/gtyhyrfrxh.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.wangdashe.top/gtsppbbeye.html

[D14] 映射转换（每个元素变形）
来源：http://hz.cqqwz.cn/gtnvlobozb.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.tian-w.cn/gtyicjcgrf.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.hywenlv.cn/gtfospposm.html

JS:   arr.map(x => x * 2)
来源：http://hz.wangdashe.top/gtfsztebow.html

TS:   arr.map(x => x * 2)
来源：http://hz.jyoumei.cn/gtwhkwxfck.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.ivvv.top/gtkahqfvom.html

Go:   // 手写循环
来源：http://hz.vqdsnc.cn/gtynujbplh.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.xylfe.cn/gtcqauylwh.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.nanxinkj.top/gtpzhxzajg.html

[D15] 去重
来源：http://hz.gogol.net.cn/gtcjfonkkx.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.zhongyouzk.top/gtnrpffrus.html

PHP:  array_unique($arr);
来源：http://hz.gaohongyu789.top/gtffndcmku.html

JS:   [...new Set(arr)]
来源：http://hz.aizwys.cn/gtrjaixihl.html

TS:   [...new Set(arr)]
来源：http://hz.meibo888.top/gtroflhxol.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.gzhubu.top/gtomepxvfe.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.jinghuilouyu.cn/gtihthbuuq.html

Ruby: arr.uniq
来源：http://hz.yj20258.top/gtshamyzjj.html

C#:   list.Distinct().ToList()
来源：http://hz.xziqi.cn/gtijwmyivw.html

[D16] 求和与平均值
来源：http://hz.yuxming.cn/gtfyhyzngr.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.wangshuangyany.cn/gtmqrinvap.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.aizwys.cn/gtwqtkwefo.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.smart0.xyz/gtjjtxcjtt.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.0kj1m.cn/gtdbbpuiot.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.tianlin.xyz/gtbtzlvnjn.html

Go:   // 手写循环累加
来源：http://hz.jinghuilouyu.cn/gtlvbfjwvu.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.zhongyouzk.top/gtrbcwcwjf.html

C#:   list.Sum();  list.Average()
来源：http://hz.havefunace.top/gtqqmejhaz.html

[D17] 最大值与最小值
来源：http://hz.pengpengdd.cyou/gtuyqrrqgo.html

Py:   max(arr);  min(arr)
来源：http://hz.redwolf501.top/gtvnumvyty.html

PHP:  max($arr);  min($arr);
来源：http://hz.hysaishi.cn/gtlwkpmwtq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.zhaomingkeji.xyz/gtjuzsaexc.html

TS:   Math.max(...arr);
来源：http://hz.fzhhl.top/gtaktcelhm.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.chenlongwang.top/gtjdnotjsp.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.daria6918.cn/gtfeilazxo.html

Ruby: arr.max;  arr.min
来源：http://hz.316326.xyz/gtujcopxzl.html

C#:   list.Max();  list.Min()
来源：http://hz.sxryk.cn/gtdyqnjiaf.html

[D18] 扁平化嵌套数组
来源：http://hz.daria6918.cn/gtdphslhgp.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.shanyushiyangkeji.top/gthrsyvklc.html

PHP:  array_merge(...$nested);
来源：http://hz.daria6918.cn/gtmmddzzrg.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.havefunace.top/gtyyrqyuuv.html

TS:   nested.flat();
来源：http://hz.jianghu66.top/gtstpbqffp.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.yj20258888.top/gtmhobsbyv.html

Go:   // 手写双层循环
来源：http://hz.jyoumei.cn/gtqigubaln.html

Ruby: nested.flatten
来源：http://hz.aizwys.cn/gtuuuucbbe.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.yj20258.top/gtwhxpmtiz.html

[D19] 按字段分组
来源：http://hz.jyoumei.cn/gtphjjupho.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.smart0.xyz/gtrrrykeph.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.shanyushiyangtech.top/gtuwrtmyvo.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.nanxinkj.top/gtaukccnmk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.vqdsnc.cn/gtotegpuec.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.havefunace.top/gtyuqnjvdy.html

Go:   // 手写 map[string][]T
来源：http://hz.sufxvd.cn/gtegewizue.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.ivvv.top/gtfzkhrzpi.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.yuxming.cn/gtvuxuffut.html

[D20] 统计每个元素出现次数
来源：http://hz.zhixingplan.top/gtazjrbntq.html

Py:   Counter(arr)
来源：http://hz.zhoulong.xyz/gtofcdehpr.html

PHP:  array_count_values($arr);
来源：http://hz.andypj.xyz/gthkhmqkil.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.sufxvd.cn/gtypbigfnh.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zhengqikj.top/gtmclvnvyu.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.nwbrower.top/gtdzrqtldz.html

Go:   // 手写 map[T]int
来源：http://hz.yangfankeji.com/gtvnsxyytc.html

Ruby: arr.tally
来源：http://hz.jinghuilouyu.cn/gtywaeqnme.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.ppjwa.cn/gthkzgffpg.html

[D21] 判断是否包含某元素
来源：http://hz.yj202588.top/gtdkgilzqf.html

Py:   x in arr
来源：http://hz.yongpay.top/gtlkepfuyy.html

PHP:  in_array($x, $arr, true);
来源：http://hz.birdmap.top/gtwjczycfh.html

JS:   arr.includes(x)
来源：http://hz.fengsongda.top/gttspsdero.html

TS:   arr.includes(x)
来源：http://hz.sufxvd.cn/gtdsfoceid.html

Java: list.contains(x)
来源：http://hz.havefunace.top/gtwhiwvqxk.html

Go:   slices.Contains(arr, x)
来源：http://hz.pycfn.com/gtvpmaaxed.html

Ruby: arr.include?(x)
来源：http://hz.guowangkeji.top/gtmkvezsbp.html

C#:   list.Contains(x)
来源：http://hz.svipenyu.cn/gtqvrchefx.html

[D22] 复制数组（避免共享引用）
来源：http://hz.sysykeji.top/gtlfduzscw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.nanxinkj.top/gtwfbndkps.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.jiagoushi.top/gtyyqpjjzl.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.jiagoushi.top/gtxjpbyfcz.html

TS:   [...arr];
来源：http://hz.jyoumei.cn/gtkexwlhze.html

Java: new ArrayList<>(list);
来源：http://hz.xingfuxueyuan.xyz/gtxfsaauts.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.haohaochexian.top/gtadkffrcw.html

Ruby: arr.dup;  arr.clone
来源：http://hz.sweek.top/gtxjzxrtuk.html

C#:   new List<int>(list);
来源：http://hz.birdmap.top/gteejkzkav.html

[D23] reduce 累积计算
来源：http://hz.zhongyouzk.top/gtnzmoynex.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.sysykeji.top/gtmcsmtnsg.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.pengpengdd.cyou/gtvcfzsizo.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ppjwa.cn/gtkdtwjkbg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.sufxvd.cn/gtuuofwpqh.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.daria6918.cn/gtoqmaplvl.html

Go:   // 手写循环
来源：http://hz.sweek.top/gtvupswkhs.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.cashguo.top/gtcyzcecbc.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.ydzc1.top/gtqlawvjuy.html

[D24] 字典 / Map 基本操作
来源：http://hz.ehwqpu.com/gtknjyjrau.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.cucudq.cn/gtgyvfdmfx.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.ehwqpu.com/gtvecmbqta.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.yuanzhike.top/gtlmijhhgj.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.wangdashe.top/gtnrrcsayq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.ppjwa.cn/gttbxdbcrt.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.c1oappe.top/gtahseycwb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.jinghuilouyu.cn/gtdjptzllk.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.xingfuxueyuan.xyz/gtmndrzoao.html

[D25] Set 集合去重与交并差
来源：http://hz.daxiang520.top/gtdickgrjg.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.ydjk.org.cn/gtvhmasfnu.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.mhx1999.top/gthyinxqwj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.hfpthk.cn/gttnphqzhg.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.hongshengwenyu.top/gtifhrvgpo.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.zhiwuduotai.top/gturxljeje.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.quarkkingdee.top/gtaevguqvo.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.yangfankeji.com/gtkezyqjmb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.yj20258888.top/gtzqrzmxln.html

[D26] 数组转字符串
来源：http://hz.9152youxi.cn/gtmgvxiwjc.html

Py:   ", ".join(map(str, arr))
来源：http://hz.shanyushiyangtech.top/gtvxtfqeik.html

PHP:  implode(", ", $arr);
来源：http://hz.xylfe.cn/gtghbttkki.html

JS:   arr.join(", ")
来源：http://hz.jinyuanbaomall.cn/gtrdecetwm.html

TS:   arr.join(", ")
来源：http://hz.vqdsnc.cn/gtswgvgmvm.html

Java: String.join(", ", list)
来源：http://hz.nwbrower.top/gtalpbrvot.html

Go:   strings.Join(strs, ", ")
来源：http://hz.zhongyouzk.top/gtiktxydpr.html

Ruby: arr.join(", ")
来源：http://hz.ppjwa.cn/gtmaigzcag.html

C#:   string.Join(", ", list)
来源：http://hz.havefunace.top/gtionjshnt.html

================================================================================
来源：http://hz.cucudq.cn/gtbarsdrcp.html

E. 字符串处理
来源：http://hz.hnqzz.top/gtidusqnto.html

================================================================================
来源：http://hz.chenzaomai.com/gtkzbaxhwf.html

[E01] 拼接字符串
来源：http://hz.jqgufenzy.top/gtjqduekiu.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.daria6918.cn/gtfmytocrk.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.ybcxt.top/gtlqrvnevs.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.daria6918.cn/gtscypmyag.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.shzxlz.cn/gtcezshlmj.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.sufxvd.cn/gtnkarefxn.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.yanxiufei.cn/gtmmswabww.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.aizwys.cn/gtrdmszgth.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.xziqi.cn/gtvapzqorp.html

[E02] 重复字符串
来源：http://hz.hfpthk.cn/gtnebpnhul.html

Py:   "ab" * 3
来源：http://hz.zhijiandao.cn/gtfsarjosg.html

PHP:  str_repeat("ab", 3);
来源：http://hz.guannengcc.top/gtqheglung.html

JS:   "ab".repeat(3)
来源：http://hz.bjfxy.top/gthtrqmesu.html


<!-- 参考信息 -->