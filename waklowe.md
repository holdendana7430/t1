代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://blog.hesvh.cn/Article/details/ggitftwzs.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.fehbvm.com/Article/details/gjzvixsct.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.hesvh.cn/Article/details/gsfovzjfy.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.zdbjq.cn/Article/details/gglmmukvk.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.zdbjq.cn/Article/details/ggldgtolc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gozvcborq.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.zdbjq.cn/Article/details/gyeswtgkr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gzdkesnjb.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gzknoimkw.sHtML

Go:   func add(a, b int) int
来源：http://read.share.zdbjq.cn/Article/details/gvzdjqvvf.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.fehbvm.com/Article/details/gcgkxrjjf.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.zdbjq.cn/Article/details/gkhirwjbh.sHtML

[C14] 泛型函数
来源：http://www.blog.fehbvm.com/Article/details/glwlrvkqe.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.zdbjq.cn/Article/details/gzynaoilo.sHtML

PHP:  // 无泛型
来源：http://www.share.fehbvm.com/Article/details/glrjukdlm.sHtML

JS:   // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gfikvgyjj.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.zdbjq.cn/Article/details/gtvsxroun.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.zdbjq.cn/Article/details/gtojsrbrm.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.fehbvm.com/Article/details/ggqxlrrsi.sHtML

Ruby: # 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gazgrueqk.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.zdbjq.cn/Article/details/gpditlabt.sHtML

[C15] 解构 / 展开参数
来源：http://blog.zdbjq.cn/Article/details/ggtvqalxk.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.zdbjq.cn/Article/details/gfumqlogn.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.zdbjq.cn/Article/details/gmjjwrihg.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.zdbjq.cn/Article/details/gjsvkbmzb.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.zdbjq.cn/Article/details/gqolotuiv.sHtML

Java: // 无解构
来源：http://mobile.zdbjq.cn/Article/details/gtwosmjfr.sHtML

Go:   // 无解构
来源：http://baike.zdbjq.cn/Article/details/gozdssjpj.sHtML

Ruby: a, b = pair
来源：http://read.share.zdbjq.cn/Article/details/gwuykmfpy.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.fehbvm.com/Article/details/gtjgmxsos.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.fehbvm.com/Article/details/gjhynezxg.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.fehbvm.com/Article/details/gnbzixfle.sHtML

PHP:  // 无重载
来源：http://blog.zdbjq.cn/Article/details/gfqwnbave.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.zdbjq.cn/Article/details/ghhwxunbe.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.zdbjq.cn/Article/details/gvocftcyw.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.hesvh.cn/Article/details/gsxzgdesf.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.hesvh.cn/Article/details/goxpqewmo.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.fehbvm.com/Article/details/gsufloake.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.fehbvm.com/Article/details/gzkqzrwtf.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gdpmrgovd.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.zdbjq.cn/Article/details/gbwwoinvx.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gphjieumu.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.fehbvm.com/Article/details/gglthupbi.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.fehbvm.com/Article/details/gzyafrkww.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.hesvh.cn/Article/details/glltarzqm.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.zdbjq.cn/Article/details/ggijaqdyw.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.hesvh.cn/Article/details/gmyfczqsk.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.zdbjq.cn/Article/details/gnkkmrned.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.zdbjq.cn/Article/details/ghczhtmda.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.hesvh.cn/Article/details/gpedeaopw.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.fehbvm.com/Article/details/gwrgevkua.sHtML

[D02] 追加元素到末尾
来源：http://wap.fehbvm.com/Article/details/gqflhhvgo.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.zdbjq.cn/Article/details/gsrajpvue.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.fehbvm.com/Article/details/gmtzkxrta.sHtML

JS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/gixxfywva.sHtML

TS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/gidurdsth.sHtML

Java: list.add(4);
来源：http://m.share.fehbvm.com/Article/details/gorrrhtko.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.fehbvm.com/Article/details/gizfnvpvt.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.zdbjq.cn/Article/details/gsiyuknem.sHtML

C#:   list.Add(4);
来源：http://baike.fehbvm.com/Article/details/gbpgrtdmp.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.hesvh.cn/Article/details/gwznzuxnl.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.fehbvm.com/Article/details/grbcnkfae.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.zdbjq.cn/Article/details/ghjdbbbqq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.zdbjq.cn/Article/details/gqireshod.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.hesvh.cn/Article/details/gxkcpzvje.sHtML

Java: list.add(0, 0);
来源：http://mobile.fehbvm.com/Article/details/gzelssrjx.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.hesvh.cn/Article/details/gnyxmzzgl.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.hesvh.cn/Article/details/gwwwdvkfw.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gqxebwqnh.sHtML

[D04] 删除元素
来源：http://www.blog.hesvh.cn/Article/details/grozezmiq.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.zdbjq.cn/Article/details/gbvghywnj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.fehbvm.com/Article/details/ghsrfkydd.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.hesvh.cn/Article/details/gfwepyrow.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.fehbvm.com/Article/details/guldhguwo.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.fehbvm.com/Article/details/gnadbgcdy.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.hesvh.cn/Article/details/glezmowvu.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.hesvh.cn/Article/details/gzqfxurlu.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.fehbvm.com/Article/details/gcjkvqoox.sHtML

[D05] 访问与修改元素
来源：http://www.share.fehbvm.com/Article/details/gfqjvlbol.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gkwnjwxzh.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gwhcjadkd.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gnulraasd.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.fehbvm.com/Article/details/gcvggwend.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.hesvh.cn/Article/details/gvwijfbbd.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gbkbkwwtx.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/glnjygbmx.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gzdstmtmc.sHtML

[D06] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/gbjmxpbmz.sHtML

Py:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gjproiobs.sHtML

PHP:  count($arr);
来源：http://wap.fehbvm.com/Article/details/gibzllqdg.sHtML

JS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/gkubrordb.sHtML

TS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/gzkubchvf.sHtML

Java: list.size();
来源：http://baike.zdbjq.cn/Article/details/gifsmhvmg.sHtML

Go:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/gjlbybefb.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.hesvh.cn/Article/details/gimmgbyov.sHtML

C#:   list.Count;
来源：http://www.share.zdbjq.cn/Article/details/glzbheayx.sHtML

[D07] 切片 / 取子数组
来源：http://blog.hesvh.cn/Article/details/gasllqsyd.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.zdbjq.cn/Article/details/gojkpexfj.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.fehbvm.com/Article/details/gkhmkncdn.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gkilkmwml.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gysucsijy.sHtML

Java: list.subList(1, 4);
来源：http://3g.hesvh.cn/Article/details/ghxtjyqzr.sHtML

Go:   arr[1:4]
来源：http://www.m.share.zdbjq.cn/Article/details/gpkuxtbej.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.zdbjq.cn/Article/details/gnflyjofi.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.hesvh.cn/Article/details/grhohxemg.sHtML

[D08] 合并两个数组
来源：http://www.blog.fehbvm.com/Article/details/ghttxlgso.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.zdbjq.cn/Article/details/gaxfnscbd.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.hesvh.cn/Article/details/gwthxqhhu.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.hesvh.cn/Article/details/giqggsaoa.sHtML

TS:   [...a, ...b];
来源：http://blog.hesvh.cn/Article/details/gtqbqwtim.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.hesvh.cn/Article/details/gwjrgdfah.sHtML

Go:   append(a, b...)
来源：http://mobile.hesvh.cn/Article/details/gsryutvxo.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gpdlflckx.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.fehbvm.com/Article/details/gjwkigwvx.sHtML

[D09] 排序（升序）
来源：http://3g.fehbvm.com/Article/details/gtdofgwgt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.hesvh.cn/Article/details/gljcubwzq.sHtML

PHP:  sort($arr);
来源：http://baike.hesvh.cn/Article/details/gptsuxgsj.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.fehbvm.com/Article/details/glwtkyrgv.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.fehbvm.com/Article/details/gcwktzqyp.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.fehbvm.com/Article/details/gvwfenipm.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/gwtbirejy.sHtML

Ruby: arr.sort
来源：http://www.m.share.hesvh.cn/Article/details/gfvwwoiph.sHtML

C#:   list.Sort();
来源：http://read.share.fehbvm.com/Article/details/glmiryzvh.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.zdbjq.cn/Article/details/gditptzqo.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.zdbjq.cn/Article/details/gueitajxp.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/gvzkbmmut.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/gkwplocpu.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gvjitadfu.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.fehbvm.com/Article/details/gvodpsvoj.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.fehbvm.com/Article/details/geqimloja.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.zdbjq.cn/Article/details/gybdsjlaw.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.hesvh.cn/Article/details/gueblllki.sHtML

[D11] 反转数组
来源：http://baike.fehbvm.com/Article/details/gshbpsqqz.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.fehbvm.com/Article/details/gilhhrlye.sHtML

PHP:  array_reverse($arr);
来源：http://baike.hesvh.cn/Article/details/gfvlwxonc.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.fehbvm.com/Article/details/gijrswyws.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.fehbvm.com/Article/details/gfekgytaf.sHtML

Java: Collections.reverse(list);
来源：http://www.share.hesvh.cn/Article/details/gjpapeypp.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.zdbjq.cn/Article/details/gjwxasztg.sHtML

Ruby: arr.reverse
来源：http://baike.fehbvm.com/Article/details/gfutyxzqs.sHtML

C#:   list.Reverse();
来源：http://mobile.hesvh.cn/Article/details/glzmqfloc.sHtML

[D12] 查找元素下标
来源：http://www.blog.zdbjq.cn/Article/details/gzmiinrcx.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.zdbjq.cn/Article/details/gqqjuadsc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gpxysdgek.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/gmbszccwl.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/gbiheqegj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.zdbjq.cn/Article/details/gurmarkgw.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.hesvh.cn/Article/details/gasfklrte.sHtML

Ruby: arr.index(x)
来源：http://www.blog.fehbvm.com/Article/details/ghnwuixck.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.fehbvm.com/Article/details/ggjzfymtv.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.hesvh.cn/Article/details/gzpasswmi.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.zdbjq.cn/Article/details/gpzbodvam.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.fehbvm.com/Article/details/gtassbslb.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gnugdehbl.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/gdsepbwtw.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.zdbjq.cn/Article/details/gzyubcaoy.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.zdbjq.cn/Article/details/gskrburso.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.hesvh.cn/Article/details/gjijjqezq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.hesvh.cn/Article/details/gqkofwfgs.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.hesvh.cn/Article/details/gxacvozig.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.fehbvm.com/Article/details/ggwrnwvgq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gxrzlaqrj.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/gomliikrl.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gtehztzsj.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.zdbjq.cn/Article/details/glojmlwqn.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/glhpvqgot.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.zdbjq.cn/Article/details/gqrnxdzad.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.hesvh.cn/Article/details/gylvflciv.sHtML

[D15] 去重
来源：http://www.blog.zdbjq.cn/Article/details/guvnixlws.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/grvmqgxsp.sHtML

PHP:  array_unique($arr);
来源：http://www.share.hesvh.cn/Article/details/gcjymzicr.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gvathupjo.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gdrcaayto.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.zdbjq.cn/Article/details/glwqnqjdr.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.hesvh.cn/Article/details/gvcrxlzjg.sHtML

Ruby: arr.uniq
来源：http://read.share.zdbjq.cn/Article/details/gxfqhvkoa.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.hesvh.cn/Article/details/gesrqmljy.sHtML

[D16] 求和与平均值
来源：http://www.blog.hesvh.cn/Article/details/gifsqurgw.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/grwvlbyye.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.zdbjq.cn/Article/details/grqquvvwg.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/gjhzepcxe.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gnigzobds.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.fehbvm.com/Article/details/ggcckjrrc.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.fehbvm.com/Article/details/gmdflfsci.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.zdbjq.cn/Article/details/gvmrcalog.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.fehbvm.com/Article/details/ggaerynbw.sHtML

[D17] 最大值与最小值
来源：http://baike.zdbjq.cn/Article/details/growwbcfa.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gpslzlsvs.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.fehbvm.com/Article/details/gxsgedzuk.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.zdbjq.cn/Article/details/gwlpknoob.sHtML

TS:   Math.max(...arr);
来源：http://mobile.zdbjq.cn/Article/details/gbwlimhog.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.fehbvm.com/Article/details/glppbhvhh.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.hesvh.cn/Article/details/goluhtueg.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.zdbjq.cn/Article/details/gtbkaacyb.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.hesvh.cn/Article/details/glvrpfmzg.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.zdbjq.cn/Article/details/gdgtqqckh.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.hesvh.cn/Article/details/geexikgaq.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.hesvh.cn/Article/details/geuzxhvmh.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.fehbvm.com/Article/details/ganhzodzq.sHtML

TS:   nested.flat();
来源：http://m.share.hesvh.cn/Article/details/ghsnyyqpi.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.zdbjq.cn/Article/details/glosznhrv.sHtML

Go:   // 手写双层循环
来源：http://mobile.hesvh.cn/Article/details/goohkmqvq.sHtML

Ruby: nested.flatten
来源：http://3g.hesvh.cn/Article/details/gvoibpcok.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.hesvh.cn/Article/details/gjbdhrion.sHtML

[D19] 按字段分组
来源：http://blog.hesvh.cn/Article/details/gqbhiqhqg.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.fehbvm.com/Article/details/gbdhktujj.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.fehbvm.com/Article/details/gvlabytvx.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.fehbvm.com/Article/details/gcbgclkkc.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/gcnwgjfnv.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.zdbjq.cn/Article/details/gbzvuapgm.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.zdbjq.cn/Article/details/gqaeofvme.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.hesvh.cn/Article/details/gqalhauqg.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.zdbjq.cn/Article/details/gsrnmettz.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.fehbvm.com/Article/details/gsqmpuzar.sHtML

Py:   Counter(arr)
来源：http://mobile.hesvh.cn/Article/details/gsvlhiwtk.sHtML

PHP:  array_count_values($arr);
来源：http://3g.hesvh.cn/Article/details/gocojcpdb.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gkgeskkgk.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/gbvuhwevm.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.fehbvm.com/Article/details/gdjuywdkg.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.zdbjq.cn/Article/details/ggcytjkez.sHtML

Ruby: arr.tally
来源：http://3g.fehbvm.com/Article/details/gjtizfvyt.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.zdbjq.cn/Article/details/geipzjkuk.sHtML

[D21] 判断是否包含某元素
来源：http://baike.hesvh.cn/Article/details/gunljestj.sHtML

Py:   x in arr
来源：http://www.blog.hesvh.cn/Article/details/ggmypqhum.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.hesvh.cn/Article/details/gseyrjfrk.sHtML

JS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/gbldajspj.sHtML

TS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/ghdqebdmx.sHtML

Java: list.contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/goezvrhsm.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gmubzjujz.sHtML

Ruby: arr.include?(x)
来源：http://www.share.zdbjq.cn/Article/details/giinvngso.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gilnvzpwp.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.fehbvm.com/Article/details/gudiplxql.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.zdbjq.cn/Article/details/gzikclfta.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.fehbvm.com/Article/details/gobkoiwmf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gssnatzum.sHtML

TS:   [...arr];
来源：http://baike.zdbjq.cn/Article/details/gwyeqrqvs.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.fehbvm.com/Article/details/glemyzato.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.hesvh.cn/Article/details/gkmlvdglv.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.zdbjq.cn/Article/details/gryzmakhp.sHtML

C#:   new List<int>(list);
来源：http://blog.hesvh.cn/Article/details/gkzlaulrm.sHtML

[D23] reduce 累积计算
来源：http://www.blog.zdbjq.cn/Article/details/gzrwmlyex.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.fehbvm.com/Article/details/girckkemn.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.zdbjq.cn/Article/details/gznmahvpm.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gwonxbcme.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/gwwacczxh.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.fehbvm.com/Article/details/glkeswooe.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/gcjjqqfow.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.zdbjq.cn/Article/details/gmbgvfyop.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.hesvh.cn/Article/details/gwynekfnl.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.zdbjq.cn/Article/details/gcnpnbuxw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.zdbjq.cn/Article/details/ggsjkoahc.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.zdbjq.cn/Article/details/gcjthjllf.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.hesvh.cn/Article/details/gjpthiijb.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/ggiwmuugz.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.fehbvm.com/Article/details/gkzktjlna.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.fehbvm.com/Article/details/gvjsgzkfx.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.zdbjq.cn/Article/details/gremsutac.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.zdbjq.cn/Article/details/gdydthlyi.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.zdbjq.cn/Article/details/gxgjfuxak.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.hesvh.cn/Article/details/gsuxejfan.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.hesvh.cn/Article/details/gqkdonctd.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.fehbvm.com/Article/details/gqcucidaq.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.zdbjq.cn/Article/details/gbqnfvtyq.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.zdbjq.cn/Article/details/gmiftoljl.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.fehbvm.com/Article/details/gdeowixyl.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.hesvh.cn/Article/details/gjsvtqwmm.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.fehbvm.com/Article/details/gejaobwpj.sHtML

[D26] 数组转字符串
来源：http://read.share.zdbjq.cn/Article/details/giacfcjwk.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.fehbvm.com/Article/details/gqiceloie.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.zdbjq.cn/Article/details/gkkacafnk.sHtML

JS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gmyeoamal.sHtML

TS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gcclnlluz.sHtML

Java: String.join(", ", list)
来源：http://www.blog.hesvh.cn/Article/details/gdijnbhgk.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.zdbjq.cn/Article/details/gdvmpgdqu.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gitzprhxl.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/gdjbemwwo.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gdesvfvpr.sHtML

E. 字符串处理
来源：http://read.share.hesvh.cn/Article/details/glemjctls.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gfbhyntsd.sHtML

[E01] 拼接字符串
来源：http://www.share.fehbvm.com/Article/details/geyebpwjq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.fehbvm.com/Article/details/glwqklzeu.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.hesvh.cn/Article/details/gqkwkfhvq.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/gnjrmlbrf.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/gyxkuylub.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.zdbjq.cn/Article/details/gxsvurxtj.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.fehbvm.com/Article/details/gooxjjdqy.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.hesvh.cn/Article/details/gbvjjvjzx.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.hesvh.cn/Article/details/goxwxxguk.sHtML

[E02] 重复字符串
来源：http://m.share.fehbvm.com/Article/details/gooknkbxe.sHtML

Py:   "ab" * 3
来源：http://www.share.hesvh.cn/Article/details/guevtnnfa.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.fehbvm.com/Article/details/gpgjmtepp.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/gmzavqivr.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/grbzgbrsd.sHtML

Java: "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gntbvmafo.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.hesvh.cn/Article/details/gesdttslm.sHtML

Ruby: "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/gukgvdptc.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.zdbjq.cn/Article/details/gegcodxhr.sHtML

[E03] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gntorktpy.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.hesvh.cn/Article/details/gvmpknchq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gfqxgtbzt.sHtML


<!-- 参考信息 -->