代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://3g.zdbjq.cn/Article/details/gqhyrrzow.sHtML

C#:   using System.Text;
来源：http://www.m.share.fehbvm.com/Article/details/ghwulujyx.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.fehbvm.com/Article/details/glpsucgth.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.fehbvm.com/Article/details/gsevuoykh.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.zdbjq.cn/Article/details/gynagiacb.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.hesvh.cn/Article/details/gfegxeuwx.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.fehbvm.com/Article/details/gqblrivhg.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.zdbjq.cn/Article/details/ghbplrrll.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.zdbjq.cn/Article/details/gyfzefjuc.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.zdbjq.cn/Article/details/gqaqthqpu.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.fehbvm.com/Article/details/gopjgtxih.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.zdbjq.cn/Article/details/gyvlorotr.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.hesvh.cn/Article/details/gqfuzvfbv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/ghnvtpdvu.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.fehbvm.com/Article/details/gvwnodzmg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gplcecxsx.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gryalcpnt.sHtML

Go:   func add(a, b int) int
来源：http://mobile.hesvh.cn/Article/details/gfdfogpvn.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.fehbvm.com/Article/details/gejqsouam.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.hesvh.cn/Article/details/gbsgbkwet.sHtML

[C14] 泛型函数
来源：http://www.m.share.hesvh.cn/Article/details/ggnrfvwnn.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.fehbvm.com/Article/details/ghgtbungh.sHtML

PHP:  // 无泛型
来源：http://wap.fehbvm.com/Article/details/gfnpnggum.sHtML

JS:   // 无泛型
来源：http://read.share.fehbvm.com/Article/details/gfwknqiqd.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.hesvh.cn/Article/details/gpjvwwjag.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.fehbvm.com/Article/details/gakgzqhhl.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.fehbvm.com/Article/details/grvnosltf.sHtML

Ruby: # 无泛型
来源：http://m.share.hesvh.cn/Article/details/grwppsipv.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.fehbvm.com/Article/details/ggffsdsmb.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.fehbvm.com/Article/details/grvnrxeor.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.zdbjq.cn/Article/details/glqlfzqxk.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.hesvh.cn/Article/details/gzxuoyvef.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.fehbvm.com/Article/details/gxqlzcuti.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.zdbjq.cn/Article/details/gqilqoyul.sHtML

Java: // 无解构
来源：http://m.share.hesvh.cn/Article/details/gixmcmnyk.sHtML

Go:   // 无解构
来源：http://wap.fehbvm.com/Article/details/gesvifyoj.sHtML

Ruby: a, b = pair
来源：http://read.share.fehbvm.com/Article/details/gqfripcbw.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.fehbvm.com/Article/details/gajqbjkob.sHtML

[C16] 函数 / 方法重载
来源：http://blog.zdbjq.cn/Article/details/grquyuutq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.zdbjq.cn/Article/details/gphcbvase.sHtML

PHP:  // 无重载
来源：http://read.share.zdbjq.cn/Article/details/gwpkrjuwi.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.zdbjq.cn/Article/details/gwojtqqqr.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.hesvh.cn/Article/details/gyvwrtrqu.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.zdbjq.cn/Article/details/geipzddzp.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.fehbvm.com/Article/details/gyugshosn.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.fehbvm.com/Article/details/gyravwczb.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.hesvh.cn/Article/details/gzpjnwvni.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gnbagztei.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.fehbvm.com/Article/details/ggukfjjcf.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gywngshlj.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.fehbvm.com/Article/details/gajbtbdid.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.hesvh.cn/Article/details/gzaqdgcuv.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.zdbjq.cn/Article/details/gpbqnoejt.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.fehbvm.com/Article/details/glzocykmc.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.hesvh.cn/Article/details/gygnebjwp.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.fehbvm.com/Article/details/gdfnusiwz.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.fehbvm.com/Article/details/gesutazdt.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.zdbjq.cn/Article/details/gawkhazxq.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.hesvh.cn/Article/details/gvxnlunzt.sHtML

[D02] 追加元素到末尾
来源：http://mobile.zdbjq.cn/Article/details/glcxlyrjk.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.fehbvm.com/Article/details/gibdwjopc.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.zdbjq.cn/Article/details/guzzktvvv.sHtML

JS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/golxotqmi.sHtML

TS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/giqprzcfz.sHtML

Java: list.add(4);
来源：http://read.share.zdbjq.cn/Article/details/gtdpwgmym.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.fehbvm.com/Article/details/gbsghiein.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.hesvh.cn/Article/details/gieguqtdk.sHtML

C#:   list.Add(4);
来源：http://wap.hesvh.cn/Article/details/gsjcufbuf.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.zdbjq.cn/Article/details/gmfsazpmm.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.hesvh.cn/Article/details/ghsqrrgcq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.zdbjq.cn/Article/details/gjcenkrcv.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.fehbvm.com/Article/details/gjdymvkwe.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gxgewrqtr.sHtML

Java: list.add(0, 0);
来源：http://blog.hesvh.cn/Article/details/gnjnchskz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.fehbvm.com/Article/details/ghncozuwl.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.hesvh.cn/Article/details/gdaoquvmn.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gvdzaavym.sHtML

[D04] 删除元素
来源：http://blog.hesvh.cn/Article/details/gqmtttbjr.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gavzcmoim.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.hesvh.cn/Article/details/gxtvzwdpn.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.zdbjq.cn/Article/details/geokunrtg.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.zdbjq.cn/Article/details/glsqzidwe.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.hesvh.cn/Article/details/gphmbqcnn.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.hesvh.cn/Article/details/gerakeiom.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gsuxywyfi.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.hesvh.cn/Article/details/gmxtycydd.sHtML

[D05] 访问与修改元素
来源：http://m.share.fehbvm.com/Article/details/gpnkbumag.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gghldbsvk.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gpjrengaf.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gfebnwmpt.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.zdbjq.cn/Article/details/gkxbmlxyf.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.fehbvm.com/Article/details/gwgktnqxk.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gmykgvhyw.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/grydoyuxj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gsrfqcype.sHtML

[D06] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/gxuwctetm.sHtML

Py:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/grsusofoy.sHtML

PHP:  count($arr);
来源：http://baike.fehbvm.com/Article/details/gnmrasutp.sHtML

JS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/gcbycjwnh.sHtML

TS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gxjznccmx.sHtML

Java: list.size();
来源：http://mobile.fehbvm.com/Article/details/ghcxslktc.sHtML

Go:   len(arr)
来源：http://wap.fehbvm.com/Article/details/gtoptmixz.sHtML

Ruby: arr.length; arr.size
来源：http://3g.zdbjq.cn/Article/details/grrwusjlx.sHtML

C#:   list.Count;
来源：http://baike.zdbjq.cn/Article/details/gydysrgvo.sHtML

[D07] 切片 / 取子数组
来源：http://blog.hesvh.cn/Article/details/gxhxxmkpw.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.zdbjq.cn/Article/details/gzcthvbbr.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.zdbjq.cn/Article/details/gbxuskyxw.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gyxwzynvf.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/goefyzmpn.sHtML

Java: list.subList(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gqlldjtvy.sHtML

Go:   arr[1:4]
来源：http://3g.zdbjq.cn/Article/details/gdahcrfta.sHtML

Ruby: arr[1, 3]
来源：http://www.share.zdbjq.cn/Article/details/gmefecnpg.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.zdbjq.cn/Article/details/grksuesmc.sHtML

[D08] 合并两个数组
来源：http://blog.zdbjq.cn/Article/details/gyghqhpgu.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gpflaavyz.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.fehbvm.com/Article/details/geuwvejcd.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.zdbjq.cn/Article/details/gauxjwlqs.sHtML

TS:   [...a, ...b];
来源：http://baike.zdbjq.cn/Article/details/gfmspczwd.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.hesvh.cn/Article/details/gqlbbcled.sHtML

Go:   append(a, b...)
来源：http://www.m.share.hesvh.cn/Article/details/gklmdytbz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.fehbvm.com/Article/details/gspyxnskt.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.hesvh.cn/Article/details/ghbmzisvz.sHtML

[D09] 排序（升序）
来源：http://baike.fehbvm.com/Article/details/gqrpdvbwj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fehbvm.com/Article/details/gftfjrsoh.sHtML

PHP:  sort($arr);
来源：http://www.share.fehbvm.com/Article/details/gzogocpoy.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.fehbvm.com/Article/details/grybwcfrp.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.fehbvm.com/Article/details/ggdttthkf.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.hesvh.cn/Article/details/gawvbzrod.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gcrlhguqe.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/gcfmmjqcq.sHtML

C#:   list.Sort();
来源：http://wap.hesvh.cn/Article/details/giwhtgphd.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.fehbvm.com/Article/details/gjoscpepb.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.hesvh.cn/Article/details/gznjzjlwq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.hesvh.cn/Article/details/guqxdiwif.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/glulatuin.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/gtypczhqd.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.zdbjq.cn/Article/details/gflzuamop.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.zdbjq.cn/Article/details/gkhhhuucn.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.hesvh.cn/Article/details/gssxalhxx.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.hesvh.cn/Article/details/gnbaciowr.sHtML

[D11] 反转数组
来源：http://www.m.share.fehbvm.com/Article/details/gvjvwivau.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.fehbvm.com/Article/details/gfzubisea.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gqrtevtws.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.hesvh.cn/Article/details/gxjnkypgn.sHtML

TS:   [...arr].reverse();
来源：http://read.share.hesvh.cn/Article/details/gqpyjuzmp.sHtML

Java: Collections.reverse(list);
来源：http://3g.zdbjq.cn/Article/details/grcoorowt.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.fehbvm.com/Article/details/gixwjvshg.sHtML

Ruby: arr.reverse
来源：http://3g.zdbjq.cn/Article/details/gbvkmvoqn.sHtML

C#:   list.Reverse();
来源：http://3g.zdbjq.cn/Article/details/gqolvvfts.sHtML

[D12] 查找元素下标
来源：http://www.share.zdbjq.cn/Article/details/ghrewhvqq.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.zdbjq.cn/Article/details/gqlkcgugb.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.hesvh.cn/Article/details/gweagkkfa.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/gufabqybd.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/gtmjdszdc.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.hesvh.cn/Article/details/gryviyklb.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gkqaruupl.sHtML

Ruby: arr.index(x)
来源：http://read.share.hesvh.cn/Article/details/gjmysjcfh.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.fehbvm.com/Article/details/gcisywwzz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.fehbvm.com/Article/details/gjqlvcjki.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.zdbjq.cn/Article/details/gjyyabvfm.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.hesvh.cn/Article/details/gghiukpjz.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gbjnbnxye.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/gusbclnod.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.zdbjq.cn/Article/details/gwwspsdvr.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.zdbjq.cn/Article/details/ghtrjppfp.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.zdbjq.cn/Article/details/grwuncexi.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.fehbvm.com/Article/details/gtadkgulu.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.zdbjq.cn/Article/details/gqmqgidkw.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.fehbvm.com/Article/details/geapkysoe.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.fehbvm.com/Article/details/glxuyeflq.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/gspmtovgh.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/guhbywqam.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gzozhteub.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/gizecdmwr.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.fehbvm.com/Article/details/gyrinstjw.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.fehbvm.com/Article/details/gbyxmwndj.sHtML

[D15] 去重
来源：http://baike.zdbjq.cn/Article/details/getaxgptq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/gkllheyhl.sHtML

PHP:  array_unique($arr);
来源：http://m.share.zdbjq.cn/Article/details/gbipvgmce.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gtqmhhdrf.sHtML

TS:   [...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gucokiezs.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.hesvh.cn/Article/details/grkqxwqlr.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.fehbvm.com/Article/details/gidjpbocw.sHtML

Ruby: arr.uniq
来源：http://read.share.fehbvm.com/Article/details/gkyovptbf.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.fehbvm.com/Article/details/gtvsynvqv.sHtML

[D16] 求和与平均值
来源：http://baike.hesvh.cn/Article/details/ghisdbiya.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.fehbvm.com/Article/details/genyyikkl.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.zdbjq.cn/Article/details/gommeybsm.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/gxagwpsxh.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/ggynhyucx.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.hesvh.cn/Article/details/glbfkoehu.sHtML

Go:   // 手写循环累加
来源：http://www.share.fehbvm.com/Article/details/geporucny.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.hesvh.cn/Article/details/geiurxsbq.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.fehbvm.com/Article/details/gncmjbqza.sHtML

[D17] 最大值与最小值
来源：http://wap.zdbjq.cn/Article/details/grrurcwzi.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.hesvh.cn/Article/details/gxoogzcgm.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.fehbvm.com/Article/details/gxqhfbjac.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.hesvh.cn/Article/details/gkimopphe.sHtML

TS:   Math.max(...arr);
来源：http://m.share.fehbvm.com/Article/details/giiubanbd.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.zdbjq.cn/Article/details/gregcpahk.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.zdbjq.cn/Article/details/gspqtikri.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.fehbvm.com/Article/details/gnxypauss.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.hesvh.cn/Article/details/gfyavrgma.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.zdbjq.cn/Article/details/ggmxrayph.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.hesvh.cn/Article/details/gebwlcsvu.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.hesvh.cn/Article/details/ggdnvzltq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.zdbjq.cn/Article/details/gnaeeiydc.sHtML

TS:   nested.flat();
来源：http://wap.zdbjq.cn/Article/details/grsvlqgtq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.zdbjq.cn/Article/details/gmrlrpixs.sHtML

Go:   // 手写双层循环
来源：http://m.share.zdbjq.cn/Article/details/glkgjxilr.sHtML

Ruby: nested.flatten
来源：http://wap.zdbjq.cn/Article/details/gadzgkfdr.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.hesvh.cn/Article/details/ggeuztbdv.sHtML

[D19] 按字段分组
来源：http://www.share.hesvh.cn/Article/details/gxlqkuthg.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.fehbvm.com/Article/details/ggtqeflce.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.fehbvm.com/Article/details/gfrebzxup.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.hesvh.cn/Article/details/ggfefuzrs.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/gbycsplud.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.zdbjq.cn/Article/details/gpeyvlgry.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.zdbjq.cn/Article/details/gvnyhaune.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.hesvh.cn/Article/details/gvtcfmcin.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.zdbjq.cn/Article/details/gmvffaqpl.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.fehbvm.com/Article/details/gjwkcqpxn.sHtML

Py:   Counter(arr)
来源：http://wap.fehbvm.com/Article/details/gtdpwjfbi.sHtML

PHP:  array_count_values($arr);
来源：http://wap.zdbjq.cn/Article/details/gjtidsmjx.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fehbvm.com/Article/details/ggkhxovdw.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/gvjniwirq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.zdbjq.cn/Article/details/gpxmmatyn.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.fehbvm.com/Article/details/gdnkqmxyr.sHtML

Ruby: arr.tally
来源：http://wap.zdbjq.cn/Article/details/gmdcrffos.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.fehbvm.com/Article/details/gqttmozca.sHtML

[D21] 判断是否包含某元素
来源：http://baike.fehbvm.com/Article/details/guwwdforl.sHtML

Py:   x in arr
来源：http://www.blog.hesvh.cn/Article/details/goksmzkvg.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.zdbjq.cn/Article/details/gfydzbuok.sHtML

JS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/gtthlnxoh.sHtML

TS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/gtkzcswkx.sHtML

Java: list.contains(x)
来源：http://blog.hesvh.cn/Article/details/ghwomolvu.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gkmpeqbak.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gabfopyto.sHtML

C#:   list.Contains(x)
来源：http://wap.hesvh.cn/Article/details/grccswjlk.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.zdbjq.cn/Article/details/gljynbyoq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.hesvh.cn/Article/details/ggmuycogs.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.hesvh.cn/Article/details/grhyuhcdl.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.hesvh.cn/Article/details/ghobqmftw.sHtML

TS:   [...arr];
来源：http://www.m.share.zdbjq.cn/Article/details/guqdnhmvu.sHtML

Java: new ArrayList<>(list);
来源：http://3g.hesvh.cn/Article/details/gufkpnlzf.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.fehbvm.com/Article/details/gijpolteb.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.zdbjq.cn/Article/details/gvlrqhplo.sHtML

C#:   new List<int>(list);
来源：http://mobile.fehbvm.com/Article/details/gxnoghqkn.sHtML

[D23] reduce 累积计算
来源：http://www.blog.fehbvm.com/Article/details/gkdfbmpfs.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gexlpmcls.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.fehbvm.com/Article/details/gjthohqnt.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/gahgywbho.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.hesvh.cn/Article/details/gjsxofppi.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.fehbvm.com/Article/details/gogkxuimp.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/goezgrrck.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.hesvh.cn/Article/details/glbeiurnc.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.hesvh.cn/Article/details/gzrstytri.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.hesvh.cn/Article/details/gwfmeilyi.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.fehbvm.com/Article/details/gzinjaowd.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.fehbvm.com/Article/details/gwwfxdvuz.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.fehbvm.com/Article/details/gqjkwwqse.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gljdbctnb.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.fehbvm.com/Article/details/gldwfskyp.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.zdbjq.cn/Article/details/gprfkdmne.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.zdbjq.cn/Article/details/gfphqfwte.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.zdbjq.cn/Article/details/gnywqmcio.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.hesvh.cn/Article/details/gnsaagcga.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.hesvh.cn/Article/details/gtqruxcuz.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.zdbjq.cn/Article/details/gjuozyzpz.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.fehbvm.com/Article/details/gdbryhqam.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.fehbvm.com/Article/details/gwebteoyk.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.hesvh.cn/Article/details/gzmxhfrnk.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.hesvh.cn/Article/details/gseramwms.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.hesvh.cn/Article/details/ggccbavtq.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.fehbvm.com/Article/details/gngecgtrr.sHtML

[D26] 数组转字符串
来源：http://3g.zdbjq.cn/Article/details/gndgvbzvm.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.hesvh.cn/Article/details/gtvstzqia.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.zdbjq.cn/Article/details/ggvbjtsgx.sHtML

JS:   arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gmkcrtcfz.sHtML

TS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gdjllvtdv.sHtML

Java: String.join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gbhttateg.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.zdbjq.cn/Article/details/gnucfsubr.sHtML

Ruby: arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gsvxsvpak.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/gohsgtwij.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gftafknoi.sHtML

E. 字符串处理
来源：http://wap.fehbvm.com/Article/details/gdyphaeol.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gplzeueua.sHtML

[E01] 拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gqabtdkmt.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.fehbvm.com/Article/details/gmxkvowjj.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.hesvh.cn/Article/details/gjajayfrz.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fehbvm.com/Article/details/guhwxolgj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/giseoadyk.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.zdbjq.cn/Article/details/gheidnqqx.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.hesvh.cn/Article/details/ghgmredsg.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.hesvh.cn/Article/details/grrbaclbi.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gzqyiutsl.sHtML

[E02] 重复字符串
来源：http://mobile.zdbjq.cn/Article/details/ggufeuhez.sHtML

Py:   "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/gtnsggtqc.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.hesvh.cn/Article/details/gzrfcqbss.sHtML

JS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gtrlgteyc.sHtML


<!-- 参考信息 -->