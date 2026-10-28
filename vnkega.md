代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://hz.zdqjudy.top/gtghjixffb.html

C#:   using System.Text;
来源：http://hz.yj20258888.top/gtzibnzfom.html

[C12] 立即执行函数 IIFE
来源：http://hz.chenlongwang.top/gtzqbdtfun.html

Py:   (lambda: print("run"))()
来源：http://hz.hnxiangtu.top/gtugnnbmbg.html

PHP:  (function () { echo "run"; })();
来源：http://hz.sxryk.cn/gtclaoryix.html

JS:   (() => { console.log("run"); })();
来源：http://hz.svipenyu.cn/gtklpwqdid.html

TS:   (() => { console.log("run"); })();
来源：http://hz.shzxlz.cn/gtwywuucba.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.ybcxt.top/gtdopotplq.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.iojbl.cn/gtabfvxxrt.html

Ruby: -> { puts "run" }.call
来源：http://hz.xinyue.icu/gtrwodruqz.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.zhoulong.xyz/gtishvfklg.html

[C13] 类型声明 / 类型注解
来源：http://hz.tanke756.top/gthheygnhn.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.cheryme.top/gtgogetdgs.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jqgufenzy.top/gtwxhnhfoe.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.shangyingyoupin.top/gtabqkeufr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.shuidangran.top/gtvlknhgaa.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.daxiang520.top/gtckhncmvv.html

Go:   func add(a, b int) int
来源：http://hz.sweek.top/gturozlbxz.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.havefunace.top/gtpfddferc.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.9152youxi.cn/gtvvzqdkbi.html

[C14] 泛型函数
来源：http://hz.zhengqikj.top/gtrocicedf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.yuanzhike.top/gtczgypugt.html

PHP:  // 无泛型
来源：http://hz.pengpengdd.cyou/gttyooznyw.html

JS:   // 无泛型
来源：http://hz.shzxlz.cn/gtxbjcnpku.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.ehwqpu.com/gtrzvappbp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.jiagoushi.top/gtnfmgbtqn.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.0kj1m.cn/gtnoxqmlot.html

Ruby: # 无泛型
来源：http://hz.aibaodan.cn/gtlyxhgpbs.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.feifeiyinyue.top/gtjrimbent.html

[C15] 解构 / 展开参数
来源：http://hz.iojbl.cn/gtsabwewwd.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.guowangkeji.top/gtrgzbdhmk.html

PHP:  [$a, $b] = $pair;
来源：http://hz.cheryme.top/gtsnrwuwfi.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.aizwys.cn/gtrupzgihj.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.daxiang520.top/gtogzbwxya.html

Java: // 无解构
来源：http://hz.feifeiyinyue.top/gteynvkbqk.html

Go:   // 无解构
来源：http://hz.cheryme.top/gtwxnoavvr.html

Ruby: a, b = pair
来源：http://hz.chenjidiqi.icu/gtntoenbre.html

C#:   var (a, b) = pair;
来源：http://hz.hammf.cn/gtqehfbkkv.html

[C16] 函数 / 方法重载
来源：http://hz.xuetiantiany.cn/gtwgddjttm.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.sysykeji.top/gtdrcfdoqt.html

PHP:  // 无重载
来源：http://hz.meibo888.top/gtgvzijark.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.hammf.cn/gtwexpvlgk.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.tanke756.top/gtmojldfxj.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.xinyue.icu/gttedlzlmm.html

Go:   // 无重载：用不同函数名
来源：http://hz.wangshuangyany.cn/gtuzdvtqlj.html

Ruby: # 无重载：靠动态参数
来源：http://hz.jiagoushi.top/gtyltdwfbb.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.jqgfzy.top/gtsbbdliuc.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtrlqcrjjr.html

D. 数组 / 列表 / 集合
来源：http://hz.bjfxy.top/gteialqnoc.html

================================================================================
来源：http://hz.zhongyouzk.top/gtryfrlaiv.html

[D01] 创建数组 / 列表
来源：http://hz.316326.xyz/gtxwdzgaww.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.jlsjyb.cn/gtximcfzvn.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.zhiwuduotai.top/gtbepyohta.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.jqgfzy.top/gtkykabmgl.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.svipenyu.cn/gtamhbrmwb.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.guannengcc.top/gtdicxyekw.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.jqgfzy.top/gtexhdwjez.html

Ruby: arr = [1, 2, 3]
来源：http://hz.meibo888.top/gtcfbmrieg.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.yonumen.top/gtktpfszqx.html

[D02] 追加元素到末尾
来源：http://hz.jyoumei.cn/gttsgiulrb.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.hammf.cn/gtgwfzffxh.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.gaohongyu789.top/gtfegbalab.html

JS:   arr.push(4);
来源：http://hz.birdmap.top/gtkwshnanx.html

TS:   arr.push(4);
来源：http://hz.svipenyu.cn/gterjxcfzo.html

Java: list.add(4);
来源：http://hz.cqqwz.cn/gthlcrhhzq.html

Go:   arr = append(arr, 4)
来源：http://hz.hongshengwenyu.top/gteihytiqm.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.xuanzx.com/gtyzxiwczq.html

C#:   list.Add(4);
来源：http://hz.cashguo.top/gtgszvuipp.html

[D03] 在指定位置插入元素
来源：http://hz.iojbl.cn/gtkyhzxcfx.html

Py:   arr.insert(0, 0)
来源：http://hz.xinyue.icu/gthmoovvmj.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.jianghu66.top/gtiztjslnq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.jqgfzy.top/gttxhspivx.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.meibo888.top/gtgjxfircn.html

Java: list.add(0, 0);
来源：http://hz.gzhubu.top/gtsywbszse.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.xingfuxueyuan.xyz/gtvwxnydfa.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.nanxuanxn.top/gtxucpdmtv.html

C#:   list.Insert(0, 0);
来源：http://hz.chenzaomai.com/gtkfaomrsh.html

[D04] 删除元素
来源：http://hz.jqgufenzy.top/gtvxiehfdu.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.redwolf501.top/gtnuzgdsic.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.chenzaomai.com/gtiquwryhz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.ppjwa.cn/gtozrcrikt.html

TS:   arr.splice(0, 1);
来源：http://hz.ppjwa.cn/gttogcxwxe.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.sxryk.cn/gttyyapwwx.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.sweek.top/gtjyzytqof.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.yanxiufei.cn/gtgmyebawu.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.chenzaomai.com/gtknswwaqd.html

[D05] 访问与修改元素
来源：http://hz.yueranfly.top/gtuasdjijs.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yvedp.cn/gtmtgxxnui.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.xinyue.icu/gtbpexuhne.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.hnxiangtu.top/gtruhwctxk.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.nanxinkj.top/gtcykucxti.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.zhengqikj.top/gtzyzxlbax.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.hysaishi.cn/gtlnqyvuly.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.nwbrower.top/gtdgnglkhf.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.jinghuilouyu.cn/gtgujgfrai.html

[D06] 数组长度
来源：http://hz.xingfuxueyuan.xyz/gtjzsjfmfg.html

Py:   len(arr)
来源：http://hz.xingfuxueyuan.xyz/gtzrocxwmy.html

PHP:  count($arr);
来源：http://hz.iojbl.cn/gtfmlxbrpz.html

JS:   arr.length
来源：http://hz.xziqi.cn/gtqrigrrlw.html

TS:   arr.length
来源：http://hz.jianghu66.top/gtkwdyduza.html

Java: list.size();
来源：http://hz.hnxiangtu.top/gtwcbmyzlg.html

Go:   len(arr)
来源：http://hz.ydzc1.top/gtkbrzbocn.html

Ruby: arr.length; arr.size
来源：http://hz.jinqigufen.top/gtvlhfekup.html

C#:   list.Count;
来源：http://hz.tianlin.xyz/gtvigdmglw.html

[D07] 切片 / 取子数组
来源：http://hz.yj20258888.top/gtdixjdoex.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.feifeiyinyue.top/gtklqakhmh.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.vqdsnc.cn/gtttbngsfs.html

JS:   arr.slice(1, 4);
来源：http://hz.hongshengwenyu.top/gtiudljkti.html

TS:   arr.slice(1, 4);
来源：http://hz.yongpay.top/gtudaotzmh.html

Java: list.subList(1, 4);
来源：http://hz.nwbrower.top/gtknuiylpv.html

Go:   arr[1:4]
来源：http://hz.zhiwuduotai.top/gtwexmmqwz.html

Ruby: arr[1, 3]
来源：http://hz.jqgfzy.top/gtagbptzje.html

C#:   list.GetRange(1, 3);
来源：http://hz.zhongyouzk.top/gtokweayai.html

[D08] 合并两个数组
来源：http://hz.zycfv.cn/gtrchxxsod.html

Py:   a + b;  a.extend(b)
来源：http://hz.meibo888.top/gthoaswfar.html

PHP:  array_merge($a, $b);
来源：http://hz.jiagoushi.top/gtajbympjr.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.dashuyun.cn/gtwzsfbbms.html

TS:   [...a, ...b];
来源：http://hz.mhx1999.top/gtdhjfyedl.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.cashguo.top/gtaglrgbqa.html

Go:   append(a, b...)
来源：http://hz.fzhhl.top/gtwugrchef.html

Ruby: a + b;  a.concat(b)
来源：http://hz.jinqigufen.top/gtvelmjewy.html

C#:   a.Concat(b).ToList()
来源：http://hz.c1oappe.top/gtnpwxbdwo.html

[D09] 排序（升序）
来源：http://hz.yanxiufei.cn/gtmzcnrklj.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.fzhhl.top/gtlyxyxbnv.html

PHP:  sort($arr);
来源：http://hz.ehwqpu.com/gtmjzyvawb.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.hysaishi.cn/gtwfthypou.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.hongshengwenyu.top/gtxjkyydca.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.redwolf501.top/gtvhbzxxtg.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.yuanzhike.top/gtbtmgrkkm.html

Ruby: arr.sort
来源：http://hz.pycfn.com/gtloknkixr.html

C#:   list.Sort();
来源：http://hz.ydjk.org.cn/gtwgwzsemh.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.yonumen.top/gtbwhntsnz.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.jinghuilouyu.cn/gtyjmpkkzp.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.pycfn.com/gttogrjoto.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zhoulong.xyz/gtqchmnfvj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.cheryme.top/gtnloayebf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.hammf.cn/gtkdjyicsy.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.jlsjyb.cn/gtedkqobyr.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.52xcode.cn/gtnsvqejif.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.kuanghao11.cn/gtvcrmowwn.html

[D11] 反转数组
来源：http://hz.gogol.net.cn/gtkeclsvcd.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.0kj1m.cn/gtjjbubzwz.html

PHP:  array_reverse($arr);
来源：http://hz.sufxvd.cn/gttirctmvv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.c1oappe.top/gtnruipxkv.html

TS:   [...arr].reverse();
来源：http://hz.ywan-chungtsiang.top/gtfcurrwub.html

Java: Collections.reverse(list);
来源：http://hz.jinyuanbaomall.cn/gtgsefnlir.html

Go:   slices.Reverse(arr)
来源：http://hz.gogol.net.cn/gtwygmtwzl.html

Ruby: arr.reverse
来源：http://hz.zhoulong.xyz/gttqyjpnsa.html

C#:   list.Reverse();
来源：http://hz.gogol.net.cn/gtvjyqtnjq.html

[D12] 查找元素下标
来源：http://hz.yj20258.top/gttfleduce.html

Py:   arr.index(x);  x in arr
来源：http://hz.guowangkeji.top/gtycekaeyn.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.yangfankeji.com/gtlbnvdzcu.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.ydjk.org.cn/gttdthrxkg.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yj20258.top/gtxaakzzke.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.tianlin.xyz/gtijgoddtn.html

Go:   slices.Index(arr, x)
来源：http://hz.wangdashe.top/gtmlufzmcq.html

Ruby: arr.index(x)
来源：http://hz.pycfn.com/gtkqcnsobp.html

C#:   list.IndexOf(x);
来源：http://hz.iojbl.cn/gtkhjkzleo.html

[D13] 过滤（保留满足条件的）
来源：http://hz.gogol.net.cn/gtibjgnmju.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.ppjwa.cn/gtpiffujdb.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.zhaomingkeji.xyz/gtzqnqirho.html

JS:   arr.filter(x => x > 3)
来源：http://hz.svipenyu.cn/gthlzrqvat.html

TS:   arr.filter(x => x > 3)
来源：http://hz.nanxinkj.top/gtszgzbrqg.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.yanxiufei.cn/gtyxmjaoby.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.dianchejie.cn/gtczpqtvdg.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.sxryk.cn/gtlasxozqv.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.daria6918.cn/gtafhxqnsw.html

[D14] 映射转换（每个元素变形）
来源：http://hz.tian-w.cn/gtaulxrytr.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.nanxuanxn.top/gtycjqpkib.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.hysaishi.cn/gtslcrfcjl.html

JS:   arr.map(x => x * 2)
来源：http://hz.sxryk.cn/gtusrcgtcc.html

TS:   arr.map(x => x * 2)
来源：http://hz.jlsjyb.cn/gtjtjnmtcd.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.xuanzx.com/gtduwjkfei.html

Go:   // 手写循环
来源：http://hz.9152youxi.cn/gtivrkblia.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.jinqigufen.top/gteiajaxcr.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.daria6918.cn/gtitafiyeu.html

[D15] 去重
来源：http://hz.fzhhl.top/gtaylplbrm.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.quarkkingdee.top/gtsddyynjm.html

PHP:  array_unique($arr);
来源：http://hz.redwolf501.top/gtcuktxkkx.html

JS:   [...new Set(arr)]
来源：http://hz.shuidangran.top/gtfvofvfmj.html

TS:   [...new Set(arr)]
来源：http://hz.yj20258888.top/gtiyigrumb.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.shangyingyoupin.top/gtkrgzzglm.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.zhijiandao.cn/gtqsdmlkpx.html

Ruby: arr.uniq
来源：http://hz.quarkkingdee.top/gtwfvuauvu.html

C#:   list.Distinct().ToList()
来源：http://hz.zhiwuduotai.top/gtgamvkhup.html

[D16] 求和与平均值
来源：http://hz.pycfn.com/gthapzglkk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.jinyuanbaomall.cn/gtscsklkwr.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.yangfankeji.com/gtbptptrpf.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.tian-w.cn/gtsjbjbsky.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.nanxuanxn.top/gtqfvenwwg.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.0kj1m.cn/gtofmbiikj.html

Go:   // 手写循环累加
来源：http://hz.jinyuanbaomall.cn/gtrlwfpotn.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.dianchejie.cn/gttmcycdap.html

C#:   list.Sum();  list.Average()
来源：http://hz.zhiwuduotai.top/gtnasidtwf.html

[D17] 最大值与最小值
来源：http://hz.yongpay.top/gtlybjuord.html

Py:   max(arr);  min(arr)
来源：http://hz.tian-w.cn/gthpgsvcvh.html

PHP:  max($arr);  min($arr);
来源：http://hz.ywan-chungtsiang.top/gtkloonqyf.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.sxryk.cn/gtmhhaukte.html

TS:   Math.max(...arr);
来源：http://hz.jlsjyb.cn/gtgayrkexc.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.haohaochexian.top/gtmcbraykf.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.wangshuangyany.cn/gtpwfktdob.html

Ruby: arr.max;  arr.min
来源：http://hz.hongshengwenyu.top/gtcdxkvysh.html

C#:   list.Max();  list.Min()
来源：http://hz.jyoumei.cn/gtxuzvihrw.html

[D18] 扁平化嵌套数组
来源：http://hz.zhixingplan.top/gtqmsjdxia.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.xziqi.cn/gtjakunjwk.html

PHP:  array_merge(...$nested);
来源：http://hz.zhongyouzk.top/gtqbaatnxu.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.shanyushiyangkeji.top/gtqbfjbyti.html

TS:   nested.flat();
来源：http://hz.wangdashe.top/gtzwlbuwxl.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.jinqigfzy.top/gtlkofvlga.html

Go:   // 手写双层循环
来源：http://hz.zhoulong.xyz/gtpajbayzu.html

Ruby: nested.flatten
来源：http://hz.chenjidiqi.icu/gtwltvvyof.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.redwolf501.top/gtetrtlbwq.html

[D19] 按字段分组
来源：http://hz.sxryk.cn/gtgcrebqnc.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.sysykeji.top/gtmliwpmye.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.shuidangran.top/gtsudnimmw.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.gotoacloud.top/gtxiwtnecq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.zdqjudy.top/gttezhgqqc.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.pengpengdd.cyou/gtjhtkdmhn.html

Go:   // 手写 map[string][]T
来源：http://hz.ydzc1.top/gteuwhkyzr.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.xingfuxueyuan.xyz/gtdstzaqys.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.gogol.net.cn/gtbpwaazoi.html

[D20] 统计每个元素出现次数
来源：http://hz.yj202588.top/gtmngovabc.html

Py:   Counter(arr)
来源：http://hz.cashguo.top/gtrpxrydat.html

PHP:  array_count_values($arr);
来源：http://hz.0kj1m.cn/gtnhqseokb.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.feifeiyinyue.top/gtwxkchpwe.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zhixingplan.top/gtrvcnvdaz.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.svipenyu.cn/gtumjxjhhm.html

Go:   // 手写 map[T]int
来源：http://hz.tian-w.cn/gtgjughiyz.html

Ruby: arr.tally
来源：http://hz.tian-w.cn/gtcycbxfzl.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.hongshengwenyu.top/gtbcqdzhns.html

[D21] 判断是否包含某元素
来源：http://hz.redwolf501.top/gtrvromxwx.html

Py:   x in arr
来源：http://hz.jqgfzy.top/gtgdlnmruj.html

PHP:  in_array($x, $arr, true);
来源：http://hz.cashguo.top/gtguskmdth.html

JS:   arr.includes(x)
来源：http://hz.shuidangran.top/gtcwczpckh.html

TS:   arr.includes(x)
来源：http://hz.fengsongda.top/gtdwkwjmck.html

Java: list.contains(x)
来源：http://hz.zhaomingkeji.xyz/gtngnifzrf.html

Go:   slices.Contains(arr, x)
来源：http://hz.cdnleiting.top/gturdxurkw.html

Ruby: arr.include?(x)
来源：http://hz.aizwys.cn/gtnthkdkkx.html

C#:   list.Contains(x)
来源：http://hz.yanxiufei.cn/gthbhmmqyw.html

[D22] 复制数组（避免共享引用）
来源：http://hz.shuidangran.top/gtmbygrarl.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.chenlongwang.top/gtekgpqcmh.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.yj20258.top/gtjnqamabv.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.aibaodan.cn/gtrzduptzp.html

TS:   [...arr];
来源：http://hz.svipenyu.cn/gtkeefuweg.html

Java: new ArrayList<>(list);
来源：http://hz.yongpay.top/gtplgcaicv.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.daria6918.cn/gtnvftrhcc.html

Ruby: arr.dup;  arr.clone
来源：http://hz.nanxinkj.top/gtvehhumrh.html

C#:   new List<int>(list);
来源：http://hz.mhx1999.top/gtvvsqtkzy.html

[D23] reduce 累积计算
来源：http://hz.ppjwa.cn/gteixcmwfr.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.zhaomingkeji.xyz/gteacanqef.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.zhengqikj.top/gterzuxqkd.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhijiandao.cn/gtqmvrnorb.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jinqigufen.top/gtmfmmweww.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.gaohongyu789.top/gthyhebnrr.html

Go:   // 手写循环
来源：http://hz.tanke756.top/gtxlnofoqd.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.cdnleiting.top/gtuplmorla.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.jlsjyb.cn/gttpcmdyav.html

[D24] 字典 / Map 基本操作
来源：http://hz.svipenyu.cn/gtuieddlop.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.sweek.top/gtreiqklce.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.shanyushiyangkeji.top/gtickcwagk.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.daria6918.cn/gtvdsuvlvi.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.0kj1m.cn/gtqtkdsvrf.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.xuetiantiany.cn/gtjoiizxve.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.havefunace.top/gtjfjgmsyu.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.chenzaomai.com/gtrymzeuom.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.shangyingyoupin.top/gtgtaktqja.html

[D25] Set 集合去重与交并差
来源：http://hz.gaohongyu789.top/gtxgbwdnvu.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.zhoulong.xyz/gtmufhppdq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.hammf.cn/gttlvmtihm.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.quarkkingdee.top/gthwjhnzmd.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.vqdsnc.cn/gtaptjpqal.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.quarkkingdee.top/gtcbntisvo.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.nanxuanxn.top/gtynfycjcs.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.aibaodan.cn/gtngqruuan.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.chenjidiqi.icu/gtajmazsiz.html

[D26] 数组转字符串
来源：http://hz.yongpay.top/gtbprntblt.html

Py:   ", ".join(map(str, arr))
来源：http://hz.guowangkeji.top/gtqgwsdakp.html

PHP:  implode(", ", $arr);
来源：http://hz.nwbrower.top/gthqfdiqqj.html

JS:   arr.join(", ")
来源：http://hz.yj202588.top/gttyjmdjdt.html

TS:   arr.join(", ")
来源：http://hz.tianlin.xyz/gtpndbhbwp.html

Java: String.join(", ", list)
来源：http://hz.sweek.top/gtfhazqrgu.html

Go:   strings.Join(strs, ", ")
来源：http://hz.yangfankeji.com/gtupeotpsb.html

Ruby: arr.join(", ")
来源：http://hz.ivvv.top/gtmzwubdfx.html

C#:   string.Join(", ", list)
来源：http://hz.tian-w.cn/gtuqxtyspr.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtjnlszqbl.html

E. 字符串处理
来源：http://hz.zycfv.cn/gtmrdavvyx.html

================================================================================
来源：http://hz.chenlongwang.top/gtabgyidll.html

[E01] 拼接字符串
来源：http://hz.sweek.top/gtbyepylfh.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.shzxlz.cn/gtqyikiejy.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.9152youxi.cn/gtccleucki.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.daria6918.cn/gteqftxgoq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.hammf.cn/gtqmfwjfcu.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.shanyushiyangkeji.top/gtufekzigi.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.yj202588.top/gtaxcvyywz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.tian-w.cn/gtulxcvbgh.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.daria6918.cn/gtqffjbjfr.html

[E02] 重复字符串
来源：http://hz.xingfuxueyuan.xyz/gtuvyxuqmk.html

Py:   "ab" * 3
来源：http://hz.zhixingplan.top/gtqwjznzdy.html

PHP:  str_repeat("ab", 3);
来源：http://hz.hnqzz.top/gtppixnppr.html

JS:   "ab".repeat(3)
来源：http://hz.mhx1999.top/gtibpdpwwt.html


<!-- 参考信息 -->