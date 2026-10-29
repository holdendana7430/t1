代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://read.share.zdbjq.cn/Article/details/gjtfvruka.sHtML

C#:   using System.Text;
来源：http://m.share.fehbvm.com/Article/details/gfxfsumhk.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.fehbvm.com/Article/details/gxugympiu.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.fehbvm.com/Article/details/gfpkpkwvw.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.zdbjq.cn/Article/details/ginpuvhfq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.zdbjq.cn/Article/details/ggfkohpin.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.fehbvm.com/Article/details/gyowbuokf.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.hesvh.cn/Article/details/gzpxshuck.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.fehbvm.com/Article/details/gmmkyakfc.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.hesvh.cn/Article/details/gnaufdeug.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.zdbjq.cn/Article/details/gxytfavdu.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.hesvh.cn/Article/details/grgjgtpol.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.fehbvm.com/Article/details/gveumvrxg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gsfxzsefh.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.zdbjq.cn/Article/details/grlzwxkpf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gffbrxaqd.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gdgrroiqv.sHtML

Go:   func add(a, b int) int
来源：http://baike.zdbjq.cn/Article/details/gljwmwyro.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.hesvh.cn/Article/details/gimphljdi.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.hesvh.cn/Article/details/gcmxzsken.sHtML

[C14] 泛型函数
来源：http://read.share.zdbjq.cn/Article/details/gojcxqgzt.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.fehbvm.com/Article/details/gtjwdrnyd.sHtML

PHP:  // 无泛型
来源：http://mobile.hesvh.cn/Article/details/gcvnxwsfb.sHtML

JS:   // 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gtvtvpabk.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.fehbvm.com/Article/details/gngmcvkuf.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.fehbvm.com/Article/details/gqbxuiawl.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.fehbvm.com/Article/details/ghwkotkuj.sHtML

Ruby: # 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gtxgcyfgv.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.fehbvm.com/Article/details/gjebeqvxq.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.hesvh.cn/Article/details/gnzuczklp.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.zdbjq.cn/Article/details/gtrvklbcu.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.zdbjq.cn/Article/details/glngfdnfy.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gsnnjwjkm.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.fehbvm.com/Article/details/gxdvvffsa.sHtML

Java: // 无解构
来源：http://3g.zdbjq.cn/Article/details/gjbjblqir.sHtML

Go:   // 无解构
来源：http://www.share.zdbjq.cn/Article/details/gmciqrntk.sHtML

Ruby: a, b = pair
来源：http://3g.fehbvm.com/Article/details/gcyyzwjmx.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.fehbvm.com/Article/details/gigagdpzm.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.zdbjq.cn/Article/details/glsdgehpn.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.fehbvm.com/Article/details/gqwwxqwbd.sHtML

PHP:  // 无重载
来源：http://www.m.share.fehbvm.com/Article/details/goubmpsaw.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.hesvh.cn/Article/details/gpusolqwt.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.hesvh.cn/Article/details/gkahqajyf.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.zdbjq.cn/Article/details/gqexyfqqo.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.hesvh.cn/Article/details/ggmngskog.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.fehbvm.com/Article/details/gwsiejfjj.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.hesvh.cn/Article/details/gwhjtmffm.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/guawbeudo.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.hesvh.cn/Article/details/gjvhgfssa.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gwdcujepy.sHtML

[D01] 创建数组 / 列表
来源：http://wap.zdbjq.cn/Article/details/ghwxdiouc.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.hesvh.cn/Article/details/gvbbuylqj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.hesvh.cn/Article/details/glqnosanm.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.zdbjq.cn/Article/details/gsvszquxp.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.hesvh.cn/Article/details/gqabgxfrx.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.zdbjq.cn/Article/details/gczklhnlv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.fehbvm.com/Article/details/grwxqsmfx.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.zdbjq.cn/Article/details/ghucjgbng.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.fehbvm.com/Article/details/ghctmahtd.sHtML

[D02] 追加元素到末尾
来源：http://wap.hesvh.cn/Article/details/gpshbrgxw.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.hesvh.cn/Article/details/ggclfkzgr.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.zdbjq.cn/Article/details/gsvpqdrdn.sHtML

JS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/gqqcktyyw.sHtML

TS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/gyohbxdmp.sHtML

Java: list.add(4);
来源：http://mobile.zdbjq.cn/Article/details/giiumdomf.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.hesvh.cn/Article/details/gcyzbyrzi.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.hesvh.cn/Article/details/gonrgbikg.sHtML

C#:   list.Add(4);
来源：http://m.share.zdbjq.cn/Article/details/gbgitazvt.sHtML

[D03] 在指定位置插入元素
来源：http://blog.zdbjq.cn/Article/details/gdldadvdb.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fehbvm.com/Article/details/ggsydabcf.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.hesvh.cn/Article/details/gsiumitze.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.fehbvm.com/Article/details/gsbsjjqxa.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gxgezvmea.sHtML

Java: list.add(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/grjyosbps.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.hesvh.cn/Article/details/gqrjkroiu.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.zdbjq.cn/Article/details/ggkwnjdap.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.fehbvm.com/Article/details/gmhswrcyc.sHtML

[D04] 删除元素
来源：http://m.share.zdbjq.cn/Article/details/gikdnugvi.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.hesvh.cn/Article/details/gskalular.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.zdbjq.cn/Article/details/gdtovjogq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.hesvh.cn/Article/details/gnlmmzhyr.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.fehbvm.com/Article/details/gcdiijwvj.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.hesvh.cn/Article/details/gtndfzuyg.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.zdbjq.cn/Article/details/gnnsbdlbl.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.fehbvm.com/Article/details/gvunfdkdx.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.zdbjq.cn/Article/details/gvrmcfhpf.sHtML

[D05] 访问与修改元素
来源：http://read.share.zdbjq.cn/Article/details/gyywnpwer.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gxuvwhafz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gqkcauadg.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gbzuhvhez.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.hesvh.cn/Article/details/gbigrpqjt.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.fehbvm.com/Article/details/gtkujzjhc.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/ghlhfppqr.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gjsumydtt.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gssezznzn.sHtML

[D06] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gnptxgery.sHtML

Py:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gtradiehn.sHtML

PHP:  count($arr);
来源：http://m.share.fehbvm.com/Article/details/geereektb.sHtML

JS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gwkxhvoms.sHtML

TS:   arr.length
来源：http://3g.fehbvm.com/Article/details/gisfzamot.sHtML

Java: list.size();
来源：http://www.share.hesvh.cn/Article/details/gwdtefjqk.sHtML

Go:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gfwqilbev.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.fehbvm.com/Article/details/glccukxxj.sHtML

C#:   list.Count;
来源：http://blog.hesvh.cn/Article/details/gqlkbukwe.sHtML

[D07] 切片 / 取子数组
来源：http://3g.fehbvm.com/Article/details/gkwiglevg.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.zdbjq.cn/Article/details/gafbwbgqg.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fehbvm.com/Article/details/gwylvzbqb.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/grdsktiqf.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/gxwnjwqis.sHtML

Java: list.subList(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gurwimqga.sHtML

Go:   arr[1:4]
来源：http://read.share.fehbvm.com/Article/details/guzhqktve.sHtML

Ruby: arr[1, 3]
来源：http://3g.zdbjq.cn/Article/details/gbdtihhqj.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.fehbvm.com/Article/details/gznzybdys.sHtML

[D08] 合并两个数组
来源：http://3g.hesvh.cn/Article/details/gttksxysv.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.hesvh.cn/Article/details/gdsuhzqwz.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.zdbjq.cn/Article/details/gmrbybinj.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.hesvh.cn/Article/details/gtkwvukcu.sHtML

TS:   [...a, ...b];
来源：http://mobile.fehbvm.com/Article/details/gfjrugsca.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.fehbvm.com/Article/details/gzyztkewr.sHtML

Go:   append(a, b...)
来源：http://mobile.hesvh.cn/Article/details/gjqlaxrtp.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.zdbjq.cn/Article/details/gcfjfdzyw.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.zdbjq.cn/Article/details/gngvjcalk.sHtML

[D09] 排序（升序）
来源：http://www.blog.hesvh.cn/Article/details/gvvteeuzv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/gzyjcxywe.sHtML

PHP:  sort($arr);
来源：http://m.share.hesvh.cn/Article/details/gbaptfhsa.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.fehbvm.com/Article/details/gskdirqny.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.zdbjq.cn/Article/details/gxzqoeerf.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.hesvh.cn/Article/details/gzhgpnskr.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/girxgwuok.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/gbcuikfko.sHtML

C#:   list.Sort();
来源：http://m.share.fehbvm.com/Article/details/ghgmeuyke.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.fehbvm.com/Article/details/gnzpdurdj.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.zdbjq.cn/Article/details/gegrvaqed.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.zdbjq.cn/Article/details/gwvoisnmu.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/gcxturswh.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/gmfajfggd.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.hesvh.cn/Article/details/gyfibzxdj.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.fehbvm.com/Article/details/gxlizuuap.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.fehbvm.com/Article/details/gwsubuowc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.hesvh.cn/Article/details/grlqflolx.sHtML

[D11] 反转数组
来源：http://read.share.fehbvm.com/Article/details/grojviwmv.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.zdbjq.cn/Article/details/glgfezepo.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.hesvh.cn/Article/details/gcgtmqhvk.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.hesvh.cn/Article/details/ggynfxfcb.sHtML

TS:   [...arr].reverse();
来源：http://wap.fehbvm.com/Article/details/gbwuqafsq.sHtML

Java: Collections.reverse(list);
来源：http://mobile.hesvh.cn/Article/details/gscwcyilv.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.fehbvm.com/Article/details/ggvvwbmix.sHtML

Ruby: arr.reverse
来源：http://baike.hesvh.cn/Article/details/gkjhxwhge.sHtML

C#:   list.Reverse();
来源：http://baike.zdbjq.cn/Article/details/geyhasurf.sHtML

[D12] 查找元素下标
来源：http://mobile.hesvh.cn/Article/details/gfxtqhzgx.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.hesvh.cn/Article/details/gghndbovb.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.fehbvm.com/Article/details/glvaceglc.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/gdtecxnmb.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/gisbeaypu.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.hesvh.cn/Article/details/gncglxhtb.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gupfwkhaf.sHtML

Ruby: arr.index(x)
来源：http://www.share.fehbvm.com/Article/details/grhobpdxo.sHtML

C#:   list.IndexOf(x);
来源：http://baike.zdbjq.cn/Article/details/gvexxsxic.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.hesvh.cn/Article/details/gqyzwlulv.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.hesvh.cn/Article/details/getztwrhi.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.hesvh.cn/Article/details/gumtjikog.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/godlbymfo.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/guuxxdbyd.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.hesvh.cn/Article/details/gaphtzreg.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.hesvh.cn/Article/details/gaehlhsdn.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.zdbjq.cn/Article/details/gfjlikdty.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gpiikfqhs.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.hesvh.cn/Article/details/gryclmnrz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.zdbjq.cn/Article/details/gnzfgmdgo.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.zdbjq.cn/Article/details/gopfxmjrr.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/gjxgmbegh.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gjyffjyvd.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/ghnylytlv.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/gdxwkgbzh.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gdseywtmt.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.fehbvm.com/Article/details/gbjtsvudo.sHtML

[D15] 去重
来源：http://blog.hesvh.cn/Article/details/gkwwlazdm.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/gpebfjpzz.sHtML

PHP:  array_unique($arr);
来源：http://3g.zdbjq.cn/Article/details/gogacqygm.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gemrpbcjh.sHtML

TS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gsmpkwvlk.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.fehbvm.com/Article/details/gohecrkfc.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.fehbvm.com/Article/details/gkeqnluey.sHtML

Ruby: arr.uniq
来源：http://mobile.fehbvm.com/Article/details/gtcppmdyn.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.zdbjq.cn/Article/details/gxnwjdfts.sHtML

[D16] 求和与平均值
来源：http://baike.hesvh.cn/Article/details/gadxnjjew.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.zdbjq.cn/Article/details/gsuvbdrnx.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.hesvh.cn/Article/details/gjyfbclme.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/gmtipnswa.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/ggihbkfbk.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.hesvh.cn/Article/details/gflkqdxbc.sHtML

Go:   // 手写循环累加
来源：http://3g.zdbjq.cn/Article/details/gsexufqhs.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.zdbjq.cn/Article/details/gbptwdddc.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.zdbjq.cn/Article/details/grxejlucz.sHtML

[D17] 最大值与最小值
来源：http://wap.hesvh.cn/Article/details/geugtopzo.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.hesvh.cn/Article/details/gmbedbeib.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.fehbvm.com/Article/details/gwwgfngob.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.hesvh.cn/Article/details/gqpcskwnr.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.hesvh.cn/Article/details/gilhxkizu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.zdbjq.cn/Article/details/gsezfckvp.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gmxdfbemp.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.zdbjq.cn/Article/details/guaimivet.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.fehbvm.com/Article/details/gydxqzqfb.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.fehbvm.com/Article/details/gmirjtcio.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.hesvh.cn/Article/details/gdnhfizhb.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.hesvh.cn/Article/details/gmlhgtoyi.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.zdbjq.cn/Article/details/gkkyvlehq.sHtML

TS:   nested.flat();
来源：http://blog.zdbjq.cn/Article/details/glvcdmxgi.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.fehbvm.com/Article/details/gfouippia.sHtML

Go:   // 手写双层循环
来源：http://mobile.fehbvm.com/Article/details/gahrawdan.sHtML

Ruby: nested.flatten
来源：http://baike.fehbvm.com/Article/details/gqhqkmpgt.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.fehbvm.com/Article/details/gxeqsjnqc.sHtML

[D19] 按字段分组
来源：http://www.share.zdbjq.cn/Article/details/gyiyizcnu.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.fehbvm.com/Article/details/gcwztaclw.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.fehbvm.com/Article/details/grvmczfxa.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.zdbjq.cn/Article/details/gktqsfklt.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.fehbvm.com/Article/details/gkbnsslzh.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.hesvh.cn/Article/details/geuvvkrbv.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.fehbvm.com/Article/details/grmgkjqiq.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.hesvh.cn/Article/details/gxzdxmiym.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.hesvh.cn/Article/details/goaaupine.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.zdbjq.cn/Article/details/giwffrduy.sHtML

Py:   Counter(arr)
来源：http://www.blog.fehbvm.com/Article/details/ghhcwgekz.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.zdbjq.cn/Article/details/glrqxfmrd.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/getfonpvj.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/gmumhalkx.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.hesvh.cn/Article/details/gkvaznqav.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.zdbjq.cn/Article/details/ggwzcnmwo.sHtML

Ruby: arr.tally
来源：http://m.share.fehbvm.com/Article/details/gyzavnyrj.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.zdbjq.cn/Article/details/glgtqwcce.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.hesvh.cn/Article/details/gxkqzstag.sHtML

Py:   x in arr
来源：http://www.m.share.hesvh.cn/Article/details/gsjkpayaf.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.zdbjq.cn/Article/details/gymuwljsw.sHtML

JS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/glyojssxc.sHtML

TS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/grtonnuhu.sHtML

Java: list.contains(x)
来源：http://baike.zdbjq.cn/Article/details/gakfmzryw.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gxvjbyrwe.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.hesvh.cn/Article/details/gtjvqfgfm.sHtML

C#:   list.Contains(x)
来源：http://wap.fehbvm.com/Article/details/gxlwssupv.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.hesvh.cn/Article/details/gkmhiwhbb.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.zdbjq.cn/Article/details/gedwniksp.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.zdbjq.cn/Article/details/guspibbnj.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gpviijrpg.sHtML

TS:   [...arr];
来源：http://3g.zdbjq.cn/Article/details/glyglvgor.sHtML

Java: new ArrayList<>(list);
来源：http://baike.hesvh.cn/Article/details/gyysqgvpo.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.hesvh.cn/Article/details/gpeszazqx.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.hesvh.cn/Article/details/gxtnxndtn.sHtML

C#:   new List<int>(list);
来源：http://mobile.hesvh.cn/Article/details/gqgywdgib.sHtML

[D23] reduce 累积计算
来源：http://read.share.zdbjq.cn/Article/details/ggjfzcaam.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.zdbjq.cn/Article/details/gvkyghhoy.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.fehbvm.com/Article/details/gnzvbowug.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/ggmycoivq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/guieajylb.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.hesvh.cn/Article/details/gdikwmfgq.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/ghyydzgaq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.hesvh.cn/Article/details/grbklhjgi.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.zdbjq.cn/Article/details/gesonwhuf.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.hesvh.cn/Article/details/gfupahmeu.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.fehbvm.com/Article/details/gkgpcbpqe.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.fehbvm.com/Article/details/gagscnkke.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.fehbvm.com/Article/details/gpjhnjnye.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gxiubunsl.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.zdbjq.cn/Article/details/gfzjnmndp.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.fehbvm.com/Article/details/ghccreqri.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.zdbjq.cn/Article/details/giorrwyzg.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.zdbjq.cn/Article/details/ghfrjixes.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.zdbjq.cn/Article/details/gosbljxmm.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.zdbjq.cn/Article/details/gpnhzpgmq.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.zdbjq.cn/Article/details/gxojrrzif.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.zdbjq.cn/Article/details/grisxacrk.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.zdbjq.cn/Article/details/gelpyytiy.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.zdbjq.cn/Article/details/gvmriaofa.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.hesvh.cn/Article/details/gwcidwsqu.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.zdbjq.cn/Article/details/gsktkicyr.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.zdbjq.cn/Article/details/gleiujywa.sHtML

[D26] 数组转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gwoaikcni.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.zdbjq.cn/Article/details/glxhuflyh.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.hesvh.cn/Article/details/gtkeawcgt.sHtML

JS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/giuygpfha.sHtML

TS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gompcfrjg.sHtML

Java: String.join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/gxwqpvmsm.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gzjurlmav.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gzijvqwsd.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gemnebnfv.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/grfuxuolx.sHtML

E. 字符串处理
来源：http://wap.fehbvm.com/Article/details/gtvrsvemn.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gpyxxndjp.sHtML

[E01] 拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gruoagmgo.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.hesvh.cn/Article/details/gyvlbslvg.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.fehbvm.com/Article/details/gzzajlulq.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/ggorikhaq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fehbvm.com/Article/details/gmnkmpjbo.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.hesvh.cn/Article/details/gqvzyahsk.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.zdbjq.cn/Article/details/gpkgqqkjx.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.zdbjq.cn/Article/details/giodujuvk.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/ghnapkdzh.sHtML

[E02] 重复字符串
来源：http://read.share.hesvh.cn/Article/details/gezxejawm.sHtML

Py:   "ab" * 3
来源：http://wap.hesvh.cn/Article/details/ghrpokwyt.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.fehbvm.com/Article/details/gxovedgze.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/goqntewnt.sHtML


<!-- 参考信息 -->