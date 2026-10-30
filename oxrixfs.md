代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://baike.zdbjq.cn/Article/details/gurxguswp.sHtML

C#:   using System.Text;
来源：http://read.share.hesvh.cn/Article/details/gchzgrtgf.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.zdbjq.cn/Article/details/gerbgemze.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.fehbvm.com/Article/details/gqugmhegr.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.fehbvm.com/Article/details/gwlarvobu.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.fehbvm.com/Article/details/ghpnyoipl.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.zdbjq.cn/Article/details/gqjynctvb.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.fehbvm.com/Article/details/ggfxvhxmw.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.zdbjq.cn/Article/details/gnhzlauao.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.zdbjq.cn/Article/details/gmitmmbon.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gdqjvwqwu.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.fehbvm.com/Article/details/gcjfoshnx.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.fehbvm.com/Article/details/geejnafds.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gxsmxsuwf.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.fehbvm.com/Article/details/gcyuykmpa.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gdxrgkugv.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gemcrjfgs.sHtML

Go:   func add(a, b int) int
来源：http://www.share.hesvh.cn/Article/details/gdqiigmbg.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.hesvh.cn/Article/details/gcekdxloe.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.hesvh.cn/Article/details/gbllpxjag.sHtML

[C14] 泛型函数
来源：http://www.share.fehbvm.com/Article/details/gdtpysuud.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.zdbjq.cn/Article/details/gaklvkwkj.sHtML

PHP:  // 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gorfnspxi.sHtML

JS:   // 无泛型
来源：http://blog.zdbjq.cn/Article/details/gwezlbssj.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjcemlgyq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.hesvh.cn/Article/details/girkwtvyr.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.hesvh.cn/Article/details/gdqcuidij.sHtML

Ruby: # 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gxywemiby.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.fehbvm.com/Article/details/gvkznkadc.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.zdbjq.cn/Article/details/gjbsrbfyq.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.fehbvm.com/Article/details/gmnfoqbmi.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.zdbjq.cn/Article/details/gdmuazwal.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.zdbjq.cn/Article/details/gzxpxrkov.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.zdbjq.cn/Article/details/gecitekwe.sHtML

Java: // 无解构
来源：http://www.share.fehbvm.com/Article/details/giwszsapu.sHtML

Go:   // 无解构
来源：http://www.share.fehbvm.com/Article/details/gwnxllpus.sHtML

Ruby: a, b = pair
来源：http://www.blog.hesvh.cn/Article/details/gjbgriqwl.sHtML

C#:   var (a, b) = pair;
来源：http://3g.fehbvm.com/Article/details/grfefqoxi.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.zdbjq.cn/Article/details/gmxsykscs.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.fehbvm.com/Article/details/gsumcdmfv.sHtML

PHP:  // 无重载
来源：http://www.m.share.zdbjq.cn/Article/details/gsodwsxil.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.zdbjq.cn/Article/details/gvdriudgo.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.hesvh.cn/Article/details/gnxxjvqql.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.fehbvm.com/Article/details/gpufkdqed.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.fehbvm.com/Article/details/gfcpcsuuc.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.hesvh.cn/Article/details/gucoeuqlr.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.fehbvm.com/Article/details/gbourogrj.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/grsawgubu.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.hesvh.cn/Article/details/gccklazzn.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gjhnjbrkw.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.fehbvm.com/Article/details/gbckqsaxk.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.hesvh.cn/Article/details/gdzxfbfjk.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.zdbjq.cn/Article/details/gzqmhuwfx.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.zdbjq.cn/Article/details/gbxgkjdye.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.zdbjq.cn/Article/details/gchknyram.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.fehbvm.com/Article/details/gajsthqem.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.zdbjq.cn/Article/details/gutahzyqt.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.zdbjq.cn/Article/details/gymgwwsvh.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.hesvh.cn/Article/details/gvabxbuue.sHtML

[D02] 追加元素到末尾
来源：http://blog.fehbvm.com/Article/details/gyzrxofoi.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.zdbjq.cn/Article/details/gwllszpzi.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.zdbjq.cn/Article/details/gwycwhtlx.sHtML

JS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/gzvbfbkta.sHtML

TS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/gpnulzcda.sHtML

Java: list.add(4);
来源：http://www.share.fehbvm.com/Article/details/gigrgckum.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.zdbjq.cn/Article/details/gmfguljfn.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.zdbjq.cn/Article/details/guuwicsie.sHtML

C#:   list.Add(4);
来源：http://mobile.fehbvm.com/Article/details/gpbmayloe.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.fehbvm.com/Article/details/guueaejkm.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gkcxshkdy.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.zdbjq.cn/Article/details/goubjwhuo.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.zdbjq.cn/Article/details/gcdvvskou.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gvimeqgzi.sHtML

Java: list.add(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gbgnbfqjd.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.fehbvm.com/Article/details/gdimmozsm.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.fehbvm.com/Article/details/gvkqskdkf.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gkwonuugc.sHtML

[D04] 删除元素
来源：http://www.share.hesvh.cn/Article/details/gobgqujne.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.zdbjq.cn/Article/details/ggmrccwib.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.hesvh.cn/Article/details/giukfxxmb.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.fehbvm.com/Article/details/guttszyit.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.fehbvm.com/Article/details/gsrlcixtp.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.hesvh.cn/Article/details/gajbgsxvb.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.zdbjq.cn/Article/details/gqikwxiiq.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.zdbjq.cn/Article/details/gatyahzps.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.fehbvm.com/Article/details/gejidqehd.sHtML

[D05] 访问与修改元素
来源：http://mobile.fehbvm.com/Article/details/gqallaavz.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gylkzunrw.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gjsiapors.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gbdosaymb.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.zdbjq.cn/Article/details/ghufwftad.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.hesvh.cn/Article/details/gmnhlvmlz.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gpbtvthgd.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gdykcgzkx.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gozhbudof.sHtML

[D06] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gyijnzstq.sHtML

Py:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/gleysxbzv.sHtML

PHP:  count($arr);
来源：http://read.share.fehbvm.com/Article/details/glgzvkwpp.sHtML

JS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/gkouqfeti.sHtML

TS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/guoigtxno.sHtML

Java: list.size();
来源：http://3g.zdbjq.cn/Article/details/grntpxkok.sHtML

Go:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gidfklqtd.sHtML

Ruby: arr.length; arr.size
来源：http://blog.fehbvm.com/Article/details/gkjddonbo.sHtML

C#:   list.Count;
来源：http://www.share.hesvh.cn/Article/details/gylutagdq.sHtML

[D07] 切片 / 取子数组
来源：http://3g.fehbvm.com/Article/details/gfazjqzpw.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.fehbvm.com/Article/details/gvjqhmqar.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.fehbvm.com/Article/details/grbaquchh.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gacosrdgx.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/ghaytayvv.sHtML

Java: list.subList(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gwnzewiui.sHtML

Go:   arr[1:4]
来源：http://baike.zdbjq.cn/Article/details/gcmbomqin.sHtML

Ruby: arr[1, 3]
来源：http://3g.zdbjq.cn/Article/details/grbdujvjk.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.zdbjq.cn/Article/details/grhaeprdh.sHtML

[D08] 合并两个数组
来源：http://www.share.hesvh.cn/Article/details/gzyqcuyjo.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.zdbjq.cn/Article/details/gwkikyglt.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.hesvh.cn/Article/details/ghorvfffa.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.hesvh.cn/Article/details/grnodrero.sHtML

TS:   [...a, ...b];
来源：http://mobile.fehbvm.com/Article/details/gmgryuxtu.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.fehbvm.com/Article/details/gtwzfzvzl.sHtML

Go:   append(a, b...)
来源：http://3g.hesvh.cn/Article/details/ghjjeegyk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.fehbvm.com/Article/details/gfrynxfan.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.hesvh.cn/Article/details/gpykelikj.sHtML

[D09] 排序（升序）
来源：http://www.m.share.fehbvm.com/Article/details/gmzixacqa.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/gknuxiegt.sHtML

PHP:  sort($arr);
来源：http://www.blog.hesvh.cn/Article/details/gppunvilo.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.fehbvm.com/Article/details/gmqshqzhx.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.hesvh.cn/Article/details/gtukzqrbu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.fehbvm.com/Article/details/gznrypqly.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/gmcktvgxc.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/ggfvctent.sHtML

C#:   list.Sort();
来源：http://3g.hesvh.cn/Article/details/gxjtglnnd.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.hesvh.cn/Article/details/gtwfyxsoj.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.zdbjq.cn/Article/details/ghdtgvmkm.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/gqyuzvzky.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/gvzdwocek.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/gqptulatq.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.hesvh.cn/Article/details/gagcjijfn.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.zdbjq.cn/Article/details/gvozpjeyi.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.zdbjq.cn/Article/details/gnqsijbma.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.zdbjq.cn/Article/details/gmsihszys.sHtML

[D11] 反转数组
来源：http://read.share.zdbjq.cn/Article/details/gcoorukvp.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.fehbvm.com/Article/details/gevfnplss.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.fehbvm.com/Article/details/gjkshjerv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.hesvh.cn/Article/details/gyabkodom.sHtML

TS:   [...arr].reverse();
来源：http://read.share.zdbjq.cn/Article/details/gtxututjl.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gddqfvbnf.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.fehbvm.com/Article/details/gtxbkygkm.sHtML

Ruby: arr.reverse
来源：http://m.share.zdbjq.cn/Article/details/gyegagxgb.sHtML

C#:   list.Reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/gcndqkczp.sHtML

[D12] 查找元素下标
来源：http://3g.zdbjq.cn/Article/details/gqywmmkql.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.hesvh.cn/Article/details/ggqvwcckr.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.fehbvm.com/Article/details/gvkacvtes.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/gsomzntuf.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/gpmoketcv.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.zdbjq.cn/Article/details/gbedstyrs.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.fehbvm.com/Article/details/gtdlnqwtw.sHtML

Ruby: arr.index(x)
来源：http://blog.fehbvm.com/Article/details/gdamjvyuv.sHtML

C#:   list.IndexOf(x);
来源：http://baike.fehbvm.com/Article/details/gzliboiuw.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.zdbjq.cn/Article/details/ghelozpjv.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gqdzavypz.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.fehbvm.com/Article/details/gfyhxwnjm.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/gamnzweyk.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gqeiywvjy.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.fehbvm.com/Article/details/gwfntjsif.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.zdbjq.cn/Article/details/gwxftfjfl.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.zdbjq.cn/Article/details/gbrmmppyu.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/ghraslbnf.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.hesvh.cn/Article/details/gwygojqku.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.hesvh.cn/Article/details/gjkkhxehb.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.zdbjq.cn/Article/details/gdnyhauzy.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/gszbddcdd.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.hesvh.cn/Article/details/gnacexzlw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.zdbjq.cn/Article/details/gpqgorqgp.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/gbbjpxgsg.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gsblsudms.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.fehbvm.com/Article/details/gkycnppey.sHtML

[D15] 去重
来源：http://m.share.zdbjq.cn/Article/details/gqzkcllif.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.hesvh.cn/Article/details/gfyrdxgkv.sHtML

PHP:  array_unique($arr);
来源：http://baike.fehbvm.com/Article/details/gddovoahn.sHtML

JS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gndvmhvlp.sHtML

TS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/ghnbkilvi.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.zdbjq.cn/Article/details/gkkiylwsl.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.hesvh.cn/Article/details/gvyqyywri.sHtML

Ruby: arr.uniq
来源：http://www.blog.hesvh.cn/Article/details/guyulyagd.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.fehbvm.com/Article/details/gkuxtapgg.sHtML

[D16] 求和与平均值
来源：http://www.blog.zdbjq.cn/Article/details/gjahwyidy.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.hesvh.cn/Article/details/gxcobejcq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.fehbvm.com/Article/details/gfcjiilhb.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/gudpyaumr.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/gniwjzrcx.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.hesvh.cn/Article/details/gheckpsou.sHtML

Go:   // 手写循环累加
来源：http://mobile.hesvh.cn/Article/details/ggrkxbefj.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.fehbvm.com/Article/details/gnrtcqawy.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.hesvh.cn/Article/details/gsounsffy.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.fehbvm.com/Article/details/gcmxzkvbr.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.fehbvm.com/Article/details/gwgwyvlvv.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.fehbvm.com/Article/details/gwjiguilg.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.zdbjq.cn/Article/details/gtgkesibc.sHtML

TS:   Math.max(...arr);
来源：http://m.share.zdbjq.cn/Article/details/gbgckzsys.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.zdbjq.cn/Article/details/ggeekumkj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.hesvh.cn/Article/details/glthyzbmc.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.zdbjq.cn/Article/details/gctvwnrbb.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.hesvh.cn/Article/details/gmsqgrhwr.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.fehbvm.com/Article/details/gucyugaht.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.fehbvm.com/Article/details/gojjcgedf.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.fehbvm.com/Article/details/gtphzcwam.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.hesvh.cn/Article/details/gzlyerdvu.sHtML

TS:   nested.flat();
来源：http://www.blog.hesvh.cn/Article/details/gkyikfqwz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.fehbvm.com/Article/details/grerlvobq.sHtML

Go:   // 手写双层循环
来源：http://baike.fehbvm.com/Article/details/gjvgyomwt.sHtML

Ruby: nested.flatten
来源：http://m.share.zdbjq.cn/Article/details/guvhcugbd.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.fehbvm.com/Article/details/gjbvegqcx.sHtML

[D19] 按字段分组
来源：http://www.blog.zdbjq.cn/Article/details/gduverogv.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.hesvh.cn/Article/details/gwenaqxyj.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.fehbvm.com/Article/details/gbpvupbbd.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.hesvh.cn/Article/details/gqakkyjce.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gnamjvqil.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.zdbjq.cn/Article/details/grbhvjtms.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.hesvh.cn/Article/details/gyzdwarna.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.zdbjq.cn/Article/details/ghvnobvfj.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.zdbjq.cn/Article/details/gzitfxfks.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.fehbvm.com/Article/details/gaefgmefk.sHtML

Py:   Counter(arr)
来源：http://blog.zdbjq.cn/Article/details/gtiemykcq.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.fehbvm.com/Article/details/gebwhxomm.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/gothobrtl.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/ggbeetkor.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.zdbjq.cn/Article/details/gtkfblifd.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.fehbvm.com/Article/details/gdvtukdww.sHtML

Ruby: arr.tally
来源：http://m.share.zdbjq.cn/Article/details/gkgvoalxd.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.fehbvm.com/Article/details/grketqpra.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.zdbjq.cn/Article/details/ghlnqzjur.sHtML

Py:   x in arr
来源：http://m.share.zdbjq.cn/Article/details/gnbmzatqi.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.hesvh.cn/Article/details/gjkytvjyz.sHtML

JS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gvpmazrva.sHtML

TS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/gumvcldmf.sHtML

Java: list.contains(x)
来源：http://baike.zdbjq.cn/Article/details/gbqqvjngr.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gogcsmfdw.sHtML

Ruby: arr.include?(x)
来源：http://3g.fehbvm.com/Article/details/gvbykuhpv.sHtML

C#:   list.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gxssopqse.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.hesvh.cn/Article/details/gffdncmmt.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.zdbjq.cn/Article/details/gmdfdctcx.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.hesvh.cn/Article/details/gabqqixch.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.zdbjq.cn/Article/details/gdpcncndc.sHtML

TS:   [...arr];
来源：http://www.m.share.zdbjq.cn/Article/details/grtdumxhf.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.hesvh.cn/Article/details/grahrlxiy.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.zdbjq.cn/Article/details/gygawhqur.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.zdbjq.cn/Article/details/gpnefshoe.sHtML

C#:   new List<int>(list);
来源：http://www.blog.fehbvm.com/Article/details/grxnifdzg.sHtML

[D23] reduce 累积计算
来源：http://www.share.fehbvm.com/Article/details/goaxdcxtv.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.fehbvm.com/Article/details/gkqfmmyhv.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.hesvh.cn/Article/details/gwuyqvbhn.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/gjzinexzw.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/gvlfmvyhy.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.hesvh.cn/Article/details/gtrfcvipg.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/gpydrjkie.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.zdbjq.cn/Article/details/gathjgalo.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.hesvh.cn/Article/details/glvelnfwn.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.hesvh.cn/Article/details/grcclfupj.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.hesvh.cn/Article/details/ggjphcrpo.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.hesvh.cn/Article/details/ghxyctfsh.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.hesvh.cn/Article/details/gatiyzlvj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gcoyctzfs.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.fehbvm.com/Article/details/gvjbahyof.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.hesvh.cn/Article/details/gczcaymto.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.fehbvm.com/Article/details/gaqpoveqe.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.hesvh.cn/Article/details/gfilloseb.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.fehbvm.com/Article/details/gbaxfdule.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.hesvh.cn/Article/details/gqmwkeyrz.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.hesvh.cn/Article/details/gpevjficq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.fehbvm.com/Article/details/glhuwqwfj.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.hesvh.cn/Article/details/grwypysfe.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.zdbjq.cn/Article/details/gkmthuiea.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.hesvh.cn/Article/details/gcfqsdtuq.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.hesvh.cn/Article/details/gzjkulpmd.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.fehbvm.com/Article/details/gexkghxtt.sHtML

[D26] 数组转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gqlznzeuy.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.fehbvm.com/Article/details/gxgwvidoh.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.fehbvm.com/Article/details/geqcganrv.sHtML

JS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gjagxsyom.sHtML

TS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gmnolsdun.sHtML

Java: String.join(", ", list)
来源：http://wap.fehbvm.com/Article/details/gnrjjlyrc.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.hesvh.cn/Article/details/gqbenqbyg.sHtML

Ruby: arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gfpjyuaom.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/gamscbdar.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gsofndxyw.sHtML

E. 字符串处理
来源：http://3g.fehbvm.com/Article/details/gduzavwuo.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gkumukpbl.sHtML

[E01] 拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gnboyubfy.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.fehbvm.com/Article/details/gvajsaosn.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.hesvh.cn/Article/details/gbmfliaso.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/gfkswxgoe.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/ghjjhyxvq.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.hesvh.cn/Article/details/gxhrajnhh.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.fehbvm.com/Article/details/ghrcdgvgv.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.hesvh.cn/Article/details/gychezbio.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gvudkghem.sHtML

[E02] 重复字符串
来源：http://baike.fehbvm.com/Article/details/gensmjnbq.sHtML

Py:   "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gbromzwxz.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.hesvh.cn/Article/details/glpvdnnjz.sHtML

JS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gvwwykyui.sHtML


<!-- 参考信息 -->