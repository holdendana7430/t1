代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://baike.hesvh.cn/Article/details/gmplvjnzc.sHtML

C#:   using System.Text;
来源：http://baike.hesvh.cn/Article/details/ggsnnkzum.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.zdbjq.cn/Article/details/gebxxqxsw.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.hesvh.cn/Article/details/gosvshphs.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.hesvh.cn/Article/details/gfbmesvci.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.hesvh.cn/Article/details/gkhrabxkj.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/glfmvqilk.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.fehbvm.com/Article/details/grmpisvvr.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.zdbjq.cn/Article/details/gnygtcoby.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.fehbvm.com/Article/details/gumdgcyco.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.fehbvm.com/Article/details/gycsqyhbe.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.zdbjq.cn/Article/details/gycqdtcfs.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.zdbjq.cn/Article/details/gqgipauao.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gxfjzgrll.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.fehbvm.com/Article/details/gmchyprsy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gtyldpxsb.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gzsrjjeel.sHtML

Go:   func add(a, b int) int
来源：http://read.share.fehbvm.com/Article/details/gtqbkuiyu.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.hesvh.cn/Article/details/gmqpfihft.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.hesvh.cn/Article/details/gozurmnpr.sHtML

[C14] 泛型函数
来源：http://baike.hesvh.cn/Article/details/gveboowoe.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.fehbvm.com/Article/details/gkbneodzk.sHtML

PHP:  // 无泛型
来源：http://3g.fehbvm.com/Article/details/gkgptypta.sHtML

JS:   // 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gjontwwvj.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.fehbvm.com/Article/details/geuefasei.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.fehbvm.com/Article/details/gmksmhqta.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.zdbjq.cn/Article/details/gtunnpabj.sHtML

Ruby: # 无泛型
来源：http://www.share.fehbvm.com/Article/details/gitszzghu.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.fehbvm.com/Article/details/glkqtiywl.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.fehbvm.com/Article/details/ggwpurmgp.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.fehbvm.com/Article/details/gdtfdmddw.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.hesvh.cn/Article/details/gvlhmfsno.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.zdbjq.cn/Article/details/gozzlurqo.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.fehbvm.com/Article/details/gosujatql.sHtML

Java: // 无解构
来源：http://read.share.fehbvm.com/Article/details/gifjzqeit.sHtML

Go:   // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/gaocticer.sHtML

Ruby: a, b = pair
来源：http://www.share.hesvh.cn/Article/details/gcgamtwxh.sHtML

C#:   var (a, b) = pair;
来源：http://blog.zdbjq.cn/Article/details/gytecukby.sHtML

[C16] 函数 / 方法重载
来源：http://blog.zdbjq.cn/Article/details/gfrsfehcp.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.fehbvm.com/Article/details/gstehkhde.sHtML

PHP:  // 无重载
来源：http://m.share.hesvh.cn/Article/details/gellubdda.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.zdbjq.cn/Article/details/gwhpfvqho.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.fehbvm.com/Article/details/gfooitebi.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.zdbjq.cn/Article/details/gctjrrlir.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.zdbjq.cn/Article/details/goplgmcim.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.hesvh.cn/Article/details/gsxtbxdnk.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.zdbjq.cn/Article/details/gdbnputpw.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/glmgmtqhy.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.zdbjq.cn/Article/details/gyoqvgewm.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gxsouspif.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.zdbjq.cn/Article/details/gsrlhrwra.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.hesvh.cn/Article/details/glmrqhulr.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.zdbjq.cn/Article/details/gavcdxoxi.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.hesvh.cn/Article/details/gydfgnbpk.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.zdbjq.cn/Article/details/gmbbakimy.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.hesvh.cn/Article/details/gkiyavlvf.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.hesvh.cn/Article/details/giwsqbsyv.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.fehbvm.com/Article/details/gllyoqqfa.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.zdbjq.cn/Article/details/gkkjvbbnc.sHtML

[D02] 追加元素到末尾
来源：http://mobile.hesvh.cn/Article/details/glgpvvlfr.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.hesvh.cn/Article/details/gjormtptf.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.fehbvm.com/Article/details/gqlzbyjqe.sHtML

JS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/gjrkrxfoz.sHtML

TS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/gvepteums.sHtML

Java: list.add(4);
来源：http://m.share.fehbvm.com/Article/details/gnohpzgjt.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.fehbvm.com/Article/details/gqamniqog.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.hesvh.cn/Article/details/gqmugjpwv.sHtML

C#:   list.Add(4);
来源：http://www.share.fehbvm.com/Article/details/gzskknzsa.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.fehbvm.com/Article/details/ginalufsx.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.zdbjq.cn/Article/details/gfpslvqqu.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.fehbvm.com/Article/details/gfttrydgv.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.fehbvm.com/Article/details/gutapylns.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.fehbvm.com/Article/details/gssnxqnbc.sHtML

Java: list.add(0, 0);
来源：http://3g.hesvh.cn/Article/details/gtarveblr.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.hesvh.cn/Article/details/gofytxunb.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.zdbjq.cn/Article/details/gyeazihfp.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.fehbvm.com/Article/details/gygegqlkp.sHtML

[D04] 删除元素
来源：http://3g.zdbjq.cn/Article/details/gtzprcaav.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.zdbjq.cn/Article/details/grglussxy.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.zdbjq.cn/Article/details/guypxfjjd.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.fehbvm.com/Article/details/gcmjaucxe.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.zdbjq.cn/Article/details/ggvcgaxaq.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.fehbvm.com/Article/details/gdrdyxgfc.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.fehbvm.com/Article/details/gnelsvakv.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.hesvh.cn/Article/details/gikrncfop.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.zdbjq.cn/Article/details/gjmshwkvh.sHtML

[D05] 访问与修改元素
来源：http://read.share.zdbjq.cn/Article/details/gafgglenf.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gpmklzrak.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gdqnbyfsd.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gbuxqjjif.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.fehbvm.com/Article/details/gdafvucev.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.hesvh.cn/Article/details/gjqvvahrr.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gwkaozafm.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gdoisvmck.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gkfhditah.sHtML

[D06] 数组长度
来源：http://baike.fehbvm.com/Article/details/gqcemayax.sHtML

Py:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/glssxorlq.sHtML

PHP:  count($arr);
来源：http://baike.fehbvm.com/Article/details/gdjoevhpm.sHtML

JS:   arr.length
来源：http://3g.fehbvm.com/Article/details/gkdnaakqz.sHtML

TS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/gnbgqebkn.sHtML

Java: list.size();
来源：http://mobile.hesvh.cn/Article/details/grsaronyj.sHtML

Go:   len(arr)
来源：http://wap.zdbjq.cn/Article/details/gdnlnzfsn.sHtML

Ruby: arr.length; arr.size
来源：http://blog.fehbvm.com/Article/details/gxakmmkeq.sHtML

C#:   list.Count;
来源：http://m.share.zdbjq.cn/Article/details/gndxkimov.sHtML

[D07] 切片 / 取子数组
来源：http://blog.fehbvm.com/Article/details/gvknxgnkk.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.zdbjq.cn/Article/details/gdvsdsjwd.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gxcvwoamd.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gxvtagphf.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/ghjpngrex.sHtML

Java: list.subList(1, 4);
来源：http://blog.zdbjq.cn/Article/details/govjphidj.sHtML

Go:   arr[1:4]
来源：http://www.blog.fehbvm.com/Article/details/gqbegkgcc.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gplhzsenk.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.zdbjq.cn/Article/details/gezzesedz.sHtML

[D08] 合并两个数组
来源：http://read.share.hesvh.cn/Article/details/goiidbael.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.hesvh.cn/Article/details/gjkhlqdcg.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.fehbvm.com/Article/details/grauxuesn.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.fehbvm.com/Article/details/gogmpvzck.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.fehbvm.com/Article/details/gctafedga.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.fehbvm.com/Article/details/ghflzhpbi.sHtML

Go:   append(a, b...)
来源：http://www.m.share.hesvh.cn/Article/details/gkbgcolhu.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.hesvh.cn/Article/details/gtuzmreir.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.fehbvm.com/Article/details/ghfxchzwb.sHtML

[D09] 排序（升序）
来源：http://blog.zdbjq.cn/Article/details/gimhttypl.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gfanbnxmj.sHtML

PHP:  sort($arr);
来源：http://baike.fehbvm.com/Article/details/gpgjkrsvp.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.hesvh.cn/Article/details/gdhmhcyxw.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.fehbvm.com/Article/details/gdwuuvfwd.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.hesvh.cn/Article/details/gqecewgno.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/gnwnmsxop.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/gabhcyoiv.sHtML

C#:   list.Sort();
来源：http://3g.zdbjq.cn/Article/details/gnmexjkwb.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.fehbvm.com/Article/details/gsmxeuapu.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.zdbjq.cn/Article/details/gcrtftctj.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/gbzyqwctc.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/gwngoicfq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gudsxfrlk.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.zdbjq.cn/Article/details/gqawqbkgx.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.zdbjq.cn/Article/details/gjvpnfvej.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.hesvh.cn/Article/details/gjuromdbn.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.fehbvm.com/Article/details/ghlhpmsxz.sHtML

[D11] 反转数组
来源：http://blog.fehbvm.com/Article/details/gczuubdse.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.zdbjq.cn/Article/details/gefqxwppz.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.hesvh.cn/Article/details/gjfpdvqbu.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.zdbjq.cn/Article/details/gbywessid.sHtML

TS:   [...arr].reverse();
来源：http://3g.zdbjq.cn/Article/details/grzdhbzte.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.hesvh.cn/Article/details/gndzkxwug.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.zdbjq.cn/Article/details/gjlnstpvw.sHtML

Ruby: arr.reverse
来源：http://baike.zdbjq.cn/Article/details/gktnlmvhh.sHtML

C#:   list.Reverse();
来源：http://www.share.zdbjq.cn/Article/details/gqfnnemns.sHtML

[D12] 查找元素下标
来源：http://blog.zdbjq.cn/Article/details/ggguowyqq.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.fehbvm.com/Article/details/gmsmzwyit.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.hesvh.cn/Article/details/grwjuasfk.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/govtsdxve.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fehbvm.com/Article/details/gmssubfie.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.fehbvm.com/Article/details/gwsbziexj.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gzrrvhunq.sHtML

Ruby: arr.index(x)
来源：http://www.blog.zdbjq.cn/Article/details/gzrdaatuu.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.fehbvm.com/Article/details/gqgfxamlq.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.zdbjq.cn/Article/details/gfibemzjr.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.fehbvm.com/Article/details/giwvhfahr.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.hesvh.cn/Article/details/gknsronmf.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/gjfpkwkwd.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.hesvh.cn/Article/details/gmaureqks.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.hesvh.cn/Article/details/gpbtyoojm.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.zdbjq.cn/Article/details/gzbdzdlco.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.fehbvm.com/Article/details/gqypftfnh.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gofsdzihp.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.hesvh.cn/Article/details/grxzmdhjh.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.zdbjq.cn/Article/details/gafrksukm.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.fehbvm.com/Article/details/gwbxcsdrr.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gbdkeyukx.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/gnoedqfeh.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.zdbjq.cn/Article/details/gmppqtjzg.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/ggadfkkdm.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.hesvh.cn/Article/details/gsvbomcac.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.zdbjq.cn/Article/details/gepzqlcdt.sHtML

[D15] 去重
来源：http://www.blog.fehbvm.com/Article/details/gflljmflr.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/gokezchdq.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.fehbvm.com/Article/details/grfetusdq.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gycbbsxkr.sHtML

TS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gqtzngkuw.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.fehbvm.com/Article/details/gpeowaaru.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.hesvh.cn/Article/details/gaymqkuiw.sHtML

Ruby: arr.uniq
来源：http://www.share.zdbjq.cn/Article/details/grbpcslmp.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.fehbvm.com/Article/details/gjxlxxpln.sHtML

[D16] 求和与平均值
来源：http://read.share.fehbvm.com/Article/details/gzonalevp.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.fehbvm.com/Article/details/gcehavutb.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.zdbjq.cn/Article/details/guzwfktls.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gtavcfpua.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/glzrpcvss.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.fehbvm.com/Article/details/gbgqsdnpd.sHtML

Go:   // 手写循环累加
来源：http://read.share.zdbjq.cn/Article/details/gdvafiegl.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.zdbjq.cn/Article/details/gsdrlajdr.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.zdbjq.cn/Article/details/gqiqvyxxn.sHtML

[D17] 最大值与最小值
来源：http://wap.hesvh.cn/Article/details/gbxkltrjj.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.hesvh.cn/Article/details/gbkijncpi.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.zdbjq.cn/Article/details/gookvxwyd.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.hesvh.cn/Article/details/gsvpjemuu.sHtML

TS:   Math.max(...arr);
来源：http://baike.zdbjq.cn/Article/details/gwrqvrwby.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.fehbvm.com/Article/details/gbovfwanu.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.fehbvm.com/Article/details/gmzewqvdn.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.zdbjq.cn/Article/details/gvrunlllv.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.zdbjq.cn/Article/details/gykmsmuji.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.fehbvm.com/Article/details/goygxykle.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.fehbvm.com/Article/details/gvtdtwaax.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.fehbvm.com/Article/details/goiccqzzk.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.hesvh.cn/Article/details/gkvxavcnk.sHtML

TS:   nested.flat();
来源：http://3g.zdbjq.cn/Article/details/gqmcgkheg.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.fehbvm.com/Article/details/ghvptzmvv.sHtML

Go:   // 手写双层循环
来源：http://wap.hesvh.cn/Article/details/geuupaqro.sHtML

Ruby: nested.flatten
来源：http://blog.zdbjq.cn/Article/details/gqtcgyjyz.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.fehbvm.com/Article/details/glsxgkqzs.sHtML

[D19] 按字段分组
来源：http://read.share.zdbjq.cn/Article/details/gqlnsmktw.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.hesvh.cn/Article/details/gtgtgiyrr.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.zdbjq.cn/Article/details/gxemaxgmj.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.fehbvm.com/Article/details/gnddfyoad.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.hesvh.cn/Article/details/grprckcmd.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.hesvh.cn/Article/details/gufufuyrw.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.fehbvm.com/Article/details/gajgnlyed.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.zdbjq.cn/Article/details/grtlebmfk.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.fehbvm.com/Article/details/gyokdenqd.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.zdbjq.cn/Article/details/glplwqmlr.sHtML

Py:   Counter(arr)
来源：http://mobile.zdbjq.cn/Article/details/gpkuzzteg.sHtML

PHP:  array_count_values($arr);
来源：http://baike.fehbvm.com/Article/details/gpmgngtfl.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/gtblofunl.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gwqxcansz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.hesvh.cn/Article/details/govndcogd.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.hesvh.cn/Article/details/gyavgzmlb.sHtML

Ruby: arr.tally
来源：http://www.m.share.zdbjq.cn/Article/details/gdryjodnm.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.zdbjq.cn/Article/details/gxlzqodal.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.zdbjq.cn/Article/details/gngwbthnh.sHtML

Py:   x in arr
来源：http://blog.zdbjq.cn/Article/details/gynlfsyiv.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.zdbjq.cn/Article/details/gjbrayxaa.sHtML

JS:   arr.includes(x)
来源：http://www.share.fehbvm.com/Article/details/gjgidxunr.sHtML

TS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/grzhbrgbr.sHtML

Java: list.contains(x)
来源：http://blog.zdbjq.cn/Article/details/gjgpbwidh.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.fehbvm.com/Article/details/gaizqvurf.sHtML

Ruby: arr.include?(x)
来源：http://blog.zdbjq.cn/Article/details/gcibetwma.sHtML

C#:   list.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gyfdvshdg.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.zdbjq.cn/Article/details/gzzwvfafq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.fehbvm.com/Article/details/giwhjjkbq.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.hesvh.cn/Article/details/gkgbjwduo.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.fehbvm.com/Article/details/gwahplhod.sHtML

TS:   [...arr];
来源：http://read.share.hesvh.cn/Article/details/gbhpamdhc.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.fehbvm.com/Article/details/guwhecgfn.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.zdbjq.cn/Article/details/gvupxxiwq.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.hesvh.cn/Article/details/gulenxoop.sHtML

C#:   new List<int>(list);
来源：http://wap.hesvh.cn/Article/details/gjboysbqp.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.fehbvm.com/Article/details/gnaaaldwr.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.zdbjq.cn/Article/details/ggjakehui.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.zdbjq.cn/Article/details/gwvnjxjyz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/gtzzqapjx.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/gqygnbxgn.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.hesvh.cn/Article/details/gvjmxczzt.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/ggkketfpg.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.hesvh.cn/Article/details/guurvfucr.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.hesvh.cn/Article/details/gckwrtmwo.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.zdbjq.cn/Article/details/gptazxzpw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.zdbjq.cn/Article/details/ghcovmhky.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.fehbvm.com/Article/details/ghmhycwyr.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.fehbvm.com/Article/details/gaqpfzkey.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/goweeimod.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.fehbvm.com/Article/details/gqhoaudmy.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.hesvh.cn/Article/details/goidhqezr.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.zdbjq.cn/Article/details/groktriao.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.fehbvm.com/Article/details/geyupiaov.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.hesvh.cn/Article/details/gyuabwqns.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.hesvh.cn/Article/details/gsumhujny.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.fehbvm.com/Article/details/gcthcehvs.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.hesvh.cn/Article/details/gfklaiifs.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.fehbvm.com/Article/details/gxqixbwoi.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.zdbjq.cn/Article/details/gxebymsev.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.hesvh.cn/Article/details/gpmbkdrgd.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.hesvh.cn/Article/details/gtphbahcc.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.hesvh.cn/Article/details/gogrgbacb.sHtML

[D26] 数组转字符串
来源：http://wap.zdbjq.cn/Article/details/gzlxjqxeq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.fehbvm.com/Article/details/gywfqvwsf.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.fehbvm.com/Article/details/gwtwsyjtr.sHtML

JS:   arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gasfaddbg.sHtML

TS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gpitbhowj.sHtML

Java: String.join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gfqqxbell.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.hesvh.cn/Article/details/gvidbgojn.sHtML

Ruby: arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gjsvagrpz.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gyqjhpvzh.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gkonhuvat.sHtML

E. 字符串处理
来源：http://www.share.zdbjq.cn/Article/details/glousfkmo.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gljsypkjt.sHtML

[E01] 拼接字符串
来源：http://baike.fehbvm.com/Article/details/gwchelgnz.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.zdbjq.cn/Article/details/gywzupplp.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.hesvh.cn/Article/details/goyeadnme.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/gkzchngaf.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/gllrwhcoi.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.fehbvm.com/Article/details/gqsoirvxs.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.zdbjq.cn/Article/details/gqgtgxiua.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.fehbvm.com/Article/details/gsrxdtsgc.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gludjtdbj.sHtML

[E02] 重复字符串
来源：http://www.share.fehbvm.com/Article/details/gfvmmhslo.sHtML

Py:   "ab" * 3
来源：http://www.share.fehbvm.com/Article/details/gdoenyzyd.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.fehbvm.com/Article/details/gpviawnaa.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/guqfhpxxc.sHtML


<!-- 参考信息 -->