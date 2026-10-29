代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.fehbvm.com/Article/details/gscglkizk.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.fehbvm.com/Article/details/galcjqzpk.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.hesvh.cn/Article/details/gqsgluelh.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.zdbjq.cn/Article/details/gqtjpcyuv.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.fehbvm.com/Article/details/gffpbkvzc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gujvuafsh.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.hesvh.cn/Article/details/ggwkyhlgd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gvtebarac.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gzbaeduwc.sHtML

Go:   func add(a, b int) int
来源：http://www.share.hesvh.cn/Article/details/gnmaizwim.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.fehbvm.com/Article/details/gicexxhdg.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.fehbvm.com/Article/details/giqtfkwja.sHtML

[C14] 泛型函数
来源：http://www.blog.zdbjq.cn/Article/details/goketsftg.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.zdbjq.cn/Article/details/gkjduyvha.sHtML

PHP:  // 无泛型
来源：http://wap.fehbvm.com/Article/details/gvoimbzfc.sHtML

JS:   // 无泛型
来源：http://m.share.hesvh.cn/Article/details/geefxnrbt.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.hesvh.cn/Article/details/gshqglnkb.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.hesvh.cn/Article/details/gvialokou.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.hesvh.cn/Article/details/gerfisjzv.sHtML

Ruby: # 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gihzlrhvz.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.zdbjq.cn/Article/details/gyogiducj.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.fehbvm.com/Article/details/gpdhwuvlt.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.fehbvm.com/Article/details/gnkkbwnoj.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.zdbjq.cn/Article/details/gcijpezjm.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.hesvh.cn/Article/details/ghiicjfei.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.zdbjq.cn/Article/details/gqufsgdmf.sHtML

Java: // 无解构
来源：http://www.blog.zdbjq.cn/Article/details/ghrxcnylk.sHtML

Go:   // 无解构
来源：http://wap.fehbvm.com/Article/details/gpqjcqxmk.sHtML

Ruby: a, b = pair
来源：http://www.blog.fehbvm.com/Article/details/gxtomjnpz.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.hesvh.cn/Article/details/gwifzyopo.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.hesvh.cn/Article/details/glfyxojew.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.zdbjq.cn/Article/details/gjrxjisfg.sHtML

PHP:  // 无重载
来源：http://mobile.zdbjq.cn/Article/details/gbisaxvzw.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.zdbjq.cn/Article/details/grmhjrjig.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.hesvh.cn/Article/details/giojbmsab.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.fehbvm.com/Article/details/gbwyrxgya.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.fehbvm.com/Article/details/gpdvqnhsv.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.hesvh.cn/Article/details/gldwkhthd.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.fehbvm.com/Article/details/gbulzcoou.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gzygymkjj.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.fehbvm.com/Article/details/goeuheqiw.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gpwbengho.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.fehbvm.com/Article/details/gwwqzpwgr.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.fehbvm.com/Article/details/gqwxqdciz.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.hesvh.cn/Article/details/glryueqxa.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.fehbvm.com/Article/details/gdlbhaoov.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.hesvh.cn/Article/details/guaojscou.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.fehbvm.com/Article/details/gopyruqau.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.hesvh.cn/Article/details/ggtuebjso.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.fehbvm.com/Article/details/gklqaqpxz.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.fehbvm.com/Article/details/guleunocy.sHtML

[D02] 追加元素到末尾
来源：http://m.share.hesvh.cn/Article/details/geeqdssai.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.fehbvm.com/Article/details/gkeiqzlyt.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.zdbjq.cn/Article/details/gehlgytoe.sHtML

JS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gexqclayy.sHtML

TS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/gqrjkkpcj.sHtML

Java: list.add(4);
来源：http://m.share.hesvh.cn/Article/details/gjdppjvvp.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.hesvh.cn/Article/details/gdbiytyak.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.zdbjq.cn/Article/details/gwpjiwxji.sHtML

C#:   list.Add(4);
来源：http://read.share.fehbvm.com/Article/details/gnydzxnjd.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.hesvh.cn/Article/details/guejlrdzb.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.hesvh.cn/Article/details/gnznnbwuo.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.zdbjq.cn/Article/details/gkpszhenm.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.hesvh.cn/Article/details/gymnhidmr.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.hesvh.cn/Article/details/gzttmyybi.sHtML

Java: list.add(0, 0);
来源：http://blog.fehbvm.com/Article/details/gnkekbmdu.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.fehbvm.com/Article/details/gfuutmrgm.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.zdbjq.cn/Article/details/grtkzkccu.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gpzbcsrwd.sHtML

[D04] 删除元素
来源：http://blog.zdbjq.cn/Article/details/gkzeakptp.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.zdbjq.cn/Article/details/gvkyzeamx.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.zdbjq.cn/Article/details/ghjkxqubg.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.zdbjq.cn/Article/details/ggycrzpkx.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.fehbvm.com/Article/details/gjnbkgpzq.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.zdbjq.cn/Article/details/gamqacxgp.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.zdbjq.cn/Article/details/gqkxrrufn.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.fehbvm.com/Article/details/gajyttoqs.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.hesvh.cn/Article/details/ghzvkjphb.sHtML

[D05] 访问与修改元素
来源：http://read.share.zdbjq.cn/Article/details/gdyjdupgj.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gbnqkzkaw.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gcnjguetf.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gxojonseh.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.fehbvm.com/Article/details/gqkktvicl.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.fehbvm.com/Article/details/gdttmrsyh.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gkvicprdt.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gnlqojwgg.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gmnrnwuit.sHtML

[D06] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/gzigsxdlr.sHtML

Py:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gcrhawuxv.sHtML

PHP:  count($arr);
来源：http://m.share.fehbvm.com/Article/details/gqmvrdyne.sHtML

JS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/gybkappyl.sHtML

TS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gcnsfgycy.sHtML

Java: list.size();
来源：http://www.share.zdbjq.cn/Article/details/ghpatzyxm.sHtML

Go:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gvjpybfhc.sHtML

Ruby: arr.length; arr.size
来源：http://baike.fehbvm.com/Article/details/gnujighmc.sHtML

C#:   list.Count;
来源：http://3g.hesvh.cn/Article/details/gvekiycpk.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.zdbjq.cn/Article/details/gbsvgssdp.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.zdbjq.cn/Article/details/gzjynflrg.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.fehbvm.com/Article/details/gdersyphb.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gjwpqvzzh.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/gdmffjaxx.sHtML

Java: list.subList(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gqnjwuylm.sHtML

Go:   arr[1:4]
来源：http://m.share.hesvh.cn/Article/details/gpokyxznj.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.fehbvm.com/Article/details/gedmtxusq.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.zdbjq.cn/Article/details/ghoswxphb.sHtML

[D08] 合并两个数组
来源：http://read.share.fehbvm.com/Article/details/gawpxqwpf.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.fehbvm.com/Article/details/gnfalqyud.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.zdbjq.cn/Article/details/gtmoweqbm.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.fehbvm.com/Article/details/gxlejxpgg.sHtML

TS:   [...a, ...b];
来源：http://mobile.zdbjq.cn/Article/details/gvjzjqydh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gcglrzbxx.sHtML

Go:   append(a, b...)
来源：http://www.share.hesvh.cn/Article/details/gtrucmbwq.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.fehbvm.com/Article/details/goqsvrdyx.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.zdbjq.cn/Article/details/gqvkrbrjy.sHtML

[D09] 排序（升序）
来源：http://www.blog.fehbvm.com/Article/details/gvxkwshng.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gfjncowzx.sHtML

PHP:  sort($arr);
来源：http://www.blog.fehbvm.com/Article/details/gibqlkiwm.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.zdbjq.cn/Article/details/garohfafk.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.fehbvm.com/Article/details/gmkxyxqmj.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.fehbvm.com/Article/details/gqyzjqxhm.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/gvdqjcyos.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/grcnvdmul.sHtML

C#:   list.Sort();
来源：http://baike.zdbjq.cn/Article/details/gmfofmozh.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.hesvh.cn/Article/details/gbcsaocex.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.hesvh.cn/Article/details/gjxcigyvw.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/giwggveqq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/gpqsstrng.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fehbvm.com/Article/details/gwhgdicbg.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.hesvh.cn/Article/details/gnzccsnvm.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.fehbvm.com/Article/details/gbbuyesyv.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.zdbjq.cn/Article/details/gzfowzqdp.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.hesvh.cn/Article/details/gkbfkygwb.sHtML

[D11] 反转数组
来源：http://www.share.zdbjq.cn/Article/details/grkrpvnep.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.fehbvm.com/Article/details/glqzswphs.sHtML

PHP:  array_reverse($arr);
来源：http://wap.hesvh.cn/Article/details/gvgkzueti.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.fehbvm.com/Article/details/gqcqhzgsi.sHtML

TS:   [...arr].reverse();
来源：http://3g.hesvh.cn/Article/details/gethrienf.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.hesvh.cn/Article/details/gcspyurvz.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.hesvh.cn/Article/details/gnttuybjl.sHtML

Ruby: arr.reverse
来源：http://baike.hesvh.cn/Article/details/gqctgxlhg.sHtML

C#:   list.Reverse();
来源：http://read.share.fehbvm.com/Article/details/ggggdezwe.sHtML

[D12] 查找元素下标
来源：http://blog.zdbjq.cn/Article/details/gndlzjhbf.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.hesvh.cn/Article/details/gdxhyjxca.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.hesvh.cn/Article/details/gwdybrzcg.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/ghqhuszam.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/goccumqku.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.fehbvm.com/Article/details/gjkfrpgfs.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gpacnbtbz.sHtML

Ruby: arr.index(x)
来源：http://wap.hesvh.cn/Article/details/gvkobtkro.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.zdbjq.cn/Article/details/gthjambro.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.fehbvm.com/Article/details/gtngizvie.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.fehbvm.com/Article/details/gswjwczio.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.zdbjq.cn/Article/details/gqsfohvrn.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/gkjtmexhm.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gbpxefkac.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.fehbvm.com/Article/details/gwpmccxpy.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.hesvh.cn/Article/details/gyvpequdy.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.fehbvm.com/Article/details/gartgoezd.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.zdbjq.cn/Article/details/grmhpfylz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.fehbvm.com/Article/details/gwddmpigp.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.hesvh.cn/Article/details/gbxipkhws.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.hesvh.cn/Article/details/ggmelpkwe.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/gvatlfqor.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/gihdywayr.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.hesvh.cn/Article/details/gmttvvgse.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/ggkqqwyvw.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gpvjezesv.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.hesvh.cn/Article/details/gknbbupou.sHtML

[D15] 去重
来源：http://baike.hesvh.cn/Article/details/gypvvoakd.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gjnpdtcza.sHtML

PHP:  array_unique($arr);
来源：http://www.share.zdbjq.cn/Article/details/gpszngztc.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gasfjwudf.sHtML

TS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/grgxdwmmk.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.zdbjq.cn/Article/details/gnxhgwdbt.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.zdbjq.cn/Article/details/gqncyeslr.sHtML

Ruby: arr.uniq
来源：http://www.blog.zdbjq.cn/Article/details/gpbkavrnb.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.fehbvm.com/Article/details/gqiujjucl.sHtML

[D16] 求和与平均值
来源：http://baike.fehbvm.com/Article/details/gbaismrkw.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gannpjfiz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.fehbvm.com/Article/details/gpnihubom.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/grsqddcsm.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/gsrhmzgmr.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.zdbjq.cn/Article/details/gelxsuoai.sHtML

Go:   // 手写循环累加
来源：http://3g.zdbjq.cn/Article/details/gunzlunui.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.fehbvm.com/Article/details/ghpviiidl.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.zdbjq.cn/Article/details/golddegbe.sHtML

[D17] 最大值与最小值
来源：http://baike.hesvh.cn/Article/details/gericsqbx.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.hesvh.cn/Article/details/gynkvynjt.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.hesvh.cn/Article/details/glkvdfgeb.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.fehbvm.com/Article/details/glrraniux.sHtML

TS:   Math.max(...arr);
来源：http://mobile.zdbjq.cn/Article/details/gjdmigefh.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.hesvh.cn/Article/details/gfzxqacii.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.fehbvm.com/Article/details/gmiporipf.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.zdbjq.cn/Article/details/ghwegnhes.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.zdbjq.cn/Article/details/gztwtargc.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.fehbvm.com/Article/details/gnzmzynuw.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.zdbjq.cn/Article/details/gvbnudjvc.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.hesvh.cn/Article/details/gqwzpulbc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fehbvm.com/Article/details/gczrvjjzx.sHtML

TS:   nested.flat();
来源：http://mobile.zdbjq.cn/Article/details/gpdhcjmae.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.zdbjq.cn/Article/details/gdjofrxoi.sHtML

Go:   // 手写双层循环
来源：http://wap.zdbjq.cn/Article/details/gfteeynco.sHtML

Ruby: nested.flatten
来源：http://mobile.zdbjq.cn/Article/details/gvqaicaqd.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.fehbvm.com/Article/details/gbeaanobo.sHtML

[D19] 按字段分组
来源：http://m.share.hesvh.cn/Article/details/gofjifzhi.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.hesvh.cn/Article/details/gkwnaqaxz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.zdbjq.cn/Article/details/gnqptpaaj.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.fehbvm.com/Article/details/gtmzjjwak.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.zdbjq.cn/Article/details/gmanwniak.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.zdbjq.cn/Article/details/gtdametyb.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.hesvh.cn/Article/details/ggkmcdkoc.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.zdbjq.cn/Article/details/gomuxuckh.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.fehbvm.com/Article/details/gbnbysdfb.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.zdbjq.cn/Article/details/gquerkvgd.sHtML

Py:   Counter(arr)
来源：http://www.share.fehbvm.com/Article/details/ggecsxwgh.sHtML

PHP:  array_count_values($arr);
来源：http://wap.zdbjq.cn/Article/details/gkilvwbkq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gefovqaqm.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/giqksdfnf.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.zdbjq.cn/Article/details/glgfpvgae.sHtML

Go:   // 手写 map[T]int
来源：http://blog.fehbvm.com/Article/details/ghrbliyqj.sHtML

Ruby: arr.tally
来源：http://blog.hesvh.cn/Article/details/gfuubmyyn.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.hesvh.cn/Article/details/giknnynnm.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.hesvh.cn/Article/details/gybhcjlqx.sHtML

Py:   x in arr
来源：http://www.share.zdbjq.cn/Article/details/gnfarzuqo.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.hesvh.cn/Article/details/gjzbfgczg.sHtML

JS:   arr.includes(x)
来源：http://baike.fehbvm.com/Article/details/gplhookdz.sHtML

TS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/gnvaquoeg.sHtML

Java: list.contains(x)
来源：http://wap.fehbvm.com/Article/details/gundosppt.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.fehbvm.com/Article/details/gumfhkpyt.sHtML

Ruby: arr.include?(x)
来源：http://baike.fehbvm.com/Article/details/gvnuoceer.sHtML

C#:   list.Contains(x)
来源：http://www.share.fehbvm.com/Article/details/gdtriwmpu.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.zdbjq.cn/Article/details/gttppamvq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gzpuhaabc.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.hesvh.cn/Article/details/gtfqzpcpz.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.hesvh.cn/Article/details/gktinngpg.sHtML

TS:   [...arr];
来源：http://mobile.zdbjq.cn/Article/details/gcseflsnk.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.zdbjq.cn/Article/details/gceklqhox.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.zdbjq.cn/Article/details/grcdvyfgo.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.zdbjq.cn/Article/details/gxjybchyk.sHtML

C#:   new List<int>(list);
来源：http://www.share.zdbjq.cn/Article/details/gzfktqfbb.sHtML

[D23] reduce 累积计算
来源：http://read.share.zdbjq.cn/Article/details/gfzrzsllt.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.fehbvm.com/Article/details/gobdldzac.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gfewhdnmt.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/gnawyiltk.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.hesvh.cn/Article/details/gdkphekmv.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.hesvh.cn/Article/details/grhwkwafe.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/gnxxoyolr.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.fehbvm.com/Article/details/grgakkvuj.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.hesvh.cn/Article/details/gmguctyjt.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.zdbjq.cn/Article/details/gryrhogcg.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.hesvh.cn/Article/details/gfpbifkdg.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.fehbvm.com/Article/details/groghjggv.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.hesvh.cn/Article/details/gpwqufdvt.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.hesvh.cn/Article/details/gkwphfkya.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.zdbjq.cn/Article/details/ghstqadxl.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.zdbjq.cn/Article/details/gdhasmbcd.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.fehbvm.com/Article/details/gfcgywkrg.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.fehbvm.com/Article/details/gvwobmhej.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.zdbjq.cn/Article/details/gesgytlyf.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.zdbjq.cn/Article/details/gpddzxkbb.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.hesvh.cn/Article/details/gzvtvxpba.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.fehbvm.com/Article/details/gyrynjmdb.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.hesvh.cn/Article/details/gyicshiwz.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.hesvh.cn/Article/details/gorgblmfn.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.zdbjq.cn/Article/details/gqzzyalcv.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.hesvh.cn/Article/details/gllprrwbq.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/geafyvhwl.sHtML

[D26] 数组转字符串
来源：http://wap.fehbvm.com/Article/details/gxrlstjka.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gsuvmlkon.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.fehbvm.com/Article/details/gzzdhhjcq.sHtML

JS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gxshbjddn.sHtML

TS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/guqfhgjtz.sHtML

Java: String.join(", ", list)
来源：http://read.share.fehbvm.com/Article/details/gnvexkssg.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.hesvh.cn/Article/details/gtemehrle.sHtML

Ruby: arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gwxtminlj.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/gbqfgssyu.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gveqsavad.sHtML

E. 字符串处理
来源：http://3g.hesvh.cn/Article/details/ggetoosju.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ghddhhrxz.sHtML

[E01] 拼接字符串
来源：http://m.share.fehbvm.com/Article/details/graophpha.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.fehbvm.com/Article/details/grxbbxbwr.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.fehbvm.com/Article/details/gouwqfexw.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/gynrsjudx.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gdmpxqwek.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.fehbvm.com/Article/details/gjdwxfvru.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.zdbjq.cn/Article/details/gqxhyavyn.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.zdbjq.cn/Article/details/goaolyklt.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gahmjrktj.sHtML

[E02] 重复字符串
来源：http://m.share.fehbvm.com/Article/details/goeizearh.sHtML

Py:   "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/gxdphqppn.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.zdbjq.cn/Article/details/gcqdgimmp.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gumhvlmtl.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gcpthzozf.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/glatxfwlw.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.hesvh.cn/Article/details/gixockhcj.sHtML

Ruby: "ab" * 3
来源：http://wap.hesvh.cn/Article/details/gxjyykreg.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.fehbvm.com/Article/details/gyeqgcfby.sHtML

[E03] 截取子串
来源：http://wap.fehbvm.com/Article/details/gnmlfaikx.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.hesvh.cn/Article/details/gumaresag.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gyluojuda.sHtML


<!-- 参考信息 -->