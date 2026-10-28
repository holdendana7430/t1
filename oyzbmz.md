代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://hz.havefunace.top/gtliwztnzb.html

C#:   using System.Text;
来源：http://hz.jyoumei.cn/gtjgjlafcc.html

[C12] 立即执行函数 IIFE
来源：http://hz.9152youxi.cn/gtkoidyuwk.html

Py:   (lambda: print("run"))()
来源：http://hz.xingfuxueyuan.xyz/gtoohwvcpq.html

PHP:  (function () { echo "run"; })();
来源：http://hz.0kj1m.cn/gtdtqtpqsx.html

JS:   (() => { console.log("run"); })();
来源：http://hz.jqgfzy.top/gtgenlresv.html

TS:   (() => { console.log("run"); })();
来源：http://hz.tian-w.cn/gtlpazzgkq.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.fzhhl.top/gtqkssyrch.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.yuanzhike.top/gttiuioexl.html

Ruby: -> { puts "run" }.call
来源：http://hz.hywenlv.cn/gtdubwemec.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.xuanzx.com/gtuqtvpksb.html

[C13] 类型声明 / 类型注解
来源：http://hz.sxryk.cn/gtzeikppcu.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.zhiwuduotai.top/gtucuowpgc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.dashuyun.cn/gtvsfizbqw.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.sxryk.cn/gtgisnzwpb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yongpay.top/gtfflyhlsm.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.shanyushiyangkeji.top/gtmbarcwpo.html

Go:   func add(a, b int) int
来源：http://hz.mhx1999.top/gtydneekzg.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.chenjidiqi.icu/gtqwkxqnvd.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.jqgufenzy.top/gtihmlyuxc.html

[C14] 泛型函数
来源：http://hz.hammf.cn/gtffoddmvq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.zhengqikj.top/gtvyaqzbsy.html

PHP:  // 无泛型
来源：http://hz.feifeiyinyue.top/gtywzqppdh.html

JS:   // 无泛型
来源：http://hz.zhoulong.xyz/gtxgxlliao.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.hongshengwenyu.top/gtjtyutact.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.xingfuxueyuan.xyz/gtzlocwqrl.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.sxryk.cn/gtnugjscig.html

Ruby: # 无泛型
来源：http://hz.cheryme.top/gttrophkyk.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.fzhhl.top/gtybguvsee.html

[C15] 解构 / 展开参数
来源：http://hz.cucudq.cn/gtgksmgzut.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.nwbrower.top/gtfysmuknh.html

PHP:  [$a, $b] = $pair;
来源：http://hz.jiagoushi.top/gtkapndzlv.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.zhixingplan.top/gtuepjggky.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.andypj.xyz/gtzanhdafv.html

Java: // 无解构
来源：http://hz.0kj1m.cn/gtnysujngt.html

Go:   // 无解构
来源：http://hz.pengpengdd.cyou/gtnrkhzbol.html

Ruby: a, b = pair
来源：http://hz.ppjwa.cn/gtdhhsroyu.html

C#:   var (a, b) = pair;
来源：http://hz.yj20258.top/gtaaaybuja.html

[C16] 函数 / 方法重载
来源：http://hz.jqgfzy.top/gtxxhqvznx.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.gzhubu.top/gtytxsedhb.html

PHP:  // 无重载
来源：http://hz.hnxiangtu.top/gttigsiecm.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.ppjwa.cn/gtltntxrnd.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.chenjidiqi.icu/gtoidemxli.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.jqgfzy.top/gtiahkavzz.html

Go:   // 无重载：用不同函数名
来源：http://hz.kuanghao11.cn/gtslozcrnn.html

Ruby: # 无重载：靠动态参数
来源：http://hz.c1oappe.top/gtlezfvcuy.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.chenjidiqi.icu/gtxuzsfksi.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtwdisxzcz.html

D. 数组 / 列表 / 集合
来源：http://hz.hongshengwenyu.top/gtcewapref.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtkjsayszo.html

[D01] 创建数组 / 列表
来源：http://hz.gzhubu.top/gtgqemltfu.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.zhaomingkeji.xyz/gtnbucywby.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.52xcode.cn/gtfoxuxrhr.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.jiagoushi.top/gtvvqxjdun.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.yj20258.top/gtpprwmyuu.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.nwbrower.top/gtsyrkzbhp.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.tian-w.cn/gtrauldvfj.html

Ruby: arr = [1, 2, 3]
来源：http://hz.fzhhl.top/gtjuewmbgh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.yueranfly.top/gtlfwczyfv.html

[D02] 追加元素到末尾
来源：http://hz.xuetiantiany.cn/gtalctvzzt.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.jlsjyb.cn/gtsjxggibk.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.jinqigfzy.top/gtcnmkwatf.html

JS:   arr.push(4);
来源：http://hz.kuanghao11.cn/gtbzzesdya.html

TS:   arr.push(4);
来源：http://hz.yj20258888.top/gtfexbaaoo.html

Java: list.add(4);
来源：http://hz.kuanghao11.cn/gtgdvgesra.html

Go:   arr = append(arr, 4)
来源：http://hz.pycfn.com/gtlzesyxou.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.gotoacloud.top/gtttyqpccc.html

C#:   list.Add(4);
来源：http://hz.fzhhl.top/gtrzpdrmbs.html

[D03] 在指定位置插入元素
来源：http://hz.chenzaomai.com/gtocqwzdhv.html

Py:   arr.insert(0, 0)
来源：http://hz.0kj1m.cn/gtmpomubcw.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.yj20258888.top/gthzuljcur.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.andypj.xyz/gtntlzqrfv.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.tianlin.xyz/gtnnsvvpfi.html

Java: list.add(0, 0);
来源：http://hz.316326.xyz/gtqfsftedt.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.shuidangran.top/gtfbfgfnfz.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.birdmap.top/gtfspftcff.html

C#:   list.Insert(0, 0);
来源：http://hz.daria6918.cn/gtbsmntinh.html

[D04] 删除元素
来源：http://hz.daxiang520.top/gtnvplxuxp.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.shanyushiyangkeji.top/gtzkjrornh.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.chenlongwang.top/gteqsondtj.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.vqdsnc.cn/gtaetjggpn.html

TS:   arr.splice(0, 1);
来源：http://hz.shangyingyoupin.top/gtvryeshdg.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.hnxiangtu.top/gtszrsrfmg.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.yvedp.cn/gtzfghfiyn.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.andypj.xyz/gtuifcqeya.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.gotoacloud.top/gtvktzxvhv.html

[D05] 访问与修改元素
来源：http://hz.zhongyouzk.top/gtzbvqoscz.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.guowangkeji.top/gtaesfylms.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.sxryk.cn/gtqwkiezqc.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.yueranfly.top/gtlxvqryix.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.xuetiantiany.cn/gtritqxwvm.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.meibo888.top/gtagwgdaqf.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.cashguo.top/gtlfqyauyl.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.pengpengdd.cyou/gthjmccaxn.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.zhijiandao.cn/gtrapdroru.html

[D06] 数组长度
来源：http://hz.hfpthk.cn/gtpdigcncx.html

Py:   len(arr)
来源：http://hz.yj202588.top/gtmwimkjrq.html

PHP:  count($arr);
来源：http://hz.daxiang520.top/gtjdbzbpoy.html

JS:   arr.length
来源：http://hz.sysykeji.top/gtbslpdhza.html

TS:   arr.length
来源：http://hz.yueranfly.top/gtwiwxznwb.html

Java: list.size();
来源：http://hz.chenzaomai.com/gtxvjhhppc.html

Go:   len(arr)
来源：http://hz.zhiwuduotai.top/gtyimiqxfk.html

Ruby: arr.length; arr.size
来源：http://hz.gzhubu.top/gtayjyotzl.html

C#:   list.Count;
来源：http://hz.jlsjyb.cn/gtbgcnwrmk.html

[D07] 切片 / 取子数组
来源：http://hz.yj202588.top/gtypeyzuob.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.hfpthk.cn/gtvpdxbkzw.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.yj20258888.top/gtkvvrwmvs.html

JS:   arr.slice(1, 4);
来源：http://hz.zhiwuduotai.top/gtedjlcpzo.html

TS:   arr.slice(1, 4);
来源：http://hz.gzhubu.top/gtvdgcczdd.html

Java: list.subList(1, 4);
来源：http://hz.zhoulong.xyz/gtwehikbfb.html

Go:   arr[1:4]
来源：http://hz.tianlin.xyz/gtxwevncxc.html

Ruby: arr[1, 3]
来源：http://hz.jyoumei.cn/gtkokfufwg.html

C#:   list.GetRange(1, 3);
来源：http://hz.zycfv.cn/gtxmucsmkz.html

[D08] 合并两个数组
来源：http://hz.xziqi.cn/gtqsexciln.html

Py:   a + b;  a.extend(b)
来源：http://hz.0kj1m.cn/gtbmrrdvzp.html

PHP:  array_merge($a, $b);
来源：http://hz.gaohongyu789.top/gtmdlurjbp.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.sweek.top/gtcopmlmxl.html

TS:   [...a, ...b];
来源：http://hz.chenlongwang.top/gtoktklllp.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.cqqwz.cn/gtkarxtlfh.html

Go:   append(a, b...)
来源：http://hz.redwolf501.top/gtopehmtbk.html

Ruby: a + b;  a.concat(b)
来源：http://hz.yongpay.top/gtsidpyoij.html

C#:   a.Concat(b).ToList()
来源：http://hz.zhijiandao.cn/gtriytqbeo.html

[D09] 排序（升序）
来源：http://hz.nanxuanxn.top/gtqiqjizal.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.meibo888.top/gtiipposfz.html

PHP:  sort($arr);
来源：http://hz.9152youxi.cn/gtghldobdd.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.haohaochexian.top/gtqpjlvhjy.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.yj202588.top/gttgzsuudz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.haohaochexian.top/gtwkszjtsw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.xinyue.icu/gtlcdupqkz.html

Ruby: arr.sort
来源：http://hz.daria6918.cn/gtfqezmvyq.html

C#:   list.Sort();
来源：http://hz.smart0.xyz/gtdvlvcvhc.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.wangshuangyany.cn/gttrehpjfz.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.cqqwz.cn/gtjsfxcidr.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zdqjudy.top/gtudxmzzfg.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.dashuyun.cn/gthjqipswy.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.daxiang520.top/gtioazahiv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.sysykeji.top/gtncjwjdlk.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.smart0.xyz/gtoqkbztxf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.jyoumei.cn/gtzcefhnut.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.hfpthk.cn/gtfqyfwsxx.html

[D11] 反转数组
来源：http://hz.yanxiufei.cn/gtrdbgclus.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.hfpthk.cn/gtzxqybkuo.html

PHP:  array_reverse($arr);
来源：http://hz.xingfuxueyuan.xyz/gtvhnzzpxz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.jinghuilouyu.cn/gtsqybytby.html

TS:   [...arr].reverse();
来源：http://hz.andypj.xyz/gtjhiquuge.html

Java: Collections.reverse(list);
来源：http://hz.yvedp.cn/gtruhwqbzh.html

Go:   slices.Reverse(arr)
来源：http://hz.yongpay.top/gtvdiotiqs.html

Ruby: arr.reverse
来源：http://hz.cheryme.top/gtlsdqzknz.html

C#:   list.Reverse();
来源：http://hz.hywenlv.cn/gtzkgxhzyi.html

[D12] 查找元素下标
来源：http://hz.ydzc1.top/gtyqcmvjlt.html

Py:   arr.index(x);  x in arr
来源：http://hz.c1oappe.top/gtoykibbir.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.guowangkeji.top/gtbugficed.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yangfankeji.com/gtpinfmagf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.sxryk.cn/gtbvqfnbph.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.birdmap.top/gtgkiddiwz.html

Go:   slices.Index(arr, x)
来源：http://hz.tianlin.xyz/gtzwcybmso.html

Ruby: arr.index(x)
来源：http://hz.pycfn.com/gtronqkyfr.html

C#:   list.IndexOf(x);
来源：http://hz.zhongyouzk.top/gtcirmpgfw.html

[D13] 过滤（保留满足条件的）
来源：http://hz.haohaochexian.top/gtsjrzbqwf.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.dianchejie.cn/gtcsolimas.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.yueranfly.top/gtitlsmqnx.html

JS:   arr.filter(x => x > 3)
来源：http://hz.shangyingyoupin.top/gtrshrhnmd.html

TS:   arr.filter(x => x > 3)
来源：http://hz.xinyue.icu/gtrxjndwta.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.yj20258.top/gtrcyzgaqu.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.dashuyun.cn/gtwskrufxp.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.yuxming.cn/gtsetfhnnq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.quarkkingdee.top/gturremqnc.html

[D14] 映射转换（每个元素变形）
来源：http://hz.aizwys.cn/gtlwkkeyva.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.yj202588.top/gthwicfqih.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.xuanzx.com/gtuspywkdn.html

JS:   arr.map(x => x * 2)
来源：http://hz.yvedp.cn/gtfkpcnjnp.html

TS:   arr.map(x => x * 2)
来源：http://hz.cucudq.cn/gtvzhsqkwj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.yueranfly.top/gtcdghpmnu.html

Go:   // 手写循环
来源：http://hz.wangdashe.top/gtgneirqqw.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.yonumen.top/gtbimfgges.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.xuanzx.com/gttgfqfsqp.html

[D15] 去重
来源：http://hz.316326.xyz/gtgqifhypc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.jqgfzy.top/gtkyqlpjqr.html

PHP:  array_unique($arr);
来源：http://hz.mhx1999.top/gtvgftacln.html

JS:   [...new Set(arr)]
来源：http://hz.wangdashe.top/gtycdwqusr.html

TS:   [...new Set(arr)]
来源：http://hz.kuanghao11.cn/gtajyawxsd.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.shanyushiyangtech.top/gtleyttfuj.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.cucudq.cn/gtohiukuzc.html

Ruby: arr.uniq
来源：http://hz.cashguo.top/gtjspmcdcj.html

C#:   list.Distinct().ToList()
来源：http://hz.zhoulong.xyz/gtlzozuoxy.html

[D16] 求和与平均值
来源：http://hz.yonumen.top/gtgjeicvcx.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.jianghu66.top/gtgsccwjnz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.c1oappe.top/gtgygddoeg.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zhixingplan.top/gtfoopodkf.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.tianlin.xyz/gtypmwfwgo.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.shanyushiyangtech.top/gtmjeagxws.html

Go:   // 手写循环累加
来源：http://hz.zhoulong.xyz/gtvrlfghjq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.sweek.top/gtgxkyxqhy.html

C#:   list.Sum();  list.Average()
来源：http://hz.ywan-chungtsiang.top/gtfojfereh.html

[D17] 最大值与最小值
来源：http://hz.svipenyu.cn/gtxbezzpuo.html

Py:   max(arr);  min(arr)
来源：http://hz.snrcjt.cn/gtvltighqn.html

PHP:  max($arr);  min($arr);
来源：http://hz.xuetiantiany.cn/gtwrlascvi.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.jqgfzy.top/gtjupusghl.html

TS:   Math.max(...arr);
来源：http://hz.redwolf501.top/gtbavndtpx.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.sweek.top/gttxblrrai.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.zhoulong.xyz/gthdojeuiz.html

Ruby: arr.max;  arr.min
来源：http://hz.ydzc1.top/gtdlsinwqx.html

C#:   list.Max();  list.Min()
来源：http://hz.aizwys.cn/gtyialnqik.html

[D18] 扁平化嵌套数组
来源：http://hz.xinyue.icu/gtnjqwmtjb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.aibaodan.cn/gtuguwakut.html

PHP:  array_merge(...$nested);
来源：http://hz.hongshengwenyu.top/gtrwtcbguz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.xylfe.cn/gtornroqxq.html

TS:   nested.flat();
来源：http://hz.fzhhl.top/gtpabzqczq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.iojbl.cn/gtsozixvqo.html

Go:   // 手写双层循环
来源：http://hz.ydjk.org.cn/gtgieptnps.html

Ruby: nested.flatten
来源：http://hz.gogol.net.cn/gttcjnwyhp.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.haohaochexian.top/gtijqgejjf.html

[D19] 按字段分组
来源：http://hz.cheryme.top/gtyjfqqlqt.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.dashuyun.cn/gtzwwyozwj.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.iojbl.cn/gtfityaedg.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.gogol.net.cn/gtceghplhk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.316326.xyz/gtuxxaebyq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.nwbrower.top/gtfndmotcc.html

Go:   // 手写 map[string][]T
来源：http://hz.sufxvd.cn/gtvheakogd.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.ydjk.org.cn/gtsigjdjuo.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.xylfe.cn/gtgjmembej.html

[D20] 统计每个元素出现次数
来源：http://hz.zhiwuduotai.top/gtelzkkfof.html

Py:   Counter(arr)
来源：http://hz.shanyushiyangkeji.top/gtbxketald.html

PHP:  array_count_values($arr);
来源：http://hz.hammf.cn/gtvvmsrxru.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.fengsongda.top/gtzxnktjoe.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.svipenyu.cn/gtdwjocwrt.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.vqdsnc.cn/gtguqzduea.html

Go:   // 手写 map[T]int
来源：http://hz.smart0.xyz/gtsgytfqxo.html

Ruby: arr.tally
来源：http://hz.cashguo.top/gtautnphyv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.meibo888.top/gtawmrdkmo.html

[D21] 判断是否包含某元素
来源：http://hz.hfpthk.cn/gtnbnglymu.html

Py:   x in arr
来源：http://hz.iojbl.cn/gtcgkrawwb.html

PHP:  in_array($x, $arr, true);
来源：http://hz.nanxinkj.top/gtvgltgzal.html

JS:   arr.includes(x)
来源：http://hz.shzxlz.cn/gtwgabdjxy.html

TS:   arr.includes(x)
来源：http://hz.jinqigufen.top/gtzxhzxcxj.html

Java: list.contains(x)
来源：http://hz.jinyuanbaomall.cn/gtiswqtreq.html

Go:   slices.Contains(arr, x)
来源：http://hz.9152youxi.cn/gtnkyvognx.html

Ruby: arr.include?(x)
来源：http://hz.daria6918.cn/gtxhurysrr.html

C#:   list.Contains(x)
来源：http://hz.zhoulong.xyz/gtvhalrnwl.html

[D22] 复制数组（避免共享引用）
来源：http://hz.cqqwz.cn/gtikmellvh.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.yonumen.top/gtpcdkusws.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.gogol.net.cn/gtuxqudxzk.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.bjfxy.top/gtinwxmhxh.html

TS:   [...arr];
来源：http://hz.tanke756.top/gtzhvwjhrk.html

Java: new ArrayList<>(list);
来源：http://hz.jinqigfzy.top/gtwyeovqfp.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.xingfuxueyuan.xyz/gthzsrmsbm.html

Ruby: arr.dup;  arr.clone
来源：http://hz.52xcode.cn/gtagderaoj.html

C#:   new List<int>(list);
来源：http://hz.chenlongwang.top/gtwkdavuhf.html

[D23] reduce 累积计算
来源：http://hz.sufxvd.cn/gteryafzjp.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.fzhhl.top/gtylclbdzt.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.chenlongwang.top/gtrrdnsdnc.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.chenlongwang.top/gtdilxnupk.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.meibo888.top/gtoszrrbjq.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.ybcxt.top/gtoqwqokkt.html

Go:   // 手写循环
来源：http://hz.jinyuanbaomall.cn/gtcxvemxrl.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.zhengqikj.top/gtksxzwjwn.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.xziqi.cn/gtzvsmnxjy.html

[D24] 字典 / Map 基本操作
来源：http://hz.ivvv.top/gtfudcdhio.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.feifeiyinyue.top/gtpfiszzql.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.cashguo.top/gthabgakrl.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.jinqigfzy.top/gthmqkltsh.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.dashuyun.cn/gticgqydqf.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.xylfe.cn/gtjbfnknkj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.xingfuxueyuan.xyz/gtvdbytseq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.wangdashe.top/gthwgwvyvk.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.zhoulong.xyz/gtvfviuhiv.html

[D25] Set 集合去重与交并差
来源：http://hz.wangdashe.top/gtkqfyanrb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.zhijiandao.cn/gtfexjjuot.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.smart0.xyz/gtnowxvfqp.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.shangyingyoupin.top/gtabxmirze.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.aizwys.cn/gtaxixwpje.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.yj202588.top/gtvyntcbxm.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.jianghu66.top/gtqlrjvhzv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.jyoumei.cn/gtukigxfln.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.pycfn.com/gtciffbtuw.html

[D26] 数组转字符串
来源：http://hz.ybcxt.top/gtumepkfqc.html

Py:   ", ".join(map(str, arr))
来源：http://hz.shangyingyoupin.top/gtetqodpsy.html

PHP:  implode(", ", $arr);
来源：http://hz.nanxinkj.top/gtkeopschj.html

JS:   arr.join(", ")
来源：http://hz.shanyushiyangkeji.top/gtehouxjxe.html

TS:   arr.join(", ")
来源：http://hz.redwolf501.top/gtmngowfqh.html

Java: String.join(", ", list)
来源：http://hz.hnqzz.top/gtcecpqswb.html

Go:   strings.Join(strs, ", ")
来源：http://hz.ppjwa.cn/gtghxosmmf.html

Ruby: arr.join(", ")
来源：http://hz.gaohongyu789.top/gtlvcgtjkz.html

C#:   string.Join(", ", list)
来源：http://hz.hywenlv.cn/gtwygfykmp.html

================================================================================
来源：http://hz.yj20258.top/gtuxnfvwey.html

E. 字符串处理
来源：http://hz.zhijiandao.cn/gtjsintxoz.html

================================================================================
来源：http://hz.aizwys.cn/gtqgtotpnk.html

[E01] 拼接字符串
来源：http://hz.mhx1999.top/gtjiwpijxg.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.0kj1m.cn/gtsfaidvhy.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.c1oappe.top/gtbbcdwmdt.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.aibaodan.cn/gtqrquwflj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.kuanghao11.cn/gtqebvojrt.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.yongpay.top/gtozrcswha.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.fzhhl.top/gtktgycxiz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.ywan-chungtsiang.top/gtrfksonnk.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.redwolf501.top/gtdsdmzdiz.html

[E02] 重复字符串
来源：http://hz.snrcjt.cn/gtulaxzmhm.html

Py:   "ab" * 3
来源：http://hz.gzhubu.top/gtqblbdcck.html

PHP:  str_repeat("ab", 3);
来源：http://hz.ybcxt.top/gtcudlsuom.html

JS:   "ab".repeat(3)
来源：http://hz.guowangkeji.top/gthihutcgf.html


<!-- 参考信息 -->