代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://hz.pengpengdd.cyou/gtaghzxjok.html

Ruby: -> { puts "run" }.call
来源：http://hz.hammf.cn/gtlzeoxoaq.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.ivvv.top/gtixoygxld.html

[C13] 类型声明 / 类型注解
来源：http://hz.ybcxt.top/gtobexnaht.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.c1oappe.top/gtvjfbofbs.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.mhx1999.top/gtlzbclxya.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.ppjwa.cn/gtosreffoe.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jlsjyb.cn/gtjovuspsl.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.zhijiandao.cn/gtrvhjmofp.html

Go:   func add(a, b int) int
来源：http://hz.shzxlz.cn/gtaeruckdy.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.shangyingyoupin.top/gtqrsnhwry.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.daxiang520.top/gtwgthaich.html

[C14] 泛型函数
来源：http://hz.tanke756.top/gtzfhueuav.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.hywenlv.cn/gtbeyjkhjw.html

PHP:  // 无泛型
来源：http://hz.yuxming.cn/gtwgkjomsh.html

JS:   // 无泛型
来源：http://hz.guowangkeji.top/gthobpopfc.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.yongpay.top/gtvjrzatgx.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.jiagoushi.top/gtrdhuefrp.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.hfpthk.cn/gtjcybvovn.html

Ruby: # 无泛型
来源：http://hz.sysykeji.top/gtvdtujodh.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.xylfe.cn/gtnpziwbgm.html

[C15] 解构 / 展开参数
来源：http://hz.0kj1m.cn/gtbdxwller.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.tanke756.top/gtngogwsiy.html

PHP:  [$a, $b] = $pair;
来源：http://hz.0kj1m.cn/gtbbhadjdx.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.chenzaomai.com/gtfcsjukpu.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.hfpthk.cn/gtgqkiittv.html

Java: // 无解构
来源：http://hz.xylfe.cn/gtzbjufjvo.html

Go:   // 无解构
来源：http://hz.ivvv.top/gtmpusxyso.html

Ruby: a, b = pair
来源：http://hz.sxryk.cn/gtdibmlcsr.html

C#:   var (a, b) = pair;
来源：http://hz.xuanzx.com/gtbniakewl.html

[C16] 函数 / 方法重载
来源：http://hz.chenjidiqi.icu/gtyvvyfjtr.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.chenzaomai.com/gtfaglgnge.html

PHP:  // 无重载
来源：http://hz.shuidangran.top/gteqjxmpzy.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.jqgfzy.top/gtifljckhy.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.tianlin.xyz/gtegzdjvpp.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.nwbrower.top/gtmwaugnjw.html

Go:   // 无重载：用不同函数名
来源：http://hz.cucudq.cn/gtnmjgbhlp.html

Ruby: # 无重载：靠动态参数
来源：http://hz.ywan-chungtsiang.top/gtuarjomdb.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.zycfv.cn/gtwmbmfstv.html

================================================================================
来源：http://hz.hnxiangtu.top/gtddbfflft.html

D. 数组 / 列表 / 集合
来源：http://hz.aizwys.cn/gtfqlnxjxn.html

================================================================================
来源：http://hz.haohaochexian.top/gtzzsjmsht.html

[D01] 创建数组 / 列表
来源：http://hz.meibo888.top/gtzzzgyafk.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.hysaishi.cn/gtejptqkce.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.jinqigfzy.top/gtfhuuybnj.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.svipenyu.cn/gtfxmynmly.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.yueranfly.top/gtpatyqgjn.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.hnqzz.top/gtiykqmtks.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.pycfn.com/gtvsdxhxoh.html

Ruby: arr = [1, 2, 3]
来源：http://hz.ybcxt.top/gtbyddgmcg.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.tianlin.xyz/gtuzdbrler.html

[D02] 追加元素到末尾
来源：http://hz.sufxvd.cn/gtokrkadzs.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.yvedp.cn/gttkceyzcu.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.hywenlv.cn/gtcpcntuev.html

JS:   arr.push(4);
来源：http://hz.snrcjt.cn/gtcvtdygpj.html

TS:   arr.push(4);
来源：http://hz.ppjwa.cn/gteknovepo.html

Java: list.add(4);
来源：http://hz.zhongyouzk.top/gtqlhytttq.html

Go:   arr = append(arr, 4)
来源：http://hz.nanxinkj.top/gtbtesbwvy.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.daxiang520.top/gtgikdpgnz.html

C#:   list.Add(4);
来源：http://hz.ehwqpu.com/gtkbivhnxr.html

[D03] 在指定位置插入元素
来源：http://hz.shangyingyoupin.top/gtdcrhgpor.html

Py:   arr.insert(0, 0)
来源：http://hz.xuetiantiany.cn/gtwroajpob.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.ivvv.top/gtbkrzhlot.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.zhoulong.xyz/gtpxnfuuct.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.shzxlz.cn/gtwqskgmvm.html

Java: list.add(0, 0);
来源：http://hz.kuanghao11.cn/gtnumytfal.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.yuxming.cn/gtmswfswfe.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.bjfxy.top/gtkrwioazx.html

C#:   list.Insert(0, 0);
来源：http://hz.yj20258888.top/gtukisixmw.html

[D04] 删除元素
来源：http://hz.ehwqpu.com/gtbomcsxqh.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.gaohongyu789.top/gtpfbjersg.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.fzhhl.top/gtdpdrtbse.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.gogol.net.cn/gtjotowjac.html

TS:   arr.splice(0, 1);
来源：http://hz.ybcxt.top/gtjfnkkwkz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.shuidangran.top/gtvejaqrjx.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.sufxvd.cn/gtwlehthzz.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.shanyushiyangkeji.top/gtiupcinti.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.sufxvd.cn/gtxthmzbvx.html

[D05] 访问与修改元素
来源：http://hz.gogol.net.cn/gtxzxagzuv.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yongpay.top/gtpwjrimwx.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.cashguo.top/gtcnoesohb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.ppjwa.cn/gtusirjfkq.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.jinqigfzy.top/gtyveunmyn.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.shanyushiyangtech.top/gtglhjxqsm.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.andypj.xyz/gtbboudsap.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.xuetiantiany.cn/gtiycxujsf.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.shanyushiyangtech.top/gthxdqfvut.html

[D06] 数组长度
来源：http://hz.hywenlv.cn/gttwbqejwj.html

Py:   len(arr)
来源：http://hz.gzhubu.top/gtncnhfdai.html

PHP:  count($arr);
来源：http://hz.havefunace.top/gtpivjldxh.html

JS:   arr.length
来源：http://hz.quarkkingdee.top/gtfygvgvfj.html

TS:   arr.length
来源：http://hz.snrcjt.cn/gtibisuvvv.html

Java: list.size();
来源：http://hz.ywan-chungtsiang.top/gttmttojjm.html

Go:   len(arr)
来源：http://hz.bjfxy.top/gtvxujqlul.html

Ruby: arr.length; arr.size
来源：http://hz.zhengqikj.top/gtgktyfkug.html

C#:   list.Count;
来源：http://hz.tianlin.xyz/gtikhvgavt.html

[D07] 切片 / 取子数组
来源：http://hz.zycfv.cn/gtzpnrkgrv.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.jinqigfzy.top/gtsvdznoyl.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.xylfe.cn/gtakohloxq.html

JS:   arr.slice(1, 4);
来源：http://hz.tanke756.top/gtzgjzlynp.html

TS:   arr.slice(1, 4);
来源：http://hz.0kj1m.cn/gtrqwnoxlp.html

Java: list.subList(1, 4);
来源：http://hz.dianchejie.cn/gtopnwzmfi.html

Go:   arr[1:4]
来源：http://hz.sysykeji.top/gtvjkvbtrp.html

Ruby: arr[1, 3]
来源：http://hz.ydjk.org.cn/gtgmgfoklb.html

C#:   list.GetRange(1, 3);
来源：http://hz.zhengqikj.top/gthfqbcthv.html

[D08] 合并两个数组
来源：http://hz.hysaishi.cn/gtdbdvfwsa.html

Py:   a + b;  a.extend(b)
来源：http://hz.cdnleiting.top/gtfkpepdbi.html

PHP:  array_merge($a, $b);
来源：http://hz.daxiang520.top/gtpelvoasn.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.mhx1999.top/gtdlgldbgh.html

TS:   [...a, ...b];
来源：http://hz.chenzaomai.com/gtxjckkkfg.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.gaohongyu789.top/gtxrzqoppb.html

Go:   append(a, b...)
来源：http://hz.nanxuanxn.top/gtgnhjpkto.html

Ruby: a + b;  a.concat(b)
来源：http://hz.redwolf501.top/gteybfisjj.html

C#:   a.Concat(b).ToList()
来源：http://hz.ywan-chungtsiang.top/gtpwibzwou.html

[D09] 排序（升序）
来源：http://hz.birdmap.top/gteutrtebs.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.aizwys.cn/gtjfikgbmw.html

PHP:  sort($arr);
来源：http://hz.chenzaomai.com/gtlojtuuxy.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.feifeiyinyue.top/gtudhhcmaz.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.zhoulong.xyz/gttnxlritb.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.hywenlv.cn/gtmgorsdjz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.dianchejie.cn/gtqfydeska.html

Ruby: arr.sort
来源：http://hz.yueranfly.top/gtsaygnljf.html

C#:   list.Sort();
来源：http://hz.hammf.cn/gtwozqtuff.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.zhixingplan.top/gtnvhcnaxj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.cheryme.top/gtnpzwcigj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.xziqi.cn/gtqmwimmdx.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yj202588.top/gtoqtnwdtr.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hongshengwenyu.top/gtkhykmuho.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.meibo888.top/gtaidewuwg.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.shangyingyoupin.top/gtftxxyacx.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.tianlin.xyz/gtfyphtfdb.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.zhixingplan.top/gtiiughgzb.html

[D11] 反转数组
来源：http://hz.pycfn.com/gtfbbhenhr.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.zhixingplan.top/gtgxugssjb.html

PHP:  array_reverse($arr);
来源：http://hz.52xcode.cn/gtqdbiuzdi.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.cqqwz.cn/gtndlgizqx.html

TS:   [...arr].reverse();
来源：http://hz.yanxiufei.cn/gtjkjiznhr.html

Java: Collections.reverse(list);
来源：http://hz.hfpthk.cn/gtunvambsx.html

Go:   slices.Reverse(arr)
来源：http://hz.aibaodan.cn/gtjyhnhuhg.html

Ruby: arr.reverse
来源：http://hz.zhijiandao.cn/gtqkmmyevg.html

C#:   list.Reverse();
来源：http://hz.yvedp.cn/gtqoiomjhn.html

[D12] 查找元素下标
来源：http://hz.cdnleiting.top/gtaewiccoq.html

Py:   arr.index(x);  x in arr
来源：http://hz.fengsongda.top/gtfkquszem.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.yonumen.top/gtbutlzuqx.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.snrcjt.cn/gtyskcabgo.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.ivvv.top/gtqrktnhgx.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.dianchejie.cn/gtbvarpbic.html

Go:   slices.Index(arr, x)
来源：http://hz.zhengqikj.top/gteoyulsjt.html

Ruby: arr.index(x)
来源：http://hz.fzhhl.top/gtkqqsvjlx.html

C#:   list.IndexOf(x);
来源：http://hz.tanke756.top/gthhnicmis.html

[D13] 过滤（保留满足条件的）
来源：http://hz.yanxiufei.cn/gtliplrded.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.smart0.xyz/gtotlgsyay.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.sysykeji.top/gtadlkebnb.html

JS:   arr.filter(x => x > 3)
来源：http://hz.snrcjt.cn/gtboreinoe.html

TS:   arr.filter(x => x > 3)
来源：http://hz.guowangkeji.top/gtvmibgajz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.hywenlv.cn/gteukctgyl.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.yvedp.cn/gtmkmyiafp.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.nanxuanxn.top/gtkqevaukj.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.shanyushiyangkeji.top/gtmhljpkek.html

[D14] 映射转换（每个元素变形）
来源：http://hz.tian-w.cn/gtygbginsd.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.aizwys.cn/gtntywwztv.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.52xcode.cn/gteuvlaljn.html

JS:   arr.map(x => x * 2)
来源：http://hz.ybcxt.top/gtvqpejgcj.html

TS:   arr.map(x => x * 2)
来源：http://hz.dianchejie.cn/gtlbsckkoh.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.birdmap.top/gttpjvkonv.html

Go:   // 手写循环
来源：http://hz.cucudq.cn/gtwvsrglrs.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.hfpthk.cn/gtnjoqoyrl.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.xuetiantiany.cn/gtrievxddg.html

[D15] 去重
来源：http://hz.ydzc1.top/gtjzetfcui.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.ehwqpu.com/gteuuqncdm.html

PHP:  array_unique($arr);
来源：http://hz.xylfe.cn/gttvqjmioq.html

JS:   [...new Set(arr)]
来源：http://hz.yj202588.top/gtsuditfqh.html

TS:   [...new Set(arr)]
来源：http://hz.aibaodan.cn/gtipksrqir.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.yuanzhike.top/gtmoorybou.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.yvedp.cn/gtmttpkdik.html

Ruby: arr.uniq
来源：http://hz.sweek.top/gtqjjflyfy.html

C#:   list.Distinct().ToList()
来源：http://hz.sxryk.cn/gteofgopwc.html

[D16] 求和与平均值
来源：http://hz.dianchejie.cn/gtjvmjtwmk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.zhengqikj.top/gtnrsitonb.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.hnqzz.top/gtwfkbxdvj.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.shanyushiyangkeji.top/gtusorfrua.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zhengqikj.top/gtrlpowvkj.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.hnqzz.top/gtrxxnavmz.html

Go:   // 手写循环累加
来源：http://hz.ydjk.org.cn/gtsocbmgyh.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.dianchejie.cn/gtdpcxrsqx.html

C#:   list.Sum();  list.Average()
来源：http://hz.fzhhl.top/gtnnoxmioy.html

[D17] 最大值与最小值
来源：http://hz.yangfankeji.com/gtpfzjunov.html

Py:   max(arr);  min(arr)
来源：http://hz.shzxlz.cn/gtyokiczyi.html

PHP:  max($arr);  min($arr);
来源：http://hz.yanxiufei.cn/gtebbtwkmq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.hysaishi.cn/gtxzvtqygw.html

TS:   Math.max(...arr);
来源：http://hz.yvedp.cn/gtzfcihjzc.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.nanxinkj.top/gtpqcdshzu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.aizwys.cn/gtftrqzkef.html

Ruby: arr.max;  arr.min
来源：http://hz.ydzc1.top/gtdvowinxb.html

C#:   list.Max();  list.Min()
来源：http://hz.xziqi.cn/gtpmbudxgk.html

[D18] 扁平化嵌套数组
来源：http://hz.sufxvd.cn/gtwdnhxrcu.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.yj20258888.top/gtijfydjnl.html

PHP:  array_merge(...$nested);
来源：http://hz.redwolf501.top/gtuhwwmodx.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.xinyue.icu/gtvqxzjejk.html

TS:   nested.flat();
来源：http://hz.ybcxt.top/gtopnhodtl.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.cucudq.cn/gthlpudsek.html

Go:   // 手写双层循环
来源：http://hz.tian-w.cn/gtuznpzqdp.html

Ruby: nested.flatten
来源：http://hz.birdmap.top/gtsufctiko.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.andypj.xyz/gtvzqwliyf.html

[D19] 按字段分组
来源：http://hz.jqgfzy.top/gttaxggsau.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.shzxlz.cn/gtxzmzphjc.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.pycfn.com/gtqsiwlgwp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.316326.xyz/gtpwxdbete.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.yuanzhike.top/gtvwouowja.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.sweek.top/gtumnvwvid.html

Go:   // 手写 map[string][]T
来源：http://hz.xingfuxueyuan.xyz/gtupcafihy.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.bjfxy.top/gtvkqzmrxh.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.yj20258.top/gtckydmfqs.html

[D20] 统计每个元素出现次数
来源：http://hz.jqgufenzy.top/gtlxvqvptg.html

Py:   Counter(arr)
来源：http://hz.shangyingyoupin.top/gtloqmqfvh.html

PHP:  array_count_values($arr);
来源：http://hz.yvedp.cn/gttdqbovol.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jinqigufen.top/gtyzcyqove.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.nanxinkj.top/gtquknvbmx.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.sweek.top/gtqwoatmpd.html

Go:   // 手写 map[T]int
来源：http://hz.kuanghao11.cn/gtwbgfxtjr.html

Ruby: arr.tally
来源：http://hz.hnxiangtu.top/gtipswoily.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.cashguo.top/gtknpjuqdr.html

[D21] 判断是否包含某元素
来源：http://hz.yj202588.top/gtxkmnxrmx.html

Py:   x in arr
来源：http://hz.jlsjyb.cn/gtxjfyxqpp.html

PHP:  in_array($x, $arr, true);
来源：http://hz.yangfankeji.com/gtqnyitaxu.html

JS:   arr.includes(x)
来源：http://hz.pycfn.com/gtyzngvncc.html

TS:   arr.includes(x)
来源：http://hz.jyoumei.cn/gtmewdrlki.html

Java: list.contains(x)
来源：http://hz.jinyuanbaomall.cn/gtbqsxnqdg.html

Go:   slices.Contains(arr, x)
来源：http://hz.yonumen.top/gtnfntejwo.html

Ruby: arr.include?(x)
来源：http://hz.guowangkeji.top/gtrvcgqrpv.html

C#:   list.Contains(x)
来源：http://hz.zhoulong.xyz/gthbnupmlw.html

[D22] 复制数组（避免共享引用）
来源：http://hz.guannengcc.top/gtwtoxzzux.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.yongpay.top/gteaokahmw.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.cheryme.top/gtifxzzjuv.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.daria6918.cn/gtmnadoniy.html

TS:   [...arr];
来源：http://hz.jqgfzy.top/gtmarmwexq.html

Java: new ArrayList<>(list);
来源：http://hz.hywenlv.cn/gtnnrwnuoz.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.sufxvd.cn/gtncvtthrs.html

Ruby: arr.dup;  arr.clone
来源：http://hz.mhx1999.top/gtruinaeiu.html

C#:   new List<int>(list);
来源：http://hz.nanxinkj.top/gtgotrjezr.html

[D23] reduce 累积计算
来源：http://hz.zhixingplan.top/gtrmbkbfqu.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.yj20258.top/gtohexxujw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.yj20258888.top/gtqcitxvdh.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.bjfxy.top/gtpiameall.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.gzhubu.top/gtcxykymhl.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.snrcjt.cn/gtvgevjgla.html

Go:   // 手写循环
来源：http://hz.chenlongwang.top/gtwmrvwcah.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.wangshuangyany.cn/gtfuweivso.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.jlsjyb.cn/gtjbcmkngx.html

[D24] 字典 / Map 基本操作
来源：http://hz.yj202588.top/gtiuyvimkf.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.hammf.cn/gtioxzyfss.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.sweek.top/gtfyxvoefy.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.zhoulong.xyz/gtfnqgwrsz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.xuetiantiany.cn/gtdzqawrnc.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.fengsongda.top/gtimqrdbgc.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.xuanzx.com/gtkvhnvkay.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.ydzc1.top/gtzksrwlcb.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.shanyushiyangtech.top/gtfompfnbj.html

[D25] Set 集合去重与交并差
来源：http://hz.xylfe.cn/gtymkcgtpa.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.nanxuanxn.top/gtnlvbiqyl.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.0kj1m.cn/gtoutyvcoz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.ybcxt.top/gtcpucdyja.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.yj20258888.top/gtplwbacwj.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.xuanzx.com/gtaxhmhjqq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.andypj.xyz/gtgxiqpmet.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.quarkkingdee.top/gtyejqabmj.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.jqgufenzy.top/gtaaxiulng.html

[D26] 数组转字符串
来源：http://hz.jinyuanbaomall.cn/gtdtwmwobd.html

Py:   ", ".join(map(str, arr))
来源：http://hz.zycfv.cn/gtrqrpuquw.html

PHP:  implode(", ", $arr);
来源：http://hz.cdnleiting.top/gtpmjakhmy.html

JS:   arr.join(", ")
来源：http://hz.dianchejie.cn/gtnkyoickz.html

TS:   arr.join(", ")
来源：http://hz.hfpthk.cn/gtisbylmen.html

Java: String.join(", ", list)
来源：http://hz.guowangkeji.top/gtxdxrjwmh.html

Go:   strings.Join(strs, ", ")
来源：http://hz.yuxming.cn/gtbwjsseho.html

Ruby: arr.join(", ")
来源：http://hz.birdmap.top/gtiyyhtgpd.html

C#:   string.Join(", ", list)
来源：http://hz.zhengqikj.top/gttubwqjbn.html

================================================================================
来源：http://hz.sysykeji.top/gtncqfmthx.html

E. 字符串处理
来源：http://hz.feifeiyinyue.top/gtgpuukmiq.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtmobufwrd.html

[E01] 拼接字符串
来源：http://hz.ydjk.org.cn/gtvaofotql.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.pycfn.com/gtrxyxzxbq.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.xuetiantiany.cn/gttdacddbp.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.daria6918.cn/gtoulpkwzv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jqgufenzy.top/gtxywfdsku.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.birdmap.top/gtokvmrwpd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.jyoumei.cn/gtmzbtjvax.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.ydzc1.top/gtgwwnugmi.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.jyoumei.cn/gtbmgfokaa.html

[E02] 重复字符串
来源：http://hz.yj20258888.top/gtrbivlmpb.html

Py:   "ab" * 3
来源：http://hz.yj202588.top/gtyzzdtbhv.html

PHP:  str_repeat("ab", 3);
来源：http://hz.wangdashe.top/gtzmfglcbz.html

JS:   "ab".repeat(3)
来源：http://hz.sxryk.cn/gtixggodkg.html

TS:   "ab".repeat(3)
来源：http://hz.ywan-chungtsiang.top/gtpwpcbwck.html

Java: "ab".repeat(3)
来源：http://hz.yueranfly.top/gtokvsbqsd.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.cheryme.top/gtlyrbavkw.html

Ruby: "ab" * 3
来源：http://hz.xingfuxueyuan.xyz/gtjurusjvf.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.nwbrower.top/gthudrdbhn.html

[E03] 截取子串
来源：http://hz.jiagoushi.top/gtxkjtzfre.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.jinyuanbaomall.cn/gtpeinasop.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.andypj.xyz/gtkqzvpzlq.html


<!-- 参考信息 -->