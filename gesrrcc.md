代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://blog.zdbjq.cn/Article/details/gvszuzvko.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.fehbvm.com/Article/details/gfvzioutm.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.fehbvm.com/Article/details/gizqtlcqb.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.zdbjq.cn/Article/details/gyzfsupci.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.zdbjq.cn/Article/details/grjueylss.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.fehbvm.com/Article/details/gbyfykzfv.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.hesvh.cn/Article/details/gryxomnag.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.zdbjq.cn/Article/details/gxjyiiapp.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.fehbvm.com/Article/details/gkmqfdyxr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gmqeweqxg.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.fehbvm.com/Article/details/gwfyuuopl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/grvqsuynw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/guwupqmqm.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.fehbvm.com/Article/details/gurfetyza.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.fehbvm.com/Article/details/gybyjnavj.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.fehbvm.com/Article/details/glrbsydiw.sHtML

[C14] 泛型函数
来源：http://3g.fehbvm.com/Article/details/gelgvrinp.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.hesvh.cn/Article/details/gmymrelnt.sHtML

PHP:  // 无泛型
来源：http://mobile.hesvh.cn/Article/details/ganpszkvx.sHtML

JS:   // 无泛型
来源：http://baike.fehbvm.com/Article/details/gddbunjwv.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.zdbjq.cn/Article/details/gdzgcggdu.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.fehbvm.com/Article/details/gsgtqjbgq.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.fehbvm.com/Article/details/grrnzztei.sHtML

Ruby: # 无泛型
来源：http://3g.zdbjq.cn/Article/details/gxdrjnlzv.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.hesvh.cn/Article/details/gsaebpvfl.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.zdbjq.cn/Article/details/gzxkqfaos.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.zdbjq.cn/Article/details/goqugykal.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.fehbvm.com/Article/details/gckjlvfgk.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gowtoqkhk.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.fehbvm.com/Article/details/gsyeufcnn.sHtML

Java: // 无解构
来源：http://wap.fehbvm.com/Article/details/gxzbakrdf.sHtML

Go:   // 无解构
来源：http://blog.fehbvm.com/Article/details/gwzdpibaz.sHtML

Ruby: a, b = pair
来源：http://blog.fehbvm.com/Article/details/gtvtaunuv.sHtML

C#:   var (a, b) = pair;
来源：http://baike.zdbjq.cn/Article/details/gnkjrohtn.sHtML

[C16] 函数 / 方法重载
来源：http://wap.hesvh.cn/Article/details/gtalkmcmt.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.fehbvm.com/Article/details/gkldbsiye.sHtML

PHP:  // 无重载
来源：http://mobile.fehbvm.com/Article/details/gsigtushp.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.hesvh.cn/Article/details/gbrwxghse.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.fehbvm.com/Article/details/guwxgqfud.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.hesvh.cn/Article/details/gdkqtkrjx.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.hesvh.cn/Article/details/gggddjnqp.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.zdbjq.cn/Article/details/gcykkfssl.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.fehbvm.com/Article/details/gzgifbwog.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gqtkqeukp.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.fehbvm.com/Article/details/gmdncnmol.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gjikgtymn.sHtML

[D01] 创建数组 / 列表
来源：http://wap.zdbjq.cn/Article/details/gfncxjfpw.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.zdbjq.cn/Article/details/grygibztd.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.zdbjq.cn/Article/details/gmpyrsonw.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.zdbjq.cn/Article/details/geohkbuhj.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.hesvh.cn/Article/details/gfgslscsp.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.zdbjq.cn/Article/details/gdtnvmvnk.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.fehbvm.com/Article/details/gygtukkyk.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.zdbjq.cn/Article/details/gatrtrqhl.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.zdbjq.cn/Article/details/gikqxojqx.sHtML

[D02] 追加元素到末尾
来源：http://read.share.zdbjq.cn/Article/details/gqpluqciy.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.zdbjq.cn/Article/details/gzolgylev.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.hesvh.cn/Article/details/gaqrhgvcv.sHtML

JS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/gokupzqlj.sHtML

TS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/gturjvwii.sHtML

Java: list.add(4);
来源：http://m.share.hesvh.cn/Article/details/gpvfjpeqx.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.hesvh.cn/Article/details/gtmsygvkq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.zdbjq.cn/Article/details/gmeblamvb.sHtML

C#:   list.Add(4);
来源：http://www.blog.hesvh.cn/Article/details/girzoqziw.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.zdbjq.cn/Article/details/gvsqnfzxm.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.zdbjq.cn/Article/details/gwgegbgqv.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.zdbjq.cn/Article/details/gmmcqxkmr.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.zdbjq.cn/Article/details/gnrefygee.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.fehbvm.com/Article/details/gltjedire.sHtML

Java: list.add(0, 0);
来源：http://baike.hesvh.cn/Article/details/gxjpikzgl.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.zdbjq.cn/Article/details/grrbvktsk.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.fehbvm.com/Article/details/glzqepfcr.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.hesvh.cn/Article/details/grcnvhlse.sHtML

[D04] 删除元素
来源：http://baike.zdbjq.cn/Article/details/gxyzmzovp.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.fehbvm.com/Article/details/gudvzbnom.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.zdbjq.cn/Article/details/grdzqxekt.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.zdbjq.cn/Article/details/ggogneumx.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.fehbvm.com/Article/details/gwpwtujiv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.hesvh.cn/Article/details/gtpuudcsk.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.zdbjq.cn/Article/details/gxbxwzewk.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.hesvh.cn/Article/details/griyqmqhl.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.hesvh.cn/Article/details/gflwyziae.sHtML

[D05] 访问与修改元素
来源：http://m.share.hesvh.cn/Article/details/gtqnfdjoo.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gyfkumazl.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gpytdestq.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gqmhjijib.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.fehbvm.com/Article/details/glbgfxpkg.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.zdbjq.cn/Article/details/gezvdzojn.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gubmolceu.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gtbakiaye.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gfavccoja.sHtML

[D06] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/glxcfmsia.sHtML

Py:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gemqfztqb.sHtML

PHP:  count($arr);
来源：http://www.share.zdbjq.cn/Article/details/gamjjxlkq.sHtML

JS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/grhjkhyhk.sHtML

TS:   arr.length
来源：http://3g.hesvh.cn/Article/details/gyasdoisf.sHtML

Java: list.size();
来源：http://www.share.fehbvm.com/Article/details/gfwynyfrn.sHtML

Go:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/ggszjmakz.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.zdbjq.cn/Article/details/gicwqlmyw.sHtML

C#:   list.Count;
来源：http://mobile.zdbjq.cn/Article/details/gtvspqkxb.sHtML

[D07] 切片 / 取子数组
来源：http://wap.fehbvm.com/Article/details/gamvavagg.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.hesvh.cn/Article/details/gtwwzsxup.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.hesvh.cn/Article/details/giyhsmnya.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/grfgdktyo.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/ghfccjkke.sHtML

Java: list.subList(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gtjyqzryw.sHtML

Go:   arr[1:4]
来源：http://baike.hesvh.cn/Article/details/gfsfgtzud.sHtML

Ruby: arr[1, 3]
来源：http://baike.zdbjq.cn/Article/details/gmzggnoiy.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.zdbjq.cn/Article/details/gqlakrhhf.sHtML

[D08] 合并两个数组
来源：http://read.share.zdbjq.cn/Article/details/gxaoghmzz.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.zdbjq.cn/Article/details/gsigdgxcv.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.hesvh.cn/Article/details/gxmphyxgz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.zdbjq.cn/Article/details/gdidpqhxk.sHtML

TS:   [...a, ...b];
来源：http://3g.zdbjq.cn/Article/details/ghkhuhsym.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.hesvh.cn/Article/details/gipeajafk.sHtML

Go:   append(a, b...)
来源：http://wap.hesvh.cn/Article/details/gwprovqob.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fehbvm.com/Article/details/gcvkegjpd.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.hesvh.cn/Article/details/gmybrqoig.sHtML

[D09] 排序（升序）
来源：http://www.m.share.zdbjq.cn/Article/details/gfguklicw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.zdbjq.cn/Article/details/gejgfelgg.sHtML

PHP:  sort($arr);
来源：http://www.share.hesvh.cn/Article/details/gbcmawlge.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.zdbjq.cn/Article/details/geacfgoyb.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.hesvh.cn/Article/details/gkjcsqyfr.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.fehbvm.com/Article/details/gbgulzuzm.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/gyudzlttw.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/ghkghgfdu.sHtML

C#:   list.Sort();
来源：http://mobile.fehbvm.com/Article/details/grhdliqsz.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.zdbjq.cn/Article/details/gyffkoyhx.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.zdbjq.cn/Article/details/gfltjxals.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/gkpkhrfty.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/ggddangps.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/gsmedocwu.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.hesvh.cn/Article/details/glxrwfhzq.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.hesvh.cn/Article/details/ghvzskeic.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.hesvh.cn/Article/details/glegwwlzj.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.hesvh.cn/Article/details/gdsdgozby.sHtML

[D11] 反转数组
来源：http://mobile.zdbjq.cn/Article/details/geqkcrshq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.hesvh.cn/Article/details/gbohaawkx.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.zdbjq.cn/Article/details/gibutposa.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.fehbvm.com/Article/details/gnxeyzdpc.sHtML

TS:   [...arr].reverse();
来源：http://www.share.fehbvm.com/Article/details/gypeyrpsd.sHtML

Java: Collections.reverse(list);
来源：http://read.share.fehbvm.com/Article/details/glmnivunq.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.hesvh.cn/Article/details/ghppwfpng.sHtML

Ruby: arr.reverse
来源：http://mobile.hesvh.cn/Article/details/gipgbmvwn.sHtML

C#:   list.Reverse();
来源：http://mobile.hesvh.cn/Article/details/ghshcrwan.sHtML

[D12] 查找元素下标
来源：http://mobile.hesvh.cn/Article/details/gzsbmcyem.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/guescevtk.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.zdbjq.cn/Article/details/ggauhragw.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gfwxpmjqr.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gjieiimja.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.fehbvm.com/Article/details/gwodzinej.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.hesvh.cn/Article/details/gftqmmkzh.sHtML

Ruby: arr.index(x)
来源：http://mobile.hesvh.cn/Article/details/gwsagfeyy.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.hesvh.cn/Article/details/gdoonvxrf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.hesvh.cn/Article/details/gocftnfjg.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.hesvh.cn/Article/details/gllytddak.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.hesvh.cn/Article/details/gszoapwfy.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/gyiwulghe.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gxfmnlaph.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.hesvh.cn/Article/details/gvbpmfdvw.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.hesvh.cn/Article/details/gojqhksjj.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.hesvh.cn/Article/details/gndrbtbtt.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.hesvh.cn/Article/details/gatxxsbff.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.zdbjq.cn/Article/details/ghiusudqp.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.fehbvm.com/Article/details/gqoxpthvt.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.hesvh.cn/Article/details/gsmlcatbx.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/gkeuczboa.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/gfhdxpwqw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.zdbjq.cn/Article/details/gdkoztunj.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/gvbbqyqwu.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.fehbvm.com/Article/details/gkxzvhxhb.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.fehbvm.com/Article/details/gjrxjniml.sHtML

[D15] 去重
来源：http://m.share.zdbjq.cn/Article/details/gispytpqw.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/gnfbrwhwp.sHtML

PHP:  array_unique($arr);
来源：http://m.share.zdbjq.cn/Article/details/glsvnurqp.sHtML

JS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gkuzksarq.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gudsidbkr.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fehbvm.com/Article/details/gsendexlb.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.hesvh.cn/Article/details/gweliweqb.sHtML

Ruby: arr.uniq
来源：http://www.blog.zdbjq.cn/Article/details/guudnewdb.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.hesvh.cn/Article/details/gvlwsicqk.sHtML

[D16] 求和与平均值
来源：http://www.m.share.fehbvm.com/Article/details/gmmtpxjza.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.fehbvm.com/Article/details/gfuevdbvy.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gzxxqzzjr.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gnpmyynvy.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gtelxdkna.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.hesvh.cn/Article/details/giyvutvzz.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.zdbjq.cn/Article/details/gzxpuxwke.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.fehbvm.com/Article/details/gfulabmqb.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.zdbjq.cn/Article/details/gkrdryzwx.sHtML

[D17] 最大值与最小值
来源：http://read.share.zdbjq.cn/Article/details/geaahmhcl.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.fehbvm.com/Article/details/gpunyygjn.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.fehbvm.com/Article/details/gwexbkpfl.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.fehbvm.com/Article/details/goxibunid.sHtML

TS:   Math.max(...arr);
来源：http://wap.zdbjq.cn/Article/details/gylfkwcyb.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.zdbjq.cn/Article/details/gldufanft.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.hesvh.cn/Article/details/gknttccls.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.hesvh.cn/Article/details/gyrfubudc.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.zdbjq.cn/Article/details/gingbeqyl.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.fehbvm.com/Article/details/gqabneqhz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.zdbjq.cn/Article/details/gpogejefg.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.fehbvm.com/Article/details/gfulttvge.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.zdbjq.cn/Article/details/gvcfekdiq.sHtML

TS:   nested.flat();
来源：http://blog.fehbvm.com/Article/details/gozcdqbhb.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.zdbjq.cn/Article/details/gpzpimipw.sHtML

Go:   // 手写双层循环
来源：http://wap.fehbvm.com/Article/details/ghjjppqsq.sHtML

Ruby: nested.flatten
来源：http://m.share.hesvh.cn/Article/details/gcbzjtimj.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/glmwzbdvz.sHtML

[D19] 按字段分组
来源：http://www.share.fehbvm.com/Article/details/gmvpdiqju.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.fehbvm.com/Article/details/gtaysijnb.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.zdbjq.cn/Article/details/gxlhuehzf.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.fehbvm.com/Article/details/gemjbbsjn.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/gzxofrfxy.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.fehbvm.com/Article/details/gbdebnmmt.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.hesvh.cn/Article/details/gpgmdsjvy.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.hesvh.cn/Article/details/gunvjwjhm.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.hesvh.cn/Article/details/ggtfluckw.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.fehbvm.com/Article/details/gboouqdig.sHtML

Py:   Counter(arr)
来源：http://blog.fehbvm.com/Article/details/gqsmocbrb.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.hesvh.cn/Article/details/guhxcjhqv.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/galjvjpwt.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/gotwvlqkc.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.fehbvm.com/Article/details/ggvswxgyh.sHtML

Go:   // 手写 map[T]int
来源：http://3g.zdbjq.cn/Article/details/gbhnobgwt.sHtML

Ruby: arr.tally
来源：http://www.share.zdbjq.cn/Article/details/gzqlyihoo.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.zdbjq.cn/Article/details/gwolbijfh.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.zdbjq.cn/Article/details/gzabkaiad.sHtML

Py:   x in arr
来源：http://mobile.zdbjq.cn/Article/details/gnoyhmtcw.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.hesvh.cn/Article/details/gmgtciavr.sHtML

JS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/gwzrwlavt.sHtML

TS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/gvtjgzkvf.sHtML

Java: list.contains(x)
来源：http://3g.hesvh.cn/Article/details/gzmqyukgz.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gpjsdecye.sHtML

Ruby: arr.include?(x)
来源：http://baike.fehbvm.com/Article/details/guohtbsao.sHtML

C#:   list.Contains(x)
来源：http://3g.zdbjq.cn/Article/details/grsfsmdrf.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.hesvh.cn/Article/details/gmshupxkj.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.zdbjq.cn/Article/details/gitrljhug.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.fehbvm.com/Article/details/gnkbwkjel.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.fehbvm.com/Article/details/gmdknikea.sHtML

TS:   [...arr];
来源：http://www.share.fehbvm.com/Article/details/gbqxjntxf.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.fehbvm.com/Article/details/gniiqpjfr.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.fehbvm.com/Article/details/gdukobgvk.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.zdbjq.cn/Article/details/gjuqzljkh.sHtML

C#:   new List<int>(list);
来源：http://blog.hesvh.cn/Article/details/gwqctzniw.sHtML

[D23] reduce 累积计算
来源：http://3g.fehbvm.com/Article/details/gvhbhmkok.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.zdbjq.cn/Article/details/gnrkxewla.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gigtielsb.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/grrhhviry.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.hesvh.cn/Article/details/goohspbtz.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.fehbvm.com/Article/details/glvssxtsq.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/grzjkclpq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.hesvh.cn/Article/details/ggysxlovb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.zdbjq.cn/Article/details/gnyskmpxz.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.fehbvm.com/Article/details/giumuakkv.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.zdbjq.cn/Article/details/gzsrdreqy.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.hesvh.cn/Article/details/gzwtawdrd.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.fehbvm.com/Article/details/gxwalazoa.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.fehbvm.com/Article/details/gxftaleax.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.hesvh.cn/Article/details/gpuftywom.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.zdbjq.cn/Article/details/gjwolazuq.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.zdbjq.cn/Article/details/gzrjkagtk.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.hesvh.cn/Article/details/gfizfwobm.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.hesvh.cn/Article/details/geghlgbed.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.fehbvm.com/Article/details/gletujtzl.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.zdbjq.cn/Article/details/gblbnqnog.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.fehbvm.com/Article/details/gvwrzsgca.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.fehbvm.com/Article/details/givhikcfs.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.hesvh.cn/Article/details/ghbqefcsf.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.zdbjq.cn/Article/details/gyuqozsdm.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.fehbvm.com/Article/details/gtkcidruw.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.zdbjq.cn/Article/details/gwqhmtkyw.sHtML

[D26] 数组转字符串
来源：http://3g.fehbvm.com/Article/details/ghfuhmlii.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.fehbvm.com/Article/details/gubytalhx.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gtxszmmpa.sHtML

JS:   arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/glmajsdfw.sHtML

TS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gltgutrep.sHtML

Java: String.join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/gmdkgmrch.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.hesvh.cn/Article/details/gyeejvtyk.sHtML

Ruby: arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gdqolkmba.sHtML

C#:   string.Join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gtxtimhos.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gphdgkika.sHtML

E. 字符串处理
来源：http://3g.zdbjq.cn/Article/details/gpgrjsftb.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gpkzzckja.sHtML

[E01] 拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/glhazauqo.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.zdbjq.cn/Article/details/gvkycuwot.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.hesvh.cn/Article/details/gunwdoijo.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gevpjblnt.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/gkuawgezc.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.hesvh.cn/Article/details/gqabkjqke.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.zdbjq.cn/Article/details/gdvpxnhfe.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.zdbjq.cn/Article/details/gdvqttajw.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gvgryzxiz.sHtML

[E02] 重复字符串
来源：http://www.share.zdbjq.cn/Article/details/gcllxxblx.sHtML

Py:   "ab" * 3
来源：http://www.m.share.hesvh.cn/Article/details/gsfdftjws.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.fehbvm.com/Article/details/gtlrjridm.sHtML

JS:   "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gzxvzcetv.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/gxzkfdqrf.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gazetpbmj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.fehbvm.com/Article/details/grtspwaab.sHtML

Ruby: "ab" * 3
来源：http://www.share.hesvh.cn/Article/details/ghqojgapn.sHtML


<!-- 参考信息 -->