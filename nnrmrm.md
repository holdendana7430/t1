代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2tsnprnsj.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2lleqvxzg.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2sowoiqwh.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2lshsecow.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2dyoasxjy.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2nfhdykut.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2bihkncbg.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2vvwtgszr.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2gefafsbv.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2djhoeloh.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2gslruzvu.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2mysocigg.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2oskfvzao.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2whubmlgw.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2nlmdvyox.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2skjbntkb.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jametfab.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2bzuycekq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2fyhmrucv.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2ukuziemu.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2plyqpjbn.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2dftbrqwx.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2xfrrnkjv.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2hpqrjuix.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2hbiulape.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2aqkqfeuq.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2ezwayijx.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2gbmjjixf.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2awawbvcq.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2rehwvqzo.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2xzerjnot.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2rwotgsef.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2opanvnfn.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2aalmpgag.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2oebkpwub.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2akkthlzr.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2luwmqefn.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2mgygipmr.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2aukucoxj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2skvbbczc.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2sbgvuhdm.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2qlutvouf.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2wtpsnkhz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2qgsghufc.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2ebrbxzsp.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2lwcwwyxu.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2jjkcvifq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uylkihkg.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2soavckyr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jsrmgiej.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2xyefftdn.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2icqwoeve.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2zyakczyp.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2yvjdmcol.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2cnlpopmj.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2ornlyvdn.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2epbqsqsu.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2hhmiarnj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2qnmoxjhd.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2zvdkegur.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2tuwtuwwa.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2cjlwgzgf.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2kmhwruto.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2susosgpi.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2etrpozed.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2unfuwzuh.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2suwqttfs.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2yfbkjbjt.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2weywtxxy.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ywxyrpxv.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2shhhjvdf.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2hulhtcnt.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2aaxjppqq.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2mstssmpn.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2wvovyfzm.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2tcwoubyb.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2klijztip.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2ivpjrehv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2akrnrvgr.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2ujknloqm.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2yhocampr.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2phasrhwt.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2erzuzozo.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2zqrbatiq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2lnysmzsr.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2cadsnqly.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2qoluaosq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2gdvwpnji.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2zjnekqct.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2jrwwajrv.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2hpiolckn.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2hwtpiiwh.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2wpeuzwcm.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2zqfwsxbt.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2mterctxk.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2xdbbntuy.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2bsztzdmb.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yvjaqhva.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2eriwiqzf.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2ahhmqmoy.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2veqajvsq.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2slmovjki.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2pbgjfayp.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2mldkufpd.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2tvmyxrix.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2ehydjyyt.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2nijlbyox.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2jsguwrks.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2gjkvwpjf.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2frdumsle.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2wrmvvnbb.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2sdgoekuu.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2giuqxmad.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2krrzwljj.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2hbqdlshw.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2dycohlna.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2vyntpoau.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2zflifwcm.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2rtpivnzo.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2obxgywsn.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2yvppztha.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2pvcidpbk.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2mgeejjiy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2gnhgjxxt.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2ecqlukuf.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2npcylwwg.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2ubqaidvy.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2xathwnrt.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kyitysvu.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2kegcmmgd.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2cfrlzwxh.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2syjeylid.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2huoykzyd.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2fjerndot.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2tmnmrtel.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2uzjuqmya.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2vvcbeflt.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2nbjgkcnc.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2odqbkbqu.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2wnrqpzeo.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2ivnflger.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2yqzbccep.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2ekopvtsg.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2drvwwpwt.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2hnyhronz.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ydimxgyk.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cawergki.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2qzmabhou.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2vahtikac.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2muyxepxk.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2pjsvoowm.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2txkiiqzv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2hdfdirhe.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ocrsjdhg.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2zbmnnogn.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gaamfwaf.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gizgddis.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2wrlpzfms.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2exkbcbev.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2igheqgdm.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mtxokmlb.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ewavxfzq.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2eayeledw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xbdaokht.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2cxtvqfzt.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2qfjcmaww.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2tknodpip.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2diilhghq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2iqcovlqz.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2ichmbgmi.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ibsspsbr.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cgmfebmp.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2gtkwwwps.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2opfsctli.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2wwhhciap.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ckrakhtp.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2yjxagpeq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2idejadja.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wwnmruqd.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2lsteewxo.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2eogxsmdr.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2qzzakusf.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2teqqmczt.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2nnxppcoa.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2mfkbbemy.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2xbmfswox.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jjenpxis.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2jmmmjyjc.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fqyqyobn.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2cvkvmkpe.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2fjanrqcf.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2faguxwnm.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2dznxooby.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2kmuotbvq.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ulxulowp.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lgenvytg.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2pxgroadv.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mucugjkf.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bwhnfpqo.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2skdkjfub.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ytunsnvo.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2iapwyqly.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2tdohbkkh.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2wyidfkkm.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2kykgulyp.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2casfjfmo.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2nhqqriqi.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2deofgmhd.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rxwmnivi.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2qijlqzem.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2niygwcsk.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2lpiqpkjq.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2eoabcfii.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2iysryldc.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2ccqkbeix.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2rbdpqazv.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2tpsihlyv.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2jvuypgls.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2jwckyayk.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2mivoieni.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2rwontutk.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2xbwbejun.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mejvtyry.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2bnannkdl.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2jyvvgqaz.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2qfbihooh.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2rogsxuwi.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2ppfmjqqx.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2enypcvzs.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2opwdvxpe.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2mcjiwiia.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2qnsnlypm.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2lzeipayv.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mlkijibi.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2zucpbrze.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2pbvjlmiq.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xcckewaj.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ceyiqpyg.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2hnhrfhea.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2jqzsokrx.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ktvkgkyk.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2diwmnevs.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2weqofvjh.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2whssqhsl.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2jqaaount.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2llqwojqx.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2ynecvtzi.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2aaywirit.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2dhgqujtb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bvqhkvgp.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2fqgarsxq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2txgurzfv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ncvpohhb.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2ikgoeerf.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2mbwfrhmo.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2btrmdbfp.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2ekjvvhuq.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2bazzxsjq.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2ozutdelg.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2hzhcfvrw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2yygjnxzm.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2gmctdttc.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2xjlymqui.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2gyylalte.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2rswiqclv.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2gkfzskik.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2yrksepni.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2hjdxjypa.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2kujughls.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2uxaqakvz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2mhhnjiqx.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ruykfvrm.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2mkayvcgi.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2xweuispz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jocjmari.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2nujjhfxb.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2mocfgegr.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2jdnwexav.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ihbpsmeb.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2uwulcnec.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2koxmdebi.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2faxeyntf.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2xscqqabv.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2wbcszdfj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oswpbnom.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2zazqalha.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jmdjbefr.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dsjwwycy.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2yffoguwd.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ssihbjqb.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jornryji.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kgdahbjp.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2ncbfkrng.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2rqncqfqf.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2yvrbgudx.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jmeyfcbv.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hzfsfblw.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2rawsozih.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ynwrrfjp.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2iivvakao.html


<!-- 参考信息 -->