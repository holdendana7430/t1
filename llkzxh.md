代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3oqpzwujw.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3igkuqnoj.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3scvpuhxu.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3niogvpmq.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3opairahh.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3jnvgvkdv.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3jokymjzk.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3kjavqsot.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3jklhxxha.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3zecoxgjd.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3jqxxepzd.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3kioggola.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3qcjfkqzd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vsqebccv.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3yxgsrpys.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gnecvurq.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3auxqofoy.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3aankgcke.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3owraxmgu.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3ikccpqpn.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3dxicgiuq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3pzuiiscc.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3kdfsaeel.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3gttgqach.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3hvlvmfjq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3edotcskt.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3uranhmsk.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3tdnkqghz.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3lhftjlfo.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3qhufrord.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3hnpukmha.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ypqebbfs.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lnohneyi.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rjugnsxo.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3zbestasx.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3fssoqjjc.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3tjzbyada.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3irbwqiqf.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3feptzciw.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3hgmjhwgx.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3yzlpgciv.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3srogigdr.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3gogcrchq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3zivyxynb.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3ovmucsgq.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3uxyslmof.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3chmojpwy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3actchxou.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3kjxhqqcl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mivboick.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3popfulbk.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3ermthaqg.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3lgqaexjo.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3jxfkbjer.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3tjvtbsfo.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3vzxcpori.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3pxvpiatf.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3irxrnfho.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3tgquduhc.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3fxedpclf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3uoqpwpvg.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3vrhztwnj.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3leiuwmwp.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3czexrxvc.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3zojwkzcq.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3wvyfgwvz.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3wnicxogr.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3kkevbffn.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3hvzzhuai.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3cbbgvemf.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3srambbbh.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3nunqwbuy.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3gyviasoo.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3iutfkulj.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3xpxobjnr.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3mebgdlgq.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3twqqjokq.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3mobicwzx.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3apyjhyok.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gdwpbntv.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3xjloppma.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3tlwbbuaw.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3kqatnnvt.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3nzqybucb.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3treeeoft.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3rromljjk.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3rcuplwbm.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3mhsjqdmg.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3okobkvtt.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ybusejnz.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3cscaxlxx.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3slnbaqna.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3wmjbbrpb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3lwdpdsxl.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3rxqhzoup.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3pxqntsfd.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cpnriqdv.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3gdnqkbfo.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3zsozpywx.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3qkjydsha.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3axqceuud.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3fxrhwxyz.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3hhuudlhx.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3csfmgbbd.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3uuamxglv.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3ccwrlubc.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3muriedqx.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3nyjuehce.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3nhyhvlfx.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3uinqeiws.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3vlxtejgu.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3vnfkfvyq.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3edaohkvl.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3ubktjmgp.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3qrpqwotr.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3xmslbgpn.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3pclghjoy.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3iefwikhi.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3orixjghi.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3lysyrqro.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3fjsngriw.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3hwpknzar.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3dhfocosw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3cdeajsqb.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sfjtkexa.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3hxlfknzt.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3hfprulpy.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3dyxmzsew.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3wwwcmqat.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3biehuubb.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3awgyaowt.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3qjwaptai.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3zmttrlvj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3viseuval.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3tzgwwolr.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3rznclroi.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3bjwemurg.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3ogeebvbj.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3rzlecfdp.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3thjjbxmw.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3tucoixje.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3godudpyq.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3fxpggqcb.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3xfnydmoj.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3yktepvir.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3cadwhiyt.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tdjvymzw.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3zldgfmyp.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3tdstwhwr.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3dperotab.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3uohwfhmd.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3oyvpqwcm.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3bajuryry.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rcrbclxs.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3vvosgqyj.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3rnijjhom.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3yplegveo.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3praffias.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3nmghvxql.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3hyhwmmfe.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3odpkbdpc.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3tshepydp.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ajexuxpi.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wmdiftyt.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3jngtzugi.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3cyfbzfqs.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rxtclikl.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3hgnohgas.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3idfbduoh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3mqhyvcab.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bmmwnzew.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3zueebbzq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3wudcdirn.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ncyneuvs.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3fbynypnv.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3taoxdkyk.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3oehdwjie.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3qtfriztw.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3vrvfcewf.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3lzeejbcx.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3fewhopeg.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3rbjdhzry.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3pjazlpgo.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3dmtilrzr.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3mukayvpq.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3cxzovsgn.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3yhclterr.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bokkzfbu.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3xflpikcp.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3ioezgdmp.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3lzssuwrq.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3cgrkywnh.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3ihpkqqda.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3dukgmkhc.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ntorlmsf.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3ncxcanpg.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3gsmjksuv.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3rthzeaqv.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3chgoeoiy.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3wzfppqce.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3mayusxvv.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3tnqekkuv.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3ampyptuo.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3uzotcslz.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3cndqhthb.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3mjpejkxf.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3zwcoztrw.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3ifywaxjf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3oivzeyfk.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3bnjwhaud.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3gketnrhv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ghghxmsf.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3zdgczqwl.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3cxdeyvzv.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3xonndglr.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3dwfgqrok.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3vyhqkjch.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3gvcqsndm.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3qwfqmebi.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3ovdnhucw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3yxfuooup.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3bgdlmzwo.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3wrumqrgm.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3gbnoakwa.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3wajlrual.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ldntetvs.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3zklwmbvb.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3zmlyqsif.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3wuoghuuk.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3klvulbid.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3apnnlyiu.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3prhnuixt.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3yblhmhzn.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3emzzwrqf.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ixzdetal.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3crgtqsue.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xwmolxwg.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nrljniyn.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3yubkwssd.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3fmilwqot.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3wsrhvsio.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3anykiqsf.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3gkccwalv.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3tijqwnxc.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3cmykxgis.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3enudalvt.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3mezyxbjc.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3lhdlgufs.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3eccoefel.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3yrtiacwj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3derwytbp.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3avmkykyn.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3bhfjzsjz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3dnpgrgqh.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3mlgdzevz.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3ssgwwpie.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3attmqyoo.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3iccbztks.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3ddttrako.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3pmhzzktk.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3coazfgol.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3wbptztnu.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3rddwuzec.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3mkpftwoz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3nnmtyosh.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3fdddnqbr.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3cqymfejz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3vfdezccg.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3ywqfsejt.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jxxerdzd.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3wyoogjnz.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3apugsyim.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3dmkmcrhg.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yxhyhxfz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yvndompi.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3parjpjml.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3gelpbqxo.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3hrxmwsiu.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3qyagjwee.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3hoycbyov.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3qblvkpqs.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3efbcxmcb.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3dpuaoypb.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3lctnoxcw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3flgufaid.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3famdyvyi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iwxziblt.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cbobsmfz.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3matpvaiv.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3rgmytjck.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3odaubnfh.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3xmwpnjds.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3ebqoyjhr.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3jqcurweh.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3nakqyqxi.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3bltlmbzo.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ysuypimq.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3rnccklhx.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3dnenkljk.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3dctjcgyi.html


<!-- 参考信息 -->