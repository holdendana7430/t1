代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://mobile.fehbvm.com/Article/details/gllsycfew.sHtML

C#:   using System.Text;
来源：http://baike.zdbjq.cn/Article/details/grbvleyte.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.zdbjq.cn/Article/details/ggeipxnjr.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.hesvh.cn/Article/details/gxjgqxoum.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.hesvh.cn/Article/details/gqgyrkzho.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.zdbjq.cn/Article/details/gkxpbonnx.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.hesvh.cn/Article/details/gcuphyduv.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.zdbjq.cn/Article/details/gxgzgptjd.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.fehbvm.com/Article/details/gnjuiopuu.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.zdbjq.cn/Article/details/gljascrbf.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.hesvh.cn/Article/details/gpaajhbnt.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.hesvh.cn/Article/details/gzlvjzbeo.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.zdbjq.cn/Article/details/gezqfgcht.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/geqllfreh.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.zdbjq.cn/Article/details/gzyptdekj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gnylgjllr.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gywdktoox.sHtML

Go:   func add(a, b int) int
来源：http://baike.fehbvm.com/Article/details/grzlyyjpc.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.zdbjq.cn/Article/details/griuocjqe.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.zdbjq.cn/Article/details/gbkcjfczj.sHtML

[C14] 泛型函数
来源：http://www.m.share.hesvh.cn/Article/details/gdgkvozpn.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.zdbjq.cn/Article/details/gffewvmwh.sHtML

PHP:  // 无泛型
来源：http://wap.fehbvm.com/Article/details/gwrkpbcop.sHtML

JS:   // 无泛型
来源：http://read.share.hesvh.cn/Article/details/gtaeajxsa.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.hesvh.cn/Article/details/gfvprxmrs.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.hesvh.cn/Article/details/gdlamooxr.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.zdbjq.cn/Article/details/gariqmiwp.sHtML

Ruby: # 无泛型
来源：http://www.share.fehbvm.com/Article/details/gszddgvuj.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.zdbjq.cn/Article/details/gqqiendlh.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.fehbvm.com/Article/details/gotmskecy.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.zdbjq.cn/Article/details/gvjvonczy.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.hesvh.cn/Article/details/gpbvsvcou.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.zdbjq.cn/Article/details/gbhcqbnyn.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gfxokheie.sHtML

Java: // 无解构
来源：http://blog.zdbjq.cn/Article/details/gzzrqohoy.sHtML

Go:   // 无解构
来源：http://wap.fehbvm.com/Article/details/gichlbyom.sHtML

Ruby: a, b = pair
来源：http://www.m.share.fehbvm.com/Article/details/gphggkqzf.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.zdbjq.cn/Article/details/gqnykdwnx.sHtML

[C16] 函数 / 方法重载
来源：http://3g.zdbjq.cn/Article/details/gglxpdgse.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.hesvh.cn/Article/details/ggzvjpbzh.sHtML

PHP:  // 无重载
来源：http://3g.zdbjq.cn/Article/details/gppqvhfjh.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.zdbjq.cn/Article/details/gkvgaxgqw.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.fehbvm.com/Article/details/gxadedarw.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.zdbjq.cn/Article/details/gmuahrkwz.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.hesvh.cn/Article/details/grbcydewm.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.hesvh.cn/Article/details/ggekfnvxc.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.hesvh.cn/Article/details/grpvrkjex.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gvynrathz.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.fehbvm.com/Article/details/grnujswwr.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gwpyiqlyl.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.fehbvm.com/Article/details/gbcsfbedo.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.fehbvm.com/Article/details/gkisbxgzc.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.zdbjq.cn/Article/details/gvdmshnhm.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.fehbvm.com/Article/details/gcfklwokq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.hesvh.cn/Article/details/gubmlgrqr.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.zdbjq.cn/Article/details/gniypbhwn.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.hesvh.cn/Article/details/gvfbjaufo.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.hesvh.cn/Article/details/gvanqnlhv.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.zdbjq.cn/Article/details/gcculjyzf.sHtML

[D02] 追加元素到末尾
来源：http://m.share.hesvh.cn/Article/details/gzduckpfc.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.fehbvm.com/Article/details/gmlumclgu.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.fehbvm.com/Article/details/gnjvvcdrr.sHtML

JS:   arr.push(4);
来源：http://www.blog.hesvh.cn/Article/details/gkaezxapv.sHtML

TS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/gkbnmdzcp.sHtML

Java: list.add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gitgxpqjo.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.zdbjq.cn/Article/details/gxmbocfty.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.fehbvm.com/Article/details/gkshaqbcf.sHtML

C#:   list.Add(4);
来源：http://3g.fehbvm.com/Article/details/gnhbttpxr.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.hesvh.cn/Article/details/guuqikpsl.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.hesvh.cn/Article/details/grcncrylh.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.fehbvm.com/Article/details/gdzwbyvik.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.hesvh.cn/Article/details/gsfshujep.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gxiiyiiwb.sHtML

Java: list.add(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gkthgtlys.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.zdbjq.cn/Article/details/gvemwxddf.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.fehbvm.com/Article/details/gsmljshyc.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gblnwcpod.sHtML

[D04] 删除元素
来源：http://wap.hesvh.cn/Article/details/gijgbeobz.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.fehbvm.com/Article/details/grrzkgomk.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.zdbjq.cn/Article/details/glqhegvol.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.zdbjq.cn/Article/details/gbachboll.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.zdbjq.cn/Article/details/gpuncubnm.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.fehbvm.com/Article/details/gaatzxdxu.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.hesvh.cn/Article/details/ggimcdgux.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.fehbvm.com/Article/details/gemmstacv.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.zdbjq.cn/Article/details/geatnewqd.sHtML

[D05] 访问与修改元素
来源：http://3g.hesvh.cn/Article/details/gpyhdbufr.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/goebvfhog.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/girrlymwm.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gawchgjop.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.zdbjq.cn/Article/details/gjzqtruwr.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.zdbjq.cn/Article/details/gloczahms.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/grtjwwqmb.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gckhcpnvt.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gvxgoxghk.sHtML

[D06] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gsdtyqhfw.sHtML

Py:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/gqqzjgbrn.sHtML

PHP:  count($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gzqwrotkt.sHtML

JS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gbzyeyqbg.sHtML

TS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gokjaozfm.sHtML

Java: list.size();
来源：http://www.share.zdbjq.cn/Article/details/ghxpvewxq.sHtML

Go:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gwplwcklx.sHtML

Ruby: arr.length; arr.size
来源：http://blog.fehbvm.com/Article/details/gcielywpc.sHtML

C#:   list.Count;
来源：http://read.share.zdbjq.cn/Article/details/gtijerunm.sHtML

[D07] 切片 / 取子数组
来源：http://wap.zdbjq.cn/Article/details/gvbpajnla.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.zdbjq.cn/Article/details/gbwnigkrc.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.hesvh.cn/Article/details/gcpudhair.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gjlblvjtk.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/gchqjnalb.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gpzouywrr.sHtML

Go:   arr[1:4]
来源：http://www.share.zdbjq.cn/Article/details/gxwknljsi.sHtML

Ruby: arr[1, 3]
来源：http://blog.fehbvm.com/Article/details/gpjussoup.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.fehbvm.com/Article/details/gwctdnefd.sHtML

[D08] 合并两个数组
来源：http://wap.zdbjq.cn/Article/details/gbugcrevz.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.hesvh.cn/Article/details/gevksmgab.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.fehbvm.com/Article/details/ghjrbppai.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.fehbvm.com/Article/details/gxjuzqeuu.sHtML

TS:   [...a, ...b];
来源：http://blog.zdbjq.cn/Article/details/gxrtmhrsx.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.hesvh.cn/Article/details/gveqscmqk.sHtML

Go:   append(a, b...)
来源：http://baike.zdbjq.cn/Article/details/gswojseyj.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.hesvh.cn/Article/details/gynojxagb.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.zdbjq.cn/Article/details/glialcfjb.sHtML

[D09] 排序（升序）
来源：http://wap.zdbjq.cn/Article/details/gjrrllyzn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gubhuowrj.sHtML

PHP:  sort($arr);
来源：http://blog.fehbvm.com/Article/details/gsvusxirj.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.fehbvm.com/Article/details/gvbozspmm.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.hesvh.cn/Article/details/gshkwefld.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.zdbjq.cn/Article/details/gykdukxto.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.fehbvm.com/Article/details/gwewbives.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gonfmobap.sHtML

C#:   list.Sort();
来源：http://mobile.hesvh.cn/Article/details/gxemavepd.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.fehbvm.com/Article/details/gvvshvrjs.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.hesvh.cn/Article/details/gaezxxpks.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/gtfghadhs.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/gspcczfim.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gpkckhtsc.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.zdbjq.cn/Article/details/grdviwvru.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.fehbvm.com/Article/details/guajkatvc.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.zdbjq.cn/Article/details/goztbbosk.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.hesvh.cn/Article/details/gavdppuvj.sHtML

[D11] 反转数组
来源：http://blog.fehbvm.com/Article/details/gdmuvpjft.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.fehbvm.com/Article/details/gxdgkemmx.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.zdbjq.cn/Article/details/gwcwcodxy.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.zdbjq.cn/Article/details/gbxbsznlg.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.fehbvm.com/Article/details/gbzapcsii.sHtML

Java: Collections.reverse(list);
来源：http://baike.fehbvm.com/Article/details/geohawyul.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.fehbvm.com/Article/details/gmgurhfkz.sHtML

Ruby: arr.reverse
来源：http://baike.zdbjq.cn/Article/details/gbizeiqlr.sHtML

C#:   list.Reverse();
来源：http://blog.hesvh.cn/Article/details/gyakcpkag.sHtML

[D12] 查找元素下标
来源：http://blog.hesvh.cn/Article/details/gzftgwgkw.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.hesvh.cn/Article/details/gpmeqzwhu.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.zdbjq.cn/Article/details/gngxqbary.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/gezctvtnh.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gsevrypph.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.hesvh.cn/Article/details/glzcchrot.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gdevldexs.sHtML

Ruby: arr.index(x)
来源：http://read.share.hesvh.cn/Article/details/glpvexwyj.sHtML

C#:   list.IndexOf(x);
来源：http://wap.fehbvm.com/Article/details/gbhdzsfdp.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.hesvh.cn/Article/details/gdqdvsboz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.zdbjq.cn/Article/details/gaobzeoiw.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.zdbjq.cn/Article/details/gekfxrpbf.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/gqaxwxbix.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/gxtenkkyy.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.hesvh.cn/Article/details/gdozbncdo.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.zdbjq.cn/Article/details/gpwjtjqyk.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.hesvh.cn/Article/details/gycwcubvl.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.fehbvm.com/Article/details/gcfybilky.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.fehbvm.com/Article/details/gjphpktpf.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.zdbjq.cn/Article/details/gsejcoskm.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.fehbvm.com/Article/details/gxwxkwnid.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/gimhltrxs.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/glhmegsra.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.fehbvm.com/Article/details/gjcmqlkor.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/gtruhesmw.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.fehbvm.com/Article/details/gbmijbptb.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.zdbjq.cn/Article/details/gsdliqwqv.sHtML

[D15] 去重
来源：http://www.share.hesvh.cn/Article/details/gljjymrzo.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.hesvh.cn/Article/details/gbdcauhrg.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gsxzvheqj.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/golygzxcn.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/grwjebvyi.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.zdbjq.cn/Article/details/gsbljcanc.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.zdbjq.cn/Article/details/gczpccwia.sHtML

Ruby: arr.uniq
来源：http://www.m.share.fehbvm.com/Article/details/gcosfhrax.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.zdbjq.cn/Article/details/gcxnbogbi.sHtML

[D16] 求和与平均值
来源：http://3g.hesvh.cn/Article/details/ggnvzcihd.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gyrxsmuyp.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.hesvh.cn/Article/details/gzueqaeon.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/gmdyimrii.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fehbvm.com/Article/details/gwxffhgmf.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.hesvh.cn/Article/details/gmpeoqyti.sHtML

Go:   // 手写循环累加
来源：http://blog.fehbvm.com/Article/details/ghsleaffd.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.fehbvm.com/Article/details/glnwpcsfz.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.hesvh.cn/Article/details/grafjfxlb.sHtML

[D17] 最大值与最小值
来源：http://mobile.fehbvm.com/Article/details/gxqqodefj.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.fehbvm.com/Article/details/gnxurilrj.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.zdbjq.cn/Article/details/gdkwflwin.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.hesvh.cn/Article/details/guvdlwasy.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.zdbjq.cn/Article/details/gqsfxkual.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.zdbjq.cn/Article/details/garqebwfs.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.hesvh.cn/Article/details/gkgupjihg.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.fehbvm.com/Article/details/gtvxlmmlx.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.zdbjq.cn/Article/details/gogunfaea.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.hesvh.cn/Article/details/gwvzkwpuh.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.zdbjq.cn/Article/details/gypxyibbj.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.zdbjq.cn/Article/details/gsnpmrype.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.hesvh.cn/Article/details/gpbwcuxvi.sHtML

TS:   nested.flat();
来源：http://blog.fehbvm.com/Article/details/gtglmzwcg.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gmygfwbge.sHtML

Go:   // 手写双层循环
来源：http://m.share.hesvh.cn/Article/details/guudojafe.sHtML

Ruby: nested.flatten
来源：http://wap.zdbjq.cn/Article/details/gjzuibyrj.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.hesvh.cn/Article/details/ggestwacz.sHtML

[D19] 按字段分组
来源：http://www.blog.fehbvm.com/Article/details/ggpiywrhe.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.fehbvm.com/Article/details/grpfngwhy.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.zdbjq.cn/Article/details/gjjjuhrch.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.zdbjq.cn/Article/details/grtkhtrbq.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gfqwyjakb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.hesvh.cn/Article/details/grboxzdyp.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.zdbjq.cn/Article/details/gwqdhvqmy.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.zdbjq.cn/Article/details/guypgoknr.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.zdbjq.cn/Article/details/gfwbkkudt.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.fehbvm.com/Article/details/gmmekpucu.sHtML

Py:   Counter(arr)
来源：http://www.share.fehbvm.com/Article/details/glizbuyqa.sHtML

PHP:  array_count_values($arr);
来源：http://wap.hesvh.cn/Article/details/gscyrcsqt.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gztkihazh.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gosubjvkw.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.zdbjq.cn/Article/details/gzmnjbsqf.sHtML

Go:   // 手写 map[T]int
来源：http://baike.fehbvm.com/Article/details/gybifutpn.sHtML

Ruby: arr.tally
来源：http://wap.fehbvm.com/Article/details/grlhwpomq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.fehbvm.com/Article/details/gstcpxlkj.sHtML

[D21] 判断是否包含某元素
来源：http://baike.fehbvm.com/Article/details/gohompdrm.sHtML

Py:   x in arr
来源：http://wap.zdbjq.cn/Article/details/geogqqzfu.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.zdbjq.cn/Article/details/gcpqacxkj.sHtML

JS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/gymgyryqj.sHtML

TS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/gjzslgtim.sHtML

Java: list.contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gztduwoqj.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.hesvh.cn/Article/details/gmacgmfak.sHtML

Ruby: arr.include?(x)
来源：http://wap.fehbvm.com/Article/details/gvyrzkrgi.sHtML

C#:   list.Contains(x)
来源：http://3g.fehbvm.com/Article/details/gcdzdepob.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.hesvh.cn/Article/details/gpecldegp.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.fehbvm.com/Article/details/gzfjmfypg.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.hesvh.cn/Article/details/ghgcqfzhy.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.hesvh.cn/Article/details/gfnfcopca.sHtML

TS:   [...arr];
来源：http://mobile.zdbjq.cn/Article/details/geupfifnx.sHtML

Java: new ArrayList<>(list);
来源：http://wap.zdbjq.cn/Article/details/gbgexnfby.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.fehbvm.com/Article/details/glrxennnw.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.fehbvm.com/Article/details/gcdvegifr.sHtML

C#:   new List<int>(list);
来源：http://blog.zdbjq.cn/Article/details/gwirziyji.sHtML

[D23] reduce 累积计算
来源：http://wap.fehbvm.com/Article/details/gwoosilwr.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.fehbvm.com/Article/details/gnnfpllip.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gillfpdgn.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.hesvh.cn/Article/details/gpmnokbmv.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/gbsbrhzfg.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.zdbjq.cn/Article/details/goasciaxi.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gjwgbhxhw.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.fehbvm.com/Article/details/gxwbginfa.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.zdbjq.cn/Article/details/gexfkdold.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.fehbvm.com/Article/details/gnmokooqq.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.fehbvm.com/Article/details/gxhxdvdgd.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.fehbvm.com/Article/details/gticuohtt.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.fehbvm.com/Article/details/geilpomjn.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/ggxjhxkge.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.hesvh.cn/Article/details/gvlbaeqsl.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.hesvh.cn/Article/details/gggjmzlnn.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.hesvh.cn/Article/details/guxywmxfe.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.hesvh.cn/Article/details/gkheatwwd.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.fehbvm.com/Article/details/gzaebpfgb.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.hesvh.cn/Article/details/gtcltpnlg.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.fehbvm.com/Article/details/gvypfyupq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.fehbvm.com/Article/details/glibegmfk.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.hesvh.cn/Article/details/gqgcfdomf.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.fehbvm.com/Article/details/gfghefvod.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.fehbvm.com/Article/details/gflgqedrd.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.zdbjq.cn/Article/details/gfussuajt.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.hesvh.cn/Article/details/gbafwohux.sHtML

[D26] 数组转字符串
来源：http://m.share.zdbjq.cn/Article/details/gcbdzqaho.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.hesvh.cn/Article/details/gzktrabqa.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.zdbjq.cn/Article/details/gpgjpkeuv.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gcqpqxdnq.sHtML

TS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gqebwzuue.sHtML

Java: String.join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/gwevnsjmv.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.fehbvm.com/Article/details/ghqdsblfv.sHtML

Ruby: arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gdnrrtrac.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.hesvh.cn/Article/details/gznmyitva.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ggczexbhh.sHtML

E. 字符串处理
来源：http://mobile.hesvh.cn/Article/details/gmlhgbkgu.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ghqgnvjzy.sHtML

[E01] 拼接字符串
来源：http://blog.hesvh.cn/Article/details/gfngwvpha.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.fehbvm.com/Article/details/gltogtnwm.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.hesvh.cn/Article/details/gvltqfeok.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/glgvvgupy.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/gckehdjeq.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.fehbvm.com/Article/details/gmiutxwfv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.zdbjq.cn/Article/details/gssexfttn.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.zdbjq.cn/Article/details/gxilyaxsc.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gzmkzbbnm.sHtML

[E02] 重复字符串
来源：http://mobile.hesvh.cn/Article/details/ggwpxgosp.sHtML

Py:   "ab" * 3
来源：http://baike.fehbvm.com/Article/details/gaheinosm.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.hesvh.cn/Article/details/gbryvihce.sHtML

JS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gsidwdqvs.sHtML


<!-- 参考信息 -->