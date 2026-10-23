代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3ibzaycji.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3jijijydq.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3szcybdoy.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3buzpkdzz.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3qnfzdhah.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3hculckac.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3sqqvkxex.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3fvifpasx.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3rnihrpek.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3jyjmxtkp.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3qponpqrj.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3jmuvcpvj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3syvaioeg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ndjssanb.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3gmllzhjx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vuvyhfpg.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3cihirlvt.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3zszyvlcv.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3rchijyvn.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3kvhhoitf.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3neyervsn.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3erijvsmq.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3uvzmkcsx.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ywietqxf.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3sovlsrfk.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3sstwhecf.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3pzryfwlt.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3cmiafpiq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3kbrjpbjn.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3dzoodjyd.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3rusxdgvg.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3jbmivyyz.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3hrixdzsw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qzibiiid.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3mzaxgcyy.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3vhzajrjn.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3vasyrdzu.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3eanfkmyj.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3qhxbhnag.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3fsktfgqj.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3mhhzpvzq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3yjdfyweq.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3ngirjvjx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tyxmuuyl.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3rrqrcryu.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3kmapwfps.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3wkmzuqif.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tthkeadl.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3kbzltnbu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ebbmgvco.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3yrkcmeam.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3gyzvrfvr.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3rlxijnov.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3abiqyali.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3gyqrgxkd.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3cyvqbwjj.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3siugbrsa.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3pgmzyfwz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3lxflpvin.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3cvfubgxq.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3qzwbuezm.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3cjchypqm.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3chqxylvn.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3pkcwicds.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3ptjwchcd.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3nptlumoj.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3hnrfhyqa.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3svvbtgsm.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3jlkaergc.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3vmjdnwbe.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3ybnvojrk.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3jfxowvem.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ofoyzcly.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ezjedwud.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3jxiewgqy.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3ivlfonaj.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lwmxxdnz.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3ogxopbie.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3igssybjf.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3awzszciy.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3kshmltlr.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3tysuifov.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3oawxcsci.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3okwydvyt.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3enkrdpfn.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3rqgqtnkw.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3hqrsvfco.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3jbsdawyj.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3aygplcln.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3hwvdfpdi.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3zzpynqra.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3nroejvja.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3wscshsbj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3lmpidrhd.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3zfodggyp.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3cgvtfmvq.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3oijvaoob.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3djkcjzgv.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3zkgzdazc.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3mdrtodlt.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3pjuzwrjg.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3puthlbuc.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3kyxvucgm.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3tlvrixzy.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3wyqrmseg.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3fhjcpakl.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3orhkchkt.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ffxkqune.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3fgnfxihp.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3tpvclzwm.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3xaobexus.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3pwdkjubr.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bdczrrtt.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3ujksxbev.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3saxrnylf.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3oeaxjgiu.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3sqqdbtpb.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3rbvronlx.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3sjeksnmz.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3fkahrkcf.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3ynbpdcqe.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3fwjbgqll.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3atotdtea.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3zpatndve.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3emdbqgnp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3wwgzkmlj.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3vmebymoh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3elooauza.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dbxetbbq.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ckpwkzwk.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3jbuvafrl.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3kffxcbmt.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3mbbmmbxb.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3cufloffq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3pxeonreq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3icblqiuo.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3pbmvwodj.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3kzgqaoqg.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3detvdtkm.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3vbwjdmov.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3ngjnwcoi.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3fmhjqtes.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3goodyara.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3upkeofti.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3stxaqidw.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3arzdeeju.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3adykyrut.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3odokwwfn.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3lxehjusz.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3hkijarzf.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3dzmzebpl.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qmihuorq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3utmjoejg.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wnzhomqr.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3ytxpmhyc.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xrmtwere.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3xybvfghq.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3sbdvcnan.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3kcmhiowe.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3krhnevmf.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wqqbsnko.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3kqspyqhj.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3frwubrut.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3pbgxqnat.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3etbmbvxj.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3jqzpgoog.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3nhvtvcvd.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3iommclib.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3agfpfjzk.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3bjhzwmuo.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3porrmxai.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wbdyyqkj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3fbzpzzlp.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3yjmekdki.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3cgkyhxxn.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vmvhhmoq.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3fxhyttpx.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3owleyvkk.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3lvxzepgo.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3egibuauj.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3wufzcgny.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3wkmyejgo.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3erlqaxeg.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3ilzgbqpo.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3cxklczht.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3rcptmemm.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pexidsur.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3rvtfgwrt.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qwuknwdr.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3fdwzpdab.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3kazffclj.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3mxrwnfdu.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3rpdabtho.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3gljfqynv.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3ezenoljx.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3erxmhkgk.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3flntghrk.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jcrczvng.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3elfafmhw.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3giabrspr.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hxjlwwiu.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3onjplzaa.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3bhrtztrn.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3kfadvkky.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3atjhddik.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3irqtslrm.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3jqmnnbsy.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3jjeqbhkt.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3mkiumcwg.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3jwmlezrx.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3iobkxniv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xtuvgmqd.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3iaiyijiz.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3tdblxeha.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3tejtpysi.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3uslgppao.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3walrpnht.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3erjqiwkf.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3xsssemra.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3lytlfqxu.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3hnabikow.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3raubtqkl.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3eiagsfwb.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3hpkygvic.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3hcryjxgc.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3dspcjbqi.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3wagtldoa.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3vxpsuxwu.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3kfuyiysw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3ijtvflcp.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3eppufpmm.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3pvfdtnlb.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3cvjjzzft.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3hacbmzee.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ubbaurzi.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3zoznsaxt.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3slvesthz.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3dfivlpcj.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fuhgpvpo.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3wpgdhkcx.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3kxthxuiv.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3akisvfzi.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3kvraabyh.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3dewzpxul.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3tepnzdws.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3artggbuj.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3bsswaqeb.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3lzngseeq.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3aupbiwoy.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3kjcefcbn.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qwruojda.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3cquqkscm.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3icjxgbmk.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3ksaylktj.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3mawbgksu.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3hhtwphnh.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3nanmqrfg.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3hfaebtky.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3sqlrvdof.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3qwftvasl.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vlhibsqs.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ivbeuskk.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3cjcjuyxh.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3bxzedynf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3dzdjrkan.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3cmyzmrpi.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3wxosnfgz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3jeitvjok.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3uhftcdju.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pzomqonc.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3dedldgwx.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3homkvmko.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3yhzwculw.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bfsmgwwz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3odocwsru.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ugpcksye.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ccyqsbqy.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cjmhpgnb.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3sihbsokd.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3xkimyjkn.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3atzvfbfw.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3fperbokh.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3vsmlrzmo.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3xleebvtm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3prjwskok.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3rlkxmoov.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cobsijcv.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3nthpmwvq.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3ofxoofkq.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3lcdimesf.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jagbfwbc.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mojvbcjh.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3vppsyfeh.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3hoyfyioo.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3wyhybbce.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wwyhbdzm.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3yvmqttqh.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3fzojwewf.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hfbxcrup.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3iqwbjngq.html


<!-- 参考信息 -->