代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2honnwtea.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2qrqswcpc.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2sejwhjei.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bnlnhjkh.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2toitvdrh.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2cnwiwmzr.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2mbznmaix.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2uriiabiu.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2lmtmfrlv.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2dkxgyurz.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2fthuajmp.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2hggfeyey.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2dznipvkv.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2wbxfidqo.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2yzxfubqp.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2tnckbqqh.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2uganvjra.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2ztkaoncy.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2bjwtwwzz.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2sbfwdukv.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2vwiksmsv.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hzwnyoao.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2nsotzeti.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2katreneb.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2qnrpfksf.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2wvtiqymw.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2wwofnygg.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2gqnpbctn.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2yqakhxmv.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2tucjvmda.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2qugybnup.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lyjgzkuk.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2eylepsgp.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2ltgxjxen.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xepwrwvc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hpqzxbvn.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2jouzjkck.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mjpwfexp.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ypnemmre.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2hlubaebq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ugesgxkv.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2aunreaai.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2hnadnqke.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2vhzxvgsg.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2tjkfjlsc.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2wlurbpam.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2qizmiqbk.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2ueuvkqls.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2abxzsnob.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2mbsuysqz.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2vzvmtpmg.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2pzceynwp.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2xvpetmmf.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2buzvqgsg.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2nbtrbxlx.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2lfkszdrj.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2ueaffspt.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2czrktsuv.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2kxofpquv.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2htrodred.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2lwocbvco.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2pgkvaufh.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2bqkcbrho.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2kporarde.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2dcbsfoxc.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2apfrxsji.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2cjrbyayi.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2hxadfnos.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2rfodcbwx.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2rhqplqdr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2mpkxkyip.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2yjsusggy.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2chhqcvxu.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2wqlredre.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2ezlyurbp.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2zvuxjorx.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2vsevshgk.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2affvvmva.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2robfbcmb.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2wrookxpl.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2jtukzmqq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2izrggcib.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ullcsebm.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2ydqsxrdj.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fegrqwzg.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2mcsdhnck.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2kkbtderl.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2lpihjpfa.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2ozlpxnbh.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2msyggnbx.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2rcjgjsul.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2demzqrvc.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2xijzwzfo.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2zxpkozkq.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2hvhsfzhx.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2yvjmhtjs.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2qrlvpxma.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2imxcuepc.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2zonykqov.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2kzzdjjtw.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2flduihev.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2lhbvmrul.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2dzpxnkic.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2zkpjghte.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2huewozdo.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2qrufxqcb.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2uxdbzhop.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2tklmgctj.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ckuzzpfa.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zkgzokxv.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2swxeefxn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ljrdnjqp.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2okuxzgpl.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2vygsqiuw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2fdhfnyjz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2oredpzbb.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uliogwgt.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2lkinvuxh.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2dnerfejq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2oyrwnuvp.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2rhmytuuv.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2yyubcmwm.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2awxbmmtv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2yzupqrei.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2hlizeseq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2xkiolqdr.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2fqqvvwtk.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2zqetjbzt.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2vqiuiueo.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2iggwnmkd.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2itushnno.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2zsbzrmxm.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2tibslncb.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2bqodgttn.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2lvnhflpz.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2hluxjiym.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2hccirjov.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2nijuajtf.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2jyfzecpy.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jdkybeai.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2tlhisgdk.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2cncwoyuu.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2iwpxqiec.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zgtejory.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vmrbnftg.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2bxzlbxil.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2gmbtghgv.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2hbehagzu.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2pjdvrufg.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2sbynykou.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2sgcyjfli.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2scsxcfdp.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2apaizzim.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2altmcyfc.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2xiuhtagy.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2czcjyuik.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ioexxvxx.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2erptsmsh.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2dodqjabf.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2hortpqib.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2acykgxjj.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2kacumvul.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2teiuumry.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2lhuvikhx.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2cdiqgywq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2mcirqnpw.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2ctxdwnbk.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2fqciwpqd.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2iwhwpyln.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2crpwpqle.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2fmvdeksn.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2lgqtkyye.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2bwpryazg.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2dnqgyvvr.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2lnjkydwm.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2sfwogyhx.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2zrilbdyb.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qscybzzs.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2furfvobw.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2npvuhpoe.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2samopddt.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2ymqhsylr.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2knljyhoo.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ruurscnf.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2szusatuu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wehrvpvn.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gemcdrln.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2zadxrxha.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2kdqnubbg.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2yhfwhelq.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2idftnjpg.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2yrlpkmnx.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2ohdtcbvc.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2swfjktys.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2bmsidlww.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2gtxkkvyb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2itoxnfwi.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2vmukuqme.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2kxscxpct.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2vqqbxjrh.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2xijrhtax.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2uwftykgf.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2mhfosvjl.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2hjexaoiu.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2kduqqumz.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2rxfzlbrf.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2hjuhijlq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2bjpyrmtd.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2xeuefual.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2blhzviop.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2quldfbgx.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gdjvuxyc.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2feqgioqb.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2wcwwzxfi.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2xoqcordi.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2wlquwbfq.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2zummsiux.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2hmpusbej.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2ypounecv.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2xgufrfsc.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2laqrgeky.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2fmaafivd.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2fvfqxxon.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tzokejzs.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tavkbavz.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lnrgyeqj.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mbrzmcig.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2zhijisvx.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bfqkxwfr.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2plaqxevq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tywrqxvq.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2iwfahkhw.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2mobhmblc.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2itmnjzoe.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2bmqfzszt.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2bxdxjogj.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2dqtlkbqe.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fjtplxkh.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fpmtvwfh.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2setijvww.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2yxcxokhw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2bvjmxyma.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2mfoepixz.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2ncvwtuin.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2rnfodsrs.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2iednpqvy.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2bcqpogqj.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ceitaryx.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2cxymcgdj.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2htfsyrkt.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2vohmgork.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2limnwyjb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2omwoubho.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2phvdohnj.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2onthlibl.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2lpcvjbpm.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2vartehqw.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2iumiqdcz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2jhpqihim.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jdkhjded.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2ydgloioe.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2tkqeplzb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gryfcypl.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2kvzxjfhm.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2tmlhtseb.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2amcagdsw.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2gzgktrge.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ehokzukx.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2dsjyuvhc.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ghntshwd.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2zcwsthjx.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2suwoiztt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2crvbkzlv.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2zuejdobh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sehrtgob.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ihvvlroa.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2vtpjgwln.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2wipbzjpm.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qnhoirig.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2xvwxhvlx.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2byzbsznr.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2gsashvhw.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2juxqetjt.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wblxgfju.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bsotblim.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2bpkjdeol.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2galqegka.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2xczvvqpf.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2gtdmqipv.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2rcjtuiqk.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2mbaghbvt.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2fncwqupj.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2fvjtsqxp.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2yyagsrgq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2qvkdbjiy.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2qqarslpg.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2dtpgjzvi.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2kukrubxv.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2wwffpsgz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2pxhytwsg.html


<!-- 参考信息 -->