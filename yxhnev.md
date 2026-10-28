代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://hz.xuetiantiany.cn/gtrcxegqtx.html

JS:   (() => { console.log("run"); })();
来源：http://hz.dashuyun.cn/gtsswuxvcb.html

TS:   (() => { console.log("run"); })();
来源：http://hz.jinghuilouyu.cn/gtxpqgjdcz.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.316326.xyz/gtxqxjbyxb.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.hywenlv.cn/gtycnkkefl.html

Ruby: -> { puts "run" }.call
来源：http://hz.birdmap.top/gtvhwyemqn.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.sweek.top/gtjezcwngt.html

[C13] 类型声明 / 类型注解
来源：http://hz.guannengcc.top/gtoibhwmfe.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.ywan-chungtsiang.top/gteatstsew.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.daxiang520.top/gtykgwkkgj.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.xinyue.icu/gtjdovhqbl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yuxming.cn/gtuitlhazg.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.ehwqpu.com/gtkalvplkx.html

Go:   func add(a, b int) int
来源：http://hz.shanyushiyangtech.top/gtdsxqcoif.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.jiagoushi.top/gtpcluiaov.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.nanxuanxn.top/gthjsegepo.html

[C14] 泛型函数
来源：http://hz.yj20258.top/gtkipiimpp.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.xuetiantiany.cn/gtrgsllmrk.html

PHP:  // 无泛型
来源：http://hz.zhongyouzk.top/gtqqioxvmx.html

JS:   // 无泛型
来源：http://hz.xuetiantiany.cn/gtuuhwkmoi.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.xuanzx.com/gtbllzcmcj.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.tian-w.cn/gtjvcipndq.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.jqgufenzy.top/gtegnxkejc.html

Ruby: # 无泛型
来源：http://hz.gogol.net.cn/gtyahnkjem.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.gotoacloud.top/gtpvnvwqop.html

[C15] 解构 / 展开参数
来源：http://hz.hnqzz.top/gtuzzhdxsq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.ydjk.org.cn/gtebpbsnzm.html

PHP:  [$a, $b] = $pair;
来源：http://hz.hnxiangtu.top/gtjjzwndlq.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.mhx1999.top/gtcwtfdmvu.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.jinqigfzy.top/gticvwgmgu.html

Java: // 无解构
来源：http://hz.yj20258888.top/gtuwhjxfze.html

Go:   // 无解构
来源：http://hz.birdmap.top/gtvgqojlww.html

Ruby: a, b = pair
来源：http://hz.shanyushiyangkeji.top/gtarohogtb.html

C#:   var (a, b) = pair;
来源：http://hz.pengpengdd.cyou/gtcafbwzbu.html

[C16] 函数 / 方法重载
来源：http://hz.nanxinkj.top/gtqkaidrmv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.vqdsnc.cn/gtkbcobgsr.html

PHP:  // 无重载
来源：http://hz.hfpthk.cn/gtiygmxgdt.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.shuidangran.top/gteeawuirx.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.yonumen.top/gtixzyhxrq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.cdnleiting.top/gtwhlgxzoe.html

Go:   // 无重载：用不同函数名
来源：http://hz.hysaishi.cn/gtdqczycgd.html

Ruby: # 无重载：靠动态参数
来源：http://hz.nanxuanxn.top/gtevyhmvkh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.chenzaomai.com/gtvnofhlex.html

================================================================================
来源：http://hz.tian-w.cn/gtljuqqhxc.html

D. 数组 / 列表 / 集合
来源：http://hz.andypj.xyz/gteinaygqx.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtivwrlgqp.html

[D01] 创建数组 / 列表
来源：http://hz.wangdashe.top/gtzbsofzxs.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.snrcjt.cn/gtnudrzcix.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.shuidangran.top/gtnltqdgtl.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.hysaishi.cn/gtkqmcoygi.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.fengsongda.top/gtkbizbuqa.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.hywenlv.cn/gtypibzkfb.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.sufxvd.cn/gthtotwtmw.html

Ruby: arr = [1, 2, 3]
来源：http://hz.yuxming.cn/gtetzeqqmo.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.vqdsnc.cn/gtllvawrgm.html

[D02] 追加元素到末尾
来源：http://hz.nanxinkj.top/gtvmundmxf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.snrcjt.cn/gtgqttzqqp.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.hfpthk.cn/gttejwefju.html

JS:   arr.push(4);
来源：http://hz.ppjwa.cn/gtuizbsaho.html

TS:   arr.push(4);
来源：http://hz.jqgfzy.top/gtzgtmaxcm.html

Java: list.add(4);
来源：http://hz.tanke756.top/gtszodmygm.html

Go:   arr = append(arr, 4)
来源：http://hz.aibaodan.cn/gtlzmrcbko.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.daxiang520.top/gtozdewjns.html

C#:   list.Add(4);
来源：http://hz.sufxvd.cn/gtaufhtkns.html

[D03] 在指定位置插入元素
来源：http://hz.haohaochexian.top/gtezupbmdx.html

Py:   arr.insert(0, 0)
来源：http://hz.quarkkingdee.top/gtzfwqvlsr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.zhongyouzk.top/gtftcljgdg.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.jlsjyb.cn/gtrmjfhrlw.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.hysaishi.cn/gtwoxhmbvw.html

Java: list.add(0, 0);
来源：http://hz.zhongyouzk.top/gtpnbtnahe.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.ehwqpu.com/gtahtnowvj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.sysykeji.top/gtaaraobyp.html

C#:   list.Insert(0, 0);
来源：http://hz.andypj.xyz/gtscxgguao.html

[D04] 删除元素
来源：http://hz.quarkkingdee.top/gtfkutapij.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.ydzc1.top/gtsipeoafk.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.aibaodan.cn/gtwwdvlsag.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.yuanzhike.top/gtiylrlumb.html

TS:   arr.splice(0, 1);
来源：http://hz.xuetiantiany.cn/gtxupcduei.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.hysaishi.cn/gtzivpwthl.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.gaohongyu789.top/gtmuuyoowj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.52xcode.cn/gtyxopfgev.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.sysykeji.top/gtwnwhkgus.html

[D05] 访问与修改元素
来源：http://hz.wangdashe.top/gtmvcyoxvi.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yuanzhike.top/gtlrppmuko.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.ehwqpu.com/gttronbqal.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.yangfankeji.com/gtvndbssif.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.fengsongda.top/gtaotzqtuj.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.xingfuxueyuan.xyz/gtoaxxybec.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.kuanghao11.cn/gteudmxdab.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zdqjudy.top/gtvwxwikka.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.wangshuangyany.cn/gtiizozizp.html

[D06] 数组长度
来源：http://hz.jinyuanbaomall.cn/gtjchvarqm.html

Py:   len(arr)
来源：http://hz.zhoulong.xyz/gtgsipivwl.html

PHP:  count($arr);
来源：http://hz.gotoacloud.top/gtuyvrxxby.html

JS:   arr.length
来源：http://hz.jyoumei.cn/gtrqnclmmz.html

TS:   arr.length
来源：http://hz.jqgufenzy.top/gtdkrwwygp.html

Java: list.size();
来源：http://hz.xuetiantiany.cn/gtoabymvhd.html

Go:   len(arr)
来源：http://hz.ydjk.org.cn/gtcfchsufx.html

Ruby: arr.length; arr.size
来源：http://hz.zdqjudy.top/gteybkkucy.html

C#:   list.Count;
来源：http://hz.sufxvd.cn/gtczocqtot.html

[D07] 切片 / 取子数组
来源：http://hz.gzhubu.top/gtmomquaaa.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.zhijiandao.cn/gtitdqqqou.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.zhoulong.xyz/gtywfzwhio.html

JS:   arr.slice(1, 4);
来源：http://hz.jianghu66.top/gtdrcttzeq.html

TS:   arr.slice(1, 4);
来源：http://hz.yangfankeji.com/gtlkqxyhby.html

Java: list.subList(1, 4);
来源：http://hz.shanyushiyangkeji.top/gtdotbzosu.html

Go:   arr[1:4]
来源：http://hz.yj20258.top/gtbaulgqjr.html

Ruby: arr[1, 3]
来源：http://hz.ydzc1.top/gtiuijqkqg.html

C#:   list.GetRange(1, 3);
来源：http://hz.cdnleiting.top/gtinctcjhm.html

[D08] 合并两个数组
来源：http://hz.yongpay.top/gtzjjusucz.html

Py:   a + b;  a.extend(b)
来源：http://hz.xingfuxueyuan.xyz/gtksupzgeu.html

PHP:  array_merge($a, $b);
来源：http://hz.mhx1999.top/gtwvabwtez.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.yj20258888.top/gtqecgznsk.html

TS:   [...a, ...b];
来源：http://hz.ybcxt.top/gtdbdevvrj.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.daxiang520.top/gtsrxxacok.html

Go:   append(a, b...)
来源：http://hz.vqdsnc.cn/gtlejylaeu.html

Ruby: a + b;  a.concat(b)
来源：http://hz.nanxuanxn.top/gtgoovcakv.html

C#:   a.Concat(b).ToList()
来源：http://hz.birdmap.top/gtqmtwklol.html

[D09] 排序（升序）
来源：http://hz.xziqi.cn/gtapscpsiz.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.pycfn.com/gthnqbezkv.html

PHP:  sort($arr);
来源：http://hz.ehwqpu.com/gtivalycqb.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.hammf.cn/gtbofesedw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.yongpay.top/gtlvkmhpza.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.ybcxt.top/gtgayjgald.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.havefunace.top/gtfcbqfnjg.html

Ruby: arr.sort
来源：http://hz.snrcjt.cn/gtnqrcrmac.html

C#:   list.Sort();
来源：http://hz.tianlin.xyz/gtfxyqrzym.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.ywan-chungtsiang.top/gtzidcorgw.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.jlsjyb.cn/gttzhlveyb.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zhongyouzk.top/gtfclhuweu.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jinghuilouyu.cn/gtvpawyouw.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.haohaochexian.top/gtilidloaz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.xingfuxueyuan.xyz/gtbixobjrq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.ybcxt.top/gtifoirjwb.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.ivvv.top/gttpfjlhmi.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.feifeiyinyue.top/gtcuvqupfo.html

[D11] 反转数组
来源：http://hz.chenlongwang.top/gtbexvedrs.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.jinghuilouyu.cn/gtxxcgxask.html

PHP:  array_reverse($arr);
来源：http://hz.cheryme.top/gtymefdgjk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.shuidangran.top/gtkuhaepzt.html

TS:   [...arr].reverse();
来源：http://hz.jinqigufen.top/gtmpqvyaga.html

Java: Collections.reverse(list);
来源：http://hz.yonumen.top/gtsuovmtev.html

Go:   slices.Reverse(arr)
来源：http://hz.ydzc1.top/gtkptsgrjc.html

Ruby: arr.reverse
来源：http://hz.fengsongda.top/gtwnpjaurd.html

C#:   list.Reverse();
来源：http://hz.tian-w.cn/gtpiuvkhgk.html

[D12] 查找元素下标
来源：http://hz.mhx1999.top/gtgfstvmeq.html

Py:   arr.index(x);  x in arr
来源：http://hz.xinyue.icu/gtrqetiodt.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.mhx1999.top/gtgbfwvokx.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zycfv.cn/gtgtrbsllj.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.cheryme.top/gtocofundb.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.pycfn.com/gtdweszden.html

Go:   slices.Index(arr, x)
来源：http://hz.sysykeji.top/gtagunmdyv.html

Ruby: arr.index(x)
来源：http://hz.zhoulong.xyz/gtnmtecjbs.html

C#:   list.IndexOf(x);
来源：http://hz.dianchejie.cn/gtsbrplhco.html

[D13] 过滤（保留满足条件的）
来源：http://hz.chenjidiqi.icu/gttbhnwtbp.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.zdqjudy.top/gtkoonfiki.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.cdnleiting.top/gtjvhzdvmo.html

JS:   arr.filter(x => x > 3)
来源：http://hz.jiagoushi.top/gtkuadwygl.html

TS:   arr.filter(x => x > 3)
来源：http://hz.smart0.xyz/gtslfomkwo.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.ywan-chungtsiang.top/gtsxrqdtao.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.jinqigufen.top/gttautkymg.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.sufxvd.cn/gtczmtqmqc.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.sxryk.cn/gtrxvjxqwd.html

[D14] 映射转换（每个元素变形）
来源：http://hz.wangshuangyany.cn/gtdiejnxtu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.xuanzx.com/gtgbxbcvjm.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.shanyushiyangtech.top/gtkvtnbeqd.html

JS:   arr.map(x => x * 2)
来源：http://hz.aizwys.cn/gtbbcvkqew.html

TS:   arr.map(x => x * 2)
来源：http://hz.hysaishi.cn/gtzyvzypky.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.xinyue.icu/gtdecvytjt.html

Go:   // 手写循环
来源：http://hz.yuanzhike.top/gtwjmyakpq.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.pycfn.com/gtxdytcmcd.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.fzhhl.top/gtktvmbfjr.html

[D15] 去重
来源：http://hz.dianchejie.cn/gthvnbxjuw.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.jlsjyb.cn/gtyseoxgql.html

PHP:  array_unique($arr);
来源：http://hz.shanyushiyangkeji.top/gtkxhotqdy.html

JS:   [...new Set(arr)]
来源：http://hz.jyoumei.cn/gtwgqkxrxm.html

TS:   [...new Set(arr)]
来源：http://hz.jinqigfzy.top/gtopkwnkob.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.mhx1999.top/gtggeswwpt.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.tian-w.cn/gtuyauforn.html

Ruby: arr.uniq
来源：http://hz.xinyue.icu/gtzcecqill.html

C#:   list.Distinct().ToList()
来源：http://hz.hywenlv.cn/gtnggbmmgn.html

[D16] 求和与平均值
来源：http://hz.zhengqikj.top/gtxhxhdueb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.ydzc1.top/gtefqlrmej.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.fengsongda.top/gtxnmrofyo.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zhijiandao.cn/gtmsonhouj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.smart0.xyz/gtxiaiqolu.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.xuetiantiany.cn/gtpywhcnli.html

Go:   // 手写循环累加
来源：http://hz.jinghuilouyu.cn/gtbhpfaotf.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.yangfankeji.com/gtepmqjrmv.html

C#:   list.Sum();  list.Average()
来源：http://hz.shanyushiyangkeji.top/gtfxcxqjyt.html

[D17] 最大值与最小值
来源：http://hz.chenzaomai.com/gtulixmqfu.html

Py:   max(arr);  min(arr)
来源：http://hz.kuanghao11.cn/gtstmjupnr.html

PHP:  max($arr);  min($arr);
来源：http://hz.9152youxi.cn/gtgqtzdcou.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.birdmap.top/gtdnzwevxj.html

TS:   Math.max(...arr);
来源：http://hz.xuetiantiany.cn/gtslczglyt.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.yuxming.cn/gtjkyznbhy.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.dashuyun.cn/gtnwdbvkbo.html

Ruby: arr.max;  arr.min
来源：http://hz.yj20258888.top/gtyoyhrqda.html

C#:   list.Max();  list.Min()
来源：http://hz.nwbrower.top/gtrotjafbr.html

[D18] 扁平化嵌套数组
来源：http://hz.daxiang520.top/gtbxbygxue.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.xinyue.icu/gtozwiemkv.html

PHP:  array_merge(...$nested);
来源：http://hz.nanxinkj.top/gtmkkjriik.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.wangdashe.top/gtloflewzd.html

TS:   nested.flat();
来源：http://hz.aizwys.cn/gtxpsytwhx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.andypj.xyz/gttexeqodi.html

Go:   // 手写双层循环
来源：http://hz.hongshengwenyu.top/gtlbggpukm.html

Ruby: nested.flatten
来源：http://hz.redwolf501.top/gtnhcdwyjg.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.wangshuangyany.cn/gtobhkneuf.html

[D19] 按字段分组
来源：http://hz.zycfv.cn/gttaplfqom.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.andypj.xyz/gtzcixlpfb.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.shanyushiyangtech.top/gtdxdrcfch.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.quarkkingdee.top/gtracheofo.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.shanyushiyangtech.top/gtlfpifrvr.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.zhiwuduotai.top/gtkpquzuqt.html

Go:   // 手写 map[string][]T
来源：http://hz.yuxming.cn/gtvugbjjzk.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.gzhubu.top/gtxxkigpqc.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.wangshuangyany.cn/gtovhlslrr.html

[D20] 统计每个元素出现次数
来源：http://hz.yueranfly.top/gtkshupqkr.html

Py:   Counter(arr)
来源：http://hz.chenzaomai.com/gtsuvxkisz.html

PHP:  array_count_values($arr);
来源：http://hz.9152youxi.cn/gtpkbdlszd.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.svipenyu.cn/gtbnoffryi.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.cheryme.top/gtuvzbzita.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.zhiwuduotai.top/gttvapspgx.html

Go:   // 手写 map[T]int
来源：http://hz.yuxming.cn/gtaypmzghc.html

Ruby: arr.tally
来源：http://hz.zhaomingkeji.xyz/gtnllwslds.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.havefunace.top/gtalttmvan.html

[D21] 判断是否包含某元素
来源：http://hz.zhengqikj.top/gtldzbcnyq.html

Py:   x in arr
来源：http://hz.nanxuanxn.top/gtbivkukbc.html

PHP:  in_array($x, $arr, true);
来源：http://hz.tian-w.cn/gtqyjsvtnn.html

JS:   arr.includes(x)
来源：http://hz.0kj1m.cn/gtoduhsxym.html

TS:   arr.includes(x)
来源：http://hz.nwbrower.top/gtqiswuaug.html

Java: list.contains(x)
来源：http://hz.yangfankeji.com/gtmetkzzat.html

Go:   slices.Contains(arr, x)
来源：http://hz.sweek.top/gtzycniqib.html

Ruby: arr.include?(x)
来源：http://hz.316326.xyz/gtfxkrsapu.html

C#:   list.Contains(x)
来源：http://hz.xingfuxueyuan.xyz/gteqkkyaji.html

[D22] 复制数组（避免共享引用）
来源：http://hz.hnxiangtu.top/gtgqzqvftt.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.jyoumei.cn/gtpibohimu.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.chenlongwang.top/gtiyoblyjq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.c1oappe.top/gttsvlkbpn.html

TS:   [...arr];
来源：http://hz.52xcode.cn/gtmdyrdenn.html

Java: new ArrayList<>(list);
来源：http://hz.snrcjt.cn/gtqjqapemr.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.yonumen.top/gtfluarvhu.html

Ruby: arr.dup;  arr.clone
来源：http://hz.cucudq.cn/gtftjexrlq.html

C#:   new List<int>(list);
来源：http://hz.iojbl.cn/gtruscxqkm.html

[D23] reduce 累积计算
来源：http://hz.chenlongwang.top/gtmyrerbcz.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.redwolf501.top/gtyqrmduvz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.jqgfzy.top/gtcsnpicqf.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.tanke756.top/gtcyxfvevh.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.pengpengdd.cyou/gtsuwbqwgn.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.iojbl.cn/gtuujwjzhi.html

Go:   // 手写循环
来源：http://hz.tianlin.xyz/gtljlmygnp.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.svipenyu.cn/gtbufqksty.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.yvedp.cn/gtfonrwxnr.html

[D24] 字典 / Map 基本操作
来源：http://hz.zhiwuduotai.top/gtnrtwjeug.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.fzhhl.top/gtnypubvkq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.iojbl.cn/gtpkmjlhdd.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.zhiwuduotai.top/gtocrmjgni.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.xuanzx.com/gtgnfihtbv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.jyoumei.cn/gtukpyvpsz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.nanxuanxn.top/gtszfckbwi.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.dashuyun.cn/gtoofdnfjt.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.kuanghao11.cn/gtntruwsrs.html

[D25] Set 集合去重与交并差
来源：http://hz.jinqigfzy.top/gtdqhgfinj.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.xuetiantiany.cn/gtoqgldkzk.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.jinqigfzy.top/gtaatwvvhd.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.pengpengdd.cyou/gttibfheca.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.chenjidiqi.icu/gttkciuump.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.hywenlv.cn/gtcvkcajza.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.guowangkeji.top/gtqnhmshvl.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.hongshengwenyu.top/gttpoxqshh.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.aizwys.cn/gtgnvridci.html

[D26] 数组转字符串
来源：http://hz.cucudq.cn/gtbpvevjbl.html

Py:   ", ".join(map(str, arr))
来源：http://hz.snrcjt.cn/gtqjgsdcyw.html

PHP:  implode(", ", $arr);
来源：http://hz.zhongyouzk.top/gtvzhaxktv.html

JS:   arr.join(", ")
来源：http://hz.chenlongwang.top/gtbiueuazt.html

TS:   arr.join(", ")
来源：http://hz.iojbl.cn/gtztzbckiu.html

Java: String.join(", ", list)
来源：http://hz.c1oappe.top/gtzeolfjgt.html

Go:   strings.Join(strs, ", ")
来源：http://hz.xuetiantiany.cn/gtxuiwtgjm.html

Ruby: arr.join(", ")
来源：http://hz.sufxvd.cn/gtlzynimyv.html

C#:   string.Join(", ", list)
来源：http://hz.iojbl.cn/gtzzbephzb.html

================================================================================
来源：http://hz.vqdsnc.cn/gtqrtetswf.html

E. 字符串处理
来源：http://hz.9152youxi.cn/gtjdpmaohs.html

================================================================================
来源：http://hz.sufxvd.cn/gtxldjlrdq.html

[E01] 拼接字符串
来源：http://hz.birdmap.top/gtfdvqeriu.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.zhiwuduotai.top/gtkbhcxmgw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.jqgufenzy.top/gtnvzyjlig.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.sysykeji.top/gtcdvzrsum.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.chenzaomai.com/gtegmkbkol.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.aibaodan.cn/gtgbwvazlq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.yanxiufei.cn/gtjaoefkxr.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.iojbl.cn/gtmmczrloo.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.yueranfly.top/gtecgbrmwp.html

[E02] 重复字符串
来源：http://hz.ybcxt.top/gtrravptva.html

Py:   "ab" * 3
来源：http://hz.pengpengdd.cyou/gtlnazjqwr.html

PHP:  str_repeat("ab", 3);
来源：http://hz.yuxming.cn/gtwooasggv.html

JS:   "ab".repeat(3)
来源：http://hz.gaohongyu789.top/gthmxhsbrh.html

TS:   "ab".repeat(3)
来源：http://hz.ivvv.top/gtclbilyaj.html

Java: "ab".repeat(3)
来源：http://hz.chenlongwang.top/gtzieqrlnz.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.ybcxt.top/gtcwfwtykq.html

Ruby: "ab" * 3
来源：http://hz.xinyue.icu/gtkyvawijx.html


<!-- 参考信息 -->