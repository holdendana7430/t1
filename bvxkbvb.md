代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://3g.hesvh.cn/Article/details/gxzugrwoq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.hesvh.cn/Article/details/gefdmjiov.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/gbfakvzzv.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.zdbjq.cn/Article/details/guigcihki.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.fehbvm.com/Article/details/gavmavlrr.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.zdbjq.cn/Article/details/gqrkzyiht.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.zdbjq.cn/Article/details/gnjgcqbxq.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.fehbvm.com/Article/details/gkyfnxcry.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.hesvh.cn/Article/details/gtdrbmodr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gsllwxilt.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.zdbjq.cn/Article/details/ggoijnsru.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/grsbzsbja.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gpheebcpr.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.fehbvm.com/Article/details/gwanpofoi.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.hesvh.cn/Article/details/gqzbkwuxf.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.fehbvm.com/Article/details/gatrbaufz.sHtML

[C14] 泛型函数
来源：http://read.share.fehbvm.com/Article/details/glhmfhnzh.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.fehbvm.com/Article/details/gettqxjbz.sHtML

PHP:  // 无泛型
来源：http://wap.fehbvm.com/Article/details/genkbqxyw.sHtML

JS:   // 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gzwoawlcc.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.fehbvm.com/Article/details/glkvejygh.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.fehbvm.com/Article/details/gebsrmbbh.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.fehbvm.com/Article/details/gcduworxb.sHtML

Ruby: # 无泛型
来源：http://mobile.zdbjq.cn/Article/details/geahdtvyc.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.fehbvm.com/Article/details/gnfocdqwl.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.zdbjq.cn/Article/details/gnsiybyzi.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.hesvh.cn/Article/details/gfjihbbmu.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.zdbjq.cn/Article/details/geirnqjzx.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.fehbvm.com/Article/details/gtsbxsuno.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.fehbvm.com/Article/details/gldqpvwww.sHtML

Java: // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gmauqcfzm.sHtML

Go:   // 无解构
来源：http://baike.zdbjq.cn/Article/details/gqexydtjl.sHtML

Ruby: a, b = pair
来源：http://mobile.fehbvm.com/Article/details/gfmmlfzol.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.hesvh.cn/Article/details/glvawslqr.sHtML

[C16] 函数 / 方法重载
来源：http://baike.zdbjq.cn/Article/details/giloxfhje.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.zdbjq.cn/Article/details/gltvlaclx.sHtML

PHP:  // 无重载
来源：http://www.blog.fehbvm.com/Article/details/gnpjdkubw.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.fehbvm.com/Article/details/gemodyobe.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.hesvh.cn/Article/details/ghiqncsme.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.zdbjq.cn/Article/details/gymqvbbww.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.zdbjq.cn/Article/details/gzraeszhc.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.hesvh.cn/Article/details/gzpadgqxu.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.hesvh.cn/Article/details/gdwmakjly.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gvrglligs.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.zdbjq.cn/Article/details/gwgpwapqv.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ggpesoxbv.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.hesvh.cn/Article/details/gskwqrqmn.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.zdbjq.cn/Article/details/gvyltpaeq.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.zdbjq.cn/Article/details/gmveacapz.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.fehbvm.com/Article/details/gljlrbgji.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.zdbjq.cn/Article/details/gcrrrrpfe.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.fehbvm.com/Article/details/gmyctndyu.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.fehbvm.com/Article/details/gnblaziqg.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.hesvh.cn/Article/details/gztxayuqk.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.fehbvm.com/Article/details/guuomlygs.sHtML

[D02] 追加元素到末尾
来源：http://3g.zdbjq.cn/Article/details/gfqxasosx.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.zdbjq.cn/Article/details/gwpeykkrg.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.fehbvm.com/Article/details/gydfqbzxh.sHtML

JS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/gtppyjojs.sHtML

TS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/goqqeuosv.sHtML

Java: list.add(4);
来源：http://www.share.zdbjq.cn/Article/details/gwdnfitwf.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.zdbjq.cn/Article/details/gejfrbnzm.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.zdbjq.cn/Article/details/gvbfkecoj.sHtML

C#:   list.Add(4);
来源：http://blog.hesvh.cn/Article/details/gcewfhxzb.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.zdbjq.cn/Article/details/gdsxybfxz.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.hesvh.cn/Article/details/gatpkbnqc.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.hesvh.cn/Article/details/gvpxneszi.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.zdbjq.cn/Article/details/geobadghc.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.fehbvm.com/Article/details/giemgljtt.sHtML

Java: list.add(0, 0);
来源：http://mobile.hesvh.cn/Article/details/grrqmcvai.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.fehbvm.com/Article/details/gwqbkspvn.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.hesvh.cn/Article/details/gfbjqwcpt.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/guxljwjja.sHtML

[D04] 删除元素
来源：http://blog.fehbvm.com/Article/details/gcmcrkzhh.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.hesvh.cn/Article/details/gipcjeouq.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.fehbvm.com/Article/details/gqcmlgmnl.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.zdbjq.cn/Article/details/gstxyczbt.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.zdbjq.cn/Article/details/gqjeemnyo.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.zdbjq.cn/Article/details/grqelxgpz.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.zdbjq.cn/Article/details/gvephstfe.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.fehbvm.com/Article/details/gfszzcwqt.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.zdbjq.cn/Article/details/gpeimhvfh.sHtML

[D05] 访问与修改元素
来源：http://mobile.fehbvm.com/Article/details/gxtsafqzt.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gbboaijer.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gbjtadicb.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gdqirtrtt.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.zdbjq.cn/Article/details/ggrlnaccx.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.fehbvm.com/Article/details/guzyfcaws.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gkejmnmyb.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gflwxbcla.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gfkwufybn.sHtML

[D06] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/gdcyiwmzh.sHtML

Py:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/gmqclkthr.sHtML

PHP:  count($arr);
来源：http://wap.hesvh.cn/Article/details/gylbrajvf.sHtML

JS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/gskirvuxl.sHtML

TS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gubmzzglk.sHtML

Java: list.size();
来源：http://baike.hesvh.cn/Article/details/glhgzinjk.sHtML

Go:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/ggyteexwf.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.zdbjq.cn/Article/details/gqlhquvxu.sHtML

C#:   list.Count;
来源：http://mobile.zdbjq.cn/Article/details/gdvezgqxy.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.fehbvm.com/Article/details/geddwfrep.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.zdbjq.cn/Article/details/ghxhulwhl.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.fehbvm.com/Article/details/gvqamdbbg.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gaqaaucms.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gzwrlwdey.sHtML

Java: list.subList(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gqfpqvwbv.sHtML

Go:   arr[1:4]
来源：http://www.blog.hesvh.cn/Article/details/godpgakno.sHtML

Ruby: arr[1, 3]
来源：http://read.share.hesvh.cn/Article/details/ggcftugot.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.fehbvm.com/Article/details/gfdnzlpmw.sHtML

[D08] 合并两个数组
来源：http://m.share.fehbvm.com/Article/details/gtwjkintv.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.fehbvm.com/Article/details/gbcuxpnoz.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.zdbjq.cn/Article/details/gidqwphlm.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.zdbjq.cn/Article/details/gvxztkqid.sHtML

TS:   [...a, ...b];
来源：http://3g.fehbvm.com/Article/details/gogfvfrwg.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.hesvh.cn/Article/details/gwzvuheha.sHtML

Go:   append(a, b...)
来源：http://read.share.fehbvm.com/Article/details/gkqegnxiq.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.hesvh.cn/Article/details/ggrvettuk.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.fehbvm.com/Article/details/guqiwnbvq.sHtML

[D09] 排序（升序）
来源：http://baike.hesvh.cn/Article/details/gszpurdip.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.zdbjq.cn/Article/details/gbgjumdqm.sHtML

PHP:  sort($arr);
来源：http://mobile.fehbvm.com/Article/details/glkagofjb.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.hesvh.cn/Article/details/glftlujmq.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.fehbvm.com/Article/details/geufutvbe.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.hesvh.cn/Article/details/gtfyjnkpk.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gmrjpltdd.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/glqnmcvkc.sHtML

C#:   list.Sort();
来源：http://3g.zdbjq.cn/Article/details/gefodnazq.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.zdbjq.cn/Article/details/gqbrouqdr.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.fehbvm.com/Article/details/getreioqf.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fehbvm.com/Article/details/grymmtong.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/gkztlkctg.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fehbvm.com/Article/details/ggqopifra.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.fehbvm.com/Article/details/gacxsqjnq.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.hesvh.cn/Article/details/gfdlwdofv.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.zdbjq.cn/Article/details/gymdvskwp.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.zdbjq.cn/Article/details/gbxswgrkj.sHtML

[D11] 反转数组
来源：http://www.m.share.fehbvm.com/Article/details/gdzqrwofx.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.fehbvm.com/Article/details/gaefyhajo.sHtML

PHP:  array_reverse($arr);
来源：http://baike.fehbvm.com/Article/details/gokrnorju.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.zdbjq.cn/Article/details/gnuhwclhi.sHtML

TS:   [...arr].reverse();
来源：http://mobile.hesvh.cn/Article/details/gnvtergoa.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.zdbjq.cn/Article/details/grqeeuzyt.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.zdbjq.cn/Article/details/gvslojiod.sHtML

Ruby: arr.reverse
来源：http://wap.fehbvm.com/Article/details/glpwujrjh.sHtML

C#:   list.Reverse();
来源：http://www.share.hesvh.cn/Article/details/gpfgxnudq.sHtML

[D12] 查找元素下标
来源：http://wap.hesvh.cn/Article/details/gxskkmotv.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.hesvh.cn/Article/details/gtkpviuif.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.fehbvm.com/Article/details/ggnqnilus.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/gggyvodrq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/glyelmfpg.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.hesvh.cn/Article/details/gduloqhkv.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.fehbvm.com/Article/details/gfkoiicul.sHtML

Ruby: arr.index(x)
来源：http://wap.fehbvm.com/Article/details/gzvrzolzz.sHtML

C#:   list.IndexOf(x);
来源：http://3g.hesvh.cn/Article/details/grcwxzyry.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.hesvh.cn/Article/details/gsubgrbvo.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.zdbjq.cn/Article/details/gntfcwijc.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.fehbvm.com/Article/details/gyabqlaxd.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gkxjbpavy.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/gbemkmzjq.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.hesvh.cn/Article/details/gkzfpdtyy.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.fehbvm.com/Article/details/glbcdjrlv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.fehbvm.com/Article/details/goleramgm.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.hesvh.cn/Article/details/gpdypsvps.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.fehbvm.com/Article/details/gicxpvyjh.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gfpcbdexl.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.zdbjq.cn/Article/details/gjpmexuyj.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/gjyhzvqyp.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/gzvhwtthk.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.fehbvm.com/Article/details/gfkqwvrhu.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/gjoawcwco.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.fehbvm.com/Article/details/gbkwjmgxu.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.fehbvm.com/Article/details/gkjkcaghk.sHtML

[D15] 去重
来源：http://read.share.fehbvm.com/Article/details/gfhjycnqh.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/gwchkbpma.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.zdbjq.cn/Article/details/guoidftlq.sHtML

JS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gyewhuycc.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gbgljhzqz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.zdbjq.cn/Article/details/gkdexdflf.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.zdbjq.cn/Article/details/gwcenyend.sHtML

Ruby: arr.uniq
来源：http://www.blog.fehbvm.com/Article/details/gyjmgxfyf.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.zdbjq.cn/Article/details/guidlhpap.sHtML

[D16] 求和与平均值
来源：http://mobile.hesvh.cn/Article/details/gxximaant.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.fehbvm.com/Article/details/gjkgcoibt.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.fehbvm.com/Article/details/gjrhxmlko.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/gmwvtyvqw.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gcuoowiqi.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.fehbvm.com/Article/details/gcwumymoh.sHtML

Go:   // 手写循环累加
来源：http://3g.zdbjq.cn/Article/details/gchkrwavf.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.zdbjq.cn/Article/details/gnvynnkyz.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.fehbvm.com/Article/details/gviofdxiq.sHtML

[D17] 最大值与最小值
来源：http://read.share.zdbjq.cn/Article/details/gakrnibka.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.zdbjq.cn/Article/details/gskyfgaqy.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.fehbvm.com/Article/details/gcfyfejwm.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.fehbvm.com/Article/details/gezgryzas.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.fehbvm.com/Article/details/ggudbvanp.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.zdbjq.cn/Article/details/gpywpnvzt.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.fehbvm.com/Article/details/gjvgssytf.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.hesvh.cn/Article/details/glgtljsda.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.hesvh.cn/Article/details/gcaodwofr.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.fehbvm.com/Article/details/gxbjsiwue.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.hesvh.cn/Article/details/gqxcvwkvc.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.zdbjq.cn/Article/details/gcpdsglav.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.hesvh.cn/Article/details/gfsprjstf.sHtML

TS:   nested.flat();
来源：http://baike.zdbjq.cn/Article/details/gsfvlocmp.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.zdbjq.cn/Article/details/gcyhlonxr.sHtML

Go:   // 手写双层循环
来源：http://www.share.hesvh.cn/Article/details/gwupkzazf.sHtML

Ruby: nested.flatten
来源：http://read.share.hesvh.cn/Article/details/gciuwccgt.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gkhcqvymb.sHtML

[D19] 按字段分组
来源：http://blog.fehbvm.com/Article/details/gvmcsusjd.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gngkpzhsl.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.hesvh.cn/Article/details/gzxvsxbcg.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.fehbvm.com/Article/details/gvxpyvtem.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/gexrxmebp.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.zdbjq.cn/Article/details/ghouqhghs.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.hesvh.cn/Article/details/gjuwaeocw.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.zdbjq.cn/Article/details/gurrblnsq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.zdbjq.cn/Article/details/giqebibmh.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.hesvh.cn/Article/details/gxalemyxt.sHtML

Py:   Counter(arr)
来源：http://www.share.zdbjq.cn/Article/details/gjwhziyso.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.hesvh.cn/Article/details/gltspfytw.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.zdbjq.cn/Article/details/ggzxmimfx.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gkbyizcok.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.fehbvm.com/Article/details/geipxhmla.sHtML

Go:   // 手写 map[T]int
来源：http://blog.zdbjq.cn/Article/details/gzsdpgimz.sHtML

Ruby: arr.tally
来源：http://www.share.zdbjq.cn/Article/details/gvimclwao.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.hesvh.cn/Article/details/gmyllxydk.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.fehbvm.com/Article/details/gltvlldyw.sHtML

Py:   x in arr
来源：http://www.blog.zdbjq.cn/Article/details/gmjehgwic.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.hesvh.cn/Article/details/gwqnkkjsm.sHtML

JS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/gqlusykel.sHtML

TS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/grdkmgilk.sHtML

Java: list.contains(x)
来源：http://www.share.hesvh.cn/Article/details/gyeojlsiu.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gdxvveohr.sHtML

Ruby: arr.include?(x)
来源：http://3g.zdbjq.cn/Article/details/gacwnbrgt.sHtML

C#:   list.Contains(x)
来源：http://3g.hesvh.cn/Article/details/gubhsctza.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.zdbjq.cn/Article/details/giozjfjed.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gygmoihnj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.zdbjq.cn/Article/details/gryfoqslf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.fehbvm.com/Article/details/gsxeksmww.sHtML

TS:   [...arr];
来源：http://www.share.zdbjq.cn/Article/details/guesuxfrr.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.fehbvm.com/Article/details/gfnhvymil.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.zdbjq.cn/Article/details/gzleycyfu.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.zdbjq.cn/Article/details/gvcfnjuuc.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gpssxuppx.sHtML

[D23] reduce 累积计算
来源：http://www.share.zdbjq.cn/Article/details/gkphzsufv.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.hesvh.cn/Article/details/gnshizrwx.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.fehbvm.com/Article/details/gphbaurbs.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/ghjwdujdb.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/gzbfrwsdo.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.zdbjq.cn/Article/details/gbervxxjz.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/goljgpprh.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.zdbjq.cn/Article/details/gzfmroswv.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.hesvh.cn/Article/details/giixozhjg.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.fehbvm.com/Article/details/gtvydwjlf.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.zdbjq.cn/Article/details/glyttbaxv.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.fehbvm.com/Article/details/gdynmqfae.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.hesvh.cn/Article/details/guhdmhloe.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.fehbvm.com/Article/details/gewrfogaw.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.fehbvm.com/Article/details/ghfgdfbdy.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.zdbjq.cn/Article/details/grwthxmam.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.hesvh.cn/Article/details/gdugyynya.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.hesvh.cn/Article/details/gztvmnxfl.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.zdbjq.cn/Article/details/gheoogffi.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.zdbjq.cn/Article/details/gbmtiojmh.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.zdbjq.cn/Article/details/gcygglvpt.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.fehbvm.com/Article/details/goxjwposa.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.fehbvm.com/Article/details/ghqdkbfes.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.hesvh.cn/Article/details/gktbxbama.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.zdbjq.cn/Article/details/gpkzccddl.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.zdbjq.cn/Article/details/ghcjsqaqj.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.zdbjq.cn/Article/details/gqgvamwpn.sHtML

[D26] 数组转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gcqksqjhr.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.hesvh.cn/Article/details/ghoydanvq.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.hesvh.cn/Article/details/gxddhhavl.sHtML

JS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/giqlcpiol.sHtML

TS:   arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gnwoerptc.sHtML

Java: String.join(", ", list)
来源：http://read.share.fehbvm.com/Article/details/grmqhztdp.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.hesvh.cn/Article/details/gnmiowfse.sHtML

Ruby: arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gfpalmjyq.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.fehbvm.com/Article/details/gcrumjxno.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gnjmykbyt.sHtML

E. 字符串处理
来源：http://wap.zdbjq.cn/Article/details/gocrbtztb.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gzryjdrmd.sHtML

[E01] 拼接字符串
来源：http://blog.hesvh.cn/Article/details/gbvlkiegy.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.fehbvm.com/Article/details/genijifgr.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.zdbjq.cn/Article/details/gzpcbnzmk.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/gizcnaaqf.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/ggebvfnli.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.hesvh.cn/Article/details/ggdxdvaol.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.zdbjq.cn/Article/details/goanwvbod.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.zdbjq.cn/Article/details/gitstcvpi.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.fehbvm.com/Article/details/ghsqopglm.sHtML

[E02] 重复字符串
来源：http://baike.fehbvm.com/Article/details/gnwnwgsra.sHtML

Py:   "ab" * 3
来源：http://3g.hesvh.cn/Article/details/gvmgddzcw.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.hesvh.cn/Article/details/gsapkotju.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gglrugkiw.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gtwwrnhmk.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/ggdcyzqor.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.fehbvm.com/Article/details/glrcgtzjm.sHtML

Ruby: "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/gmkaezrhs.sHtML


<!-- 参考信息 -->