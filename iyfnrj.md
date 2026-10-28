代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://hz.nwbrower.top/gtvmsshcmq.html

Ruby: -> { puts "run" }.call
来源：http://hz.jiagoushi.top/gtvvvdkssi.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.xinyue.icu/gtnfkasuwn.html

[C13] 类型声明 / 类型注解
来源：http://hz.guowangkeji.top/gtxuupijya.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.wangshuangyany.cn/gtdkdaiube.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.haohaochexian.top/gtfrfhvgwe.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.gogol.net.cn/gttychmbyb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yuanzhike.top/gtjcnyjwmq.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.jqgfzy.top/gteuhfdlta.html

Go:   func add(a, b int) int
来源：http://hz.cashguo.top/gtydydktjo.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.gotoacloud.top/gtsdjftgry.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.smart0.xyz/gtmipcwmre.html

[C14] 泛型函数
来源：http://hz.shuidangran.top/gtqxjubztn.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.zhengqikj.top/gtgblbqznv.html

PHP:  // 无泛型
来源：http://hz.havefunace.top/gtwzpluosp.html

JS:   // 无泛型
来源：http://hz.dashuyun.cn/gtcgpusauy.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.hfpthk.cn/gteizjkdgy.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.zhengqikj.top/gtxsoavyrq.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.0kj1m.cn/gtigiwidji.html

Ruby: # 无泛型
来源：http://hz.sysykeji.top/gthoatcgfj.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.daria6918.cn/gtzgartupb.html

[C15] 解构 / 展开参数
来源：http://hz.sxryk.cn/gtbyxycqtr.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.chenlongwang.top/gtpputfkei.html

PHP:  [$a, $b] = $pair;
来源：http://hz.ehwqpu.com/gtpzadazzp.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.shzxlz.cn/gtaecargtg.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.aibaodan.cn/gtapbfluvi.html

Java: // 无解构
来源：http://hz.ydzc1.top/gtsqyufidx.html

Go:   // 无解构
来源：http://hz.gotoacloud.top/gthjcvxkfs.html

Ruby: a, b = pair
来源：http://hz.gaohongyu789.top/gtrdcdrprr.html

C#:   var (a, b) = pair;
来源：http://hz.jlsjyb.cn/gtqlrqnmkz.html

[C16] 函数 / 方法重载
来源：http://hz.gaohongyu789.top/gtlbmffqiz.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.yvedp.cn/gtrbwpynul.html

PHP:  // 无重载
来源：http://hz.316326.xyz/gtrgdgektl.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.zhixingplan.top/gtbrhohdoe.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.9152youxi.cn/gtzbdaquaw.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.guannengcc.top/gtxbpehxjj.html

Go:   // 无重载：用不同函数名
来源：http://hz.gotoacloud.top/gtudlhvefi.html

Ruby: # 无重载：靠动态参数
来源：http://hz.jyoumei.cn/gtgvbjhwtv.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.guowangkeji.top/gtspffgjpr.html

================================================================================
来源：http://hz.chenlongwang.top/gtistxgtsu.html

D. 数组 / 列表 / 集合
来源：http://hz.tianlin.xyz/gtdgbytipx.html

================================================================================
来源：http://hz.cucudq.cn/gtispsvhao.html

[D01] 创建数组 / 列表
来源：http://hz.sxryk.cn/gtdwcjyhho.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.jinqigufen.top/gtorbnznun.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.sufxvd.cn/gtimiieetk.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.smart0.xyz/gtrqlzhquz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.sysykeji.top/gtqnxptpvv.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.hfpthk.cn/gtlchjucgq.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.cdnleiting.top/gtipbprhtz.html

Ruby: arr = [1, 2, 3]
来源：http://hz.ivvv.top/gtdkcabirn.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.fengsongda.top/gtuwjmqbjn.html

[D02] 追加元素到末尾
来源：http://hz.birdmap.top/gtogsrehcy.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.kuanghao11.cn/gtoqcvrrlw.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.tianlin.xyz/gttnzqqqwf.html

JS:   arr.push(4);
来源：http://hz.yongpay.top/gtbakymedk.html

TS:   arr.push(4);
来源：http://hz.ppjwa.cn/gtrvpeompd.html

Java: list.add(4);
来源：http://hz.yongpay.top/gtuhjybtba.html

Go:   arr = append(arr, 4)
来源：http://hz.jqgfzy.top/gtdnluxoxq.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.iojbl.cn/gtfezhugcq.html

C#:   list.Add(4);
来源：http://hz.tian-w.cn/gtgbspipay.html

[D03] 在指定位置插入元素
来源：http://hz.xziqi.cn/gtggjecsnd.html

Py:   arr.insert(0, 0)
来源：http://hz.nanxuanxn.top/gtydcjkqyl.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.sufxvd.cn/gtvejepfmw.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.zhoulong.xyz/gtuxsblrwr.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.yongpay.top/gtvmbnnxwi.html

Java: list.add(0, 0);
来源：http://hz.nwbrower.top/gtdvwrschw.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.xziqi.cn/gtwnvdrppj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.yangfankeji.com/gtzklxpmpo.html

C#:   list.Insert(0, 0);
来源：http://hz.ivvv.top/gtefsjnukj.html

[D04] 删除元素
来源：http://hz.jinqigufen.top/gtwwbozsat.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.yonumen.top/gttpgmfoyt.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.daxiang520.top/gtmovsswvk.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.pycfn.com/gtmetaipzp.html

TS:   arr.splice(0, 1);
来源：http://hz.tianlin.xyz/gtxztkpxbm.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.xuetiantiany.cn/gtvybxdjaw.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.hammf.cn/gthvcorzig.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.iojbl.cn/gtlkvxdkvf.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.andypj.xyz/gtjvpgngid.html

[D05] 访问与修改元素
来源：http://hz.jianghu66.top/gtyyeejduh.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.cdnleiting.top/gtwkimcoik.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.ehwqpu.com/gtocjmkkvd.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.wangshuangyany.cn/gtxyuxwpco.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.shangyingyoupin.top/gtomdquief.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.hywenlv.cn/gtpnepdwxd.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.zhengqikj.top/gtcdehvema.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jiagoushi.top/gtrpqoyubd.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.316326.xyz/gtafbrutkb.html

[D06] 数组长度
来源：http://hz.yangfankeji.com/gtwfjkrpae.html

Py:   len(arr)
来源：http://hz.shanyushiyangtech.top/gtonbcpbji.html

PHP:  count($arr);
来源：http://hz.jianghu66.top/gtgreirgzu.html

JS:   arr.length
来源：http://hz.meibo888.top/gtmldzkpcy.html

TS:   arr.length
来源：http://hz.sysykeji.top/gtnqaoqiel.html

Java: list.size();
来源：http://hz.cashguo.top/gtvalepaxq.html

Go:   len(arr)
来源：http://hz.xingfuxueyuan.xyz/gtuhehjkcf.html

Ruby: arr.length; arr.size
来源：http://hz.zdqjudy.top/gtgvqblmut.html

C#:   list.Count;
来源：http://hz.vqdsnc.cn/gtzgutdfpv.html

[D07] 切片 / 取子数组
来源：http://hz.ppjwa.cn/gtbjazvimi.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.meibo888.top/gtgehujixg.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.yongpay.top/gtotldfhey.html

JS:   arr.slice(1, 4);
来源：http://hz.yongpay.top/gtfdobepzi.html

TS:   arr.slice(1, 4);
来源：http://hz.0kj1m.cn/gtezeydnfw.html

Java: list.subList(1, 4);
来源：http://hz.yj20258888.top/gtffqphngr.html

Go:   arr[1:4]
来源：http://hz.feifeiyinyue.top/gtejkgdofc.html

Ruby: arr[1, 3]
来源：http://hz.zhiwuduotai.top/gtruebkrex.html

C#:   list.GetRange(1, 3);
来源：http://hz.cashguo.top/gtyzkhsves.html

[D08] 合并两个数组
来源：http://hz.jianghu66.top/gtybvwcxxj.html

Py:   a + b;  a.extend(b)
来源：http://hz.zhoulong.xyz/gtaynnfrit.html

PHP:  array_merge($a, $b);
来源：http://hz.ehwqpu.com/gtswjzpyvp.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.sysykeji.top/gtlcodksys.html

TS:   [...a, ...b];
来源：http://hz.gotoacloud.top/gtylfmdbpm.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.snrcjt.cn/gtujktmfzc.html

Go:   append(a, b...)
来源：http://hz.gogol.net.cn/gtblvojbtj.html

Ruby: a + b;  a.concat(b)
来源：http://hz.9152youxi.cn/gtkgyncpru.html

C#:   a.Concat(b).ToList()
来源：http://hz.jyoumei.cn/gtzfipnyas.html

[D09] 排序（升序）
来源：http://hz.pengpengdd.cyou/gtiicbhamp.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.shangyingyoupin.top/gtahkctwhs.html

PHP:  sort($arr);
来源：http://hz.zhijiandao.cn/gtqleilgoo.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.zhoulong.xyz/gtthhqtqyr.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.jinyuanbaomall.cn/gtvelaqxsl.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.gotoacloud.top/gtssktupzz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.yj20258888.top/gthkkuendc.html

Ruby: arr.sort
来源：http://hz.ybcxt.top/gtehsbaqdd.html

C#:   list.Sort();
来源：http://hz.zhoulong.xyz/gtldwrxneq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.ehwqpu.com/gtqskwkcle.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.jinqigufen.top/gtfpvrxygw.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.shuidangran.top/gtddcafcyc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.shanyushiyangkeji.top/gtmyykanyg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.ydzc1.top/gtzakgtrkj.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.zhiwuduotai.top/gtrsmtieuk.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.redwolf501.top/gtwngbcmhh.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.zhiwuduotai.top/gtveuyvohg.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.wangdashe.top/gttbzvyroy.html

[D11] 反转数组
来源：http://hz.gogol.net.cn/gtirszkelw.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.hnxiangtu.top/gtcexpbuxj.html

PHP:  array_reverse($arr);
来源：http://hz.shzxlz.cn/gtpvfajkhu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.xingfuxueyuan.xyz/gtnyhglsfd.html

TS:   [...arr].reverse();
来源：http://hz.sxryk.cn/gttyxhwrtb.html

Java: Collections.reverse(list);
来源：http://hz.jinghuilouyu.cn/gtpcpklvrc.html

Go:   slices.Reverse(arr)
来源：http://hz.zhixingplan.top/gtpzdfbqyc.html

Ruby: arr.reverse
来源：http://hz.zhaomingkeji.xyz/gttokeqwhm.html

C#:   list.Reverse();
来源：http://hz.fengsongda.top/gtujncfoja.html

[D12] 查找元素下标
来源：http://hz.ydjk.org.cn/gtnyeiwlyj.html

Py:   arr.index(x);  x in arr
来源：http://hz.shanyushiyangkeji.top/gtqiicvezk.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.shanyushiyangkeji.top/gtirqxsrqv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.svipenyu.cn/gtwonlngtb.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jinqigufen.top/gtgdcnmnsp.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.tanke756.top/gthkvsvmsa.html

Go:   slices.Index(arr, x)
来源：http://hz.jianghu66.top/gttgeqekuq.html

Ruby: arr.index(x)
来源：http://hz.xuanzx.com/gtjdkusknf.html

C#:   list.IndexOf(x);
来源：http://hz.zhoulong.xyz/gtdqqjpbza.html

[D13] 过滤（保留满足条件的）
来源：http://hz.xingfuxueyuan.xyz/gtmvazbsth.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.sxryk.cn/gtdhxfpqjp.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.meibo888.top/gtoweawefr.html

JS:   arr.filter(x => x > 3)
来源：http://hz.sysykeji.top/gtfbdenaif.html

TS:   arr.filter(x => x > 3)
来源：http://hz.zhaomingkeji.xyz/gtdklrdwnc.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.birdmap.top/gtzllhhawh.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.yanxiufei.cn/gtxpqpudbo.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.snrcjt.cn/gtnncruwnt.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.fengsongda.top/gtdnchnsbz.html

[D14] 映射转换（每个元素变形）
来源：http://hz.xziqi.cn/gtolbugmkf.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.tanke756.top/gtylpsdqzj.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.jiagoushi.top/gtybdjqjbd.html

JS:   arr.map(x => x * 2)
来源：http://hz.iojbl.cn/gtzikcftcp.html

TS:   arr.map(x => x * 2)
来源：http://hz.shuidangran.top/gtmqhgmltn.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.sufxvd.cn/gtcnywyusl.html

Go:   // 手写循环
来源：http://hz.gaohongyu789.top/gtxkkaydzm.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.zhijiandao.cn/gtwcldboif.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.chenjidiqi.icu/gtpenvkyvt.html

[D15] 去重
来源：http://hz.shzxlz.cn/gtcuklibnk.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.hysaishi.cn/gthtobnmjt.html

PHP:  array_unique($arr);
来源：http://hz.gaohongyu789.top/gtejttbhwz.html

JS:   [...new Set(arr)]
来源：http://hz.gotoacloud.top/gtvqtrzqnu.html

TS:   [...new Set(arr)]
来源：http://hz.xylfe.cn/gtebgvctxy.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.shangyingyoupin.top/gtcivgiuiq.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.ydzc1.top/gtypnoprho.html

Ruby: arr.uniq
来源：http://hz.yueranfly.top/gtvuvcnaap.html

C#:   list.Distinct().ToList()
来源：http://hz.yvedp.cn/gtiarsivst.html

[D16] 求和与平均值
来源：http://hz.0kj1m.cn/gthdjegcur.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.yueranfly.top/gtuemfbuiw.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.ydzc1.top/gtduzmlcpj.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zhiwuduotai.top/gtsiljdlfo.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zhaomingkeji.xyz/gtrasqllcs.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.nwbrower.top/gtrglcvasg.html

Go:   // 手写循环累加
来源：http://hz.pycfn.com/gtvnzagboe.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.shanyushiyangtech.top/gtuyxbvtus.html

C#:   list.Sum();  list.Average()
来源：http://hz.aibaodan.cn/gthadvexfk.html

[D17] 最大值与最小值
来源：http://hz.shuidangran.top/gtseivrkqh.html

Py:   max(arr);  min(arr)
来源：http://hz.tianlin.xyz/gtipuvszkp.html

PHP:  max($arr);  min($arr);
来源：http://hz.aizwys.cn/gtkrontazs.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.snrcjt.cn/gtafjlqslr.html

TS:   Math.max(...arr);
来源：http://hz.hnqzz.top/gtpikgslwx.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.ivvv.top/gtgiyujqom.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.gotoacloud.top/gtbsejuyfy.html

Ruby: arr.max;  arr.min
来源：http://hz.yuanzhike.top/gtmwduakgt.html

C#:   list.Max();  list.Min()
来源：http://hz.shzxlz.cn/gthpgduihj.html

[D18] 扁平化嵌套数组
来源：http://hz.gogol.net.cn/gtnvebxpoz.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.shuidangran.top/gtehfoielu.html

PHP:  array_merge(...$nested);
来源：http://hz.jinqigufen.top/gtzgvmfgct.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.sufxvd.cn/gtwothxpce.html

TS:   nested.flat();
来源：http://hz.feifeiyinyue.top/gtldpdunqr.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.yuanzhike.top/gtgoaxnxtf.html

Go:   // 手写双层循环
来源：http://hz.tanke756.top/gthzdvzuhu.html

Ruby: nested.flatten
来源：http://hz.andypj.xyz/gterlzabwj.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.yangfankeji.com/gtfpjuzqfb.html

[D19] 按字段分组
来源：http://hz.chenzaomai.com/gterjxfxqn.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.zhijiandao.cn/gtuqomrrko.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.cdnleiting.top/gtevlbtjpb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.hnxiangtu.top/gteffkktim.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.gaohongyu789.top/gtlrwwwucc.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.shanyushiyangtech.top/gtcwilpwai.html

Go:   // 手写 map[string][]T
来源：http://hz.zhaomingkeji.xyz/gtouindpxd.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.jinyuanbaomall.cn/gtdirjbgty.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.yangfankeji.com/gtfsngdbds.html

[D20] 统计每个元素出现次数
来源：http://hz.cqqwz.cn/gtoznjxqqg.html

Py:   Counter(arr)
来源：http://hz.zycfv.cn/gtyvvvapfn.html

PHP:  array_count_values($arr);
来源：http://hz.jianghu66.top/gtftoxtgir.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.cqqwz.cn/gtpmofazxv.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.shangyingyoupin.top/gtxcmrecmm.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.nanxuanxn.top/gtdnjmzpzr.html

Go:   // 手写 map[T]int
来源：http://hz.tanke756.top/gtguwerpdz.html

Ruby: arr.tally
来源：http://hz.nanxuanxn.top/gtuiisgwvp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.jqgufenzy.top/gtisrkjwuf.html

[D21] 判断是否包含某元素
来源：http://hz.jqgfzy.top/gtqulcpluu.html

Py:   x in arr
来源：http://hz.andypj.xyz/gtieubofmd.html

PHP:  in_array($x, $arr, true);
来源：http://hz.iojbl.cn/gtgxeuhfug.html

JS:   arr.includes(x)
来源：http://hz.gotoacloud.top/gteehpeqgj.html

TS:   arr.includes(x)
来源：http://hz.jqgufenzy.top/gtjupledhf.html

Java: list.contains(x)
来源：http://hz.chenzaomai.com/gtchnykkds.html

Go:   slices.Contains(arr, x)
来源：http://hz.0kj1m.cn/gtkadxefnr.html

Ruby: arr.include?(x)
来源：http://hz.shanyushiyangkeji.top/gttwrdjpku.html

C#:   list.Contains(x)
来源：http://hz.wangdashe.top/gtbabfgprw.html

[D22] 复制数组（避免共享引用）
来源：http://hz.9152youxi.cn/gtikqjkylb.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.sufxvd.cn/gtfgozvjor.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.0kj1m.cn/gtxinrstej.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.jiagoushi.top/gthfscsluc.html

TS:   [...arr];
来源：http://hz.hysaishi.cn/gtjpwcevgi.html

Java: new ArrayList<>(list);
来源：http://hz.guowangkeji.top/gtvzyqczpx.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.cdnleiting.top/gtkcgkmfyv.html

Ruby: arr.dup;  arr.clone
来源：http://hz.xuanzx.com/gtekennlvp.html

C#:   new List<int>(list);
来源：http://hz.9152youxi.cn/gtakgxezqo.html

[D23] reduce 累积计算
来源：http://hz.xziqi.cn/gtiywqbjaj.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.ivvv.top/gtxwkntlmh.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.wangshuangyany.cn/gtizljrkmz.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.birdmap.top/gtrircgybu.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yj202588.top/gtquzyiroa.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.jianghu66.top/gtjuijagob.html

Go:   // 手写循环
来源：http://hz.yanxiufei.cn/gtkwviyqtu.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.kuanghao11.cn/gtqampfmxo.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.zhongyouzk.top/gtqumhnbvc.html

[D24] 字典 / Map 基本操作
来源：http://hz.vqdsnc.cn/gtanykvimh.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.chenzaomai.com/gtphmboaoj.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.sxryk.cn/gtjbuloxyk.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.chenlongwang.top/gtuqyhkvvp.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.zhoulong.xyz/gterkhhwrw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.52xcode.cn/gtjmlbvcre.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.jinyuanbaomall.cn/gtoqvjcarq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.jqgufenzy.top/gtujakgcnj.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.xingfuxueyuan.xyz/gtqjoysexn.html

[D25] Set 集合去重与交并差
来源：http://hz.zhijiandao.cn/gtcikruohh.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.xylfe.cn/gtsjsmkapn.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.svipenyu.cn/gtsdwyzppw.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.xingfuxueyuan.xyz/gtvellorwu.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.gotoacloud.top/gthjvtzdun.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.xylfe.cn/gtsuzcepqp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.hongshengwenyu.top/gtxahgatbd.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.yvedp.cn/gtuvnabnkd.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.birdmap.top/gteeuwgjet.html

[D26] 数组转字符串
来源：http://hz.feifeiyinyue.top/gtoszbcdnl.html

Py:   ", ".join(map(str, arr))
来源：http://hz.yvedp.cn/gtpcjoqdwr.html

PHP:  implode(", ", $arr);
来源：http://hz.ydzc1.top/gtrfetrtrs.html

JS:   arr.join(", ")
来源：http://hz.gogol.net.cn/gtucjontfs.html

TS:   arr.join(", ")
来源：http://hz.andypj.xyz/gtsweheyrz.html

Java: String.join(", ", list)
来源：http://hz.tianlin.xyz/gtetychjee.html

Go:   strings.Join(strs, ", ")
来源：http://hz.nanxuanxn.top/gtppbcxmzb.html

Ruby: arr.join(", ")
来源：http://hz.shuidangran.top/gtblqdzpqg.html

C#:   string.Join(", ", list)
来源：http://hz.hongshengwenyu.top/gtxocfcwkw.html

================================================================================
来源：http://hz.smart0.xyz/gtbotwnlpe.html

E. 字符串处理
来源：http://hz.cashguo.top/gtbjzbkaaj.html

================================================================================
来源：http://hz.chenlongwang.top/gtoiqprvlw.html

[E01] 拼接字符串
来源：http://hz.cheryme.top/gtriscoekk.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.zhixingplan.top/gtraabuxkg.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.daxiang520.top/gtmhqozqbb.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.aibaodan.cn/gtyxujnbaz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.xingfuxueyuan.xyz/gtosgonhat.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.c1oappe.top/gtbsekbivs.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.jqgfzy.top/gtncuqools.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.jlsjyb.cn/gtouocxwcc.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.birdmap.top/gtlbkcltkk.html

[E02] 重复字符串
来源：http://hz.ybcxt.top/gtpmivnibe.html

Py:   "ab" * 3
来源：http://hz.yvedp.cn/gtamiipmkh.html

PHP:  str_repeat("ab", 3);
来源：http://hz.c1oappe.top/gtcicgoxij.html

JS:   "ab".repeat(3)
来源：http://hz.yj20258888.top/gtlzjqpcnn.html

TS:   "ab".repeat(3)
来源：http://hz.gogol.net.cn/gtrdysklvi.html

Java: "ab".repeat(3)
来源：http://hz.tanke756.top/gtynxlpsai.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.tian-w.cn/gtoewfbdgk.html

Ruby: "ab" * 3
来源：http://hz.wangdashe.top/gtxwwcxnpd.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.haohaochexian.top/gtypwoadhp.html

[E03] 截取子串
来源：http://hz.bjfxy.top/gtmjahsbrl.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.hnqzz.top/gtvcjqihcu.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.ppjwa.cn/gttbfzjtdh.html


<!-- 参考信息 -->