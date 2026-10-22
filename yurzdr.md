代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2bkbyjjje.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2engzvkct.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2evkoigyh.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2dvawttue.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2htvjbzdv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jehiwqbo.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2pscsiscw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lfbcyoho.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hsjvwbyq.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2hodqgopf.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2ujsxpvzf.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2svauptws.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2dgyrakna.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2uddwmdkt.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2bpdkirhh.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2qcnncbvh.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2yyjiiaxh.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2kgyvuzce.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2rcvmryya.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2czzcsvti.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2kewadalo.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2zwjhilvo.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2bhtfqwwh.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2vyxhvbyn.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xavxmdqy.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2tngcshlq.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2qmevfdze.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2hyeqsrwc.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2nvyymdif.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2smmmjsvl.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2imrawkwg.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2tdmwhgoe.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2izodlvzs.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2etzhkuxw.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2tddlrrku.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2jsjqbzny.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2weqfytbc.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2mpimjomu.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2guieszrx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nuloamnm.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2gyoovfce.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ldfcktoj.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2amzsqwvw.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2coneymul.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ygppcmjw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2whrusyyj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2cwccyrvx.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2kiisgeam.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2edrclbye.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2tnhvzyfh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2tlomjbyg.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2yvbdjniv.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2cyfcyhra.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2molwpvkp.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2odbyxffx.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2zfqnrshh.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2yfafgcuk.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2yyhuislv.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2ggyijbat.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2hlofjvhp.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2qcsloycf.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2durwnawg.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2lsheeogw.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2htwpnyjj.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2soqiactw.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2dwcqvvmk.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2silkjzsz.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2yzjgzajp.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2amqtvwal.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2rkonsaeg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2mhogpesn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yemxlpln.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2etypmpok.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2etimnpld.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2srrgwgyh.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2nmhqurzg.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2tvebhkwt.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2zynleeke.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2kuparaer.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2imylqggq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2dcgyknqb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ptblbfry.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2kzdqojpz.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2htijupng.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2pbbblnzn.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2zsgntuqs.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2mwqcedez.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2qpurucuq.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2waifjwxo.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2noytjhuz.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2vlyttllx.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2vjwompit.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2eusvoqsi.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hutscilh.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2ekxrtbll.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2zpgnyjbn.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2cczmvlue.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2ssiavhwv.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hzzuaekt.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2zrghnhlt.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2qrroxmoj.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2gpxoolff.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2vkfdkiyd.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2qzdncesj.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2lcomzmlb.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2waugwkyb.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2hzkrfqwp.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2iqsurndl.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2dumgjrum.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2frqlsjaz.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2inmoxbuu.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2wcqsuroo.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2mgoigojq.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2gptaqflh.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2vazegher.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2xjrftqju.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2equtdudw.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2tdeovsqh.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2tiyzhchx.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2shtlrbeq.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2chaonekq.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2nnvdcduz.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2vjmzblqc.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2jfksdrry.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2jdlzcfdz.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2vwwyyabu.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2lmcvkoik.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2hwjxmffn.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2sapjybza.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2bazqjeyx.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2usiearvp.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2fsfvpjzm.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2fqrtqswn.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2lozcibiv.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2zrnlgzzy.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2zknuelvd.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2ogidqtej.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2iouidajq.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wobwttic.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2lixcjwgr.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2pcvzpmoa.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2fhkzteub.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2fiqmtjkw.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2mvveqcpy.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2wjtmtuma.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2rctfmnqo.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2wxrxxuah.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2twhdulex.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2fsivovgl.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2moemjggx.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2tbhilajs.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ffjvpnfi.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ghuphotd.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2gzbkgfuj.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2mxxjspfg.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zbniowin.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2nxwrjloi.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2kxnmwvwu.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2mcblyuiz.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2znbxoumb.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2kjjjteks.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2uyxsakqb.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2absbmxji.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fehlvwfw.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2loatuixv.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2tncuvvga.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2zmacagwu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2oeqkoobq.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2hkweyyte.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ycsqypum.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2zaawpgbs.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2gjkvoyub.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2dncsmcyf.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2ugyvqyvt.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2podrunvm.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2juzyzcgu.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ksqzkjbq.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2kxvqfnwd.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2abvqkclb.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ladkfjqx.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wrzwcxpj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2mtdyfheb.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2wqgsvpum.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2vrojjags.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2ylbcthog.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2dykylvpt.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ubpiquhl.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2tdqgqswh.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wzgrimow.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gzbiumux.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kitvjsgv.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2rgwrhavz.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2pzimxrps.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2klosuwfj.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2xbwvvddq.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2lasnarny.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2qbbvxfgm.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2xknmgajt.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2oqrbxbco.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2aosquyek.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2yxhjuinv.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2jjcgnzem.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2moeygnou.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2djlhsrhw.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2pqzhpvfr.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jcfmbptg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2dfticzvs.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2dtepejmv.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2nmlyxhgk.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2fsafqhkz.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2wzkwoqpn.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2olhbghbe.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2wqhtduaz.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2exsqqtic.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pybpmpev.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2dfdjzxny.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2clwwcdxx.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2qwihvipa.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2yuvezflw.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2bguxrabd.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2wkrffopy.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2afbucuin.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2imimlacf.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2ouslotre.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2tpzyvovl.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zfkpgghp.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ptzjuotd.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lkhhmmog.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2sgkjvfde.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2nqcvnpcf.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uxtpefai.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2szrcgbgq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jkaqyxkg.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2ixlezley.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dwlfffco.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2gtwdlgdh.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2mnwmxwza.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2vcyiikmp.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2gfpjnnfu.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2enhxcdvw.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2zckxjqui.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2frkxygjg.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2objbnrjh.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tugahqxj.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2narahgvy.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2gtwcvdyr.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2aspmgkga.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2eiwugrmb.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2cqlgxlgy.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2qkmtfwaf.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2yfomsalp.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2hluhurgu.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2ekurxjxu.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2omvuqlum.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2gyclujnd.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2vdwwgwfd.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2rtaefyne.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2jnzgdwed.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2ammemphw.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2fhzulcwl.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2jpycqade.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2zkbglpby.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2zkndbqye.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fqghqlyj.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2bfwelbru.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2vwqvlvgb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bkxkauhl.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2wraooxfo.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2wshbzxqa.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2xqogqhcq.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2sdngqtee.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2zyacxtmy.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2yikaxowr.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2oijfptez.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ffqtqpjp.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2tfpxship.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2poksuzgs.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2pnvwooyx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eeqdxton.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rvxdfavf.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2dxqhxkww.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xktoheew.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vpvxrlln.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mrkqihkq.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2arncqznd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2adkxqbbr.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2wrncylzu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jgmpuogj.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gmbfsuvz.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2ynyowjdy.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2evasnaja.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2poufgpkm.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2pivywuyu.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2jshlqiiy.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2qenqxmcs.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2chbtqznl.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2lgkevrig.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ucfzovqt.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2xzrxgaho.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2biaueakk.html


<!-- 参考信息 -->