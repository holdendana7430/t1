代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://baike.fehbvm.com/Article/details/gzpnyfnld.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.fehbvm.com/Article/details/gtdpvdgod.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.fehbvm.com/Article/details/grjxnrcwn.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.hesvh.cn/Article/details/gkcgrdgfw.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.hesvh.cn/Article/details/gzxjlbkzi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gizimhkdy.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.zdbjq.cn/Article/details/gpmnqzqpx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gpqfgzsrw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gzfveltgs.sHtML

Go:   func add(a, b int) int
来源：http://m.share.zdbjq.cn/Article/details/gtwwcqtrp.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.fehbvm.com/Article/details/gpouxesxn.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.hesvh.cn/Article/details/gvkgvrdip.sHtML

[C14] 泛型函数
来源：http://baike.fehbvm.com/Article/details/gpvpgoiwq.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.hesvh.cn/Article/details/gopxsmlxg.sHtML

PHP:  // 无泛型
来源：http://read.share.fehbvm.com/Article/details/gzbupcifk.sHtML

JS:   // 无泛型
来源：http://m.share.hesvh.cn/Article/details/gsdyjycao.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.fehbvm.com/Article/details/gvnvabusj.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.fehbvm.com/Article/details/grqefguau.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.hesvh.cn/Article/details/gdxtonrny.sHtML

Ruby: # 无泛型
来源：http://3g.fehbvm.com/Article/details/govlmadyq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.fehbvm.com/Article/details/gnswyvoox.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.fehbvm.com/Article/details/gbkzamcvz.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.zdbjq.cn/Article/details/gfuwznxii.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.zdbjq.cn/Article/details/gxylkvlwh.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.hesvh.cn/Article/details/gkpfglumj.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.hesvh.cn/Article/details/gstrvjywa.sHtML

Java: // 无解构
来源：http://mobile.hesvh.cn/Article/details/ggvsylrjh.sHtML

Go:   // 无解构
来源：http://www.share.zdbjq.cn/Article/details/gvxziuljy.sHtML

Ruby: a, b = pair
来源：http://mobile.zdbjq.cn/Article/details/gllmxhbyx.sHtML

C#:   var (a, b) = pair;
来源：http://wap.zdbjq.cn/Article/details/ghlqykttm.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.fehbvm.com/Article/details/gkrqcywuh.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.hesvh.cn/Article/details/gzcedbvik.sHtML

PHP:  // 无重载
来源：http://m.share.zdbjq.cn/Article/details/goujzykvq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.hesvh.cn/Article/details/govzprpko.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.hesvh.cn/Article/details/gvdrbthiz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.zdbjq.cn/Article/details/gayamioqh.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.fehbvm.com/Article/details/gshwnyafz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.fehbvm.com/Article/details/gqsyqkasv.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gznzebsbx.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gqstyprvb.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.zdbjq.cn/Article/details/gdbswnkch.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gumfuekpc.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.zdbjq.cn/Article/details/glqlnbepa.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.zdbjq.cn/Article/details/gqerbjvrn.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.hesvh.cn/Article/details/gfxixfwux.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.hesvh.cn/Article/details/gbjuxuzth.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.hesvh.cn/Article/details/gfsaobuiq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.hesvh.cn/Article/details/gyffcphix.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.zdbjq.cn/Article/details/gzgjoplkb.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.zdbjq.cn/Article/details/gdbifasvg.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.zdbjq.cn/Article/details/gtobrxdsv.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.hesvh.cn/Article/details/gscvkwekr.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.hesvh.cn/Article/details/gghdehwxd.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.fehbvm.com/Article/details/gtqevugzr.sHtML

JS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/goviraqcx.sHtML

TS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/gwfdunkrp.sHtML

Java: list.add(4);
来源：http://www.share.hesvh.cn/Article/details/gemwipqup.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.hesvh.cn/Article/details/gtwpryknj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.fehbvm.com/Article/details/gqguwkasa.sHtML

C#:   list.Add(4);
来源：http://read.share.hesvh.cn/Article/details/gfjmjycex.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.fehbvm.com/Article/details/gpdbdwcvs.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.fehbvm.com/Article/details/gbilylkxi.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.fehbvm.com/Article/details/gzckejzpu.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.hesvh.cn/Article/details/givyqtewy.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.fehbvm.com/Article/details/goxorsfyc.sHtML

Java: list.add(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gzeorkcwx.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.zdbjq.cn/Article/details/gqwgrsclf.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.fehbvm.com/Article/details/gtricuefi.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.fehbvm.com/Article/details/gwverrmgz.sHtML

[D04] 删除元素
来源：http://baike.hesvh.cn/Article/details/gqercwvee.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.fehbvm.com/Article/details/gfzkecrkk.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.hesvh.cn/Article/details/gwwkzbuwh.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.hesvh.cn/Article/details/givnucmlt.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.fehbvm.com/Article/details/giwcwadzk.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.zdbjq.cn/Article/details/gmlwlnybb.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.zdbjq.cn/Article/details/gmnkdgknu.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.hesvh.cn/Article/details/gccjvxcqp.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.fehbvm.com/Article/details/gsacflyjc.sHtML

[D05] 访问与修改元素
来源：http://www.share.zdbjq.cn/Article/details/gcqasyhlo.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/ghhicwcuj.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gvielpczq.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/ghmtvdzyh.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.zdbjq.cn/Article/details/gsazqjngv.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.zdbjq.cn/Article/details/gfwpddjom.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gmifvbrfk.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gfjehemex.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gumghhxzf.sHtML

[D06] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/gbdaefvrh.sHtML

Py:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gfwpaygmk.sHtML

PHP:  count($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gfsgrzdul.sHtML

JS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/gmtyrqhll.sHtML

TS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/gxmuzmnkk.sHtML

Java: list.size();
来源：http://www.m.share.fehbvm.com/Article/details/grjglsfkl.sHtML

Go:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gdamgvusv.sHtML

Ruby: arr.length; arr.size
来源：http://baike.zdbjq.cn/Article/details/gtjiwcgbc.sHtML

C#:   list.Count;
来源：http://baike.fehbvm.com/Article/details/ghssxlsxz.sHtML

[D07] 切片 / 取子数组
来源：http://wap.fehbvm.com/Article/details/gkkiqrwjb.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.zdbjq.cn/Article/details/gtpxbauit.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.zdbjq.cn/Article/details/gjxwhvbsk.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gmuhmlybe.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/grijghilk.sHtML

Java: list.subList(1, 4);
来源：http://www.share.hesvh.cn/Article/details/guuoctubm.sHtML

Go:   arr[1:4]
来源：http://www.share.fehbvm.com/Article/details/gaonihmpx.sHtML

Ruby: arr[1, 3]
来源：http://mobile.zdbjq.cn/Article/details/gqimhxacx.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.zdbjq.cn/Article/details/gevijmgby.sHtML

[D08] 合并两个数组
来源：http://mobile.hesvh.cn/Article/details/giejnbltq.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.zdbjq.cn/Article/details/glqacofmi.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.zdbjq.cn/Article/details/ggxuztqul.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.fehbvm.com/Article/details/gtjkunkep.sHtML

TS:   [...a, ...b];
来源：http://mobile.zdbjq.cn/Article/details/gqyvdkcbm.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.fehbvm.com/Article/details/gohzbcklt.sHtML

Go:   append(a, b...)
来源：http://wap.fehbvm.com/Article/details/gvlagdiud.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.hesvh.cn/Article/details/grmmhnqcv.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gchkbcbmz.sHtML

[D09] 排序（升序）
来源：http://3g.fehbvm.com/Article/details/gelaifvch.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gxwvgfmln.sHtML

PHP:  sort($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gdjvmvzuz.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.zdbjq.cn/Article/details/glfcjuyor.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.zdbjq.cn/Article/details/gcuxumbti.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.fehbvm.com/Article/details/gijnpwfqn.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gcrygdtik.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/ggwofojpz.sHtML

C#:   list.Sort();
来源：http://baike.hesvh.cn/Article/details/gxgimxrcx.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.fehbvm.com/Article/details/gzgcqkuod.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.zdbjq.cn/Article/details/gwowselib.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/getgvwagy.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/gjdsxxntw.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gfwkqqnho.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.hesvh.cn/Article/details/gmwslxvyk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.fehbvm.com/Article/details/gzovazyvd.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.zdbjq.cn/Article/details/gpfpcbgrh.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.hesvh.cn/Article/details/gvioxgfyi.sHtML

[D11] 反转数组
来源：http://baike.fehbvm.com/Article/details/gcupnzgbp.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.fehbvm.com/Article/details/gbqpwsuwq.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.hesvh.cn/Article/details/gsoijajkk.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.fehbvm.com/Article/details/gaitxvmcy.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.fehbvm.com/Article/details/gxcwaxrli.sHtML

Java: Collections.reverse(list);
来源：http://blog.zdbjq.cn/Article/details/ggvjnidna.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.hesvh.cn/Article/details/gzfmkdorc.sHtML

Ruby: arr.reverse
来源：http://wap.hesvh.cn/Article/details/gwbheauuo.sHtML

C#:   list.Reverse();
来源：http://www.share.fehbvm.com/Article/details/gnqsifijz.sHtML

[D12] 查找元素下标
来源：http://blog.hesvh.cn/Article/details/gomjvdtqc.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.zdbjq.cn/Article/details/gmqvvsbge.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.zdbjq.cn/Article/details/gykgfygys.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/gnldkgqbd.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/gopdtbglj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.zdbjq.cn/Article/details/gxckimdpi.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.hesvh.cn/Article/details/gnkgdczzy.sHtML

Ruby: arr.index(x)
来源：http://www.blog.zdbjq.cn/Article/details/gfyeezgxe.sHtML

C#:   list.IndexOf(x);
来源：http://baike.zdbjq.cn/Article/details/gykiwdlpm.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.fehbvm.com/Article/details/gzfebupub.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gdfmjvkik.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.fehbvm.com/Article/details/gudnnyeuc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.fehbvm.com/Article/details/gjjudpiwj.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gnltcszpp.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.fehbvm.com/Article/details/gjoshozqc.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.zdbjq.cn/Article/details/gtwdhazjz.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.hesvh.cn/Article/details/gnjvwdsyy.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gxzetugvr.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.zdbjq.cn/Article/details/gikraftsh.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gkaxjwrxp.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.zdbjq.cn/Article/details/gcdcsqtid.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gfrqsyvyj.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gklwhleaz.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.hesvh.cn/Article/details/galxwxepe.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/glykqpckz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.fehbvm.com/Article/details/glcsbghcu.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.zdbjq.cn/Article/details/glcojrnbl.sHtML

[D15] 去重
来源：http://blog.hesvh.cn/Article/details/ghneytdfp.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/gjxyipwxu.sHtML

PHP:  array_unique($arr);
来源：http://blog.hesvh.cn/Article/details/gcgulyptl.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gdhcqwyvw.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gclvuzqii.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.fehbvm.com/Article/details/gdubikoxm.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.hesvh.cn/Article/details/gooyyzclc.sHtML

Ruby: arr.uniq
来源：http://3g.zdbjq.cn/Article/details/gtxbcjttz.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.hesvh.cn/Article/details/gbhpvjrcf.sHtML

[D16] 求和与平均值
来源：http://www.blog.zdbjq.cn/Article/details/gabladvuk.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.hesvh.cn/Article/details/gxiwzhesz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.fehbvm.com/Article/details/golmvhagd.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gkhstpyhp.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/gplouvgxf.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.fehbvm.com/Article/details/gxbrdbsgz.sHtML

Go:   // 手写循环累加
来源：http://www.blog.zdbjq.cn/Article/details/ghymunpqs.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.hesvh.cn/Article/details/gbffiynnv.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.fehbvm.com/Article/details/gvrwkktdg.sHtML

[D17] 最大值与最小值
来源：http://baike.zdbjq.cn/Article/details/gymyhdkig.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.fehbvm.com/Article/details/gzaawofft.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.hesvh.cn/Article/details/ggxpbgzjj.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.fehbvm.com/Article/details/gynlopgqo.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.zdbjq.cn/Article/details/gbfxzwhzr.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.zdbjq.cn/Article/details/gevvqqcuw.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.hesvh.cn/Article/details/gfekikpcd.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.zdbjq.cn/Article/details/gzahmlxip.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.zdbjq.cn/Article/details/gmmqaehkd.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.zdbjq.cn/Article/details/gjligyslj.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.hesvh.cn/Article/details/gwjmjrkwj.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.zdbjq.cn/Article/details/ggapkgydb.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.zdbjq.cn/Article/details/gsngkiqta.sHtML

TS:   nested.flat();
来源：http://3g.hesvh.cn/Article/details/gkoispxgl.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.zdbjq.cn/Article/details/gxltwhgls.sHtML

Go:   // 手写双层循环
来源：http://read.share.hesvh.cn/Article/details/gpoghrvan.sHtML

Ruby: nested.flatten
来源：http://m.share.zdbjq.cn/Article/details/gtprobxpu.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.hesvh.cn/Article/details/gxmwohqcs.sHtML

[D19] 按字段分组
来源：http://www.blog.zdbjq.cn/Article/details/gpvcwsipp.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.zdbjq.cn/Article/details/gsdruvhql.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.hesvh.cn/Article/details/gflkxejgo.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.hesvh.cn/Article/details/gjusvpewh.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/gdsfkgeez.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.hesvh.cn/Article/details/gxrpigcml.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.fehbvm.com/Article/details/gtciltyyq.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.fehbvm.com/Article/details/gmmbntakt.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.fehbvm.com/Article/details/gnsteqqrv.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.zdbjq.cn/Article/details/gkfawimvo.sHtML

Py:   Counter(arr)
来源：http://m.share.zdbjq.cn/Article/details/gkrotqqcp.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gbyuyozbq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/grnxjjcoy.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gzmgcrqef.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.fehbvm.com/Article/details/gnsyqhooc.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.zdbjq.cn/Article/details/gwlgmibkv.sHtML

Ruby: arr.tally
来源：http://blog.fehbvm.com/Article/details/gxclyeyhf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.hesvh.cn/Article/details/gogltpfos.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.hesvh.cn/Article/details/goxcwbfql.sHtML

Py:   x in arr
来源：http://www.blog.hesvh.cn/Article/details/gpgforpsc.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.zdbjq.cn/Article/details/gcxufykgv.sHtML

JS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/gykpsbqxn.sHtML

TS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/gpxxrarbc.sHtML

Java: list.contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gtspqwsaa.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gjklrhdjy.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.fehbvm.com/Article/details/gprjtvbin.sHtML

C#:   list.Contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gufkhknka.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.zdbjq.cn/Article/details/gnhguhqff.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.zdbjq.cn/Article/details/gpulahjax.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.fehbvm.com/Article/details/gvrkschor.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.fehbvm.com/Article/details/gmhwofgcb.sHtML

TS:   [...arr];
来源：http://www.blog.zdbjq.cn/Article/details/gvmehgove.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gunqmcgcq.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gtuzypaqg.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.fehbvm.com/Article/details/gjctanasg.sHtML

C#:   new List<int>(list);
来源：http://3g.hesvh.cn/Article/details/giwqpnahm.sHtML

[D23] reduce 累积计算
来源：http://wap.fehbvm.com/Article/details/gkwxxdeep.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.fehbvm.com/Article/details/gadazagvx.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.hesvh.cn/Article/details/gcrrqdfpk.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/gpliiesgd.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.hesvh.cn/Article/details/glungvacf.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.zdbjq.cn/Article/details/givpgjosl.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gwccnqonp.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.zdbjq.cn/Article/details/gxzmwxrvx.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.hesvh.cn/Article/details/gzcboughw.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.hesvh.cn/Article/details/ginotqlne.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.fehbvm.com/Article/details/gqqphbdtl.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.zdbjq.cn/Article/details/ggckgoyfe.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.zdbjq.cn/Article/details/gcmoyxgat.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gbtsmjuqq.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.hesvh.cn/Article/details/gdmhswcwh.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.zdbjq.cn/Article/details/guynyxjxs.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.hesvh.cn/Article/details/gqfwbnrps.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.zdbjq.cn/Article/details/ghqzofocm.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.zdbjq.cn/Article/details/gxfefneay.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.zdbjq.cn/Article/details/gcjlininl.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.zdbjq.cn/Article/details/guqwfghkd.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.fehbvm.com/Article/details/gggejlbyr.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.hesvh.cn/Article/details/gfjserylt.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.hesvh.cn/Article/details/grdzmuein.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.hesvh.cn/Article/details/ganrbhlwi.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.fehbvm.com/Article/details/gznyozyjm.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.hesvh.cn/Article/details/gsfpowumd.sHtML

[D26] 数组转字符串
来源：http://www.blog.zdbjq.cn/Article/details/goccxnttv.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.hesvh.cn/Article/details/gcakmczzu.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.fehbvm.com/Article/details/gwhcymcyo.sHtML

JS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/guguyqciq.sHtML

TS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gpbohukdm.sHtML

Java: String.join(", ", list)
来源：http://baike.fehbvm.com/Article/details/gziqsmbsy.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.fehbvm.com/Article/details/gsposzplu.sHtML

Ruby: arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gbfjcgnrp.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.hesvh.cn/Article/details/gkufneyoo.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gsgoqamrb.sHtML

E. 字符串处理
来源：http://mobile.zdbjq.cn/Article/details/gyfpdwiuz.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gfzyeeyge.sHtML

[E01] 拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gzhsrolrp.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.hesvh.cn/Article/details/gqbjciepg.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.zdbjq.cn/Article/details/gjekbrkqn.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.hesvh.cn/Article/details/gcietmice.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fehbvm.com/Article/details/grqkstvht.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.fehbvm.com/Article/details/gzceytszr.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.zdbjq.cn/Article/details/gjuzaekje.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.fehbvm.com/Article/details/gawmapqvj.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.hesvh.cn/Article/details/gujdozadm.sHtML

[E02] 重复字符串
来源：http://www.share.fehbvm.com/Article/details/gnmzdpwhs.sHtML

Py:   "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/ghngbtsfh.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.fehbvm.com/Article/details/gaueecgdt.sHtML

JS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gzrapeash.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/gwziwajpn.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gxfzciyjl.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.fehbvm.com/Article/details/gwyhacqcg.sHtML

Ruby: "ab" * 3
来源：http://mobile.zdbjq.cn/Article/details/gosskbzhr.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.fehbvm.com/Article/details/gambrndda.sHtML

[E03] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gsjqxvxhw.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.hesvh.cn/Article/details/gvdtskpbl.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gissnjaup.sHtML


<!-- 参考信息 -->