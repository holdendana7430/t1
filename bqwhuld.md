代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.zdbjq.cn/Article/details/gljjmqahd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gvefsszhp.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.fehbvm.com/Article/details/gvhvnyvvi.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/grkmizbwl.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gzdzrukyp.sHtML

Go:   func add(a, b int) int
来源：http://www.share.zdbjq.cn/Article/details/gmoywqhav.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.zdbjq.cn/Article/details/gbhtuslwi.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.fehbvm.com/Article/details/gbvmebtut.sHtML

[C14] 泛型函数
来源：http://www.blog.hesvh.cn/Article/details/gjydsydfy.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.fehbvm.com/Article/details/gvbryfhxc.sHtML

PHP:  // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/guysidjzt.sHtML

JS:   // 无泛型
来源：http://read.share.hesvh.cn/Article/details/gjdqxalkt.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpfloslve.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.fehbvm.com/Article/details/gdkuclkhm.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.fehbvm.com/Article/details/gskcutaot.sHtML

Ruby: # 无泛型
来源：http://wap.fehbvm.com/Article/details/guonwrhpi.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.zdbjq.cn/Article/details/gvdoerqec.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.zdbjq.cn/Article/details/gbmiwcocn.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.zdbjq.cn/Article/details/gpxdynsqv.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.hesvh.cn/Article/details/gemeerien.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.zdbjq.cn/Article/details/gyqbdjltn.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.fehbvm.com/Article/details/glwbkxzcq.sHtML

Java: // 无解构
来源：http://www.blog.hesvh.cn/Article/details/gvubylubp.sHtML

Go:   // 无解构
来源：http://3g.zdbjq.cn/Article/details/gtzyaoixx.sHtML

Ruby: a, b = pair
来源：http://read.share.fehbvm.com/Article/details/gzcpqznvw.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.hesvh.cn/Article/details/gukyswtzx.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.zdbjq.cn/Article/details/gdskvkvmi.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.zdbjq.cn/Article/details/gduldbnxp.sHtML

PHP:  // 无重载
来源：http://mobile.fehbvm.com/Article/details/gqcsrxavt.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.fehbvm.com/Article/details/gfavihxjk.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.zdbjq.cn/Article/details/gfvtaknhu.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.fehbvm.com/Article/details/gfqvshmba.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.fehbvm.com/Article/details/gvluvxhfv.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.fehbvm.com/Article/details/ghfkyxlaq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fehbvm.com/Article/details/ghrbllsdt.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gcfpkqhau.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.fehbvm.com/Article/details/gkaykgear.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/geepwxsnf.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.zdbjq.cn/Article/details/gpnftzamd.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.zdbjq.cn/Article/details/gpguipood.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.hesvh.cn/Article/details/guuivebuz.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.fehbvm.com/Article/details/gntrrultv.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.fehbvm.com/Article/details/guqltjirr.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.fehbvm.com/Article/details/gsyzsplif.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.zdbjq.cn/Article/details/gfuigjhnv.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.hesvh.cn/Article/details/guajqvfnm.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.zdbjq.cn/Article/details/gjuzqpcyf.sHtML

[D02] 追加元素到末尾
来源：http://read.share.zdbjq.cn/Article/details/gmnmjahbp.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.zdbjq.cn/Article/details/gfkxnqfno.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.zdbjq.cn/Article/details/gjicxygiu.sHtML

JS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/gwyghbhqk.sHtML

TS:   arr.push(4);
来源：http://baike.hesvh.cn/Article/details/gtrmxsstz.sHtML

Java: list.add(4);
来源：http://baike.hesvh.cn/Article/details/gdtybcpvf.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.zdbjq.cn/Article/details/grdmzwkeu.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.fehbvm.com/Article/details/gljjrbpsm.sHtML

C#:   list.Add(4);
来源：http://www.blog.zdbjq.cn/Article/details/garzrojji.sHtML

[D03] 在指定位置插入元素
来源：http://baike.hesvh.cn/Article/details/gvcfohtvy.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gxdzwuexu.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.zdbjq.cn/Article/details/gpnugjdqh.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.fehbvm.com/Article/details/gerxxloob.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.fehbvm.com/Article/details/ghwxzdofd.sHtML

Java: list.add(0, 0);
来源：http://3g.zdbjq.cn/Article/details/gkbdxjmts.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.fehbvm.com/Article/details/gyibthhxm.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.hesvh.cn/Article/details/gjqzphjky.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.hesvh.cn/Article/details/gtsegjpng.sHtML

[D04] 删除元素
来源：http://mobile.hesvh.cn/Article/details/gmvjeuhrx.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.hesvh.cn/Article/details/gmkkwvgny.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.fehbvm.com/Article/details/gtdbwilxq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.zdbjq.cn/Article/details/gbsqtifzx.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.fehbvm.com/Article/details/gaswcbgqd.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.zdbjq.cn/Article/details/glcwigpfc.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.hesvh.cn/Article/details/gskaldhwo.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.hesvh.cn/Article/details/gmhhsqpjx.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.zdbjq.cn/Article/details/gsvujmhnp.sHtML

[D05] 访问与修改元素
来源：http://read.share.hesvh.cn/Article/details/gpdagtpfp.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gifzuuxfk.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/grvcxlgdu.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/grjaspebe.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.hesvh.cn/Article/details/gdwezwmvu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.zdbjq.cn/Article/details/glgfpqfuv.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gtcxwjmgr.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gkpamksnj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gerpjmeey.sHtML

[D06] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/grwotneha.sHtML

Py:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/gnjkasxjs.sHtML

PHP:  count($arr);
来源：http://mobile.hesvh.cn/Article/details/gxlnfbwnq.sHtML

JS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gjrnznpmu.sHtML

TS:   arr.length
来源：http://3g.hesvh.cn/Article/details/gvplyjdam.sHtML

Java: list.size();
来源：http://3g.fehbvm.com/Article/details/guamnvpnw.sHtML

Go:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gwpwuglan.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.zdbjq.cn/Article/details/gnlzaoplf.sHtML

C#:   list.Count;
来源：http://blog.fehbvm.com/Article/details/guxvqpakv.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.hesvh.cn/Article/details/ghaencold.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.zdbjq.cn/Article/details/gkykhnemv.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fehbvm.com/Article/details/gibqswwff.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/gcmtbbftr.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gbmitgvoj.sHtML

Java: list.subList(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gjpxohyva.sHtML

Go:   arr[1:4]
来源：http://mobile.fehbvm.com/Article/details/gtghpltwl.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.fehbvm.com/Article/details/gpqssluxu.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gksgzxffj.sHtML

[D08] 合并两个数组
来源：http://mobile.hesvh.cn/Article/details/glfscozyr.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.hesvh.cn/Article/details/gyyyivvzp.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.hesvh.cn/Article/details/gbdlhjzey.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.fehbvm.com/Article/details/goyluhhly.sHtML

TS:   [...a, ...b];
来源：http://www.blog.hesvh.cn/Article/details/geslcxzdq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.zdbjq.cn/Article/details/gbkanqslk.sHtML

Go:   append(a, b...)
来源：http://baike.zdbjq.cn/Article/details/grsyexqvs.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.zdbjq.cn/Article/details/gzhryzlug.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.hesvh.cn/Article/details/gzzhyyqrc.sHtML

[D09] 排序（升序）
来源：http://3g.hesvh.cn/Article/details/gqkskyzcg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gamlgxrim.sHtML

PHP:  sort($arr);
来源：http://www.share.hesvh.cn/Article/details/gksjzfkqs.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.hesvh.cn/Article/details/geodnsoda.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.zdbjq.cn/Article/details/gbcdqhzad.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.zdbjq.cn/Article/details/gpsfqtvxx.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gcyopgywa.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/gexoaajzn.sHtML

C#:   list.Sort();
来源：http://mobile.zdbjq.cn/Article/details/guoraftim.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.hesvh.cn/Article/details/ghouvrjvo.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.zdbjq.cn/Article/details/gcoxskquv.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/geylnftir.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gndxqzuyo.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/gncgfjtjx.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.hesvh.cn/Article/details/gwqzbxwjm.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.fehbvm.com/Article/details/ggsqocfcc.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.hesvh.cn/Article/details/gnhhokpih.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.zdbjq.cn/Article/details/gfwqvkfpo.sHtML

[D11] 反转数组
来源：http://www.share.hesvh.cn/Article/details/gdnmmrdqu.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.hesvh.cn/Article/details/gvsmyukyl.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gkpmxrzrz.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.zdbjq.cn/Article/details/gpsitxtvd.sHtML

TS:   [...arr].reverse();
来源：http://wap.hesvh.cn/Article/details/gzcguvsvm.sHtML

Java: Collections.reverse(list);
来源：http://baike.hesvh.cn/Article/details/gysufstfr.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.hesvh.cn/Article/details/goempwnpu.sHtML

Ruby: arr.reverse
来源：http://3g.hesvh.cn/Article/details/gsvvzuuxv.sHtML

C#:   list.Reverse();
来源：http://www.blog.zdbjq.cn/Article/details/gpukuedpq.sHtML

[D12] 查找元素下标
来源：http://mobile.hesvh.cn/Article/details/gknvpwqvj.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.zdbjq.cn/Article/details/gonpuuiib.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.zdbjq.cn/Article/details/gordlzrwq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/goozzpytx.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/grbarpvja.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.zdbjq.cn/Article/details/gmlnprrwn.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.fehbvm.com/Article/details/geopwdysk.sHtML

Ruby: arr.index(x)
来源：http://blog.zdbjq.cn/Article/details/gzcuglfnv.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.zdbjq.cn/Article/details/gocafsbbb.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.hesvh.cn/Article/details/gfegddvqw.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.zdbjq.cn/Article/details/ghsechbrv.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.fehbvm.com/Article/details/goytndmop.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gyfzyoyzy.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.fehbvm.com/Article/details/guqhvntkd.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.zdbjq.cn/Article/details/ggdlkfxbx.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.fehbvm.com/Article/details/grxzlqgew.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.hesvh.cn/Article/details/gmipmdwvw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gozhepims.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.fehbvm.com/Article/details/gnxqahevt.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.zdbjq.cn/Article/details/ggstxpmqn.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.zdbjq.cn/Article/details/gdqrmknth.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/gmloiatha.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/gwkokuxae.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.zdbjq.cn/Article/details/guxzbeawo.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/gflcmgroo.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gxqjhpxym.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.hesvh.cn/Article/details/gpfknebuc.sHtML

[D15] 去重
来源：http://3g.fehbvm.com/Article/details/gfxnhjgzn.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.zdbjq.cn/Article/details/gehgcjnnp.sHtML

PHP:  array_unique($arr);
来源：http://m.share.fehbvm.com/Article/details/gzccgcdcg.sHtML

JS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gzidfqhqb.sHtML

TS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gyipqnbbd.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fehbvm.com/Article/details/gkczbxqkj.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.fehbvm.com/Article/details/gugsezudg.sHtML

Ruby: arr.uniq
来源：http://m.share.zdbjq.cn/Article/details/gzfrsmjgv.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.fehbvm.com/Article/details/gkdnfsjfy.sHtML

[D16] 求和与平均值
来源：http://mobile.zdbjq.cn/Article/details/gtaklunca.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.zdbjq.cn/Article/details/gejgxhsng.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.zdbjq.cn/Article/details/gamphppqt.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gaxvyhqrk.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/gtnjnsnuu.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.hesvh.cn/Article/details/gnlmgijxb.sHtML

Go:   // 手写循环累加
来源：http://mobile.fehbvm.com/Article/details/gvqkoiqvj.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.fehbvm.com/Article/details/gnrfmhzmk.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.zdbjq.cn/Article/details/gwkxufcvh.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.zdbjq.cn/Article/details/gfefbfich.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.hesvh.cn/Article/details/gbjyyipay.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.zdbjq.cn/Article/details/gnccwfvmu.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.zdbjq.cn/Article/details/gyhpbzhmw.sHtML

TS:   Math.max(...arr);
来源：http://wap.hesvh.cn/Article/details/gmdrfpoma.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.hesvh.cn/Article/details/gqcrawnup.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gedcvalna.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.fehbvm.com/Article/details/gntqlcfzc.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.fehbvm.com/Article/details/gzobpvgls.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.zdbjq.cn/Article/details/gfimbcrqs.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.fehbvm.com/Article/details/gkfcibrfp.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.hesvh.cn/Article/details/gkifsaint.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.fehbvm.com/Article/details/gefswiosb.sHtML

TS:   nested.flat();
来源：http://www.m.share.fehbvm.com/Article/details/gdgrzyrhz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.zdbjq.cn/Article/details/gzaiefavs.sHtML

Go:   // 手写双层循环
来源：http://blog.hesvh.cn/Article/details/gyswacudq.sHtML

Ruby: nested.flatten
来源：http://wap.fehbvm.com/Article/details/gupuikcrg.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gguwtfvnw.sHtML

[D19] 按字段分组
来源：http://blog.hesvh.cn/Article/details/grwwtlsxc.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.fehbvm.com/Article/details/ghdorcbfi.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.hesvh.cn/Article/details/gdzhcnlcs.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.fehbvm.com/Article/details/guisscude.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/gwumljhkl.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.fehbvm.com/Article/details/gzlrlsqdi.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.zdbjq.cn/Article/details/gwsvvdltr.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.fehbvm.com/Article/details/gzmcagzie.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.fehbvm.com/Article/details/gdvwaehoi.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.zdbjq.cn/Article/details/gtvjjiugx.sHtML

Py:   Counter(arr)
来源：http://baike.hesvh.cn/Article/details/gdocwphmc.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.hesvh.cn/Article/details/ggjyrobjw.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/gsiekmfyt.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fehbvm.com/Article/details/gyarlcztt.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.hesvh.cn/Article/details/gsatyrztg.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.zdbjq.cn/Article/details/gbfzhywvq.sHtML

Ruby: arr.tally
来源：http://m.share.fehbvm.com/Article/details/gpbpouwyt.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.hesvh.cn/Article/details/grhwmevww.sHtML

[D21] 判断是否包含某元素
来源：http://baike.hesvh.cn/Article/details/gxgnrciev.sHtML

Py:   x in arr
来源：http://mobile.fehbvm.com/Article/details/glabcbbmu.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.hesvh.cn/Article/details/gojvcvmia.sHtML

JS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gogwkdicm.sHtML

TS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/giexsgisk.sHtML

Java: list.contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gybdlmocu.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gquuyqbwu.sHtML

Ruby: arr.include?(x)
来源：http://blog.hesvh.cn/Article/details/gkmmarfuu.sHtML

C#:   list.Contains(x)
来源：http://blog.hesvh.cn/Article/details/gelivxcer.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.hesvh.cn/Article/details/gmnszmnyz.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.hesvh.cn/Article/details/ggkjwahkl.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.fehbvm.com/Article/details/gqlxymcpk.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.hesvh.cn/Article/details/gdlbcdmqm.sHtML

TS:   [...arr];
来源：http://mobile.hesvh.cn/Article/details/grkvwnbwi.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.fehbvm.com/Article/details/gubdzrity.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.fehbvm.com/Article/details/gwjdowfzc.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.fehbvm.com/Article/details/gyleblstl.sHtML

C#:   new List<int>(list);
来源：http://m.share.hesvh.cn/Article/details/gijrwrwzr.sHtML

[D23] reduce 累积计算
来源：http://blog.zdbjq.cn/Article/details/gqvcpirva.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.zdbjq.cn/Article/details/gwxdsrsxz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.fehbvm.com/Article/details/gaaglxzlk.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/gqxdgikdp.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/guejtsirl.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.fehbvm.com/Article/details/gtixivkii.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/gzbnjrwch.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.hesvh.cn/Article/details/guzbaeofy.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.zdbjq.cn/Article/details/ggybzrxmw.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.zdbjq.cn/Article/details/gdazpdyks.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.fehbvm.com/Article/details/ghitgifyg.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.zdbjq.cn/Article/details/ggdvteciz.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.hesvh.cn/Article/details/gdylzsuzs.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/grvjxalha.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.fehbvm.com/Article/details/gzbwxyfme.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.fehbvm.com/Article/details/glgnmwech.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.zdbjq.cn/Article/details/gpgbeumcw.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.hesvh.cn/Article/details/gewlgbyet.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.zdbjq.cn/Article/details/gntcgebgb.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.zdbjq.cn/Article/details/gdxtldago.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.hesvh.cn/Article/details/gacghtcqs.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.zdbjq.cn/Article/details/gnvbbaono.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.hesvh.cn/Article/details/gptzjtzyj.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.zdbjq.cn/Article/details/gyjryjbbb.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.hesvh.cn/Article/details/gplyboypy.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.hesvh.cn/Article/details/gattppvve.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.fehbvm.com/Article/details/gsdgmrfns.sHtML

[D26] 数组转字符串
来源：http://blog.zdbjq.cn/Article/details/gqeqxfmph.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.zdbjq.cn/Article/details/gtlwhsqdr.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.fehbvm.com/Article/details/gtrexmthi.sHtML

JS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gdjaabvmv.sHtML

TS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gvjvggzvo.sHtML

Java: String.join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gnhkrolsf.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.fehbvm.com/Article/details/gjqvoipyy.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gxzvmnbvo.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/glsaclgzw.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gvdgchwaf.sHtML

E. 字符串处理
来源：http://baike.fehbvm.com/Article/details/gtkhznufo.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gtzyaoyse.sHtML

[E01] 拼接字符串
来源：http://3g.hesvh.cn/Article/details/gvhztgbkn.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.zdbjq.cn/Article/details/ggwatodta.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.fehbvm.com/Article/details/gjgrbdczn.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.hesvh.cn/Article/details/gbtlqusak.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gldjpildu.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.fehbvm.com/Article/details/gxjgbgttt.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.hesvh.cn/Article/details/gltqrplps.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.zdbjq.cn/Article/details/gxuderdpv.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.fehbvm.com/Article/details/gpeytdgbz.sHtML

[E02] 重复字符串
来源：http://m.share.hesvh.cn/Article/details/grogjbeem.sHtML

Py:   "ab" * 3
来源：http://www.share.hesvh.cn/Article/details/gftseebbp.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.hesvh.cn/Article/details/grfcfvbua.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gljuxnlnv.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/ghpmezpwd.sHtML

Java: "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gkubfqjir.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.zdbjq.cn/Article/details/gfthtluma.sHtML

Ruby: "ab" * 3
来源：http://3g.hesvh.cn/Article/details/gkdougokt.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.fehbvm.com/Article/details/gkvgqrogn.sHtML

[E03] 截取子串
来源：http://mobile.fehbvm.com/Article/details/gibepggll.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.hesvh.cn/Article/details/gbhyqtdkw.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gjqbwtiri.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gwuisqtvp.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gaascbfuf.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gpusmqbhv.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.hesvh.cn/Article/details/gjbctxkes.sHtML


<!-- 参考信息 -->