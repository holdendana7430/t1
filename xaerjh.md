代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2qgvcgeag.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2vysljdkj.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2tcaeqggy.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2zxzoqsuo.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2jdejzbxx.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2zlxxqklj.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2zrfbuqfg.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2jhqcpjbn.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2rqfpyzbm.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2byfxfnqd.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2gwfcuglo.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2dtolxywj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2jbtkixlp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2gmljwsnl.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2otfskgzz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2vzvhtfag.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bgvkqham.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2ohyqsbkh.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2injqwtqz.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2fklfkeeh.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2olvaqfuj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2itdydlcw.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2jlqdvbeo.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2kzfpbnob.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2lqdvyvtm.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2tseutavf.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2jekedlgc.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2mrwduvbl.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2doglvzxz.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2wqepkhed.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2hpgtizol.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2fxbfwpys.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2akwxfijn.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2clcdsxur.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2oeopesmq.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2iaqyiydb.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2kbrvlsps.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2wssjiedd.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2rqjijyoi.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2sznomfxu.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2mijbvydz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2qslopgax.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2wofxofbe.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fadyxhno.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2tlizmojs.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2itjcgohm.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2vvyrewgp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rwvboypa.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2twrdqemo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cchaumbs.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2mddjnbnb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2lzvauhvf.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2wjtxxbss.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2kpycpwpw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2ckshfctj.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2lublnyiz.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2mumgmepr.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2otqeeasi.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2aykeeasi.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2yfpyuytp.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2hfjzpeqo.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2zmclyiuk.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2cdnpglqo.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2dtqewcfj.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2fmbjxind.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2ieluanun.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2uqmqkgdr.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2srxemgmo.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2kycovyjo.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2koyfsgye.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2edgmmfcs.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2ggdgyocl.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ierhxyib.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2yhybcuud.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2efysjsrt.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2epvgjvkj.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2tmkgjhqq.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2hzmpmodq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2rfgrgbme.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2sjwmwwbj.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2dkpxccsm.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2uurucvnn.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jxtthdvs.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2rynaozho.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2pulzssud.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2fjabvufx.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2nckslhqr.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2yyfwudoi.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2lfgzzhrx.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2qqxwgnne.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2zgkgqzgn.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2yzqmcrvc.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2tqogjjuc.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ozrgycbt.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2iszrfoji.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2djqmrmjn.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zakmjbiz.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rcvtgwao.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2hilpopwo.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2howbgmfp.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2jkppmmiq.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ewvfkqtd.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2lzjdjvpg.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2jwgypsfg.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2nxmolkis.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2lgwimrqf.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lhnunizl.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2iobdouww.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2knwzcoua.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2gavttcow.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2stjyyacq.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2alzqvpvj.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2psgqqtql.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2srjaxjzx.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2trhdqyco.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2yjcvjmow.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2wnacmdyg.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2qmoeejox.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2ucesblnv.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2dyovhejz.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2zbuhrupf.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2lwuphuxh.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2jrxtnqnn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2rszoqjvw.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cegoenlb.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2ppcnudeb.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2cbqedvkb.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2guljzjds.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bwasbjeg.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2yqgkdzhm.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2kvkkhdyn.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2vwegntub.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2gqdcnaup.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ijdftmdp.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2zhhtgymf.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2uezuqlbd.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2vyqnpwys.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2hlqifcve.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2kcfvfyax.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2gvojbexo.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2hblgeiih.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2eqzjdjra.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2gzbsnqvd.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2tjfwswai.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2vjtnbzta.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2gccpxnbg.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2mryxrlcf.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2kzyvcxut.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2zzjorvac.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2penvcnld.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2kexggozu.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pprfmblc.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2vveermks.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2fqxrdcso.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2fignnvpj.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dydplgrz.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2whgtzzyn.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2xqxkuxhj.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2tuxgpboc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2myupyhht.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kfgzppgu.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2bixmtcii.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2mtxjxvpn.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2nlhzypte.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2ymhceynu.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2wksixshg.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2meptysza.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2rmpfiwxo.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2fyjwoixx.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2ewzqkgcn.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2djzwjknd.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xiyguxft.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2mtfazzry.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2lvkxrinf.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2owdsycry.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ninjuhwy.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2gfbcxwwe.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2zmlpcqbc.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ehjxuszq.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2iyhmynek.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2wcivibul.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2cfwlpnjj.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2zbpmlefd.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2xwbqkyzh.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2upvehzss.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2euqtwuei.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2gtplbjuk.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bvcagsid.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zdmbhfha.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2izykrrui.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2evnrsean.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2upigjpeh.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2nafemvyv.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2itqjjdgx.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2ohkkdvhd.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2srjffokz.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ylrysahh.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2fwrkcunq.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tbryfofp.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2szrhrueg.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2imyckhsq.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2yhzhidrh.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2hutkhlil.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2jxzbtbju.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2dbtjtkql.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2qwjggwej.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2thbldflq.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2trigeizz.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2iuvydpca.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ixazxwvl.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2jzvnqbmd.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2qkdxlquk.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2oybjchsh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rlmfhrdk.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2mnjqtmvs.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2ccmoqxsk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2ubzqjqfn.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2eaaetkvr.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2gvtasdqb.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2fqeimcek.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2imqrjrsg.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2ubstsyce.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fwmebuvg.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ytdzcvvd.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2yfgbmxic.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2vjwtokwj.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2rrtsmnqn.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2xjkrgmcm.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2fuavhagh.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2vwnwlgng.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2oumzbsye.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2sjoziyay.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2yhkhycfp.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2suzbnhof.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ecdfeljo.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bybcvbxt.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2sovrcxiz.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fqbfejaa.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2loxndaet.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2stittbdb.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2zlgzzvzq.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2zxqvumjr.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2grdotjiy.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2jchmefyq.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2ktgmejof.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2eoucamgq.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2etbdqyoy.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2cbyxhwtj.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2sgnxuebn.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xizmbtot.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2aqskewgf.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vyxlnpdv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tlsvrhox.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2vtrgpzqv.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2fvorndky.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2uqiifmlq.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2zehayxtw.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2etyjqmga.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2edqkzygi.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2qxaxzhav.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nredyquf.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xwbcesyq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2rmyoibiw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2djrsshlh.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2jsyyowej.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2rxbuiume.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2qdyffqai.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2gmvqnwwl.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2wpjlmsif.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nmhoosac.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2zvaitdra.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2aatcjysa.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2zbyfabdp.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bvbwxbla.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bnhlabau.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2tdeltvkn.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2qwatouvw.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2wupfwnpn.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ytymsnft.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2itcknyxg.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2ywbbmkio.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2lcyuekzt.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2nsimjhsu.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2mutulqsv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sfibvmcn.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2gtsrtrmx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ktilmzxy.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2cfqewrhw.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2uuasnjsh.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2nvvrshix.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zplldivm.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fjsdthnl.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2rojhhxsw.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2gsbtgrab.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2ggcvrjai.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2torxniye.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2xlhdjmqp.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2vrmbypyb.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2vxjuvlmv.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2krrgynsy.html


<!-- 参考信息 -->