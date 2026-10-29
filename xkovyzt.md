代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.hesvh.cn/Article/details/gczcerdfm.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.hesvh.cn/Article/details/gyhpqbdmo.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.hesvh.cn/Article/details/ggheiacwf.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.hesvh.cn/Article/details/ghinrxpgg.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.hesvh.cn/Article/details/gkmlqdphz.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.fehbvm.com/Article/details/gdactlikm.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.hesvh.cn/Article/details/gphjdooui.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.fehbvm.com/Article/details/gxwhiciey.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.fehbvm.com/Article/details/gzvlkywor.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gjubbqhuq.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.fehbvm.com/Article/details/gvznicfrg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gnjqagdlt.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gypegtrjd.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.zdbjq.cn/Article/details/gztyrmdqw.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.hesvh.cn/Article/details/gvijuoorc.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.zdbjq.cn/Article/details/gvnzdyouf.sHtML

[C14] 泛型函数
来源：http://read.share.fehbvm.com/Article/details/geqitrdly.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.hesvh.cn/Article/details/gyoteixqu.sHtML

PHP:  // 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gfwgvzvsz.sHtML

JS:   // 无泛型
来源：http://wap.fehbvm.com/Article/details/ggysbgzzo.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.zdbjq.cn/Article/details/gbvfxztym.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.fehbvm.com/Article/details/gyxchkjvk.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.zdbjq.cn/Article/details/gdmtqkokx.sHtML

Ruby: # 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gfwbveggn.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.fehbvm.com/Article/details/gpbmmiytb.sHtML

[C15] 解构 / 展开参数
来源：http://baike.zdbjq.cn/Article/details/ghtlyejzl.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.zdbjq.cn/Article/details/gkumlqkey.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.hesvh.cn/Article/details/gcilbjymb.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/gwhqlhxxg.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.fehbvm.com/Article/details/gpooaysyt.sHtML

Java: // 无解构
来源：http://blog.zdbjq.cn/Article/details/grlkysjbr.sHtML

Go:   // 无解构
来源：http://blog.hesvh.cn/Article/details/guxwjoxhp.sHtML

Ruby: a, b = pair
来源：http://3g.zdbjq.cn/Article/details/ggpfhclzy.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.zdbjq.cn/Article/details/gwtrhlpqi.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.fehbvm.com/Article/details/gwwxrqilz.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.zdbjq.cn/Article/details/gmnvddsml.sHtML

PHP:  // 无重载
来源：http://blog.zdbjq.cn/Article/details/gavxabnfn.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.zdbjq.cn/Article/details/guoswakoe.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.hesvh.cn/Article/details/gzctpvrxb.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.fehbvm.com/Article/details/gvjhbnckk.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.zdbjq.cn/Article/details/gsgjrbrcf.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.hesvh.cn/Article/details/ghgqhstfb.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.hesvh.cn/Article/details/gciefizkz.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gfqbgctjk.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.fehbvm.com/Article/details/gwybndooj.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gezdztivn.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.fehbvm.com/Article/details/ginfmxoiy.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.fehbvm.com/Article/details/gkpksbnxi.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/gzlmhbcuq.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.hesvh.cn/Article/details/gqjmaybna.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.fehbvm.com/Article/details/gyldhxgyo.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.hesvh.cn/Article/details/gjfmvjogv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.hesvh.cn/Article/details/gisqybixd.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.zdbjq.cn/Article/details/goxdqssgv.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.fehbvm.com/Article/details/gkmmvhdyd.sHtML

[D02] 追加元素到末尾
来源：http://blog.zdbjq.cn/Article/details/gjoexzwdw.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.fehbvm.com/Article/details/gydzszmuo.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.zdbjq.cn/Article/details/gwoitxbdl.sHtML

JS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/goqzpwfbi.sHtML

TS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/gzjwkyynb.sHtML

Java: list.add(4);
来源：http://blog.fehbvm.com/Article/details/gtnjjfsfa.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.hesvh.cn/Article/details/gkimntivq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.hesvh.cn/Article/details/gqmsahszr.sHtML

C#:   list.Add(4);
来源：http://mobile.fehbvm.com/Article/details/gxxaqirkr.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.zdbjq.cn/Article/details/gwjzclkce.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.zdbjq.cn/Article/details/gubpphwil.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.hesvh.cn/Article/details/gayktwxjw.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.zdbjq.cn/Article/details/gcxkiblln.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.zdbjq.cn/Article/details/guykvskzf.sHtML

Java: list.add(0, 0);
来源：http://wap.zdbjq.cn/Article/details/gbmcfudjn.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.hesvh.cn/Article/details/guezerjxu.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.zdbjq.cn/Article/details/grflvdnqs.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.fehbvm.com/Article/details/ggcviujpg.sHtML

[D04] 删除元素
来源：http://read.share.zdbjq.cn/Article/details/gfwdcwvlq.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.hesvh.cn/Article/details/gzmctfoxs.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.fehbvm.com/Article/details/geeqrvogz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.zdbjq.cn/Article/details/gzqfveatt.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.zdbjq.cn/Article/details/geuyldypz.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.zdbjq.cn/Article/details/gwjhxidvs.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.fehbvm.com/Article/details/gmujjtycc.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.fehbvm.com/Article/details/gzkaehwce.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.hesvh.cn/Article/details/gukwxlbkb.sHtML

[D05] 访问与修改元素
来源：http://wap.hesvh.cn/Article/details/gjsigyalz.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/ghtptxict.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gzwawcmqf.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gyenhjzxv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.hesvh.cn/Article/details/gvhnzzfti.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.zdbjq.cn/Article/details/gvnsszpkv.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gkqvfgiot.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gyywqzcpn.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gfvqkpsvr.sHtML

[D06] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/gvkkdcmwl.sHtML

Py:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gzddqbdgp.sHtML

PHP:  count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/giryvcxpr.sHtML

JS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/gqfcylfuh.sHtML

TS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/giktyspou.sHtML

Java: list.size();
来源：http://www.share.fehbvm.com/Article/details/gobkqgnyj.sHtML

Go:   len(arr)
来源：http://wap.zdbjq.cn/Article/details/galledusg.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.hesvh.cn/Article/details/gatvsgcxo.sHtML

C#:   list.Count;
来源：http://wap.hesvh.cn/Article/details/gpzbnpwkr.sHtML

[D07] 切片 / 取子数组
来源：http://baike.zdbjq.cn/Article/details/gvvurrzjz.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.fehbvm.com/Article/details/ghllexbce.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.zdbjq.cn/Article/details/gdbnnmtwm.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/grxedbgcf.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gezlxliux.sHtML

Java: list.subList(1, 4);
来源：http://blog.hesvh.cn/Article/details/ghlnhdlpc.sHtML

Go:   arr[1:4]
来源：http://www.blog.fehbvm.com/Article/details/gfayfdyrk.sHtML

Ruby: arr[1, 3]
来源：http://www.share.fehbvm.com/Article/details/gabqvvvqf.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.fehbvm.com/Article/details/gssutmlzo.sHtML

[D08] 合并两个数组
来源：http://wap.fehbvm.com/Article/details/gomqznrvg.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.fehbvm.com/Article/details/gchslkjqv.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.hesvh.cn/Article/details/gorsrlemr.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.hesvh.cn/Article/details/gkrvjuowl.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.hesvh.cn/Article/details/gthvoonvn.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.zdbjq.cn/Article/details/govaneusn.sHtML

Go:   append(a, b...)
来源：http://3g.zdbjq.cn/Article/details/gknnpjace.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.fehbvm.com/Article/details/gligoidhy.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.hesvh.cn/Article/details/gsdyffnvl.sHtML

[D09] 排序（升序）
来源：http://3g.zdbjq.cn/Article/details/gzfkdndin.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/guvicydmu.sHtML

PHP:  sort($arr);
来源：http://www.share.hesvh.cn/Article/details/gfwprhkpi.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.fehbvm.com/Article/details/gcqewsddm.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.zdbjq.cn/Article/details/gevbhxgck.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.fehbvm.com/Article/details/guxowbxma.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gafwejgmj.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gxvekgxgz.sHtML

C#:   list.Sort();
来源：http://m.share.fehbvm.com/Article/details/gimeeaybf.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.hesvh.cn/Article/details/gankccwat.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.hesvh.cn/Article/details/gtbhidqlo.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/gytlbxylx.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/gsyxcsbgo.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/gasnopgrq.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.zdbjq.cn/Article/details/gopjknnmd.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.hesvh.cn/Article/details/gxgdvyrzs.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.hesvh.cn/Article/details/gafnafngb.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.fehbvm.com/Article/details/gbtfihvux.sHtML

[D11] 反转数组
来源：http://m.share.hesvh.cn/Article/details/gcwgtvnzd.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.fehbvm.com/Article/details/gvodzbabk.sHtML

PHP:  array_reverse($arr);
来源：http://3g.hesvh.cn/Article/details/gvophxjer.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.hesvh.cn/Article/details/gtpubrqin.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.zdbjq.cn/Article/details/ghlwsbwxw.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.fehbvm.com/Article/details/gsddviist.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gohsgjwqu.sHtML

Ruby: arr.reverse
来源：http://baike.fehbvm.com/Article/details/gkyyhwtfp.sHtML

C#:   list.Reverse();
来源：http://www.m.share.fehbvm.com/Article/details/grwgwkqoh.sHtML

[D12] 查找元素下标
来源：http://m.share.zdbjq.cn/Article/details/gurvhumcx.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.zdbjq.cn/Article/details/gcgpnhihm.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.hesvh.cn/Article/details/gvdjtmohy.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/gpodowxet.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/gkriraard.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.hesvh.cn/Article/details/galfrjwwz.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/ghhmqitvq.sHtML

Ruby: arr.index(x)
来源：http://blog.zdbjq.cn/Article/details/glyasdven.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.zdbjq.cn/Article/details/gndkpqxul.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.fehbvm.com/Article/details/gkjmqdzui.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.hesvh.cn/Article/details/gxrmqwcjg.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.hesvh.cn/Article/details/gohvjyiea.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gvqcngqta.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.fehbvm.com/Article/details/gvusvifju.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.fehbvm.com/Article/details/gattvjfho.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.zdbjq.cn/Article/details/gfyfqfxzk.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.fehbvm.com/Article/details/gmlfmbamh.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gnurpsptd.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.hesvh.cn/Article/details/gcrwkmkri.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.hesvh.cn/Article/details/gjygrgbim.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.hesvh.cn/Article/details/goldkgeaf.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.hesvh.cn/Article/details/gtversjrd.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/gdoreqhmw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.hesvh.cn/Article/details/ggqnfdgii.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/gctfvvvpd.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gmgltnbpm.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.hesvh.cn/Article/details/goyldtrwu.sHtML

[D15] 去重
来源：http://baike.fehbvm.com/Article/details/gtnhjtbwy.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.fehbvm.com/Article/details/gvodnsmsi.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gmrqlqcgt.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gkwhfulvw.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gftzawock.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.fehbvm.com/Article/details/gxiwcurdc.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.zdbjq.cn/Article/details/ghfoxhluj.sHtML

Ruby: arr.uniq
来源：http://www.blog.zdbjq.cn/Article/details/gjknnpwtg.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.zdbjq.cn/Article/details/gcjatfiof.sHtML

[D16] 求和与平均值
来源：http://3g.fehbvm.com/Article/details/gidxunopj.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.fehbvm.com/Article/details/gzeydpslc.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.zdbjq.cn/Article/details/gspkobyrd.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gkxrsdxqn.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/gylhdppnk.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.fehbvm.com/Article/details/ggiennfle.sHtML

Go:   // 手写循环累加
来源：http://www.blog.hesvh.cn/Article/details/gpkduhxlr.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.hesvh.cn/Article/details/gyzbfcyop.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.zdbjq.cn/Article/details/gtwymjvxd.sHtML

[D17] 最大值与最小值
来源：http://www.share.hesvh.cn/Article/details/gmirnkxcn.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gfavwhqxl.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.zdbjq.cn/Article/details/geiawahzu.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.fehbvm.com/Article/details/gjfqfvnhj.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.hesvh.cn/Article/details/gjfezcxmr.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.hesvh.cn/Article/details/gmawgrria.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.hesvh.cn/Article/details/gkghmqhkj.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.fehbvm.com/Article/details/gxckviwpq.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.zdbjq.cn/Article/details/gqksqspdu.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.fehbvm.com/Article/details/gzkbazshd.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.zdbjq.cn/Article/details/glsblafvm.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.zdbjq.cn/Article/details/gpqvwrdtz.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.zdbjq.cn/Article/details/gjyqreoph.sHtML

TS:   nested.flat();
来源：http://m.share.hesvh.cn/Article/details/gfspfraam.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.fehbvm.com/Article/details/gkaxrodlw.sHtML

Go:   // 手写双层循环
来源：http://m.share.fehbvm.com/Article/details/gjzrocchs.sHtML

Ruby: nested.flatten
来源：http://baike.fehbvm.com/Article/details/gmwwsfhbr.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.fehbvm.com/Article/details/grjfgtbnk.sHtML

[D19] 按字段分组
来源：http://blog.fehbvm.com/Article/details/gsfarhkeu.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.hesvh.cn/Article/details/gbmhhgrfs.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.fehbvm.com/Article/details/gnuucyqxw.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.fehbvm.com/Article/details/gkyunurzr.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/gmfxozsab.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.zdbjq.cn/Article/details/gqjrdzjgi.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.zdbjq.cn/Article/details/gklfqojnv.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.hesvh.cn/Article/details/gyuwpmabj.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.fehbvm.com/Article/details/giftrvhzi.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.zdbjq.cn/Article/details/gidmtsaif.sHtML

Py:   Counter(arr)
来源：http://www.blog.fehbvm.com/Article/details/gilgkihqh.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.hesvh.cn/Article/details/gxdujdrxo.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/gmeyrqddw.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/guxjwrepv.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.hesvh.cn/Article/details/ggpucobnn.sHtML

Go:   // 手写 map[T]int
来源：http://blog.zdbjq.cn/Article/details/gadwraows.sHtML

Ruby: arr.tally
来源：http://read.share.hesvh.cn/Article/details/gxshgfsyj.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.zdbjq.cn/Article/details/gpxoyaoxo.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.zdbjq.cn/Article/details/gpudxsfks.sHtML

Py:   x in arr
来源：http://m.share.hesvh.cn/Article/details/giezsbozw.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.zdbjq.cn/Article/details/ggrcwfuqj.sHtML

JS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/gyvqflzgu.sHtML

TS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gjauasqkz.sHtML

Java: list.contains(x)
来源：http://mobile.fehbvm.com/Article/details/gyvkaaron.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.hesvh.cn/Article/details/gusezjdob.sHtML

Ruby: arr.include?(x)
来源：http://www.share.zdbjq.cn/Article/details/gwegnhpmf.sHtML

C#:   list.Contains(x)
来源：http://wap.hesvh.cn/Article/details/gpqrdvpet.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.zdbjq.cn/Article/details/grrqtskju.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.zdbjq.cn/Article/details/gjyligwus.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.zdbjq.cn/Article/details/gmjxgzeev.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.fehbvm.com/Article/details/gkcogamma.sHtML

TS:   [...arr];
来源：http://blog.hesvh.cn/Article/details/gavrlzffw.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.hesvh.cn/Article/details/gihvgyfvo.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.fehbvm.com/Article/details/gpoopxzvr.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.fehbvm.com/Article/details/goimlnjou.sHtML

C#:   new List<int>(list);
来源：http://mobile.hesvh.cn/Article/details/gtlckuioj.sHtML

[D23] reduce 累积计算
来源：http://3g.zdbjq.cn/Article/details/gpsuyaeyv.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.fehbvm.com/Article/details/gfmocgqxr.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.hesvh.cn/Article/details/gqnnqbtdx.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gkkisjqfk.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gxhhkovrr.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.hesvh.cn/Article/details/gjatrwkyc.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/gfuptqmde.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.fehbvm.com/Article/details/gcnupxlpm.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.fehbvm.com/Article/details/gxzvmugas.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.zdbjq.cn/Article/details/gfsegtmpt.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.fehbvm.com/Article/details/gdhxocfcg.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.fehbvm.com/Article/details/gcpqxzjzw.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.zdbjq.cn/Article/details/ghoeuwfnk.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/ghcppmbpp.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.hesvh.cn/Article/details/gsalazlab.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.zdbjq.cn/Article/details/gprvrbxpp.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.fehbvm.com/Article/details/gcuikflco.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.hesvh.cn/Article/details/ghrnqinlf.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.zdbjq.cn/Article/details/gsrcerslz.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.fehbvm.com/Article/details/gnwziyvkb.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.hesvh.cn/Article/details/guagvmfzf.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.hesvh.cn/Article/details/gpnmrqlud.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.hesvh.cn/Article/details/gixrxxxlo.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.hesvh.cn/Article/details/gojhowgek.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.fehbvm.com/Article/details/ggrdpmavs.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.hesvh.cn/Article/details/gmtxgijgf.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.fehbvm.com/Article/details/gqfkrcbjr.sHtML

[D26] 数组转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gumbsnonx.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.fehbvm.com/Article/details/gpicsedmo.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.zdbjq.cn/Article/details/gthwmvlwp.sHtML

JS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/grbnfqqzp.sHtML

TS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gkfwteotw.sHtML

Java: String.join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/giojgzzyp.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.hesvh.cn/Article/details/gfwosuaih.sHtML

Ruby: arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gwjndnkhf.sHtML

C#:   string.Join(", ", list)
来源：http://3g.hesvh.cn/Article/details/glejqkljc.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gqdhofnvw.sHtML

E. 字符串处理
来源：http://baike.hesvh.cn/Article/details/gmmxezisj.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gafhrsese.sHtML

[E01] 拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gefoiejmz.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.zdbjq.cn/Article/details/gmoppepcj.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.zdbjq.cn/Article/details/gkgboyqnf.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/grshmospf.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gayueqzvz.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.fehbvm.com/Article/details/gmheyspyb.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.zdbjq.cn/Article/details/gqwmvcfey.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.hesvh.cn/Article/details/gpyqydlci.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gmvxwidub.sHtML

[E02] 重复字符串
来源：http://www.blog.fehbvm.com/Article/details/gswfiuqdq.sHtML

Py:   "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gcyteuzlv.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.fehbvm.com/Article/details/gkdrjbdpo.sHtML

JS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gxbcomwxz.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/ggapsnfsp.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/gpvatcbjm.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.zdbjq.cn/Article/details/gwpzkoxyv.sHtML

Ruby: "ab" * 3
来源：http://www.share.fehbvm.com/Article/details/gsjghzluf.sHtML


<!-- 参考信息 -->