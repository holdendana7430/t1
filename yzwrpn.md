代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2ydslseon.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2hajvxtpr.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2nknwmjnp.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2bkzjfvcx.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2btlkvlng.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2vysclzen.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2qlwcewyu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2fatbuexi.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2bhgfmjrh.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2pjzudpon.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2ykokikvb.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2xlsdhkkf.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2sqxwihui.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2qkfowcdt.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2aizveguh.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2dshqafpw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2ozjwpnnv.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2dyqnjula.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2tsgdsnwk.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2xmgxyzai.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2rzeqrvad.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2rcghxzpf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2jjjlugso.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2gekpjtym.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zbsouryo.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2lniavpvp.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2nqppjtdg.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2eiryqozj.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2dbvakmsl.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2kkfpyuls.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2hkvjsmmn.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2wfipcfsu.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2ikslzpii.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2zpjohshv.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2hwbfhpbg.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rfsicwhj.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2gqhjzyqh.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2mvifuhst.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2jsriptvw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lacutmrl.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2pemlaldc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xoabzelf.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2nennxxjv.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2hzmveiib.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2hgyrpwaz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2xkpwvesj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2jzdrdeki.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2kgswnagn.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2fksyhjle.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2wsvldbbr.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2tnwdlzfa.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2urqjzutf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2fskdvuni.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2pruujzsg.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2mjcfbxft.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2kzljsasm.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2zojvnclb.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2ibxcbmdy.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2pbrsqtwp.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2mvhzmubv.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2guqtgkcw.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2jrjtzdsx.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2johygaim.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2yhcneick.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tijnjijc.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mvmmnvwr.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2mgoldvyv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2howwrcdv.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2wnureyij.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2sewamxiv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2mdliicvi.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ooofbdor.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2ojbmchie.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2pkwhzdso.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2qgeesvxs.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2wcwysqde.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2goixsyzu.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2dpyhhosk.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2npuhlgbr.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2neifbeml.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2boiiragp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2uefbaqht.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2dodcjeam.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2soqukgcl.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2zjcafvce.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2algceyyj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2fsejoyre.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2mioagiod.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jqtnydnv.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2yclgjbti.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2vesceemp.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2aaendbtv.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2mfsrvgur.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2reqmrmds.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2iloduiwr.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2myryimup.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2bmqtixnz.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2jrxbzizc.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2sowbivpa.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2tbnshzhe.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2jpevwtyj.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ugcymlze.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2pafoerjg.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2afznnonx.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dpyeydrf.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2wudckmek.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2iazgcxgf.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2afxfsijg.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2bmcsmhos.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2bwsieilf.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2olstgydv.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2zsakyyxo.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ctrskyki.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ykkcmweb.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2ruvgvloy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2qvmchida.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2awohmcpe.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2fzapfjcd.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2wzoitfqe.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2lxxmczdk.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2lvmknrmr.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2mknejzzj.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2cqxdtkwk.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2wquxqzwi.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2flwbpqlm.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2fyokqcko.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2suzhklga.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2heclojew.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2vvxxaktl.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2uqoljgre.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2cprwxohs.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2usvggtst.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2qqdcjbug.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2wpaflspm.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ivlasctk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2xndhpgxr.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2iqbjcgln.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2onhipyic.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2paoobwrj.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2dutbwnru.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2ejxlfhtx.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2pulyuqbj.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2ymfsipyz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2nrgxajnb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2syzkejjn.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2zwudfjiw.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2jdiajhmo.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ihiygkol.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2qelkzboy.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2pbugfjuo.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2timqdyde.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2avvxchxw.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2wyghuzba.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2fullcubk.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2iybwcuml.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2xkqeswtw.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2utpdzijs.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2gyunrtwd.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2jgpowvsb.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2zppzfuqs.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2vndliqxe.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bnamltnv.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2xeowkygi.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ikxrpmmv.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lqsykptg.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2yebwwhkz.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2uuttxzye.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2xtbtoxdf.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2gedgrcpq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2klodtifg.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2zfdylhsz.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2acdivgwa.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2nlfjojhb.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2fwklilne.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2cszhbjnn.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2ybjcgtgw.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2smzenftc.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2hofbdggz.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2oewfumct.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2oxkdddck.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lsvgdhwo.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2scgofbep.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2fuvlgrnu.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2oavruhnk.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2tygjrgbi.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2izgtigor.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2bziqssrd.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2jbhkrqym.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2jjztolzr.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tnpwgfyf.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jxacmyjc.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2ahyqkclo.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2xlyqqnrt.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2jghivsgh.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2wchxvugq.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2whxuacyj.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2hygqftwb.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2uxtyqjcz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2hagzfgqi.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2cmyipwkv.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2wwhwxnhy.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2tudlheiv.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2apxenxew.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2pvttghqf.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2ufxmdogt.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2otkkejvr.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2tljyensm.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2dezxfrdj.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2nloyiylh.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2ibavzsex.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2txrqrfxh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2whyglyqg.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2pmndjbfb.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2syhftlts.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lcmxoyfe.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2ahfhavdo.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2qkduowst.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ipptsbuf.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2hfcdxyhp.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2gwrnxhni.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2epygjzjj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2tawqrrwn.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2imzjfyjw.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2ugisrkkj.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2yoylkseh.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2kcnbzsms.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2apczhyoq.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2styrpaav.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2yyszhsxt.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2rtsefoyy.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2remnotqr.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2rfgmmuwd.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gjyjwyrs.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2iptarvxa.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2qytszriy.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2wzvgvnqc.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2wqtvviso.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2pnvnzdjw.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2yjzrpaba.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2siddcaem.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2gvgwzjvn.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mndkezml.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2hnkkxyup.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2watyoeam.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2mtqxsswl.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2amprvrxe.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2yahszsbk.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2uhoxcrla.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2rjjtgmvm.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2buhvodns.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2lxkxcuay.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2humbfvxy.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tmorjzfj.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2tdlaamln.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2iagrxsml.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2luzlegph.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2lvibkyfw.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2swabcbzy.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2trunknnw.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2rdmbxdcm.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2ioqdumdn.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tgzmbrcx.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2qgnxgalc.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2fbfywynh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2kdnantxk.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2igsqvkgg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2piplwsqg.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2znifyjaz.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2znnmixlz.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2ybpaexvm.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2jypxnrhe.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2gtjmbcbi.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ruxnngmz.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2mlekhcrd.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2whfpkmlm.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2htgdxhpy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2alzjxcth.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2vmqljlie.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rgewzamh.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2qcomsplm.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2uvsdpwby.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vjtyzmrr.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2irdpefjz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ldtspwel.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2rplnwdyd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2njqwsufo.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2avqcispg.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2asmxyjxy.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2asmmeltc.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2mbzvmcog.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2utrlylva.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2wgmxxhjf.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ordaibps.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ljxldfsq.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2tlguaxor.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2hzhaqpbe.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2wwieqygh.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2tzphdsvj.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2ftbdxyvj.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2zdlnmtru.html


<!-- 参考信息 -->