代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2tnxekyyi.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2njklpyxh.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2hqkuwcqz.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2vehslvln.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2gxugadio.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2gvtdocwv.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2fzmjwcrh.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2jlgrkxxz.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2lwzxxqhb.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2ugpfubzk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2wgscqiou.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2uwaeasxk.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2yiyquioe.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ebiwhytm.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2masepjuq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jxbvodnx.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2cbsniqzd.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2evydujoz.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2sqefggni.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2ujdoeizp.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2fnhqxwef.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2hupveesk.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2oqmgnchq.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2kntnasak.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2nclwmren.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2upvprzhw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2fdkgzvcz.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2lzgwtkhu.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2mvvpzrgy.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2dpvhiqmj.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2ylcwoegd.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2zjasvpey.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2mrfxtkid.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2redershq.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2dvvgjsov.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2qbccehie.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2kvvtfrkj.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ggcnkttz.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2myosjkjg.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2cxjbqiog.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2sqmawbwc.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2wiwoeoir.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2fkqdfoar.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2riqjwexb.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2bzvxflvx.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2otrmyyso.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2moftegvb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wnvvpyvm.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2dlojgncx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pxanhqwh.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2tdbsntuq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2bdzxnuul.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2xtvmdwpa.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2iepttokq.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2gswdafeq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2iierelag.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2zqeruclp.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2ffeweczm.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2petgnlmk.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2rhdvvsrb.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2atexhrbu.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2zahgrkuq.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2eipyanqk.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jcwwsipe.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2azgkwtvc.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2yeekswjp.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2mrcdscic.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2ctabvkmv.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2ojountse.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2eyspsicg.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2yxrxwvee.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2gjhlolvz.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bcvjsidv.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bdifkerl.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2gihgwyms.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2hlaoinla.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2syewounl.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2zfidsrgo.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2qfppeicc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2mhfmjqer.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2lqviagth.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2hizpoout.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2roigbhey.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2fqryljdf.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2dzmptkyo.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2eammrbno.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2sevnmgmz.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2twzmltpg.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2flgoxpnq.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2eixxybya.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2crbggtqm.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2wepnzrix.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2noxavopx.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2toaornqr.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2rsecxcne.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2bklsbsuu.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zntkvqnd.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ezcmwdin.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2igduzcsy.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2oxpznhyb.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2mheebiwi.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2iujzvohf.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2lpcepoxm.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2sgaftthx.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2gyigmeol.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2jnflywks.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zwzgkuce.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ddukqyeo.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2kmztfoop.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2awfwxohj.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2btlvaoyz.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2ufguupsm.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lxnfaqvb.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2bukwodmj.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2tgogeqea.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2mqicjapy.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2vwsyihqe.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2zwhkleyi.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xrtozvbq.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2fybjtrzc.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2uuzfqqzt.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2kyonswgz.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2jqwtvhke.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2craawzpw.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ayuggwwx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2fyexdfnd.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2ywzovost.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2ffrlzlul.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2plwauvwx.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2tqoenoxh.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2mlnpvsxp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2qjdmhgmp.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2hmyebtxc.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2ldxatjzl.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2amyljtcl.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2toqjonbc.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2mpmwhzdu.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2ypntbafk.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2bkspodqo.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2fjyymfyq.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2glfzlokf.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2hcbthwib.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2ujsmygru.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2ngsjyrjv.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2lxbhngvq.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2ezhbijas.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bybhdsga.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2bmsdqwdg.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2omomovlw.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2welxonxf.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2izymwdhm.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2gfgxwpwl.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2iprdzlhy.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2tfpbykmv.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2cazpospf.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2yhzyywgp.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2fynsyxpd.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2expfhyuk.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2dyleizir.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2tiglwyyd.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2pnafekwa.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2cugufenx.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2asapqtyo.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2oedxmlmc.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2raxxqimv.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2bwzxrvrg.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2lhqnxvnb.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2nbjlqhts.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2zfsgejqx.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2fuoyfica.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gkzaznha.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2psaybchf.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2cxqsunte.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2ydxtsfkc.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2qavrvkhv.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2qizlhfve.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2auxbsysb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2pcipkrvy.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2wradvpwq.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2sgqmnbia.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2zvhjgdhc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2zavyqhwy.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2dzsvuozy.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2azyuiguj.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2oaqooyve.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2cxkukbff.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2uypyomqm.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ezqnpulb.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2pagagbhg.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2vuipgiqg.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2rbpggclu.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2pjcniiyy.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2eqmzicbe.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2hdwxaqbm.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2pkoumzee.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gvwhfzws.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2owpdkwfu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2expqwgao.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vxorhmbw.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2phqaqqgm.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2rlbzjllr.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2sevbcqhx.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2zgqmayic.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2vqajgbxk.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2xlpigmfd.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2supfbkok.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2qzvrqsio.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2srpnnqoc.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2weikvbfb.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ehkszqes.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2cfzyrrbf.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2mbgzcekd.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2esugeedc.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2mbahuxzj.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2obbvuqat.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2yvcrxfng.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2bjuuvhqs.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2ujyoyhyx.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2markzmed.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2dqkqiwvw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2hklmjfsu.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2lxuqkmmg.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nuuleuif.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2bwlxafsu.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2fziuvnud.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2tyxxvxxc.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2xiqlqodm.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2hdlndqdd.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2zpegfrwu.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2balhftms.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2rnjjmbet.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2umbejyzd.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2sbcyjeit.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2jurohwtp.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2jriqwmpj.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2stogifdg.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xejfqmdq.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2gbarfhbm.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dlbrhwkr.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2gprlbaxd.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2rebzdydh.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2jusqwdox.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2yrgxilmy.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2elqewuze.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2qywlobfq.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2udssnehi.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2eomtkkar.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2hgwbgbhh.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2hmpkgjqt.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2bqacmczc.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2cpfmqzxo.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jltpdihz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2sdmmnxxx.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2tuaidted.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2jycmxzcy.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2xdfpvsmt.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2dchudpku.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2pxyzqxnl.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2lqtskrnq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2rrddsqnq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2kcvmffoe.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2pmcwrotd.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2hlbbwwdw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2wqanqqdz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2ntuesske.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2frjjgxxx.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2vqrcwvwb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2pkehfzff.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2bwtrcfpp.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2mfqjhoyy.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2aaevsmde.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ymwtqlxl.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2fqjpheum.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2wmpvinoo.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2piexfunc.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2rantfwah.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2hbvlwswz.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2mbopytrl.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2srysxild.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ybxgoffs.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2nuntlmje.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2ibnxbejj.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ajqofwzc.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ckgepdqk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nrlfzdxv.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2vryiytdn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tnrylmbq.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wkfgwzhl.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2czbjtmbg.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2cnmkzhxi.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2legkgwtq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nrytfhaw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2mferegee.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2jypbasmy.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2fwnqbslb.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wzsasbgv.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2yeughhlc.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2xkzvwzmq.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2dcdezixm.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hteidyax.html


<!-- 参考信息 -->