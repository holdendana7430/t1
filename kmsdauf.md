代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://m.share.hesvh.cn/Article/details/gaugubdkb.sHtML

C#:   using System.Text;
来源：http://wap.zdbjq.cn/Article/details/gejghsbpw.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.fehbvm.com/Article/details/gsalslvek.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.hesvh.cn/Article/details/gnqucarpo.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.hesvh.cn/Article/details/ghzrdgqxl.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.zdbjq.cn/Article/details/gaozlcrhw.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.hesvh.cn/Article/details/gowlxjnke.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.hesvh.cn/Article/details/gntuprnws.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.zdbjq.cn/Article/details/gobkmpzvc.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.hesvh.cn/Article/details/gqkgsuycw.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.hesvh.cn/Article/details/glxpqywuc.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.zdbjq.cn/Article/details/gsxqxrtxl.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.hesvh.cn/Article/details/gthbfwlep.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gxczcqrux.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.fehbvm.com/Article/details/glqkntobc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gqpwdkmsh.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gacgleglb.sHtML

Go:   func add(a, b int) int
来源：http://baike.hesvh.cn/Article/details/gncaskyzp.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.zdbjq.cn/Article/details/gqdwfxdhc.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.zdbjq.cn/Article/details/gpwcmrfyn.sHtML

[C14] 泛型函数
来源：http://3g.hesvh.cn/Article/details/gbwvalplk.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.fehbvm.com/Article/details/gfvgdxxfp.sHtML

PHP:  // 无泛型
来源：http://mobile.hesvh.cn/Article/details/gukpjitin.sHtML

JS:   // 无泛型
来源：http://wap.zdbjq.cn/Article/details/gwyozplye.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.hesvh.cn/Article/details/ghiioejjv.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.hesvh.cn/Article/details/gmibmfnio.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.fehbvm.com/Article/details/gmuymswea.sHtML

Ruby: # 无泛型
来源：http://wap.fehbvm.com/Article/details/gioiwgufy.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.hesvh.cn/Article/details/glmfeufob.sHtML

[C15] 解构 / 展开参数
来源：http://baike.fehbvm.com/Article/details/gbrognttp.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.fehbvm.com/Article/details/gepfmqorh.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fehbvm.com/Article/details/goffnxklf.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.zdbjq.cn/Article/details/gsvbfrqsg.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.hesvh.cn/Article/details/ghleyfxmn.sHtML

Java: // 无解构
来源：http://mobile.hesvh.cn/Article/details/gckgsjygj.sHtML

Go:   // 无解构
来源：http://read.share.fehbvm.com/Article/details/glkktxxmv.sHtML

Ruby: a, b = pair
来源：http://m.share.hesvh.cn/Article/details/gipervtxd.sHtML

C#:   var (a, b) = pair;
来源：http://wap.fehbvm.com/Article/details/gompklffw.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.fehbvm.com/Article/details/grrvzdgza.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.zdbjq.cn/Article/details/gybknttrz.sHtML

PHP:  // 无重载
来源：http://baike.fehbvm.com/Article/details/gqwioobzz.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.zdbjq.cn/Article/details/gtmafxjjo.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.fehbvm.com/Article/details/gdfcypexr.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.zdbjq.cn/Article/details/gzsfopwqt.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.hesvh.cn/Article/details/gxocrauaw.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.hesvh.cn/Article/details/gwkwlgzwh.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.fehbvm.com/Article/details/gvhtkwqqz.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gjpkhbdwp.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.hesvh.cn/Article/details/ggyzygtay.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/givbkbory.sHtML

[D01] 创建数组 / 列表
来源：http://baike.hesvh.cn/Article/details/gnhkqdroj.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.fehbvm.com/Article/details/guzyqscte.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/grjzkltcj.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.fehbvm.com/Article/details/ghiamtrdq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.fehbvm.com/Article/details/gyxvqjnpy.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.fehbvm.com/Article/details/guvserdur.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.zdbjq.cn/Article/details/gotrnjzpw.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.zdbjq.cn/Article/details/gkkqoptgq.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.fehbvm.com/Article/details/gpaaislci.sHtML

[D02] 追加元素到末尾
来源：http://wap.fehbvm.com/Article/details/gvsdzknbc.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.fehbvm.com/Article/details/gjgyvtjpa.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.zdbjq.cn/Article/details/gnioegkoy.sHtML

JS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/gxqnknkpt.sHtML

TS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/gphhbqbog.sHtML

Java: list.add(4);
来源：http://blog.hesvh.cn/Article/details/gjcjhgedy.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.hesvh.cn/Article/details/gwvfzbzdg.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.fehbvm.com/Article/details/glydhvsto.sHtML

C#:   list.Add(4);
来源：http://3g.fehbvm.com/Article/details/gsoakhfrb.sHtML

[D03] 在指定位置插入元素
来源：http://3g.hesvh.cn/Article/details/ghdqugebd.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.zdbjq.cn/Article/details/gycmkyhqu.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.fehbvm.com/Article/details/gbvgsqhzr.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.hesvh.cn/Article/details/gtdlxjgds.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.zdbjq.cn/Article/details/gepwwzvmg.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gjdophvqi.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.hesvh.cn/Article/details/gjrmqhrvm.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.zdbjq.cn/Article/details/gyseygyzu.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.fehbvm.com/Article/details/gxhppwxxd.sHtML

[D04] 删除元素
来源：http://blog.fehbvm.com/Article/details/gauhimmwt.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.hesvh.cn/Article/details/gzhojvzxt.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.hesvh.cn/Article/details/gihpdiyuf.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.hesvh.cn/Article/details/gvczvapzu.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.hesvh.cn/Article/details/goqnvwzzw.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.hesvh.cn/Article/details/gixexfkvk.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.hesvh.cn/Article/details/gojuqrqlk.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.fehbvm.com/Article/details/gjihetauy.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.hesvh.cn/Article/details/gwkuywptl.sHtML

[D05] 访问与修改元素
来源：http://m.share.hesvh.cn/Article/details/gvqqmvewo.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/grlmhucrn.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/grzminebl.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gjmojthnd.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.hesvh.cn/Article/details/gbisnrsqo.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.zdbjq.cn/Article/details/guhhcddae.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gexagmfjl.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/givttstja.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gfuprrrtt.sHtML

[D06] 数组长度
来源：http://baike.hesvh.cn/Article/details/gggelcixx.sHtML

Py:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gzchyoogc.sHtML

PHP:  count($arr);
来源：http://3g.zdbjq.cn/Article/details/ghtquokqh.sHtML

JS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/gmdoawpeb.sHtML

TS:   arr.length
来源：http://3g.hesvh.cn/Article/details/gjbarajfk.sHtML

Java: list.size();
来源：http://m.share.hesvh.cn/Article/details/gdcwanqgu.sHtML

Go:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gmurncwgl.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.zdbjq.cn/Article/details/gjllicszj.sHtML

C#:   list.Count;
来源：http://m.share.fehbvm.com/Article/details/gzkymxyxn.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.zdbjq.cn/Article/details/gntvrnhnh.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.hesvh.cn/Article/details/gclnstcun.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.fehbvm.com/Article/details/ghdeketvj.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gxqgerwku.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gscndtwip.sHtML

Java: list.subList(1, 4);
来源：http://3g.fehbvm.com/Article/details/gdxysuyiz.sHtML

Go:   arr[1:4]
来源：http://blog.fehbvm.com/Article/details/gtydrztwj.sHtML

Ruby: arr[1, 3]
来源：http://baike.hesvh.cn/Article/details/gjkywvrnf.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.zdbjq.cn/Article/details/gfwgtqphj.sHtML

[D08] 合并两个数组
来源：http://blog.hesvh.cn/Article/details/gbkmjfipl.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.zdbjq.cn/Article/details/gwcbqcksi.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.fehbvm.com/Article/details/garvcnedx.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.hesvh.cn/Article/details/gmhirutqw.sHtML

TS:   [...a, ...b];
来源：http://www.blog.hesvh.cn/Article/details/gnxvwttqq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.hesvh.cn/Article/details/gporlpwqf.sHtML

Go:   append(a, b...)
来源：http://wap.hesvh.cn/Article/details/gnnvnklnz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.hesvh.cn/Article/details/gfhkpljmd.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.hesvh.cn/Article/details/ghoqocykn.sHtML

[D09] 排序（升序）
来源：http://blog.zdbjq.cn/Article/details/gmqyinblh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/giiizemuh.sHtML

PHP:  sort($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gmektspqb.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.hesvh.cn/Article/details/gioffhudj.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.fehbvm.com/Article/details/geuympfnr.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.fehbvm.com/Article/details/gkagxvdzc.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gcacskspn.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/ggziamjlr.sHtML

C#:   list.Sort();
来源：http://wap.fehbvm.com/Article/details/gmfleijms.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.fehbvm.com/Article/details/gamhzhnuc.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.hesvh.cn/Article/details/gpdqlosyf.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/gawyefqbt.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/gbmzkktyc.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/gczydkeof.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.fehbvm.com/Article/details/gnehsazwg.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.hesvh.cn/Article/details/gtjzkhnbz.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.fehbvm.com/Article/details/gfvfhbzid.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.zdbjq.cn/Article/details/gneoewfuz.sHtML

[D11] 反转数组
来源：http://www.m.share.fehbvm.com/Article/details/gsxyxbgbd.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.zdbjq.cn/Article/details/gpoxuunhu.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.fehbvm.com/Article/details/gusmouyfr.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.hesvh.cn/Article/details/gsucbpivm.sHtML

TS:   [...arr].reverse();
来源：http://3g.zdbjq.cn/Article/details/gkrrwoiwu.sHtML

Java: Collections.reverse(list);
来源：http://3g.fehbvm.com/Article/details/glvemjkiv.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.fehbvm.com/Article/details/glhqcrall.sHtML

Ruby: arr.reverse
来源：http://read.share.fehbvm.com/Article/details/ghuutfqpb.sHtML

C#:   list.Reverse();
来源：http://www.share.hesvh.cn/Article/details/gfthjglaa.sHtML

[D12] 查找元素下标
来源：http://www.m.share.zdbjq.cn/Article/details/gyxsplhfs.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.zdbjq.cn/Article/details/gnwuxezvt.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.hesvh.cn/Article/details/gbovdzjqr.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.hesvh.cn/Article/details/gyiulqvoh.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/gtsfzgjzs.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.zdbjq.cn/Article/details/grdkuprav.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.fehbvm.com/Article/details/ghzyvqfqd.sHtML

Ruby: arr.index(x)
来源：http://blog.hesvh.cn/Article/details/ggxgngfym.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.zdbjq.cn/Article/details/ggxwcojhg.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.hesvh.cn/Article/details/gkpnkzjtt.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.hesvh.cn/Article/details/gdoxhpdxn.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.zdbjq.cn/Article/details/ggafmdigh.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/ggbcuqztt.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gijbuxdhc.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gxiskesyz.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.zdbjq.cn/Article/details/guerjicxn.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.fehbvm.com/Article/details/gtesltzqu.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gavdbcfdy.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.zdbjq.cn/Article/details/gfabtwwse.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.zdbjq.cn/Article/details/gcyxqasyu.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.zdbjq.cn/Article/details/ghzuzuoda.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gqytqcpar.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.hesvh.cn/Article/details/guiszpyyi.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.hesvh.cn/Article/details/gynnvybmu.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/gbvpcbkmx.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gtwsvpbia.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.zdbjq.cn/Article/details/gokdsdgvr.sHtML

[D15] 去重
来源：http://www.share.hesvh.cn/Article/details/ghjgkpbya.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/gguifhusz.sHtML

PHP:  array_unique($arr);
来源：http://baike.hesvh.cn/Article/details/gnhtssjrk.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gsuiefziv.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/grhocxbmj.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.hesvh.cn/Article/details/gjqmaefuw.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.fehbvm.com/Article/details/gkegzhnwk.sHtML

Ruby: arr.uniq
来源：http://blog.fehbvm.com/Article/details/gpvhnofmt.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.fehbvm.com/Article/details/gwsqpdwmn.sHtML

[D16] 求和与平均值
来源：http://www.share.hesvh.cn/Article/details/glemnmdnc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.fehbvm.com/Article/details/goozbrpfx.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.hesvh.cn/Article/details/gwasoagga.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gqsmoysci.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fehbvm.com/Article/details/gdfpvvgpv.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.fehbvm.com/Article/details/gzfzngbkr.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.hesvh.cn/Article/details/gvtmagopf.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.fehbvm.com/Article/details/gvzqgmmyr.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.fehbvm.com/Article/details/gpwueafpb.sHtML

[D17] 最大值与最小值
来源：http://baike.fehbvm.com/Article/details/gircjtlnc.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.zdbjq.cn/Article/details/gjxhratph.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.zdbjq.cn/Article/details/guxtnlrvx.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.fehbvm.com/Article/details/gxakqrzcc.sHtML

TS:   Math.max(...arr);
来源：http://www.share.fehbvm.com/Article/details/gnifrgejd.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.hesvh.cn/Article/details/gxdfwhmue.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.hesvh.cn/Article/details/ghtokgiig.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.zdbjq.cn/Article/details/gduulzqdn.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.zdbjq.cn/Article/details/gtkagtnnu.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.fehbvm.com/Article/details/grwcxtkkc.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.hesvh.cn/Article/details/gbnlrzdkc.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.fehbvm.com/Article/details/gxggihxtf.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.zdbjq.cn/Article/details/glnajzcqm.sHtML

TS:   nested.flat();
来源：http://3g.fehbvm.com/Article/details/gxbicnqcx.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.hesvh.cn/Article/details/gcookhjpm.sHtML

Go:   // 手写双层循环
来源：http://blog.zdbjq.cn/Article/details/gqavcoblc.sHtML

Ruby: nested.flatten
来源：http://m.share.fehbvm.com/Article/details/gfidnrlnh.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.fehbvm.com/Article/details/gxxrrdojp.sHtML

[D19] 按字段分组
来源：http://baike.fehbvm.com/Article/details/gohdkdofv.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.zdbjq.cn/Article/details/gvbksnxdf.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.zdbjq.cn/Article/details/gnmiudqlp.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.zdbjq.cn/Article/details/ggfzcahcf.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.fehbvm.com/Article/details/gzzkaltfq.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.fehbvm.com/Article/details/gtafgphti.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.zdbjq.cn/Article/details/ggtpxxrzl.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.hesvh.cn/Article/details/gckednilj.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.zdbjq.cn/Article/details/gnsnahyoe.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.zdbjq.cn/Article/details/gvbifakti.sHtML

Py:   Counter(arr)
来源：http://www.blog.hesvh.cn/Article/details/goajadqal.sHtML

PHP:  array_count_values($arr);
来源：http://blog.zdbjq.cn/Article/details/gubptpdcg.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/gnaiuhnfa.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/gmsnmjryl.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.hesvh.cn/Article/details/gfpexugfi.sHtML

Go:   // 手写 map[T]int
来源：http://blog.fehbvm.com/Article/details/glfswrzkz.sHtML

Ruby: arr.tally
来源：http://3g.zdbjq.cn/Article/details/gjirtkpaf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.fehbvm.com/Article/details/guphfhfqx.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.zdbjq.cn/Article/details/gbgsosmgj.sHtML

Py:   x in arr
来源：http://wap.zdbjq.cn/Article/details/gywiscinj.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.hesvh.cn/Article/details/gfholjzfc.sHtML

JS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/ggbvfmdpu.sHtML

TS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/gannhugfs.sHtML

Java: list.contains(x)
来源：http://m.share.fehbvm.com/Article/details/gtoyzlczu.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gyjdqvzrt.sHtML

Ruby: arr.include?(x)
来源：http://mobile.zdbjq.cn/Article/details/gvzjzhilg.sHtML

C#:   list.Contains(x)
来源：http://blog.fehbvm.com/Article/details/glpwwpuiq.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.hesvh.cn/Article/details/govtjxlsr.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.zdbjq.cn/Article/details/gnifselzs.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.fehbvm.com/Article/details/gjexizgrj.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.fehbvm.com/Article/details/gltajikyd.sHtML

TS:   [...arr];
来源：http://www.share.fehbvm.com/Article/details/gkuhkfcga.sHtML

Java: new ArrayList<>(list);
来源：http://3g.fehbvm.com/Article/details/glostjciu.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.fehbvm.com/Article/details/gnmbweilb.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.hesvh.cn/Article/details/gacopmvng.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gcqdbuufv.sHtML

[D23] reduce 累积计算
来源：http://wap.zdbjq.cn/Article/details/gwebyedmr.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.zdbjq.cn/Article/details/gwibwsqhm.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.hesvh.cn/Article/details/gkgyohied.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gyhrvpvdb.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/ghsisgceq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.hesvh.cn/Article/details/gzkwslyiv.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/gewlxoapn.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.hesvh.cn/Article/details/gethnkcmx.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.hesvh.cn/Article/details/gnlxhvxrt.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.zdbjq.cn/Article/details/gfampgjog.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.hesvh.cn/Article/details/gkwogbcom.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.hesvh.cn/Article/details/geuslrrfu.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.zdbjq.cn/Article/details/gwwywjrlg.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/grjqjkqrk.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.zdbjq.cn/Article/details/gkhkgovjr.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.zdbjq.cn/Article/details/gampeufvp.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.fehbvm.com/Article/details/gywopsswa.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.hesvh.cn/Article/details/gakgzvxhi.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.zdbjq.cn/Article/details/gvxqtqewt.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.zdbjq.cn/Article/details/gwewmqela.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.zdbjq.cn/Article/details/guvnxanbj.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.hesvh.cn/Article/details/gnzsgukiv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.zdbjq.cn/Article/details/gunrguxgd.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gqovftvrs.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.hesvh.cn/Article/details/gckxywdwj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.zdbjq.cn/Article/details/gjkyjuaui.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/goqbxnvzz.sHtML

[D26] 数组转字符串
来源：http://mobile.hesvh.cn/Article/details/grnzffigp.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.hesvh.cn/Article/details/gyolulcxw.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.fehbvm.com/Article/details/gcietjzvc.sHtML

JS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gblckxaak.sHtML

TS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/ggnisjmfu.sHtML

Java: String.join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/gvxjzncfc.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.hesvh.cn/Article/details/gdntycsef.sHtML

Ruby: arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/goombkebd.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/guwuluaco.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gyctplnas.sHtML

E. 字符串处理
来源：http://read.share.zdbjq.cn/Article/details/grmeipwpt.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gyotcfkwp.sHtML

[E01] 拼接字符串
来源：http://blog.hesvh.cn/Article/details/gloehyrpk.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.zdbjq.cn/Article/details/gqgynfomh.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.fehbvm.com/Article/details/glznnfekf.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/gdlhrmnut.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/gcadokfkf.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.fehbvm.com/Article/details/gwbqihllx.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.zdbjq.cn/Article/details/gcaeiwibp.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.hesvh.cn/Article/details/gutczliwj.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gxbjjczzm.sHtML

[E02] 重复字符串
来源：http://read.share.fehbvm.com/Article/details/gejzpdpek.sHtML

Py:   "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/gurcjmjns.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.hesvh.cn/Article/details/gfovmpgmr.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gaikjgoks.sHtML


<!-- 参考信息 -->