代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://blog.zdbjq.cn/Article/details/gilktpame.sHtML

C#:   using System.Text;
来源：http://wap.fehbvm.com/Article/details/ghamuzlue.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.fehbvm.com/Article/details/ggzqsbfap.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.hesvh.cn/Article/details/glraeqjtu.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.hesvh.cn/Article/details/gypxxwaah.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.zdbjq.cn/Article/details/gqsaspryu.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.fehbvm.com/Article/details/gmvmigxqk.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.hesvh.cn/Article/details/gjjfiboxv.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.hesvh.cn/Article/details/gdfdnuiae.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.zdbjq.cn/Article/details/gcuehlcfm.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.hesvh.cn/Article/details/gomvuukiu.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.fehbvm.com/Article/details/gpjffncbs.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.zdbjq.cn/Article/details/gjwvscbct.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gdtrvazgz.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.hesvh.cn/Article/details/ggmuwnqjc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gdktxjqgn.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gpvbkcxkq.sHtML

Go:   func add(a, b int) int
来源：http://baike.hesvh.cn/Article/details/gvsyrnftw.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.fehbvm.com/Article/details/ghhlpvucl.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.hesvh.cn/Article/details/gucjzbhfo.sHtML

[C14] 泛型函数
来源：http://mobile.fehbvm.com/Article/details/gowflebst.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.fehbvm.com/Article/details/gjrhctsgl.sHtML

PHP:  // 无泛型
来源：http://baike.fehbvm.com/Article/details/gngqymlxy.sHtML

JS:   // 无泛型
来源：http://wap.zdbjq.cn/Article/details/golucuubv.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.zdbjq.cn/Article/details/gkihjdxfl.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.zdbjq.cn/Article/details/ggrdfmimy.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.zdbjq.cn/Article/details/ghtexvfah.sHtML

Ruby: # 无泛型
来源：http://blog.hesvh.cn/Article/details/grhawkumh.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.fehbvm.com/Article/details/gcyttfpji.sHtML

[C15] 解构 / 展开参数
来源：http://3g.hesvh.cn/Article/details/gluqebmcd.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.fehbvm.com/Article/details/gamzevpax.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.hesvh.cn/Article/details/gdwkbinxn.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.hesvh.cn/Article/details/gqqjdplbl.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.zdbjq.cn/Article/details/gatizchxg.sHtML

Java: // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gtcilqknv.sHtML

Go:   // 无解构
来源：http://read.share.hesvh.cn/Article/details/gufglyxwp.sHtML

Ruby: a, b = pair
来源：http://blog.fehbvm.com/Article/details/gmltfjyqt.sHtML

C#:   var (a, b) = pair;
来源：http://wap.fehbvm.com/Article/details/gtqdwbcjp.sHtML

[C16] 函数 / 方法重载
来源：http://3g.zdbjq.cn/Article/details/gqeyfuxef.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.fehbvm.com/Article/details/gdqydnbaw.sHtML

PHP:  // 无重载
来源：http://m.share.fehbvm.com/Article/details/gsamkgqkf.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.hesvh.cn/Article/details/gplbvasvu.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.fehbvm.com/Article/details/gkzholrtv.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.hesvh.cn/Article/details/gywmiixko.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.zdbjq.cn/Article/details/grqghgbgu.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.zdbjq.cn/Article/details/gnlcfywjm.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.fehbvm.com/Article/details/gfikdgeap.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gwcxxkzew.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.fehbvm.com/Article/details/goxxikklr.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/guwdfjwvz.sHtML

[D01] 创建数组 / 列表
来源：http://baike.fehbvm.com/Article/details/gqxifgmwg.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.zdbjq.cn/Article/details/gbeoglojw.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/gksfqrcsl.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/gyipffeie.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.zdbjq.cn/Article/details/gqhpnjeva.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.fehbvm.com/Article/details/gmtupgkwl.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.fehbvm.com/Article/details/gpfzzzvcg.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.zdbjq.cn/Article/details/gfwtducmy.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.fehbvm.com/Article/details/gdfnhuqtn.sHtML

[D02] 追加元素到末尾
来源：http://blog.zdbjq.cn/Article/details/ggqczdatw.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.zdbjq.cn/Article/details/gfqufweyp.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.hesvh.cn/Article/details/gerssblhs.sHtML

JS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/gshtbtrwn.sHtML

TS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/gxqvqjtox.sHtML

Java: list.add(4);
来源：http://blog.zdbjq.cn/Article/details/gthnptzif.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gevcgbbyd.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.hesvh.cn/Article/details/gvpvmwewq.sHtML

C#:   list.Add(4);
来源：http://read.share.zdbjq.cn/Article/details/goqsmvzvw.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.hesvh.cn/Article/details/gilhspirj.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gxrvacpfb.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.hesvh.cn/Article/details/gnjqlmjvu.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.zdbjq.cn/Article/details/gixbljmdz.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.zdbjq.cn/Article/details/gcqljbbvo.sHtML

Java: list.add(0, 0);
来源：http://wap.hesvh.cn/Article/details/gzmrobkgs.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.fehbvm.com/Article/details/gsdmqivqy.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.hesvh.cn/Article/details/gaxrglzif.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gejzmbfcw.sHtML

[D04] 删除元素
来源：http://m.share.zdbjq.cn/Article/details/gkejnikbt.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.zdbjq.cn/Article/details/gftsyxyyb.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.hesvh.cn/Article/details/gegzvpulp.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.hesvh.cn/Article/details/gpbncuqyo.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.zdbjq.cn/Article/details/gspltopcb.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.zdbjq.cn/Article/details/gfptrjomf.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.zdbjq.cn/Article/details/gwbckjsdh.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.zdbjq.cn/Article/details/gkctcqapd.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.zdbjq.cn/Article/details/gglwphpay.sHtML

[D05] 访问与修改元素
来源：http://3g.hesvh.cn/Article/details/gkreyyamo.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/glryuhdvj.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gauqpgybn.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gpgavfhqw.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.hesvh.cn/Article/details/gphplzamh.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.hesvh.cn/Article/details/gvzymubch.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/ggigsqrki.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gjprcktij.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gqdmiejtn.sHtML

[D06] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gcjsrvrst.sHtML

Py:   len(arr)
来源：http://wap.zdbjq.cn/Article/details/gbodwtavd.sHtML

PHP:  count($arr);
来源：http://3g.fehbvm.com/Article/details/gyvyxrwxg.sHtML

JS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gxkslamox.sHtML

TS:   arr.length
来源：http://blog.hesvh.cn/Article/details/gaivhzjum.sHtML

Java: list.size();
来源：http://www.share.hesvh.cn/Article/details/gjezqgneh.sHtML

Go:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gsuvrzsmj.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/ggyppcqhn.sHtML

C#:   list.Count;
来源：http://read.share.fehbvm.com/Article/details/gwfobmmpd.sHtML

[D07] 切片 / 取子数组
来源：http://3g.hesvh.cn/Article/details/gddrntkbv.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.hesvh.cn/Article/details/gsbtqzvxt.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.hesvh.cn/Article/details/gmxkqixky.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gkxlowbwh.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gkcezcclx.sHtML

Java: list.subList(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gpxtpzkop.sHtML

Go:   arr[1:4]
来源：http://mobile.fehbvm.com/Article/details/gzaulfeec.sHtML

Ruby: arr[1, 3]
来源：http://mobile.zdbjq.cn/Article/details/gbmupqbcb.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gjchubsot.sHtML

[D08] 合并两个数组
来源：http://www.share.fehbvm.com/Article/details/gjdewovpy.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.hesvh.cn/Article/details/gilleipzj.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.zdbjq.cn/Article/details/gslggukbr.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.fehbvm.com/Article/details/ggnbsmtjp.sHtML

TS:   [...a, ...b];
来源：http://m.share.fehbvm.com/Article/details/geivcircd.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.zdbjq.cn/Article/details/gyvmmtvgt.sHtML

Go:   append(a, b...)
来源：http://mobile.zdbjq.cn/Article/details/ghrsrhetg.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.hesvh.cn/Article/details/gmfsuhmie.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gomaipjzq.sHtML

[D09] 排序（升序）
来源：http://mobile.zdbjq.cn/Article/details/gfzsuhiuo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gyutbkjzv.sHtML

PHP:  sort($arr);
来源：http://blog.fehbvm.com/Article/details/gtyteocti.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.zdbjq.cn/Article/details/gibywrntn.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.fehbvm.com/Article/details/gqfvvyols.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.fehbvm.com/Article/details/gchxdqffa.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/gtcckfomf.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/gzegdpwvs.sHtML

C#:   list.Sort();
来源：http://read.share.zdbjq.cn/Article/details/gezszwhvv.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.hesvh.cn/Article/details/gdpfgvntd.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.zdbjq.cn/Article/details/gjwqcsjat.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/guiefxjsq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gfsqjwhtv.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.zdbjq.cn/Article/details/gpkkrjjth.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.hesvh.cn/Article/details/gxyokgnnb.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.zdbjq.cn/Article/details/gggsfujyv.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.hesvh.cn/Article/details/gulzhdpnl.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.fehbvm.com/Article/details/gpnktxqdb.sHtML

[D11] 反转数组
来源：http://read.share.hesvh.cn/Article/details/gzbrumnft.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.fehbvm.com/Article/details/gtxgwwwln.sHtML

PHP:  array_reverse($arr);
来源：http://blog.hesvh.cn/Article/details/ghrtocuwx.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.zdbjq.cn/Article/details/gqnuwszop.sHtML

TS:   [...arr].reverse();
来源：http://mobile.fehbvm.com/Article/details/grhhrhvre.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.fehbvm.com/Article/details/gchftemda.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.fehbvm.com/Article/details/gfsvlpndy.sHtML

Ruby: arr.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gcmzukrty.sHtML

C#:   list.Reverse();
来源：http://3g.hesvh.cn/Article/details/gotzlphmq.sHtML

[D12] 查找元素下标
来源：http://blog.zdbjq.cn/Article/details/gzmftpzom.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.hesvh.cn/Article/details/gdscipccp.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.hesvh.cn/Article/details/goilfxulz.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/gbetbrxrg.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/ghgzbrmjt.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.fehbvm.com/Article/details/gkyjzgfjo.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.fehbvm.com/Article/details/gsyggepje.sHtML

Ruby: arr.index(x)
来源：http://mobile.fehbvm.com/Article/details/ghfzvdpkm.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.fehbvm.com/Article/details/gvupmbfrm.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.zdbjq.cn/Article/details/galijhaxx.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.zdbjq.cn/Article/details/gttnurwms.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.fehbvm.com/Article/details/gzbwrpcht.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/ggwoirdnm.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/glrmfuydt.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.hesvh.cn/Article/details/gzlqofbso.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.zdbjq.cn/Article/details/gkcvhqiqz.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.fehbvm.com/Article/details/ginwfiloc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.fehbvm.com/Article/details/grivzoxao.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.fehbvm.com/Article/details/gnjxyuhnn.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gbzxwracs.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.hesvh.cn/Article/details/gxbcyshzf.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/gykxbdjax.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.hesvh.cn/Article/details/gkiihvbez.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gzhoufybb.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/gtadsssgu.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gtpzmftup.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/ginitimcp.sHtML

[D15] 去重
来源：http://3g.zdbjq.cn/Article/details/gchzrzkig.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.zdbjq.cn/Article/details/gzvbkhsmg.sHtML

PHP:  array_unique($arr);
来源：http://read.share.zdbjq.cn/Article/details/gsaxguure.sHtML

JS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gqxlaaotp.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gwtjwcfgf.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.fehbvm.com/Article/details/gugrckwwd.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.fehbvm.com/Article/details/gyfwifuik.sHtML

Ruby: arr.uniq
来源：http://m.share.fehbvm.com/Article/details/gzsgkzfml.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.hesvh.cn/Article/details/gumqtjplq.sHtML

[D16] 求和与平均值
来源：http://www.m.share.hesvh.cn/Article/details/gpsackynl.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gamtidlpz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.zdbjq.cn/Article/details/gsrxsgyvh.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gjehnarzf.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fehbvm.com/Article/details/givlrrvul.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.hesvh.cn/Article/details/goqrxftom.sHtML

Go:   // 手写循环累加
来源：http://3g.hesvh.cn/Article/details/gouhwhrmg.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.zdbjq.cn/Article/details/gkjadkkba.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.hesvh.cn/Article/details/gcfhkndwy.sHtML

[D17] 最大值与最小值
来源：http://baike.zdbjq.cn/Article/details/gkbfeucng.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.hesvh.cn/Article/details/gutrylpba.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.zdbjq.cn/Article/details/gflhcotxz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.fehbvm.com/Article/details/gsysmslly.sHtML

TS:   Math.max(...arr);
来源：http://blog.hesvh.cn/Article/details/gacdszgww.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.hesvh.cn/Article/details/germsffxw.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.zdbjq.cn/Article/details/gzdkoerew.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.hesvh.cn/Article/details/gsutyyscg.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.zdbjq.cn/Article/details/grtkpxapu.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.zdbjq.cn/Article/details/gmgkkbyad.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.fehbvm.com/Article/details/guivkgcru.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.fehbvm.com/Article/details/gtiyluaph.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.zdbjq.cn/Article/details/gdqdabpzi.sHtML

TS:   nested.flat();
来源：http://3g.fehbvm.com/Article/details/gqtjrlmym.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.fehbvm.com/Article/details/gzphrmlac.sHtML

Go:   // 手写双层循环
来源：http://blog.fehbvm.com/Article/details/gltjgbrzc.sHtML

Ruby: nested.flatten
来源：http://www.m.share.fehbvm.com/Article/details/gvhrxfdiv.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.fehbvm.com/Article/details/gjdsxnybc.sHtML

[D19] 按字段分组
来源：http://www.share.fehbvm.com/Article/details/grqtljiqt.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.zdbjq.cn/Article/details/ghjqjkhkx.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.hesvh.cn/Article/details/gwmivdsiy.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.fehbvm.com/Article/details/gppanlwxj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.hesvh.cn/Article/details/gqdgbdabv.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.hesvh.cn/Article/details/gezogpnbc.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.hesvh.cn/Article/details/gzpgknozu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.zdbjq.cn/Article/details/gbrithefs.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.fehbvm.com/Article/details/gwvxswfhm.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.fehbvm.com/Article/details/ghybacmwq.sHtML

Py:   Counter(arr)
来源：http://www.share.zdbjq.cn/Article/details/gjjcqavls.sHtML

PHP:  array_count_values($arr);
来源：http://blog.hesvh.cn/Article/details/gcbehogds.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.hesvh.cn/Article/details/gcmfxotxv.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/gonvdiwea.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.fehbvm.com/Article/details/gbzdjwpjb.sHtML

Go:   // 手写 map[T]int
来源：http://blog.fehbvm.com/Article/details/gxkzhrqmh.sHtML

Ruby: arr.tally
来源：http://read.share.zdbjq.cn/Article/details/gpcarduye.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.hesvh.cn/Article/details/gvyfgalxl.sHtML

[D21] 判断是否包含某元素
来源：http://blog.hesvh.cn/Article/details/gyejmedkf.sHtML

Py:   x in arr
来源：http://www.blog.zdbjq.cn/Article/details/gzrjmzbnu.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gmkcupxgk.sHtML

JS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/glxaepawt.sHtML

TS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/glkcmvwsp.sHtML

Java: list.contains(x)
来源：http://blog.zdbjq.cn/Article/details/gpypruwtg.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gazdybkpo.sHtML

Ruby: arr.include?(x)
来源：http://baike.zdbjq.cn/Article/details/gxmlsarks.sHtML

C#:   list.Contains(x)
来源：http://wap.fehbvm.com/Article/details/gesogssjz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.hesvh.cn/Article/details/gtokcctdx.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.zdbjq.cn/Article/details/gxewovrkj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.fehbvm.com/Article/details/gljwlcocf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.hesvh.cn/Article/details/gyccnlbql.sHtML

TS:   [...arr];
来源：http://blog.hesvh.cn/Article/details/gqswcypaa.sHtML

Java: new ArrayList<>(list);
来源：http://baike.hesvh.cn/Article/details/gewlkanys.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.hesvh.cn/Article/details/giohbnval.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.fehbvm.com/Article/details/gywghtbty.sHtML

C#:   new List<int>(list);
来源：http://m.share.fehbvm.com/Article/details/gftfmzoey.sHtML

[D23] reduce 累积计算
来源：http://mobile.fehbvm.com/Article/details/gfwdpqgmk.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.fehbvm.com/Article/details/ghhpfjjsl.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.hesvh.cn/Article/details/gplcqzalf.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gdvdsrzdp.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gnfxqdovj.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.zdbjq.cn/Article/details/glridvqrm.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/gprmecbpj.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.fehbvm.com/Article/details/guqddiwoc.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.zdbjq.cn/Article/details/gapskfrdq.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.fehbvm.com/Article/details/gksvjjikj.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.zdbjq.cn/Article/details/gbvsxuzke.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.zdbjq.cn/Article/details/gowpdbdfa.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.hesvh.cn/Article/details/gyhfcviga.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gybkikvhs.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gsogbdhjw.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.hesvh.cn/Article/details/gqwemxnmk.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.hesvh.cn/Article/details/gtcnbjywc.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.fehbvm.com/Article/details/gjufpzgbv.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.hesvh.cn/Article/details/gmjlbuvbh.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.zdbjq.cn/Article/details/glmklprja.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.zdbjq.cn/Article/details/gkhqsyxhw.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.zdbjq.cn/Article/details/gqdzjovng.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.hesvh.cn/Article/details/grgmjlipv.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.hesvh.cn/Article/details/ghiqlgesi.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.fehbvm.com/Article/details/gqysscfjf.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.fehbvm.com/Article/details/gsuiulmri.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.fehbvm.com/Article/details/gevboujhs.sHtML

[D26] 数组转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gmmnbkmch.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.fehbvm.com/Article/details/gwjlsylhr.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gllrganfl.sHtML

JS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/grqwowswf.sHtML

TS:   arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gxwvblvjd.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/gpysxpznj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.zdbjq.cn/Article/details/ggliruptc.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/ghvxorpke.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/gewxngqdz.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gkuriipif.sHtML

E. 字符串处理
来源：http://baike.hesvh.cn/Article/details/gyecllbxd.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gvjgfulyn.sHtML

[E01] 拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gguzohjds.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.hesvh.cn/Article/details/ghofgwrjs.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.fehbvm.com/Article/details/gqaracpbp.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/gwuevbhlq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fehbvm.com/Article/details/gjvkketkf.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.fehbvm.com/Article/details/gojhoexsl.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.hesvh.cn/Article/details/gcdsgqxgr.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.fehbvm.com/Article/details/gopchtjfb.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.fehbvm.com/Article/details/gkkdfddws.sHtML

[E02] 重复字符串
来源：http://mobile.zdbjq.cn/Article/details/geiodmhtn.sHtML

Py:   "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gbtjsdafu.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.fehbvm.com/Article/details/grxmawwsu.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gjsjstajw.sHtML


<!-- 参考信息 -->