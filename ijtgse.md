代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3ocmapkcw.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3clfbxxnb.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3rxvbdgvy.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3abjoqqxt.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3njhknlgy.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3ypkzsajw.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3tssmtaob.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3dnfrtmhu.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3zmexaynu.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3mjeuwdev.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ahjlqawq.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3rfedgswg.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3gkkptqan.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cyxlicjq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3ufnntezl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ovttmbqj.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gmucghai.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3ltsggtiv.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3lxyqhigo.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3shkjhqla.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3fhkeavjf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3dprqijij.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ewuymzqu.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3boiumeoi.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3petnhgac.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3iefrqrpk.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3ueirlleh.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3vwvwusmq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3nmdnarwc.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3cfcisiqx.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3zpdtpuuk.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3foyucvul.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3xnthdarh.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3glgarubo.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3hpwbjmmd.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3ufhwelaz.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3ydmskubo.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3ibmibpgx.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3ujjasnwa.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3empzfaaa.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3vkckamqp.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3lwgdapnm.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3vgwfhogd.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dyhjnxtl.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3mccuelnt.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3jbthtgst.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3kgntefnd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qlogztnt.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3kuwipkuv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xcycemsv.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3ydcjvvcl.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3ytobzyvt.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3fmtzgmve.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3qycssfvc.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3gqlvfiid.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3pwajxvgd.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3gvqowfbu.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3cxipxzzi.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3wxqewnmi.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3cwhzyrie.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3oxcfxtvu.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3bhyodzov.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3kuinocic.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3uupdjanx.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3popzusnq.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3eikamofo.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3gooraxlt.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3wpplfoit.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3pmcdhmwr.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3eezdqyqs.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3kypeepfc.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3ccbdanmt.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ckwovuzg.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3gumvrlvr.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3tqbghhku.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3uslezksp.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3fvvpovog.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ugubfnva.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xrrdxrzb.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3knruvgtp.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3uptaaywn.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3qkveikkl.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wnegfrqm.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3wgotychc.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3rtbrcjdv.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3tkdlaict.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3nvtcaslv.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3enwhilgl.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3dhkujury.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3xbupallc.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3vzjenurj.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3mpgqlpcm.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3hoxcehbs.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3dnbwuxdq.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3jyldjeww.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3xklcxais.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3oxvgnmbb.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ygdvvcvz.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3kslvwzxr.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3jywfbwkt.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3dwtpuekq.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3jyytfequ.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3cgdsvybi.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3kwxokbtm.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3azsfiuik.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3qknzvnbk.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3hbythxud.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3nhifqqvv.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3kvfgtmwf.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3rrrkopng.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3rpqvhemv.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3pfywrdye.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hjwgumjz.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3imxyejow.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3hwzkglfi.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3rqxndqoj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3vrnajpcx.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3dgktmbmi.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rnxaozhp.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3smxjjzmg.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ohmnbthu.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3rvfaqgpp.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3whaurrgp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3oxtpnkat.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3mquexxsd.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3zaxqkwco.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3kztteoly.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3zbaxuxui.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lqmzdvuj.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3dlkclyqn.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3efatvoue.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3brzbklhc.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3kgvjqzms.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3eliwigdt.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3stmzuijn.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3nuuigpow.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3qifovhhs.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3fhnynuna.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3cimvhaqx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3flbraxlu.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3qqzasbbh.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3sousfqrj.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wlrvrtsk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3ykjrjozb.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3ghtpufct.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3kgxzfkmv.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ckwmbnul.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3phszmyer.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3xyndidap.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3liylxbbc.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3bxozfvpf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3lzlmlemq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3pcbkifrs.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3muwkydru.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3dpnpiuon.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ahvexeuj.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xtaxhtps.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3eeubtbnv.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3oxhbblzk.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3jrrxbcrn.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mcbhdubu.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3juwqlmhn.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3vunmdjqo.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3amfgutxf.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3izlbhiap.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3dpkmmwbf.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ucmwgill.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3pjzkhcad.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3xztdezhe.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xphmqsrt.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uztfodvn.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mklnszvm.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3qmzjryiw.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3tpnwonmz.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3iktxwawq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3dphztudd.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3xmcervkd.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3jcaagdfx.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rvmdsugr.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3yzghmfgj.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3qbdvgxrj.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3xlyngcta.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3wiheofli.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3zulgbygn.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3pzfnwacp.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3yskueqtm.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3lvmlngjg.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rsmtqyos.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ufjrfwyi.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yeijkayh.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3ommhfrpc.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3imabwbqm.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3hxnwxbng.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3sollnzpr.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3zgzifbny.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3awthwkuo.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lehbtwhg.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lxiqebgv.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3hsbguzlz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3trsurrns.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lettjvix.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3jlskqagh.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3iicluofo.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3hvexqonj.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3hwbazfbu.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3wyvgpjba.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3pobhohma.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3rmcpardz.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xsjashbz.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3olwziqoy.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3nmofnpew.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3iylqqckd.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3okikqxjh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3poayelas.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3ociuavpg.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3chlzxqqx.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3hwovmvns.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3vnsvdgzu.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3txewsdsj.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3qteuguwi.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3cfbwtguh.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3ymxcqutv.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3qgsxouyr.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3ylopssyn.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3kuranvvy.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3jwjyfkch.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3wsczmrqe.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3ugluedpo.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3cvnytarg.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3twvpxmmj.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3ejyobewa.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3iwgxrkly.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3dnssxowu.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3tqbkqgok.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3kniuonam.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3sjveazwj.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3nenzxglx.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3trjaovpm.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3eicpjwse.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3fgsxvndc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gxoajldg.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3ynsfalpf.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3boxbigoq.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3qdoqlrfz.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3fjqrhsaf.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3rxzizpxi.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3izonyiwe.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3ghbvqwuj.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3lxeobdir.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nginnrmv.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3amducdcu.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3fsrtbdvl.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3qzixxhci.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3hefwmkvf.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3ztglirma.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3mjvtavyu.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3bvsvsyvl.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3gzppubho.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3imbmezyd.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3kfcgkauu.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3scvxofip.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3rgwixfvf.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3wgikyjtb.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3gtphrfcb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3zjndtpss.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3ozadpkpb.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3orheqamo.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3zadkdiki.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3zjvhoztx.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3ptgtgnpo.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3hsfuuakt.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3jubwhuvq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3ttcynanv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3vvoeevgl.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wdyciwvk.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3iwuekfzc.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3kbezujui.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ejxlihlg.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3jqlllhiu.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3jevobltr.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3ktetiihm.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3vkzzglfs.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3kpekuhup.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3bqzykini.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nevcraci.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3zndiqjsc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xiswwxyi.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3pabjevsn.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3ygdbwiss.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3htcrsyjp.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jyltaxqz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3maiicihx.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3tjpmfojd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3tmnjlurg.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3llnlleuj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vxyrqlyz.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mavhssxl.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3qkthqiro.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3badtaxud.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3yltnttjv.html


<!-- 参考信息 -->