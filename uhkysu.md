代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://hz.yj202588.top/gtzkpteqci.html

Ruby: -> { puts "run" }.call
来源：http://hz.yj20258888.top/gtfqmlaiyl.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.daxiang520.top/gtypwwrgbk.html

[C13] 类型声明 / 类型注解
来源：http://hz.jqgfzy.top/gtamtsmxmc.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.gzhubu.top/gtlranmzsl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.pycfn.com/gtebjzijes.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.redwolf501.top/gthhdbtyqh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.shuidangran.top/gtloaxhmrm.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.daxiang520.top/gtoxduufdj.html

Go:   func add(a, b int) int
来源：http://hz.yonumen.top/gtkxwubrga.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.xingfuxueyuan.xyz/gtqgrlairi.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.jinghuilouyu.cn/gtrnenalsd.html

[C14] 泛型函数
来源：http://hz.quarkkingdee.top/gtuvbtkvcs.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.gzhubu.top/gtdomghpgi.html

PHP:  // 无泛型
来源：http://hz.chenzaomai.com/gtfdltrjqr.html

JS:   // 无泛型
来源：http://hz.shzxlz.cn/gtvnnkcbtq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.yj202588.top/gtqruqkwyi.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.meibo888.top/gtebthmncb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.ywan-chungtsiang.top/gtacjaqeph.html

Ruby: # 无泛型
来源：http://hz.hywenlv.cn/gtjzklxwjp.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.316326.xyz/gtywsmifte.html

[C15] 解构 / 展开参数
来源：http://hz.shzxlz.cn/gtphlmfnzs.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.hywenlv.cn/gtnemrrchu.html

PHP:  [$a, $b] = $pair;
来源：http://hz.yonumen.top/gtuerdmrmx.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.jiagoushi.top/gtlmoavswm.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.cqqwz.cn/gtfexufyzx.html

Java: // 无解构
来源：http://hz.chenzaomai.com/gtelrqkqkv.html

Go:   // 无解构
来源：http://hz.fengsongda.top/gtgcfxtgra.html

Ruby: a, b = pair
来源：http://hz.sxryk.cn/gtaqwtzjdw.html

C#:   var (a, b) = pair;
来源：http://hz.nanxinkj.top/gtqdcqjwsm.html

[C16] 函数 / 方法重载
来源：http://hz.ydzc1.top/gtjdcpvhvn.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.birdmap.top/gtbrrrkpcj.html

PHP:  // 无重载
来源：http://hz.xingfuxueyuan.xyz/gtualiyoer.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.guannengcc.top/gtkqtkcfht.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.aizwys.cn/gtkntdywxc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.dashuyun.cn/gtazmasqqm.html

Go:   // 无重载：用不同函数名
来源：http://hz.vqdsnc.cn/gtiqmkejlt.html

Ruby: # 无重载：靠动态参数
来源：http://hz.mhx1999.top/gtajikhtdy.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.hongshengwenyu.top/gtcgqyjfzt.html

================================================================================
来源：http://hz.ydjk.org.cn/gtxgcshpcp.html

D. 数组 / 列表 / 集合
来源：http://hz.zhongyouzk.top/gtlxdwwuyh.html

================================================================================
来源：http://hz.haohaochexian.top/gtseyasmnd.html

[D01] 创建数组 / 列表
来源：http://hz.sysykeji.top/gtrshlmkbc.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.snrcjt.cn/gtlvasikzy.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.aizwys.cn/gtxjicuexf.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.nanxuanxn.top/gthhpacwry.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.hysaishi.cn/gtztyiandn.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.guowangkeji.top/gtpeixyocj.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.xingfuxueyuan.xyz/gtvluerlso.html

Ruby: arr = [1, 2, 3]
来源：http://hz.zycfv.cn/gtvdvqnxcc.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.zhoulong.xyz/gtddjkzxmi.html

[D02] 追加元素到末尾
来源：http://hz.chenlongwang.top/gtiiuijull.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.xuanzx.com/gtwsnakvbr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.hfpthk.cn/gtkfukiapq.html

JS:   arr.push(4);
来源：http://hz.chenzaomai.com/gtfyjbdwhs.html

TS:   arr.push(4);
来源：http://hz.shanyushiyangkeji.top/gtwisrmwgl.html

Java: list.add(4);
来源：http://hz.dashuyun.cn/gtgxcojpuu.html

Go:   arr = append(arr, 4)
来源：http://hz.snrcjt.cn/gtqhmxeqxw.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.xuanzx.com/gtgiosbvih.html

C#:   list.Add(4);
来源：http://hz.dianchejie.cn/gtmscdscod.html

[D03] 在指定位置插入元素
来源：http://hz.yj20258.top/gtyfzkkbqi.html

Py:   arr.insert(0, 0)
来源：http://hz.andypj.xyz/gtwpcfwhil.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.ydjk.org.cn/gtcdwcpihy.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.guannengcc.top/gtzfkeimne.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.ppjwa.cn/gtvilrebcw.html

Java: list.add(0, 0);
来源：http://hz.hongshengwenyu.top/gtqsbqjcsh.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.zhoulong.xyz/gtuzusfkdx.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.jinghuilouyu.cn/gtghyjwwcl.html

C#:   list.Insert(0, 0);
来源：http://hz.fzhhl.top/gtrhjaveri.html

[D04] 删除元素
来源：http://hz.shzxlz.cn/gtcdsweyas.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.jlsjyb.cn/gterlzemvg.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.fzhhl.top/gtcjjuwyrt.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.guannengcc.top/gtfiawbwtc.html

TS:   arr.splice(0, 1);
来源：http://hz.hfpthk.cn/gtcgtotfor.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.jianghu66.top/gtcylqfqut.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.vqdsnc.cn/gttpdiihgj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.ivvv.top/gththvfvep.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.kuanghao11.cn/gtxunqljdv.html

[D05] 访问与修改元素
来源：http://hz.ivvv.top/gthqgrujav.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhengqikj.top/gtenvtxpzv.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.iojbl.cn/gtocllzwoo.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.jqgfzy.top/gtwlrrgjep.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.chenjidiqi.icu/gtjmlqvict.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.tianlin.xyz/gtywnmhosg.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.yongpay.top/gtmreigido.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yj20258888.top/gtposuvskd.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.ivvv.top/gtbywweyuq.html

[D06] 数组长度
来源：http://hz.haohaochexian.top/gtcjyyzojr.html

Py:   len(arr)
来源：http://hz.gzhubu.top/gtkjqnloyz.html

PHP:  count($arr);
来源：http://hz.yj202588.top/gtdtvbqnmj.html

JS:   arr.length
来源：http://hz.sxryk.cn/gtqtcmkujj.html

TS:   arr.length
来源：http://hz.gogol.net.cn/gtgnlvahaa.html

Java: list.size();
来源：http://hz.hongshengwenyu.top/gtumpzbcjm.html

Go:   len(arr)
来源：http://hz.birdmap.top/gtirnbpylw.html

Ruby: arr.length; arr.size
来源：http://hz.gzhubu.top/gtkrddfgzz.html

C#:   list.Count;
来源：http://hz.kuanghao11.cn/gtubjhzohf.html

[D07] 切片 / 取子数组
来源：http://hz.smart0.xyz/gtkqwzpvsr.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.shangyingyoupin.top/gtlhqokyzr.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.bjfxy.top/gtfzervcqb.html

JS:   arr.slice(1, 4);
来源：http://hz.sufxvd.cn/gtjnmddxwd.html

TS:   arr.slice(1, 4);
来源：http://hz.hfpthk.cn/gttxsiimyg.html

Java: list.subList(1, 4);
来源：http://hz.tanke756.top/gtyqjhtjyy.html

Go:   arr[1:4]
来源：http://hz.jinqigfzy.top/gtvdhabxvu.html

Ruby: arr[1, 3]
来源：http://hz.chenjidiqi.icu/gtuuuygvro.html

C#:   list.GetRange(1, 3);
来源：http://hz.daria6918.cn/gtmbkzdlkj.html

[D08] 合并两个数组
来源：http://hz.xylfe.cn/gtrdpnmbkq.html

Py:   a + b;  a.extend(b)
来源：http://hz.sufxvd.cn/gtyxtejwnl.html

PHP:  array_merge($a, $b);
来源：http://hz.52xcode.cn/gttydoyvnz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.sufxvd.cn/gtiyjemskj.html

TS:   [...a, ...b];
来源：http://hz.ydjk.org.cn/gtbvhtkxga.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.havefunace.top/gtwdtgjklt.html

Go:   append(a, b...)
来源：http://hz.jianghu66.top/gtnauejmri.html

Ruby: a + b;  a.concat(b)
来源：http://hz.xingfuxueyuan.xyz/gtondwcixx.html

C#:   a.Concat(b).ToList()
来源：http://hz.tianlin.xyz/gtprbnwsba.html

[D09] 排序（升序）
来源：http://hz.hywenlv.cn/gtetcrarli.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ivvv.top/gtmkztmyxp.html

PHP:  sort($arr);
来源：http://hz.zycfv.cn/gtmbeqqyiw.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.meibo888.top/gtwszhdczg.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.zhaomingkeji.xyz/gtnkkpiuap.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.yuanzhike.top/gtapwnqifj.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.fengsongda.top/gtltrgxtnh.html

Ruby: arr.sort
来源：http://hz.9152youxi.cn/gtofwcvdbt.html

C#:   list.Sort();
来源：http://hz.ybcxt.top/gtlxfxsmgn.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.chenzaomai.com/gtkwxtcgky.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.jqgfzy.top/gtjbtebggk.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.hongshengwenyu.top/gtfeyynuvq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.cucudq.cn/gtzqxmcmtz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hywenlv.cn/gtannrqyzz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.bjfxy.top/gthpniwkgf.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.sufxvd.cn/gttcvnlnjh.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.tanke756.top/gtsmgrhjye.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.zdqjudy.top/gthxyfotav.html

[D11] 反转数组
来源：http://hz.jqgufenzy.top/gtspqkmpgz.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.dashuyun.cn/gttnopragi.html

PHP:  array_reverse($arr);
来源：http://hz.zhongyouzk.top/gttaaxsfnz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.xziqi.cn/gtnhxoqyno.html

TS:   [...arr].reverse();
来源：http://hz.9152youxi.cn/gtwakwzykn.html

Java: Collections.reverse(list);
来源：http://hz.xylfe.cn/gtttlbblpx.html

Go:   slices.Reverse(arr)
来源：http://hz.ivvv.top/gtszwnpejj.html

Ruby: arr.reverse
来源：http://hz.snrcjt.cn/gtgbpfrubw.html

C#:   list.Reverse();
来源：http://hz.snrcjt.cn/gtoxqfpcfn.html

[D12] 查找元素下标
来源：http://hz.pycfn.com/gtntaeaueq.html

Py:   arr.index(x);  x in arr
来源：http://hz.yj202588.top/gtxsquxwuv.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.wangdashe.top/gtecmzpwae.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.gaohongyu789.top/gtfermmeni.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.wangdashe.top/gtnjerfmtp.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.hammf.cn/gtqrogssuo.html

Go:   slices.Index(arr, x)
来源：http://hz.zhoulong.xyz/gtxnozptmw.html

Ruby: arr.index(x)
来源：http://hz.haohaochexian.top/gtjkpagjkv.html

C#:   list.IndexOf(x);
来源：http://hz.fzhhl.top/gtwhzbjixj.html

[D13] 过滤（保留满足条件的）
来源：http://hz.zhoulong.xyz/gtlsbcqrvf.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.shangyingyoupin.top/gtzhucplvu.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.xinyue.icu/gtxayhuhcr.html

JS:   arr.filter(x => x > 3)
来源：http://hz.daria6918.cn/gterkuiexv.html

TS:   arr.filter(x => x > 3)
来源：http://hz.smart0.xyz/gtdwzhipda.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.c1oappe.top/gtwadcowdl.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.cashguo.top/gthfbihswe.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.svipenyu.cn/gtyjkvawck.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.yj20258.top/gtcxlrgnuw.html

[D14] 映射转换（每个元素变形）
来源：http://hz.svipenyu.cn/gtywictzxn.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.havefunace.top/gtolhafdzm.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.vqdsnc.cn/gtmerdxcuu.html

JS:   arr.map(x => x * 2)
来源：http://hz.zhongyouzk.top/gthqlmumuh.html

TS:   arr.map(x => x * 2)
来源：http://hz.wangdashe.top/gtrrlahejx.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.gogol.net.cn/gtfshhyzjf.html

Go:   // 手写循环
来源：http://hz.cheryme.top/gtmpujdris.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.ehwqpu.com/gtweupugqo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.yuanzhike.top/gtpzcmapds.html

[D15] 去重
来源：http://hz.jinqigfzy.top/gtkicpvkdt.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.meibo888.top/gteckxxdjz.html

PHP:  array_unique($arr);
来源：http://hz.gaohongyu789.top/gtygsvpzsk.html

JS:   [...new Set(arr)]
来源：http://hz.hnqzz.top/gthvajgdku.html

TS:   [...new Set(arr)]
来源：http://hz.hywenlv.cn/gtufywhftz.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.daxiang520.top/gtsykspjnr.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.nanxinkj.top/gtzhhoitjq.html

Ruby: arr.uniq
来源：http://hz.xuetiantiany.cn/gtpdetcvoh.html

C#:   list.Distinct().ToList()
来源：http://hz.c1oappe.top/gtbrgqwuaw.html

[D16] 求和与平均值
来源：http://hz.cashguo.top/gtaywiddrd.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.jinqigufen.top/gtwshiubyb.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.nanxuanxn.top/gtsamjcluh.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.xuetiantiany.cn/gtkoftdgxk.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.daria6918.cn/gtkkumhiyn.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.shangyingyoupin.top/gtzwofoqpi.html

Go:   // 手写循环累加
来源：http://hz.ydzc1.top/gtwnqawrrn.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.ywan-chungtsiang.top/gtiwpxybru.html

C#:   list.Sum();  list.Average()
来源：http://hz.pycfn.com/gtfqmarjak.html

[D17] 最大值与最小值
来源：http://hz.yongpay.top/gtkacbigvz.html

Py:   max(arr);  min(arr)
来源：http://hz.hnqzz.top/gtchvgykkl.html

PHP:  max($arr);  min($arr);
来源：http://hz.guowangkeji.top/gtvymvqpvh.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.havefunace.top/gthixpbfar.html

TS:   Math.max(...arr);
来源：http://hz.tianlin.xyz/gtifvhrafx.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.jyoumei.cn/gtmqfnbxvx.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.cheryme.top/gtkwwvwfxf.html

Ruby: arr.max;  arr.min
来源：http://hz.hywenlv.cn/gtllpjitkx.html

C#:   list.Max();  list.Min()
来源：http://hz.guannengcc.top/gtxjyjmiag.html

[D18] 扁平化嵌套数组
来源：http://hz.chenjidiqi.icu/gtfvsswhpb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.316326.xyz/gtkgsqlqsp.html

PHP:  array_merge(...$nested);
来源：http://hz.jinghuilouyu.cn/gtapvgzjqa.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.cheryme.top/gtuolcjbsc.html

TS:   nested.flat();
来源：http://hz.nanxinkj.top/gtnbiqnwqa.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.ydjk.org.cn/gtydifxkbg.html

Go:   // 手写双层循环
来源：http://hz.cucudq.cn/gtldtfgbwn.html

Ruby: nested.flatten
来源：http://hz.dashuyun.cn/gtfoooselq.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.sweek.top/gtngkmmaks.html

[D19] 按字段分组
来源：http://hz.zdqjudy.top/gtvrxedzyn.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.aizwys.cn/gtvizujicu.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.zhongyouzk.top/gtvwwlfivl.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.c1oappe.top/gtqafzifrn.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.hysaishi.cn/gtlgqaalha.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.chenzaomai.com/gtrzwsknne.html

Go:   // 手写 map[string][]T
来源：http://hz.yj202588.top/gtpmeubgsn.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.jinqigfzy.top/gtemiylwju.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.ydzc1.top/gtvgnkpdec.html

[D20] 统计每个元素出现次数
来源：http://hz.jyoumei.cn/gtdtwuwnxu.html

Py:   Counter(arr)
来源：http://hz.aizwys.cn/gtptkoygdn.html

PHP:  array_count_values($arr);
来源：http://hz.tianlin.xyz/gtqlqgtnjn.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.havefunace.top/gtbiirhpxs.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yueranfly.top/gtyhldttqu.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.snrcjt.cn/gtvmhvwgtg.html

Go:   // 手写 map[T]int
来源：http://hz.aibaodan.cn/gtmsxdojip.html

Ruby: arr.tally
来源：http://hz.kuanghao11.cn/gtiqsweuzr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.smart0.xyz/gtkzceakfp.html

[D21] 判断是否包含某元素
来源：http://hz.feifeiyinyue.top/gtdhfzgtlz.html

Py:   x in arr
来源：http://hz.svipenyu.cn/gtygezokdz.html

PHP:  in_array($x, $arr, true);
来源：http://hz.yanxiufei.cn/gtoaaasjxw.html

JS:   arr.includes(x)
来源：http://hz.ywan-chungtsiang.top/gtwjkwgwse.html

TS:   arr.includes(x)
来源：http://hz.yueranfly.top/gtitpehcgt.html

Java: list.contains(x)
来源：http://hz.52xcode.cn/gtowwpxxyw.html

Go:   slices.Contains(arr, x)
来源：http://hz.tian-w.cn/gttyyqxfbx.html

Ruby: arr.include?(x)
来源：http://hz.jiagoushi.top/gtiawzhoob.html

C#:   list.Contains(x)
来源：http://hz.hysaishi.cn/gtjfmbvqte.html

[D22] 复制数组（避免共享引用）
来源：http://hz.ywan-chungtsiang.top/gtefeuyapb.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.c1oappe.top/gtdwvcuuly.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.xylfe.cn/gtiyphltcs.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.snrcjt.cn/gtowklspqv.html

TS:   [...arr];
来源：http://hz.mhx1999.top/gtmkxgpges.html

Java: new ArrayList<>(list);
来源：http://hz.zhixingplan.top/gtddyettud.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.jqgfzy.top/gtdhielsqn.html

Ruby: arr.dup;  arr.clone
来源：http://hz.wangshuangyany.cn/gtrjmkmmvi.html

C#:   new List<int>(list);
来源：http://hz.jyoumei.cn/gtlwverqzs.html

[D23] reduce 累积计算
来源：http://hz.ehwqpu.com/gtvabyhlht.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.sxryk.cn/gtpozrdxxa.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.gaohongyu789.top/gthsdvkttw.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhengqikj.top/gtsgtxycxz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.9152youxi.cn/gtqxuaatcb.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.wangshuangyany.cn/gtaulxnruc.html

Go:   // 手写循环
来源：http://hz.wangshuangyany.cn/gtikqlesrg.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.316326.xyz/gtgcbjqvdw.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.316326.xyz/gtorlfiqpc.html

[D24] 字典 / Map 基本操作
来源：http://hz.cqqwz.cn/gtrctkheir.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.shzxlz.cn/gtreatwcqk.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.shanyushiyangkeji.top/gtqcpothrk.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.yj202588.top/gtwdmllnol.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.52xcode.cn/gtubypqryo.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.yuxming.cn/gtakydshra.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.guowangkeji.top/gtpqmlydev.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.wangshuangyany.cn/gtwmlscxnc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.snrcjt.cn/gtqijgpztv.html

[D25] Set 集合去重与交并差
来源：http://hz.yonumen.top/gtcsololzw.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.jlsjyb.cn/gtlvxbqurs.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.jinyuanbaomall.cn/gthhxwxftu.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.hnqzz.top/gtpunsjctr.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.chenlongwang.top/gtywqhhaka.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.smart0.xyz/gtszqdkfuu.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.tianlin.xyz/gtbazssykk.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.ywan-chungtsiang.top/gtdmkwmndm.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.feifeiyinyue.top/gtzfqtqava.html

[D26] 数组转字符串
来源：http://hz.yangfankeji.com/gtsarocgxz.html

Py:   ", ".join(map(str, arr))
来源：http://hz.xuanzx.com/gtyhsqelgs.html

PHP:  implode(", ", $arr);
来源：http://hz.c1oappe.top/gttwdrtyrr.html

JS:   arr.join(", ")
来源：http://hz.mhx1999.top/gtnzcfzift.html

TS:   arr.join(", ")
来源：http://hz.xziqi.cn/gturyzhbdl.html

Java: String.join(", ", list)
来源：http://hz.hysaishi.cn/gtlmoymlxk.html

Go:   strings.Join(strs, ", ")
来源：http://hz.yuxming.cn/gtyozfpuhq.html

Ruby: arr.join(", ")
来源：http://hz.guannengcc.top/gtfhhminpx.html

C#:   string.Join(", ", list)
来源：http://hz.guowangkeji.top/gtfonxdoxy.html

================================================================================
来源：http://hz.quarkkingdee.top/gtiuloncnn.html

E. 字符串处理
来源：http://hz.yj202588.top/gtbaqtpuec.html

================================================================================
来源：http://hz.hysaishi.cn/gtbcpgfaul.html

[E01] 拼接字符串
来源：http://hz.tanke756.top/gtqjmlbdbw.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.zhijiandao.cn/gtweazzebk.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.mhx1999.top/gtmugtekki.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.316326.xyz/gtcpycuzvd.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.gotoacloud.top/gtsdqnadpb.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.9152youxi.cn/gtczebosdd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.sufxvd.cn/gtkesqtejz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.tian-w.cn/gtbdvujiyz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.0kj1m.cn/gtwuxqrdli.html

[E02] 重复字符串
来源：http://hz.0kj1m.cn/gtonyylgse.html

Py:   "ab" * 3
来源：http://hz.ywan-chungtsiang.top/gtpldzwdwy.html

PHP:  str_repeat("ab", 3);
来源：http://hz.jinqigufen.top/gtquoschju.html

JS:   "ab".repeat(3)
来源：http://hz.quarkkingdee.top/gtgjlbdimn.html

TS:   "ab".repeat(3)
来源：http://hz.dianchejie.cn/gtbvrufsdw.html

Java: "ab".repeat(3)
来源：http://hz.nanxuanxn.top/gtcjtcernp.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.52xcode.cn/gtyztrhvnc.html

Ruby: "ab" * 3
来源：http://hz.shanyushiyangtech.top/gtazmeahhu.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.yvedp.cn/gtabeixcix.html

[E03] 截取子串
来源：http://hz.yj20258888.top/gtubufkabe.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.iojbl.cn/gtzxnbbepq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.aibaodan.cn/gtxaezdtar.html


<!-- 参考信息 -->