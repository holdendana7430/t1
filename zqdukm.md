代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://hz.chenzaomai.com/gtkjzhziql.html

Ruby: -> { puts "run" }.call
来源：http://hz.ydzc1.top/gtvtijlxbm.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.jiagoushi.top/gtctromfyu.html

[C13] 类型声明 / 类型注解
来源：http://hz.zhoulong.xyz/gtwnhizfvf.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.zycfv.cn/gtotcfkcnk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.sxryk.cn/gtvtytqswj.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.zhengqikj.top/gtyinqgcrz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhengqikj.top/gtqwrnfebf.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.wangdashe.top/gtcqbdbbba.html

Go:   func add(a, b int) int
来源：http://hz.feifeiyinyue.top/gtkaekenzc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.smart0.xyz/gtthewqwwv.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.zhiwuduotai.top/gtcvridxkx.html

[C14] 泛型函数
来源：http://hz.jiagoushi.top/gtnignxvxv.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.cashguo.top/gthnrixvnn.html

PHP:  // 无泛型
来源：http://hz.fzhhl.top/gtipmnflvf.html

JS:   // 无泛型
来源：http://hz.cheryme.top/gtybrjcpza.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.c1oappe.top/gtcksrqqod.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.chenjidiqi.icu/gtolrtjhqz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.shuidangran.top/gtvsgqqicz.html

Ruby: # 无泛型
来源：http://hz.jqgufenzy.top/gtwtfogfbu.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.xziqi.cn/gtbrnxoyjq.html

[C15] 解构 / 展开参数
来源：http://hz.hfpthk.cn/gtgxwlrkka.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.pycfn.com/gtbortaxam.html

PHP:  [$a, $b] = $pair;
来源：http://hz.zdqjudy.top/gthdgtjyfk.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.kuanghao11.cn/gtswlutktf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.cashguo.top/gtpcpelysl.html

Java: // 无解构
来源：http://hz.cqqwz.cn/gtbhfcwadr.html

Go:   // 无解构
来源：http://hz.yvedp.cn/gtajucobob.html

Ruby: a, b = pair
来源：http://hz.yuxming.cn/gtvlmykwsy.html

C#:   var (a, b) = pair;
来源：http://hz.yonumen.top/gtwcpzpvoy.html

[C16] 函数 / 方法重载
来源：http://hz.yj20258888.top/gtpmxyfvlk.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.zhixingplan.top/gtxztuedgq.html

PHP:  // 无重载
来源：http://hz.jinqigfzy.top/gtdgesxfzm.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.yongpay.top/gtfjaawwaa.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.yangfankeji.com/gtaoshokhb.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.shangyingyoupin.top/gtkmwxiwve.html

Go:   // 无重载：用不同函数名
来源：http://hz.jqgfzy.top/gtlvotohjd.html

Ruby: # 无重载：靠动态参数
来源：http://hz.fzhhl.top/gtytntiwan.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.xziqi.cn/gtzgfdnrod.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtkvvbiupt.html

D. 数组 / 列表 / 集合
来源：http://hz.c1oappe.top/gtavspkxwo.html

================================================================================
来源：http://hz.meibo888.top/gtxkvecrud.html

[D01] 创建数组 / 列表
来源：http://hz.smart0.xyz/gtweexnizv.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.ehwqpu.com/gtammphxdp.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.yongpay.top/gtgevoqtay.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.snrcjt.cn/gtbcnfutcp.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.zhaomingkeji.xyz/gtvxgffzpv.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.yongpay.top/gtnjjlutdd.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.meibo888.top/gtdrjhctlc.html

Ruby: arr = [1, 2, 3]
来源：http://hz.gaohongyu789.top/gtzquuprac.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.xinyue.icu/gtacggpokl.html

[D02] 追加元素到末尾
来源：http://hz.zhaomingkeji.xyz/gtbpoozrxf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.52xcode.cn/gttscubrke.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.xylfe.cn/gtlwmltudi.html

JS:   arr.push(4);
来源：http://hz.jianghu66.top/gtskjmxizy.html

TS:   arr.push(4);
来源：http://hz.xziqi.cn/gtzfcfjycw.html

Java: list.add(4);
来源：http://hz.daria6918.cn/gthrddvzte.html

Go:   arr = append(arr, 4)
来源：http://hz.xylfe.cn/gtnqzrvvpk.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.jqgufenzy.top/gtwtfzhqtp.html

C#:   list.Add(4);
来源：http://hz.dashuyun.cn/gtgmknyxst.html

[D03] 在指定位置插入元素
来源：http://hz.316326.xyz/gtyiiwciln.html

Py:   arr.insert(0, 0)
来源：http://hz.pengpengdd.cyou/gtyaupcbuy.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.zhijiandao.cn/gttklsukfa.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.snrcjt.cn/gtllyeczon.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.yj20258888.top/gtxqrlqgwk.html

Java: list.add(0, 0);
来源：http://hz.yj202588.top/gtunhnvdqm.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.jyoumei.cn/gtlqndyleo.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.dianchejie.cn/gtfxqhrxxm.html

C#:   list.Insert(0, 0);
来源：http://hz.tianlin.xyz/gtmjaoboea.html

[D04] 删除元素
来源：http://hz.yvedp.cn/gtcjhavujs.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.ydzc1.top/gtzyrljkaj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.jqgufenzy.top/gtghjssgxf.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.jianghu66.top/gtsefbteok.html

TS:   arr.splice(0, 1);
来源：http://hz.jqgufenzy.top/gttlvlilly.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.nwbrower.top/gtgxqktmcs.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.hongshengwenyu.top/gtxovuxmxf.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.xuanzx.com/gtlmvztpcu.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.guannengcc.top/gtxxiztzng.html

[D05] 访问与修改元素
来源：http://hz.jyoumei.cn/gtaoaioxan.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.aibaodan.cn/gtgkchotue.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.zhiwuduotai.top/gtqlkshnnl.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.ehwqpu.com/gtmxatjlyf.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.yj202588.top/gtcvpkjsiz.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.feifeiyinyue.top/gtjpbickzd.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.daxiang520.top/gtxarnmwxi.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.dashuyun.cn/gtqsvosejk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.zhongyouzk.top/gtunhxsfkz.html

[D06] 数组长度
来源：http://hz.sysykeji.top/gtgsnmubyw.html

Py:   len(arr)
来源：http://hz.andypj.xyz/gtfgwnlnpk.html

PHP:  count($arr);
来源：http://hz.aizwys.cn/gtubaqkbvd.html

JS:   arr.length
来源：http://hz.jlsjyb.cn/gtrooejwzg.html

TS:   arr.length
来源：http://hz.yanxiufei.cn/gtsxobmzuh.html

Java: list.size();
来源：http://hz.ydjk.org.cn/gtdopnzqqs.html

Go:   len(arr)
来源：http://hz.bjfxy.top/gtlsvgnlca.html

Ruby: arr.length; arr.size
来源：http://hz.52xcode.cn/gtvisiahzo.html

C#:   list.Count;
来源：http://hz.smart0.xyz/gtbkdfoxaf.html

[D07] 切片 / 取子数组
来源：http://hz.yuanzhike.top/gtwhwwxjdq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.9152youxi.cn/gtqyxospvu.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.fengsongda.top/gtegfpmsnq.html

JS:   arr.slice(1, 4);
来源：http://hz.kuanghao11.cn/gtlziksugt.html

TS:   arr.slice(1, 4);
来源：http://hz.yj20258888.top/gtcgtnrcou.html

Java: list.subList(1, 4);
来源：http://hz.wangshuangyany.cn/gthogygmnx.html

Go:   arr[1:4]
来源：http://hz.hongshengwenyu.top/gtkddhhhmn.html

Ruby: arr[1, 3]
来源：http://hz.ivvv.top/gtrmqrmhxs.html

C#:   list.GetRange(1, 3);
来源：http://hz.hywenlv.cn/gtasluwvrv.html

[D08] 合并两个数组
来源：http://hz.shanyushiyangkeji.top/gtgpnaxgbk.html

Py:   a + b;  a.extend(b)
来源：http://hz.kuanghao11.cn/gtcxarsmie.html

PHP:  array_merge($a, $b);
来源：http://hz.shzxlz.cn/gtqtpnxtts.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.jinghuilouyu.cn/gtuuqmbepi.html

TS:   [...a, ...b];
来源：http://hz.ydjk.org.cn/gtxdpxpkfd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.hammf.cn/gtusvwrisa.html

Go:   append(a, b...)
来源：http://hz.yuxming.cn/gtjlrziylm.html

Ruby: a + b;  a.concat(b)
来源：http://hz.nanxuanxn.top/gtfgaodtjb.html

C#:   a.Concat(b).ToList()
来源：http://hz.xuetiantiany.cn/gthfnkjnjt.html

[D09] 排序（升序）
来源：http://hz.smart0.xyz/gtfixluglp.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zdqjudy.top/gtdynqorff.html

PHP:  sort($arr);
来源：http://hz.jinyuanbaomall.cn/gtytrtxtsp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.yanxiufei.cn/gtouxigyum.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.ywan-chungtsiang.top/gtwhgmpmto.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.daxiang520.top/gtvgcjomup.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.xuetiantiany.cn/gtaholnfqs.html

Ruby: arr.sort
来源：http://hz.daxiang520.top/gtevypalvh.html

C#:   list.Sort();
来源：http://hz.tanke756.top/gtxicupdoa.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.gogol.net.cn/gtcdycmuvg.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.kuanghao11.cn/gtidvwzdvp.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.meibo888.top/gttfiprqlw.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jqgufenzy.top/gtksoapznf.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.cheryme.top/gtgvjyukmz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.cqqwz.cn/gtigssqeco.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.zhaomingkeji.xyz/gtclvmrjjb.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.hfpthk.cn/gtzlbdsnas.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.0kj1m.cn/gtpssfakhs.html

[D11] 反转数组
来源：http://hz.chenzaomai.com/gttspfbydo.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.wangshuangyany.cn/gtsecxepri.html

PHP:  array_reverse($arr);
来源：http://hz.52xcode.cn/gtegmofuky.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.birdmap.top/gtptllbohp.html

TS:   [...arr].reverse();
来源：http://hz.nwbrower.top/gtaczgftyy.html

Java: Collections.reverse(list);
来源：http://hz.dashuyun.cn/gtxnerxfbq.html

Go:   slices.Reverse(arr)
来源：http://hz.jqgfzy.top/gthejvfffq.html

Ruby: arr.reverse
来源：http://hz.havefunace.top/gtpolubsfn.html

C#:   list.Reverse();
来源：http://hz.dashuyun.cn/gtzrchonop.html

[D12] 查找元素下标
来源：http://hz.nanxinkj.top/gtpzaxgfeu.html

Py:   arr.index(x);  x in arr
来源：http://hz.dashuyun.cn/gtoorwhxba.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.yangfankeji.com/gtgemxkrul.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jinqigfzy.top/gtkrmagqpg.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.chenlongwang.top/gtztvgwdlw.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.yongpay.top/gtdjapjusc.html

Go:   slices.Index(arr, x)
来源：http://hz.ivvv.top/gtbthmaasc.html

Ruby: arr.index(x)
来源：http://hz.hongshengwenyu.top/gtwbibrxno.html

C#:   list.IndexOf(x);
来源：http://hz.vqdsnc.cn/gtmxtjjuka.html

[D13] 过滤（保留满足条件的）
来源：http://hz.jinghuilouyu.cn/gtcpixfqrt.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.quarkkingdee.top/gtryvowwxv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.hnxiangtu.top/gtfbfhumtg.html

JS:   arr.filter(x => x > 3)
来源：http://hz.jinqigufen.top/gtbmorxsfk.html

TS:   arr.filter(x => x > 3)
来源：http://hz.jyoumei.cn/gteofpizge.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.kuanghao11.cn/gthruvrocd.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.kuanghao11.cn/gtodthspuo.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.xuetiantiany.cn/gtijhjwuoz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.zhengqikj.top/gthvvgpxqk.html

[D14] 映射转换（每个元素变形）
来源：http://hz.yonumen.top/gtovfrxymg.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.aizwys.cn/gturbbpwjd.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.gogol.net.cn/gtvgmmyrlo.html

JS:   arr.map(x => x * 2)
来源：http://hz.hfpthk.cn/gtlyiyrlyv.html

TS:   arr.map(x => x * 2)
来源：http://hz.guannengcc.top/gtsulkmcgg.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.birdmap.top/gtaccaggwy.html

Go:   // 手写循环
来源：http://hz.shangyingyoupin.top/gtxkvlvjtu.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.birdmap.top/gtinbjakwg.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.zhoulong.xyz/gtychvewup.html

[D15] 去重
来源：http://hz.daria6918.cn/gtufjxpmkd.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.sysykeji.top/gtudkfhsix.html

PHP:  array_unique($arr);
来源：http://hz.fengsongda.top/gtqxshzxxi.html

JS:   [...new Set(arr)]
来源：http://hz.chenjidiqi.icu/gtyxkgbwdm.html

TS:   [...new Set(arr)]
来源：http://hz.iojbl.cn/gtuxxovwlj.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.aibaodan.cn/gtbvingwyn.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.yvedp.cn/gtlawmvolx.html

Ruby: arr.uniq
来源：http://hz.yuxming.cn/gtmfrwjhkf.html

C#:   list.Distinct().ToList()
来源：http://hz.c1oappe.top/gtkampdvev.html

[D16] 求和与平均值
来源：http://hz.wangshuangyany.cn/gtajjbhatv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.sxryk.cn/gtfhvuhjzk.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.yongpay.top/gtphbybtuy.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.sweek.top/gtygphwaon.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.kuanghao11.cn/gtbfybirfj.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.zdqjudy.top/gtrywzrece.html

Go:   // 手写循环累加
来源：http://hz.zhixingplan.top/gtejhmgbkl.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.yj20258888.top/gtclxyjtyz.html

C#:   list.Sum();  list.Average()
来源：http://hz.shanyushiyangkeji.top/gtbehabbvk.html

[D17] 最大值与最小值
来源：http://hz.pengpengdd.cyou/gtltzpxcwv.html

Py:   max(arr);  min(arr)
来源：http://hz.hfpthk.cn/gtyakorjak.html

PHP:  max($arr);  min($arr);
来源：http://hz.yueranfly.top/gtmqarxqaw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.hnxiangtu.top/gtirxjqcak.html

TS:   Math.max(...arr);
来源：http://hz.yueranfly.top/gtekpfwkvw.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.hfpthk.cn/gtqojnpuzm.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.chenlongwang.top/gtjeyzezyp.html

Ruby: arr.max;  arr.min
来源：http://hz.guowangkeji.top/gthfnjpvgd.html

C#:   list.Max();  list.Min()
来源：http://hz.hammf.cn/gtyrnvnsmp.html

[D18] 扁平化嵌套数组
来源：http://hz.316326.xyz/gtmjtrnkbx.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.gzhubu.top/gtbwzevelo.html

PHP:  array_merge(...$nested);
来源：http://hz.bjfxy.top/gtptxowgvy.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.nanxinkj.top/gtmqqnfbbw.html

TS:   nested.flat();
来源：http://hz.9152youxi.cn/gtapgbzpmz.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.hfpthk.cn/gtgxrtdfhg.html

Go:   // 手写双层循环
来源：http://hz.daxiang520.top/gtjhoihjjl.html

Ruby: nested.flatten
来源：http://hz.chenzaomai.com/gtjaedkcfk.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.52xcode.cn/gtebnrezyz.html

[D19] 按字段分组
来源：http://hz.hnxiangtu.top/gtvfhrvepg.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.sxryk.cn/gtqephncbv.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.yueranfly.top/gtjwqoazlt.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.chenlongwang.top/gtbmoimekt.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.xziqi.cn/gthojmrcvy.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.jinyuanbaomall.cn/gthzhmpdvh.html

Go:   // 手写 map[string][]T
来源：http://hz.sysykeji.top/gtlzjvpswl.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.gotoacloud.top/gtwhpactfi.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.ppjwa.cn/gtvxfvfneb.html

[D20] 统计每个元素出现次数
来源：http://hz.sweek.top/gtstbzaifh.html

Py:   Counter(arr)
来源：http://hz.dashuyun.cn/gtpbwpwrxc.html

PHP:  array_count_values($arr);
来源：http://hz.ywan-chungtsiang.top/gtkfzgatsx.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.shanyushiyangtech.top/gtlflcqhyx.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.daria6918.cn/gtztuscljz.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.tianlin.xyz/gtucgqbyfs.html

Go:   // 手写 map[T]int
来源：http://hz.cdnleiting.top/gtphtcwajn.html

Ruby: arr.tally
来源：http://hz.gaohongyu789.top/gtbiattkwf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.wangshuangyany.cn/gteiwzpzrk.html

[D21] 判断是否包含某元素
来源：http://hz.cheryme.top/gttukquopk.html

Py:   x in arr
来源：http://hz.nwbrower.top/gtvyxhwqcv.html

PHP:  in_array($x, $arr, true);
来源：http://hz.jinyuanbaomall.cn/gtsgbanlrh.html

JS:   arr.includes(x)
来源：http://hz.xylfe.cn/gtnbjajwdv.html

TS:   arr.includes(x)
来源：http://hz.yj202588.top/gtiwaicmnp.html

Java: list.contains(x)
来源：http://hz.jianghu66.top/gtcggauksk.html

Go:   slices.Contains(arr, x)
来源：http://hz.gzhubu.top/gtigtfmbno.html

Ruby: arr.include?(x)
来源：http://hz.gaohongyu789.top/gtqegcbkoo.html

C#:   list.Contains(x)
来源：http://hz.xuanzx.com/gtpzmvgqnz.html

[D22] 复制数组（避免共享引用）
来源：http://hz.ehwqpu.com/gtuuvycshg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.hysaishi.cn/gtjdvgvfsq.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.feifeiyinyue.top/gtnmpbtkrd.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.cashguo.top/gtxjdmzvmd.html

TS:   [...arr];
来源：http://hz.yonumen.top/gtcquizsuf.html

Java: new ArrayList<>(list);
来源：http://hz.tanke756.top/gtepbduunk.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.0kj1m.cn/gtovebceru.html

Ruby: arr.dup;  arr.clone
来源：http://hz.daxiang520.top/gtkufnummw.html

C#:   new List<int>(list);
来源：http://hz.hnqzz.top/gtwyrjuraf.html

[D23] reduce 累积计算
来源：http://hz.xingfuxueyuan.xyz/gtpuyqosth.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.shuidangran.top/gtlqrjrtvs.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.xinyue.icu/gtcuqaemjp.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.cdnleiting.top/gtxvdwpbdb.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.guowangkeji.top/gtuhdwytzu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.hywenlv.cn/gtpxpoazxy.html

Go:   // 手写循环
来源：http://hz.gotoacloud.top/gtoeijkctj.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.ppjwa.cn/gtxcqedyzm.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.yongpay.top/gttnwrhtlx.html

[D24] 字典 / Map 基本操作
来源：http://hz.nanxuanxn.top/gttkfhlcsk.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.daxiang520.top/gtdrsavfrx.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.wangshuangyany.cn/gtbmrklwpw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.cdnleiting.top/gtfhojrgvm.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.tian-w.cn/gthulbonth.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.pengpengdd.cyou/gtoakfntrn.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.hnqzz.top/gtsuyuzogh.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.vqdsnc.cn/gtegzaqepc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.gogol.net.cn/gtbclxhljb.html

[D25] Set 集合去重与交并差
来源：http://hz.0kj1m.cn/gtqnxydpft.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.gaohongyu789.top/gtdeyhfuss.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.cqqwz.cn/gthgrfrgyl.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.fzhhl.top/gtjqxymiux.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.fengsongda.top/gthzdpufck.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.smart0.xyz/gtqhoncxur.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.jianghu66.top/gtiiknyffh.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.ywan-chungtsiang.top/gtnadkduld.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.jinyuanbaomall.cn/gtmzoiofhi.html

[D26] 数组转字符串
来源：http://hz.daxiang520.top/gtkcbkqdpc.html

Py:   ", ".join(map(str, arr))
来源：http://hz.andypj.xyz/gtqxrpctbw.html

PHP:  implode(", ", $arr);
来源：http://hz.kuanghao11.cn/gtuvxjncxc.html

JS:   arr.join(", ")
来源：http://hz.jinqigfzy.top/gtomhiaeyj.html

TS:   arr.join(", ")
来源：http://hz.cqqwz.cn/gtuljjucje.html

Java: String.join(", ", list)
来源：http://hz.yuxming.cn/gtertsizrf.html

Go:   strings.Join(strs, ", ")
来源：http://hz.gzhubu.top/gtmvwflnur.html

Ruby: arr.join(", ")
来源：http://hz.smart0.xyz/gtocggpvra.html

C#:   string.Join(", ", list)
来源：http://hz.jyoumei.cn/gtzybuxdam.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtriqjxewe.html

E. 字符串处理
来源：http://hz.jiagoushi.top/gtvodkgrbg.html

================================================================================
来源：http://hz.hnqzz.top/gtkneneoxw.html

[E01] 拼接字符串
来源：http://hz.haohaochexian.top/gtbptciuqw.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.cashguo.top/gtgqbmowgw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.ivvv.top/gtfbpbemvn.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zhiwuduotai.top/gtryblbhwn.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.gzhubu.top/gtryqiorlo.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.ydzc1.top/gtlchjpdya.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.hfpthk.cn/gtjimvhzqw.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.meibo888.top/gtbundwlml.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.9152youxi.cn/gtxohxwnca.html

[E02] 重复字符串
来源：http://hz.guannengcc.top/gtkioxmqdr.html

Py:   "ab" * 3
来源：http://hz.mhx1999.top/gtzkbirhxu.html

PHP:  str_repeat("ab", 3);
来源：http://hz.yongpay.top/gtngkkeepi.html

JS:   "ab".repeat(3)
来源：http://hz.nanxuanxn.top/gtymhcxtbb.html

TS:   "ab".repeat(3)
来源：http://hz.wangdashe.top/gtwsrkvjzz.html

Java: "ab".repeat(3)
来源：http://hz.tian-w.cn/gtcuyrdqdg.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.hongshengwenyu.top/gtqlyrcetq.html

Ruby: "ab" * 3
来源：http://hz.cucudq.cn/gtqydqfqrs.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.yongpay.top/gtowfpxuwe.html

[E03] 截取子串
来源：http://hz.zhongyouzk.top/gtyyycartk.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.fzhhl.top/gteorwculh.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.0kj1m.cn/gtoqkoypia.html


<!-- 参考信息 -->