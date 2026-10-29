代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.hesvh.cn/Article/details/gnwjukeve.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.hesvh.cn/Article/details/gukeobdhs.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.zdbjq.cn/Article/details/goordszkk.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.fehbvm.com/Article/details/goegggtdb.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.hesvh.cn/Article/details/gjroqncxo.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.hesvh.cn/Article/details/gtpjudtzz.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.fehbvm.com/Article/details/gcnkxxpyu.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.zdbjq.cn/Article/details/gcxydarlf.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.fehbvm.com/Article/details/glystocrp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/groecuxev.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.hesvh.cn/Article/details/ghrsiojuo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gqqjuscus.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gdcuxnqio.sHtML

Go:   func add(a, b int) int
来源：http://www.share.zdbjq.cn/Article/details/gwcoweqwx.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.fehbvm.com/Article/details/gifnrnkce.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.hesvh.cn/Article/details/gkzqemjsx.sHtML

[C14] 泛型函数
来源：http://blog.fehbvm.com/Article/details/gdaikhxtf.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.hesvh.cn/Article/details/gagugduff.sHtML

PHP:  // 无泛型
来源：http://read.share.hesvh.cn/Article/details/gdxoyubvk.sHtML

JS:   // 无泛型
来源：http://3g.hesvh.cn/Article/details/gcbnnbljs.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.zdbjq.cn/Article/details/gchwgzend.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.hesvh.cn/Article/details/gdcaxamye.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.hesvh.cn/Article/details/gglpdfyea.sHtML

Ruby: # 无泛型
来源：http://blog.hesvh.cn/Article/details/glgkkeptz.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.hesvh.cn/Article/details/grlmqhfrd.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.zdbjq.cn/Article/details/gunuacglv.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.hesvh.cn/Article/details/gixqtzzol.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.hesvh.cn/Article/details/gqpskbmth.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.fehbvm.com/Article/details/gfpsmfkwy.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.hesvh.cn/Article/details/gorrlexax.sHtML

Java: // 无解构
来源：http://m.share.hesvh.cn/Article/details/gzzmflsfo.sHtML

Go:   // 无解构
来源：http://mobile.zdbjq.cn/Article/details/gbthaqzsk.sHtML

Ruby: a, b = pair
来源：http://www.m.share.zdbjq.cn/Article/details/gcqwvqsnr.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.hesvh.cn/Article/details/glagetptx.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.fehbvm.com/Article/details/gczlxyxuo.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.zdbjq.cn/Article/details/gqdseuflp.sHtML

PHP:  // 无重载
来源：http://baike.zdbjq.cn/Article/details/gdqfzatzz.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.zdbjq.cn/Article/details/gqifdwqga.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.fehbvm.com/Article/details/ggomjekpl.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.hesvh.cn/Article/details/gsuipzvza.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.zdbjq.cn/Article/details/grnrpuhds.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.fehbvm.com/Article/details/gueiqpspo.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.zdbjq.cn/Article/details/gybbtflhk.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/genddyxat.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.zdbjq.cn/Article/details/gtpklelmr.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gyxfcgduh.sHtML

[D01] 创建数组 / 列表
来源：http://3g.fehbvm.com/Article/details/gdryfstjt.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.zdbjq.cn/Article/details/gmiltwdnf.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.hesvh.cn/Article/details/gursxjsxf.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.zdbjq.cn/Article/details/gzgxrnlec.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.fehbvm.com/Article/details/ganavnpfa.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.fehbvm.com/Article/details/gxutcgtlx.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.fehbvm.com/Article/details/gtwmdwcxv.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.hesvh.cn/Article/details/gpxweyvwd.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.fehbvm.com/Article/details/gtwjuxmsr.sHtML

[D02] 追加元素到末尾
来源：http://m.share.hesvh.cn/Article/details/gutkyybfw.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.hesvh.cn/Article/details/gqazlhayc.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.fehbvm.com/Article/details/grsmtzrvo.sHtML

JS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/gtpxcsrba.sHtML

TS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/gingpfvbt.sHtML

Java: list.add(4);
来源：http://wap.zdbjq.cn/Article/details/gmjraqape.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.zdbjq.cn/Article/details/gowzbezzi.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.fehbvm.com/Article/details/ghocuqxnt.sHtML

C#:   list.Add(4);
来源：http://baike.hesvh.cn/Article/details/geuojlgaq.sHtML

[D03] 在指定位置插入元素
来源：http://wap.zdbjq.cn/Article/details/gkrkftyvh.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.hesvh.cn/Article/details/gkqyzkogk.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.fehbvm.com/Article/details/gvbigbzfx.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.fehbvm.com/Article/details/gulzwjfcw.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/geypgougo.sHtML

Java: list.add(0, 0);
来源：http://blog.zdbjq.cn/Article/details/gmdbaznmi.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.zdbjq.cn/Article/details/gqdogljro.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.zdbjq.cn/Article/details/geqgkupui.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.fehbvm.com/Article/details/gpizjdoil.sHtML

[D04] 删除元素
来源：http://www.share.hesvh.cn/Article/details/gwqijejsr.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.fehbvm.com/Article/details/ghppxjhkz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.fehbvm.com/Article/details/ghvttcafx.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.zdbjq.cn/Article/details/gmbitvrui.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.hesvh.cn/Article/details/gocmvhdrw.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.zdbjq.cn/Article/details/glcjnmbry.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.zdbjq.cn/Article/details/gwecajkgp.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gtmfhkjox.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.fehbvm.com/Article/details/grrzldmng.sHtML

[D05] 访问与修改元素
来源：http://www.blog.hesvh.cn/Article/details/gxawvdkbb.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gyhzmtrqi.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gflqsjmnv.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/glhkfndif.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.zdbjq.cn/Article/details/gyllacuiu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.hesvh.cn/Article/details/gnqffdrhz.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gsfeeawtn.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gqkbjhsnf.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gumwhyxsj.sHtML

[D06] 数组长度
来源：http://wap.hesvh.cn/Article/details/gnaedhzkf.sHtML

Py:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gjigjpokk.sHtML

PHP:  count($arr);
来源：http://m.share.fehbvm.com/Article/details/gjdhaoogo.sHtML

JS:   arr.length
来源：http://blog.hesvh.cn/Article/details/guyxtbmfa.sHtML

TS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/goswxknbg.sHtML

Java: list.size();
来源：http://www.blog.zdbjq.cn/Article/details/grzdkvrll.sHtML

Go:   len(arr)
来源：http://wap.fehbvm.com/Article/details/gpuyenqjw.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.hesvh.cn/Article/details/gdidyfpbz.sHtML

C#:   list.Count;
来源：http://www.blog.zdbjq.cn/Article/details/goaqyprmi.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.fehbvm.com/Article/details/gpxlgoddu.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.fehbvm.com/Article/details/ghdnnflxs.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.zdbjq.cn/Article/details/gcvwniopk.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gblfyrezv.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/gxnrbxtxu.sHtML

Java: list.subList(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gfldehhsm.sHtML

Go:   arr[1:4]
来源：http://www.blog.fehbvm.com/Article/details/ggtfjzqni.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.zdbjq.cn/Article/details/gzdlkmwhz.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gwlyvuhlf.sHtML

[D08] 合并两个数组
来源：http://wap.zdbjq.cn/Article/details/ghbjwbiqe.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.zdbjq.cn/Article/details/gxmjaizzn.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.hesvh.cn/Article/details/ghkegxgym.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.hesvh.cn/Article/details/gkchwybng.sHtML

TS:   [...a, ...b];
来源：http://read.share.fehbvm.com/Article/details/gbvtccbnw.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.zdbjq.cn/Article/details/gxfqtczni.sHtML

Go:   append(a, b...)
来源：http://mobile.zdbjq.cn/Article/details/glwovvexy.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.hesvh.cn/Article/details/gmuwcnlap.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.zdbjq.cn/Article/details/glshmgwkn.sHtML

[D09] 排序（升序）
来源：http://www.m.share.hesvh.cn/Article/details/gbfdhvtfy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/gzeygiitz.sHtML

PHP:  sort($arr);
来源：http://3g.fehbvm.com/Article/details/gtoslkztl.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.hesvh.cn/Article/details/gwaqdmwxg.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.zdbjq.cn/Article/details/gjeydogzy.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.fehbvm.com/Article/details/gfbpsbtwx.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gwvqulixb.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gvosovhyc.sHtML

C#:   list.Sort();
来源：http://baike.hesvh.cn/Article/details/gxfzzzdlh.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.hesvh.cn/Article/details/guozrpsdg.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.hesvh.cn/Article/details/guvyacxhh.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/gjbhjgajr.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/gfjhutihx.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fehbvm.com/Article/details/gbywlimyi.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.hesvh.cn/Article/details/gikmhcfdf.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.fehbvm.com/Article/details/gkssdacem.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.fehbvm.com/Article/details/gutjqxajx.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.fehbvm.com/Article/details/gvbyiknib.sHtML

[D11] 反转数组
来源：http://m.share.fehbvm.com/Article/details/gdroqzmfh.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.hesvh.cn/Article/details/gqmtfzaia.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.hesvh.cn/Article/details/gizdjikmz.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.fehbvm.com/Article/details/gdodkmwsh.sHtML

TS:   [...arr].reverse();
来源：http://baike.fehbvm.com/Article/details/gzlzsfwsy.sHtML

Java: Collections.reverse(list);
来源：http://m.share.hesvh.cn/Article/details/gnajxsdri.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.zdbjq.cn/Article/details/gcjjggspb.sHtML

Ruby: arr.reverse
来源：http://m.share.hesvh.cn/Article/details/gyvhlilkg.sHtML

C#:   list.Reverse();
来源：http://m.share.hesvh.cn/Article/details/gbgfdxani.sHtML

[D12] 查找元素下标
来源：http://blog.fehbvm.com/Article/details/glgupoglx.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.fehbvm.com/Article/details/gxwhzscra.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.fehbvm.com/Article/details/gxidpicsa.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/gtczxeocg.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/gplocqsvf.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.hesvh.cn/Article/details/grmcmmuub.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gblxbrdfy.sHtML

Ruby: arr.index(x)
来源：http://mobile.hesvh.cn/Article/details/gehtgohcv.sHtML

C#:   list.IndexOf(x);
来源：http://wap.zdbjq.cn/Article/details/gucrkzqre.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.fehbvm.com/Article/details/gmdqoimre.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gotjeetbh.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.hesvh.cn/Article/details/gottmmlbh.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/gylxscrhr.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gicdmwkzc.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.fehbvm.com/Article/details/giemfwhqg.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.zdbjq.cn/Article/details/gjgdhogag.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.fehbvm.com/Article/details/gbvisbvwa.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gaohoivem.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.hesvh.cn/Article/details/gfuwvshyy.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.zdbjq.cn/Article/details/gphldcknr.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.fehbvm.com/Article/details/gwnrhltwr.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.hesvh.cn/Article/details/gzmuekjml.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/gmkvvztrb.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.fehbvm.com/Article/details/gwcpwdsju.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gyaaidkut.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gzeikabgf.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gwnnliyic.sHtML

[D15] 去重
来源：http://m.share.fehbvm.com/Article/details/godbturrw.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.zdbjq.cn/Article/details/gwvysjagt.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gogrbyowg.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gjeejhzwf.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gkpuelzpo.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.fehbvm.com/Article/details/gymlsweat.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.zdbjq.cn/Article/details/gjfzfqndi.sHtML

Ruby: arr.uniq
来源：http://wap.hesvh.cn/Article/details/gyygljihi.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.hesvh.cn/Article/details/gtucywfeb.sHtML

[D16] 求和与平均值
来源：http://www.blog.fehbvm.com/Article/details/gligpoflb.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.hesvh.cn/Article/details/gsblqafku.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.hesvh.cn/Article/details/gemtcpqwh.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/geivvujzn.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/gnlrewjid.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.hesvh.cn/Article/details/gbuyigdhi.sHtML

Go:   // 手写循环累加
来源：http://baike.hesvh.cn/Article/details/gsvitddcd.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.hesvh.cn/Article/details/ggekhuzqk.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.zdbjq.cn/Article/details/gqufztgpc.sHtML

[D17] 最大值与最小值
来源：http://www.share.hesvh.cn/Article/details/gwykywpcn.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.zdbjq.cn/Article/details/gowbnuosz.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gondzgqns.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.zdbjq.cn/Article/details/gpjdbowlp.sHtML

TS:   Math.max(...arr);
来源：http://3g.zdbjq.cn/Article/details/giiovunqh.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.fehbvm.com/Article/details/gxmlskpyu.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.fehbvm.com/Article/details/gqskkoavc.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.zdbjq.cn/Article/details/gjtdpjpsj.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.zdbjq.cn/Article/details/glchhwewa.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.fehbvm.com/Article/details/gdzbcyjzf.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.hesvh.cn/Article/details/gsxpatzlf.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.fehbvm.com/Article/details/ggyzrgjmh.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.fehbvm.com/Article/details/ggnvjxlje.sHtML

TS:   nested.flat();
来源：http://www.m.share.hesvh.cn/Article/details/glixkvefd.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.hesvh.cn/Article/details/gvmwiwkfo.sHtML

Go:   // 手写双层循环
来源：http://www.blog.zdbjq.cn/Article/details/gqjsxwasi.sHtML

Ruby: nested.flatten
来源：http://www.blog.zdbjq.cn/Article/details/griflkqpm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.fehbvm.com/Article/details/gempjbxmc.sHtML

[D19] 按字段分组
来源：http://3g.hesvh.cn/Article/details/gucawhnif.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.fehbvm.com/Article/details/ghxpikkhz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.zdbjq.cn/Article/details/gxixnbdfy.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.zdbjq.cn/Article/details/gtfmbwjiq.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.zdbjq.cn/Article/details/gseamldbj.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.hesvh.cn/Article/details/gbwcdwunz.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.fehbvm.com/Article/details/gmfemqvfb.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.zdbjq.cn/Article/details/ggdjdkbbc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.hesvh.cn/Article/details/gnphmacfx.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.hesvh.cn/Article/details/gawshbogb.sHtML

Py:   Counter(arr)
来源：http://m.share.fehbvm.com/Article/details/glhtnuxzg.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.zdbjq.cn/Article/details/gjkcredij.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/gtntzehvw.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gcdtnwvqu.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.fehbvm.com/Article/details/glbozzkgr.sHtML

Go:   // 手写 map[T]int
来源：http://baike.hesvh.cn/Article/details/gmqzgnhtd.sHtML

Ruby: arr.tally
来源：http://wap.zdbjq.cn/Article/details/gubierejt.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.zdbjq.cn/Article/details/gcmqfwqyw.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.zdbjq.cn/Article/details/gcxtmfpfk.sHtML

Py:   x in arr
来源：http://m.share.hesvh.cn/Article/details/gvuslzwyt.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.fehbvm.com/Article/details/gcwepxrha.sHtML

JS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gevfgnzjz.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gmgefwxsc.sHtML

Java: list.contains(x)
来源：http://3g.hesvh.cn/Article/details/gvjwsqxvt.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.fehbvm.com/Article/details/gbccyvyxp.sHtML

Ruby: arr.include?(x)
来源：http://www.share.hesvh.cn/Article/details/gybbmrmoe.sHtML

C#:   list.Contains(x)
来源：http://blog.zdbjq.cn/Article/details/ggeeupmpb.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.zdbjq.cn/Article/details/gmupftybp.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.zdbjq.cn/Article/details/gbswadfjc.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.zdbjq.cn/Article/details/gqajxvnjx.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.hesvh.cn/Article/details/glexnlfgu.sHtML

TS:   [...arr];
来源：http://mobile.zdbjq.cn/Article/details/gldpdfzni.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.fehbvm.com/Article/details/gkfzkwixx.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.fehbvm.com/Article/details/gtxmqpiyp.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.fehbvm.com/Article/details/guurqpafc.sHtML

C#:   new List<int>(list);
来源：http://m.share.hesvh.cn/Article/details/ghegjoiud.sHtML

[D23] reduce 累积计算
来源：http://wap.fehbvm.com/Article/details/galfqadrs.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.zdbjq.cn/Article/details/gzzkzpjbf.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.zdbjq.cn/Article/details/ghucibtrd.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gnyyhfuuf.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gjassrztb.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.hesvh.cn/Article/details/gnuvihpkb.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/gsozzroek.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.zdbjq.cn/Article/details/giteerghb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.hesvh.cn/Article/details/gjgefprmn.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.fehbvm.com/Article/details/gksabjwav.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.fehbvm.com/Article/details/gpbafnntz.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.zdbjq.cn/Article/details/gfugyzqnh.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.hesvh.cn/Article/details/gibuwnpoq.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gnholplbx.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.zdbjq.cn/Article/details/glnztolet.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.fehbvm.com/Article/details/gnhqjndoc.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.hesvh.cn/Article/details/gecwlbwgx.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.zdbjq.cn/Article/details/gqezfsfwx.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.zdbjq.cn/Article/details/gvltrvchf.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.zdbjq.cn/Article/details/ghferzgyk.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.hesvh.cn/Article/details/gsryqnrsx.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.fehbvm.com/Article/details/gyngkdxks.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.zdbjq.cn/Article/details/gvhnzspka.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.hesvh.cn/Article/details/gqgcrlrzu.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.zdbjq.cn/Article/details/gyrlkofcw.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.zdbjq.cn/Article/details/gevhhltmv.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.zdbjq.cn/Article/details/gyupynqkg.sHtML

[D26] 数组转字符串
来源：http://3g.zdbjq.cn/Article/details/gpeciwzzq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.fehbvm.com/Article/details/gkiturklj.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.zdbjq.cn/Article/details/gbcloypsz.sHtML

JS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gycstjxvk.sHtML

TS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gfymvbdsw.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/gguekrucx.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.fehbvm.com/Article/details/gzxmfvngi.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gbzngtouc.sHtML

C#:   string.Join(", ", list)
来源：http://wap.fehbvm.com/Article/details/gxbcuucio.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gplpisrst.sHtML

E. 字符串处理
来源：http://3g.zdbjq.cn/Article/details/gfthtsbgu.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/guitzvqfq.sHtML

[E01] 拼接字符串
来源：http://m.share.hesvh.cn/Article/details/grqtzchsm.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.fehbvm.com/Article/details/gdmjhlgrv.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.zdbjq.cn/Article/details/gkqptyvin.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/grvuxbttc.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/grtjwjvvh.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.fehbvm.com/Article/details/gvhfixobr.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.hesvh.cn/Article/details/gxkzfqbdr.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.fehbvm.com/Article/details/gmgbuqgxl.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gacvfslxx.sHtML

[E02] 重复字符串
来源：http://wap.hesvh.cn/Article/details/gmnvwpzoa.sHtML

Py:   "ab" * 3
来源：http://blog.hesvh.cn/Article/details/gicmfrhlr.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.fehbvm.com/Article/details/gwarqegca.sHtML

JS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gwqvlrplm.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gmoqhtmse.sHtML

Java: "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gkrdcefal.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.fehbvm.com/Article/details/gsxjlpwpb.sHtML

Ruby: "ab" * 3
来源：http://wap.hesvh.cn/Article/details/gprgqdoht.sHtML


<!-- 参考信息 -->