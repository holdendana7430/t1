代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3iyknelwa.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3teuhybna.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3gaawsvwd.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3klipuhhu.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3kmfukkrt.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3dcspzuhy.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ywuzzjkp.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3yyvvloni.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3kgdyajdh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3rzqsvtxa.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3nekrlpds.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3kitgrckt.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3viizeqci.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3fscorjdu.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3miqqgmnn.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3xihcwgjx.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3nzelveqs.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3xpnvdpzv.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3mtqaqhdk.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3dmwvgvqt.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3mubmylje.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3qilpemhs.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3xrlhvmoq.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3eygglwye.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3uprqbpnf.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3lzdbufup.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3hxykzzcb.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3vlsrjxdy.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jibkcjul.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3qfduuagt.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3tmbusqqv.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3ipiocbqy.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3fjctuikt.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3kohoreld.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3exaailnm.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3quboveoh.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3hfckjzex.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3syoozeeq.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3zkhbwhvr.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3clepkfsy.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3girvztar.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3swumjuej.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xeafryvr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qvszslqv.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3zutniiao.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yuhvhzte.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3rkbynbxf.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3xgbuldzm.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3jrgvkain.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3fvujdwaz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3qfycssgt.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3mhhbedcv.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3lxqwgvvr.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3snwnunbu.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3yjmgyyna.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3eblqhgph.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3ajftygni.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3mfkdumcg.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3divkabyf.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3rjykjcbi.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3tljwtapa.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3zrfhqicr.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3wfcnezyf.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3fzzilotv.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3jocqirqy.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mepxtpty.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3fjzcncpx.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3uwsvsupo.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3otrnsrgc.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3gmnsbkjk.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3somrzwsc.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3whtwoboq.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hqomtzbv.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3nqvxyhom.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3aavyhzar.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3onvcwvve.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3metzhgee.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3cfhmejgs.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3sygbitde.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3zoxzlgoq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3huoooehp.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3lykvdyoy.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3opikvjrp.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3gnyajvxz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3gvskktmw.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3gskpdcid.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3wtwzndpd.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3xdewunfp.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3swxntygi.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ddyxywwe.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3aethxurw.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3rewiopkg.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3cyceoayi.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3ajtmzcod.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ncjjeuuc.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3fxjxjukx.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3vylimows.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bnfezswh.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3ydxlxkxd.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3fbblhujc.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3feppquya.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3kaegbxbj.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dxywgbsi.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3jueojptp.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3neukhwqk.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3calhujiv.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3hdshvbjt.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3nigkxitl.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3zqfrgmww.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3ynvrzajx.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ccojltha.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3lafksxnk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3wfxvjveo.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3sdbybhok.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3yuemrydi.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3nohyqmjf.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ixnwpbul.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3pudxswwo.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3koiiazdh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3okfollqj.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3fecovpbe.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3vkdxxiaf.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3twjemhpg.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3snhywtqb.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pexoidhc.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3salwgpbz.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3ozqfxjtd.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3gfiazyqv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3hwikxozw.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3efmwkmxw.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3pgkjzacr.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3xudzxzpn.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3zneqsftd.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3fnsjvvsw.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3ebphilxx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3tdpljjxt.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3yobfjsxh.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3mbxriqbd.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3bbijkdfm.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3esaubqge.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3svkcmjxf.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3wawhhyup.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3edzzllrp.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3mapmwysw.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3nrjbrwnk.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3copbdplc.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3whjymwlc.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3xwqufnxy.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3jybqiiki.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3wauxgkkw.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3llqgyatn.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qtxrsqhb.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3apgwfkuq.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3deoouvvv.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3uzxtqoqr.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3nroqydqu.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3esxnfksz.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3tivrtomm.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3fzbydrwn.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3tepweiqk.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3nluebvoc.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3rdsvpxdq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3qreniqwy.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3avnkakuj.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3srqqfmnp.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3koznekby.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xxokcxgi.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3tqxskipa.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3pdxqsrgj.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3bbwffdqs.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qpibpore.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3mbvdyxms.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3ytzpmmvl.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ualnogzn.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3bvjdduqq.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3bseprlto.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3znvgrjvz.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3stzorxzc.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3hmdbyxek.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3fzrqerlp.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hpkyzgdn.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3qssyytwc.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3hybboqee.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3gsgehcmq.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3zchtuugv.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ndaxxmeb.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3wzyizdvp.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3sckhfthn.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3tlgxzanc.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3igkjnsvg.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3tololrdq.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jewurvpf.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bvfwhazw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3rjqfhteh.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vbdhcyqj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3mgiivnta.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nwhwcbyk.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3kyjnbnrb.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3hmzmntcc.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3tayegimi.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3vcopahwr.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3tnjdhtfb.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3elpflymj.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3ldmzpaxl.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vrywepun.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3sluflzsw.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3iejzkums.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3duqjvfoh.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3kjinnjng.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3stjqjpzm.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3adhespjl.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3zvvqzhlm.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3briexuxs.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3uvkxmkem.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3dfsvnaks.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3zlekpybj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3equnqgqu.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3ozgbifxx.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3virqshfe.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qeumcaez.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3rqudhtkk.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3mgcpnnwd.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3rxjixiix.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3mpppbkds.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3cnmfvgme.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3pveiptix.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3pdzejdit.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3pkokcpdi.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3ubozpuxc.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vqwbvyjs.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dbhesyby.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jsrlevif.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3szixqlvq.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qktfditd.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3eaicehvj.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3ffdukzuw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3bckpsmni.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3jyvoyvif.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3hxvjgxsv.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3fvoljzzi.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3dbzyhspa.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3asmwfnka.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3wkpluuda.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3gokrromp.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3jhvluwbe.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xnbweygv.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rifznoku.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3amtgnwxe.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3hovhhpsy.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3qqvsfcjc.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3mmitmqga.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3yquqqins.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3cdtakeiu.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3mmlxnzdc.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ntnhjkxr.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3rvmvcpuz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3sflcbozb.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3aimocwyu.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3igpiupqu.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3dhfrrfdd.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3pkqbbgrh.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3yvuzsxor.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3zzjfjhnu.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3tvfvzvxv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3imkkmvku.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3esesuytj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3sjxhkpnn.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3mycbdsfc.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3wwelbwwz.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3puogucxv.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ikccruxg.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3acimhlwe.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ruzicvso.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3jtssqwwy.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3hgvakpvr.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3hegfmaeu.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3hpnfmiem.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3bjkwnuws.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3zgnytpxh.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3ckjoftvy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lgllauwz.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3qajmhrwm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fygxygur.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cktmnnxw.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3rohsbfru.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3rmbwltgw.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3rduxmsyo.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3nevhcwbe.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3nvcrqqzi.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3bfhgimjy.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3fykbfopa.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3zkkvjbzd.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lgvpsbop.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3bspezbwf.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3iwtrwojp.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3nrzcavzf.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mwycozqd.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3mmsfwpae.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3xfjhksmb.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3knhprvyg.html


<!-- 参考信息 -->