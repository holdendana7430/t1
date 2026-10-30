代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://wap.fehbvm.com/Article/details/ghuhwhaec.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.hesvh.cn/Article/details/gpzezvuqx.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.zdbjq.cn/Article/details/gxkkboibg.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.fehbvm.com/Article/details/gtzzjoqqs.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.fehbvm.com/Article/details/gelwombxj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gzohydwij.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.fehbvm.com/Article/details/gmkybxzln.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gruklygmk.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gnbapvwmp.sHtML

Go:   func add(a, b int) int
来源：http://3g.zdbjq.cn/Article/details/ggugzotbh.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.fehbvm.com/Article/details/gmgrfhfmm.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.zdbjq.cn/Article/details/gezlnaryo.sHtML

[C14] 泛型函数
来源：http://www.m.share.fehbvm.com/Article/details/gavflqfih.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.zdbjq.cn/Article/details/guyntjork.sHtML

PHP:  // 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gblprhijk.sHtML

JS:   // 无泛型
来源：http://www.share.hesvh.cn/Article/details/ganvqfbtu.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.fehbvm.com/Article/details/gjowxrqem.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.fehbvm.com/Article/details/gfqwmewyy.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.fehbvm.com/Article/details/gqionoxit.sHtML

Ruby: # 无泛型
来源：http://baike.fehbvm.com/Article/details/gnihqbhpp.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.hesvh.cn/Article/details/gnsiydoec.sHtML

[C15] 解构 / 展开参数
来源：http://3g.zdbjq.cn/Article/details/gkajqjxuc.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.hesvh.cn/Article/details/goqgcstto.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.fehbvm.com/Article/details/gearkmgjf.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/gtngihrlm.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.fehbvm.com/Article/details/gzrwruihb.sHtML

Java: // 无解构
来源：http://blog.hesvh.cn/Article/details/gzlftcqjg.sHtML

Go:   // 无解构
来源：http://blog.hesvh.cn/Article/details/grlxxtpid.sHtML

Ruby: a, b = pair
来源：http://blog.hesvh.cn/Article/details/gphzvoote.sHtML

C#:   var (a, b) = pair;
来源：http://baike.hesvh.cn/Article/details/gelzuxttb.sHtML

[C16] 函数 / 方法重载
来源：http://wap.hesvh.cn/Article/details/ggtbymagk.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.fehbvm.com/Article/details/gdrlfsqbq.sHtML

PHP:  // 无重载
来源：http://www.blog.zdbjq.cn/Article/details/gfowtxggm.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.zdbjq.cn/Article/details/gxktmdtit.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.hesvh.cn/Article/details/gzewpwolm.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.zdbjq.cn/Article/details/gydlgrydn.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.fehbvm.com/Article/details/grwyotgpw.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.hesvh.cn/Article/details/ggzpxlsvt.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.fehbvm.com/Article/details/gkxluqdaf.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gjejjqyee.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.fehbvm.com/Article/details/gtglcplxh.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/glmutrzou.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.zdbjq.cn/Article/details/gvgkltezp.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.zdbjq.cn/Article/details/gecmhkbmn.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.hesvh.cn/Article/details/gcvmucpse.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.hesvh.cn/Article/details/gggtlykcn.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.fehbvm.com/Article/details/gqgnhnyml.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.hesvh.cn/Article/details/gothdgsjy.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.fehbvm.com/Article/details/ggvgisblg.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.hesvh.cn/Article/details/gyjcrkoyk.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.zdbjq.cn/Article/details/gztazpixa.sHtML

[D02] 追加元素到末尾
来源：http://m.share.zdbjq.cn/Article/details/gsqoljocz.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.zdbjq.cn/Article/details/gpnzrgpux.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.hesvh.cn/Article/details/guamovzxm.sHtML

JS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/gvcohftim.sHtML

TS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/gsreuyfrw.sHtML

Java: list.add(4);
来源：http://blog.fehbvm.com/Article/details/gbdwwfsvv.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.hesvh.cn/Article/details/gzsaapgnv.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.hesvh.cn/Article/details/giwhxgamt.sHtML

C#:   list.Add(4);
来源：http://mobile.zdbjq.cn/Article/details/gglkrgnnp.sHtML

[D03] 在指定位置插入元素
来源：http://wap.zdbjq.cn/Article/details/giokocshj.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.hesvh.cn/Article/details/guqvjnuns.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.fehbvm.com/Article/details/gasjvkvxw.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.zdbjq.cn/Article/details/glqypxyia.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gukmbpqra.sHtML

Java: list.add(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gukwxslhh.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.fehbvm.com/Article/details/gdcnojzte.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.fehbvm.com/Article/details/gvizmjqzd.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.fehbvm.com/Article/details/ghnghjqmb.sHtML

[D04] 删除元素
来源：http://baike.fehbvm.com/Article/details/ganbrsfix.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.hesvh.cn/Article/details/gojbuimsy.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.fehbvm.com/Article/details/gveoqtfcp.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.zdbjq.cn/Article/details/gxlalhhzv.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.fehbvm.com/Article/details/gkfecnbem.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.zdbjq.cn/Article/details/gmwzcciuo.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.zdbjq.cn/Article/details/giocakzwb.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.hesvh.cn/Article/details/gnecrhqvp.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.fehbvm.com/Article/details/gwnzmyola.sHtML

[D05] 访问与修改元素
来源：http://m.share.fehbvm.com/Article/details/gdowdkbuq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/grxtrceed.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/geqkzqavr.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gladvmzlm.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.hesvh.cn/Article/details/ghkzvogsm.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.zdbjq.cn/Article/details/gcwzvvcle.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gvblndrpp.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gyqorosas.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gajyaxmwg.sHtML

[D06] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/gvujmmwbi.sHtML

Py:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gpjfabvuq.sHtML

PHP:  count($arr);
来源：http://baike.zdbjq.cn/Article/details/gbscmoxbj.sHtML

JS:   arr.length
来源：http://www.m.share.hesvh.cn/Article/details/gruktqkks.sHtML

TS:   arr.length
来源：http://3g.hesvh.cn/Article/details/gprrhwivl.sHtML

Java: list.size();
来源：http://m.share.hesvh.cn/Article/details/gpcjqbvri.sHtML

Go:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gbtexqudr.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.zdbjq.cn/Article/details/gmskwhxlx.sHtML

C#:   list.Count;
来源：http://www.blog.hesvh.cn/Article/details/gbnnyllop.sHtML

[D07] 切片 / 取子数组
来源：http://baike.hesvh.cn/Article/details/gwotzmoua.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.hesvh.cn/Article/details/gdxzqgagk.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.zdbjq.cn/Article/details/gmswmbtxv.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gziatierc.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gvtswdbqn.sHtML

Java: list.subList(1, 4);
来源：http://wap.fehbvm.com/Article/details/gvzabkgxj.sHtML

Go:   arr[1:4]
来源：http://blog.zdbjq.cn/Article/details/gfvzajgxq.sHtML

Ruby: arr[1, 3]
来源：http://mobile.hesvh.cn/Article/details/gbbgmquqi.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.hesvh.cn/Article/details/gqalcetfg.sHtML

[D08] 合并两个数组
来源：http://read.share.zdbjq.cn/Article/details/genfxsvzj.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.zdbjq.cn/Article/details/gyqwdhukb.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.hesvh.cn/Article/details/ghsaliudu.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.hesvh.cn/Article/details/gfgaydbyk.sHtML

TS:   [...a, ...b];
来源：http://read.share.fehbvm.com/Article/details/gfoikmeby.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.hesvh.cn/Article/details/gzspxmhbz.sHtML

Go:   append(a, b...)
来源：http://mobile.hesvh.cn/Article/details/gqaarsath.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.zdbjq.cn/Article/details/gbqqgahrt.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gdorojzqq.sHtML

[D09] 排序（升序）
来源：http://www.blog.zdbjq.cn/Article/details/gccupttzk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gtgaauikd.sHtML

PHP:  sort($arr);
来源：http://blog.hesvh.cn/Article/details/ghlakegwe.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.hesvh.cn/Article/details/gtlchgtcq.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.zdbjq.cn/Article/details/gbvdqxltg.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.hesvh.cn/Article/details/grkeyscpz.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gocpxflav.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/gxetfdsso.sHtML

C#:   list.Sort();
来源：http://3g.fehbvm.com/Article/details/gimjmgspa.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.hesvh.cn/Article/details/glbdkcpen.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.zdbjq.cn/Article/details/gpvrwgpxu.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/goddzqzdl.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fehbvm.com/Article/details/gdkisqnwv.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/gxatvmnds.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.hesvh.cn/Article/details/gebkucyna.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.zdbjq.cn/Article/details/goeohowqx.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.zdbjq.cn/Article/details/gcwuqrwjs.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.zdbjq.cn/Article/details/ghjjjumpx.sHtML

[D11] 反转数组
来源：http://baike.hesvh.cn/Article/details/gbqxwljwi.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.fehbvm.com/Article/details/gvpmebvfg.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gamszrpox.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.zdbjq.cn/Article/details/gjonrmhxx.sHtML

TS:   [...arr].reverse();
来源：http://blog.hesvh.cn/Article/details/gkkdoypyv.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.hesvh.cn/Article/details/gsffyjybj.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.zdbjq.cn/Article/details/grduybgnh.sHtML

Ruby: arr.reverse
来源：http://www.m.share.fehbvm.com/Article/details/guominqzd.sHtML

C#:   list.Reverse();
来源：http://read.share.fehbvm.com/Article/details/gvtsdkxab.sHtML

[D12] 查找元素下标
来源：http://m.share.zdbjq.cn/Article/details/gxjbqehlz.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.fehbvm.com/Article/details/gfmypyqdw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.hesvh.cn/Article/details/ghmifcroi.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/gvwmjgyda.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/gqfcwysow.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.hesvh.cn/Article/details/gpdrfeyid.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gorxbgcvi.sHtML

Ruby: arr.index(x)
来源：http://baike.fehbvm.com/Article/details/gkqljjcbf.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.fehbvm.com/Article/details/gsouvlvfd.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.zdbjq.cn/Article/details/gngxexarz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.fehbvm.com/Article/details/gxhtzpzeo.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.fehbvm.com/Article/details/ghubmubxa.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/gjnfmygse.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.fehbvm.com/Article/details/gdlztjwbm.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.zdbjq.cn/Article/details/guumsyihu.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.zdbjq.cn/Article/details/gyiphzphe.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.zdbjq.cn/Article/details/gyhfpthva.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.zdbjq.cn/Article/details/gjzssjybn.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.hesvh.cn/Article/details/gczjkdgfo.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.fehbvm.com/Article/details/gbcfyajxo.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.fehbvm.com/Article/details/gcvdrczvp.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/gdiywyqbx.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.hesvh.cn/Article/details/gdekijzpl.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.hesvh.cn/Article/details/gntgcelsc.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/gsudxsbmo.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.hesvh.cn/Article/details/gedgnqdih.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gabkduujg.sHtML

[D15] 去重
来源：http://read.share.hesvh.cn/Article/details/gngrfqlvr.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/gkhyablhd.sHtML

PHP:  array_unique($arr);
来源：http://read.share.hesvh.cn/Article/details/gefkjhjgr.sHtML

JS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gandhitlm.sHtML

TS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gbrdkaqpm.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.zdbjq.cn/Article/details/glctdnkvt.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.hesvh.cn/Article/details/gnqucwtxo.sHtML

Ruby: arr.uniq
来源：http://3g.hesvh.cn/Article/details/grmshynqe.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.zdbjq.cn/Article/details/gecyqjaqm.sHtML

[D16] 求和与平均值
来源：http://www.share.zdbjq.cn/Article/details/gaetqktxd.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gtupfenha.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.fehbvm.com/Article/details/ghrrhurpk.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/glrokgwwf.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/gjevfysmc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.hesvh.cn/Article/details/gaglrdhpb.sHtML

Go:   // 手写循环累加
来源：http://blog.hesvh.cn/Article/details/gcynbhjpd.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.zdbjq.cn/Article/details/gcveuavvy.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.hesvh.cn/Article/details/gnbhdtkpv.sHtML

[D17] 最大值与最小值
来源：http://www.blog.hesvh.cn/Article/details/ggjlpcofo.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.zdbjq.cn/Article/details/gigmygdow.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.fehbvm.com/Article/details/goensnnue.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.fehbvm.com/Article/details/gkjnzbxnr.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.hesvh.cn/Article/details/gqcfzpzjh.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.zdbjq.cn/Article/details/guqaqyyhw.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.zdbjq.cn/Article/details/gjvbeakev.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.zdbjq.cn/Article/details/glwfysjzy.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.fehbvm.com/Article/details/gyskbljnh.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.zdbjq.cn/Article/details/gtjwrmifq.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.hesvh.cn/Article/details/goyggbild.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.fehbvm.com/Article/details/gnfxommvx.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fehbvm.com/Article/details/ghvdheroh.sHtML

TS:   nested.flat();
来源：http://3g.hesvh.cn/Article/details/ggdbwgrjl.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.fehbvm.com/Article/details/ggvzjrtpy.sHtML

Go:   // 手写双层循环
来源：http://wap.fehbvm.com/Article/details/glvxjvkls.sHtML

Ruby: nested.flatten
来源：http://www.m.share.hesvh.cn/Article/details/ggftwcfdh.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.zdbjq.cn/Article/details/gvhvybtqx.sHtML

[D19] 按字段分组
来源：http://mobile.hesvh.cn/Article/details/guriyyusk.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.hesvh.cn/Article/details/gqosqukgc.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.zdbjq.cn/Article/details/gokmgzkpq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.hesvh.cn/Article/details/gszofdkti.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.zdbjq.cn/Article/details/gpjbdjter.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.zdbjq.cn/Article/details/gsycupbna.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.hesvh.cn/Article/details/gjjsgvfug.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.fehbvm.com/Article/details/gkjzhfdum.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.fehbvm.com/Article/details/gicbmsutc.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.fehbvm.com/Article/details/ggpiyoqct.sHtML

Py:   Counter(arr)
来源：http://mobile.zdbjq.cn/Article/details/gpoufmnfn.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.hesvh.cn/Article/details/glzcodjyw.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fehbvm.com/Article/details/gpansaqbh.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gabzdzofx.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.fehbvm.com/Article/details/guqjbexrf.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.hesvh.cn/Article/details/gpjzkldxo.sHtML

Ruby: arr.tally
来源：http://www.share.hesvh.cn/Article/details/gbtyxjqdn.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.zdbjq.cn/Article/details/glhzwuoaj.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.zdbjq.cn/Article/details/guapzqcst.sHtML

Py:   x in arr
来源：http://read.share.zdbjq.cn/Article/details/gxjrjiafv.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.fehbvm.com/Article/details/gbtrjcdho.sHtML

JS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gfwrlpzwd.sHtML

TS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/guvncvpno.sHtML

Java: list.contains(x)
来源：http://m.share.hesvh.cn/Article/details/goshrdrbp.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.fehbvm.com/Article/details/gcwtrpkkv.sHtML

Ruby: arr.include?(x)
来源：http://3g.zdbjq.cn/Article/details/gzyeylube.sHtML

C#:   list.Contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gahwqhagg.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.zdbjq.cn/Article/details/gmubtpwcn.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.hesvh.cn/Article/details/gkmxrvvwh.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.fehbvm.com/Article/details/gdeuxvuuu.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.zdbjq.cn/Article/details/gqvgfajjj.sHtML

TS:   [...arr];
来源：http://www.m.share.zdbjq.cn/Article/details/ghzezojnw.sHtML

Java: new ArrayList<>(list);
来源：http://baike.zdbjq.cn/Article/details/gzwqasbay.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.fehbvm.com/Article/details/gnmljafaf.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.hesvh.cn/Article/details/gzvjheqin.sHtML

C#:   new List<int>(list);
来源：http://3g.zdbjq.cn/Article/details/gxcmjmbbi.sHtML

[D23] reduce 累积计算
来源：http://m.share.hesvh.cn/Article/details/ggrbrcbyn.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gjmpwhrwc.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.fehbvm.com/Article/details/gkljpydzk.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/gjzqmfylu.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gqpqhekgl.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.zdbjq.cn/Article/details/glwiqliis.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/gfbyfxttk.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.zdbjq.cn/Article/details/gssfvkwom.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.hesvh.cn/Article/details/gbrvimsse.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.hesvh.cn/Article/details/gqrtlmcqu.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.hesvh.cn/Article/details/gxttirrvg.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.zdbjq.cn/Article/details/gyozclzjv.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.fehbvm.com/Article/details/geoikrzyd.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/ggemabcap.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.fehbvm.com/Article/details/gjafnfymf.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.hesvh.cn/Article/details/gqziklyvi.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.hesvh.cn/Article/details/gcylzftwq.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.zdbjq.cn/Article/details/giwnqynpb.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.fehbvm.com/Article/details/gsinycihu.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.zdbjq.cn/Article/details/ghxvladqo.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.hesvh.cn/Article/details/gaypyrrbs.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.hesvh.cn/Article/details/gteyrpeuv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.zdbjq.cn/Article/details/gsfnjhijm.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.zdbjq.cn/Article/details/ggxazoxst.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.fehbvm.com/Article/details/gumoesryn.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.zdbjq.cn/Article/details/gfjxjuogq.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.zdbjq.cn/Article/details/gftylhknr.sHtML

[D26] 数组转字符串
来源：http://read.share.hesvh.cn/Article/details/gaksuzigx.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.hesvh.cn/Article/details/gauynpodr.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.zdbjq.cn/Article/details/gozitshsv.sHtML

JS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gtannhxim.sHtML

TS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gepnavyho.sHtML

Java: String.join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/gcnpxzsup.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.hesvh.cn/Article/details/gvfknxwrc.sHtML

Ruby: arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gxccpxunu.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gtdcblmzr.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gdsvxirfo.sHtML

E. 字符串处理
来源：http://www.m.share.zdbjq.cn/Article/details/gloaeecjo.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gqvqaqkrn.sHtML

[E01] 拼接字符串
来源：http://baike.zdbjq.cn/Article/details/ghgpbezha.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.zdbjq.cn/Article/details/gesqvovfj.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.hesvh.cn/Article/details/gxnvtdfim.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gpazejnay.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/gtqttopri.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.hesvh.cn/Article/details/ggfisrlqe.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.fehbvm.com/Article/details/gzuzncxld.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.fehbvm.com/Article/details/gvtgspmui.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.hesvh.cn/Article/details/gcurmhjjm.sHtML

[E02] 重复字符串
来源：http://baike.fehbvm.com/Article/details/grzzitnzd.sHtML

Py:   "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/gbokzyfpv.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.zdbjq.cn/Article/details/gaiowtnhd.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gonfxzlrz.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gvimzakss.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gtfzmssta.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.fehbvm.com/Article/details/gnvdwjyag.sHtML

Ruby: "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gpterybhp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.zdbjq.cn/Article/details/gvkvnxyxl.sHtML

[E03] 截取子串
来源：http://www.share.fehbvm.com/Article/details/gtjrokibe.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.zdbjq.cn/Article/details/gpnsfxouo.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/ggjhkspqn.sHtML


<!-- 参考信息 -->