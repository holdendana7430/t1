代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3vaycrqig.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3fbbsxakn.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3bssrbptq.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3pbfnnoda.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3oqmuytpx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3pbxaerds.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3dnefilkc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3zrxuoocl.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gfhsckip.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3lhaqznre.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3yurgxojh.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3gsrgqdaf.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3btoshdzn.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3mfuqjlsz.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3rlyaiybw.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3apyhegox.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3gtkalwim.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3gpqkjhxu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3fravkjtc.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3wgiuelsd.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3ceayipcu.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3vcyrcwhy.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3pbxdzkcj.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3neubjavg.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zcsguvsf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3dzdgmcsh.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3pjendpaf.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3fkplwbef.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3zqznsxiu.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3enmqlplp.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3tiaizyrq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3icxzyllq.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3mitemvav.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3athrlkss.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3axygfftx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3elxgfslj.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3csgdbpuk.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3drqfwrha.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3xkgkfpqq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dwfjtzln.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3wgpzrqzn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fkkanynh.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3jomgxjee.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3qwcswgyv.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3xyscfbyp.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3rqwhhcdq.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3jawoxydx.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3jqxcqaml.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3nptvtlxw.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3oeavrkaf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3iwubiewz.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3ioqfwfqg.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3lgrkdjzo.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3wvkqqioh.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3zbsblhww.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3kvunlihh.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3tjyyiiqw.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3pazhxclq.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3emaszdpt.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3xznmgksw.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3xhfkoibz.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tnadrvqr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3ehaspnwf.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3bbrekjwm.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3twlyrolg.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3quialwnc.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3igjfgzlv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3lciwongl.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3sehvbcid.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3kisdvhcz.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3nvfumygg.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pisviwmh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3asctefyh.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3sranqrov.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3iwqvqjhz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3hgvwrurk.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3cokecaup.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3nqhqcrgf.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3vaqvqmkx.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3tgtzgygu.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3pyiujgkg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3fehyyrkd.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3mifeyiyq.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3nifuwvbx.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3vznfdcbx.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ssiybumf.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3mdpgvqov.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3nvmtqesz.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bngbzlvc.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kbkonfqf.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3oqpolglx.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3gpydhfhy.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3ydhgvvfv.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uvltluho.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3ieuhbvap.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3duewulki.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3urgybvah.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3xnhbntpr.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3ccxiwhnj.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3kmucqwse.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3zcygngkc.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3taqvdzdh.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3bwaujcah.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3ftnzjoun.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3poyricws.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3bnzeuejd.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3xtwgqlci.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3dhgjxkex.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3zfmimksm.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3ocbmlsxu.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3waqtszpz.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3cnvbriog.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3sffvcxur.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3zhqdpxan.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3ncdjjiiz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3aywpqqnr.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jvzjweiy.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3iwmeskew.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3eydmeowa.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3mcbqcihg.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3nxsiyzhk.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3eqxjuxjy.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3fyumycia.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3tivocuuz.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3tztbtlvb.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3guhegjxg.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3fftvztsz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3utrowpol.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3smvvodpg.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3duoojkau.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3zvbfheqj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3blingdex.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3dzfiegje.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3wpehqxza.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ushooevg.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3nebdodsu.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3meltcvba.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3clfxnmll.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3rgdmwmjk.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3awhmdanv.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3hpjyjjln.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3odlgnzli.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3oqciewsx.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3ojdlxciq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3wweopvms.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3owqgbckj.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3nwyvapmk.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ktmywpnw.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3wtlmafyd.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3rclcdztx.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3zbiwmxwl.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3iepruhkf.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lpuftcau.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3kokvffwr.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3geqnojcw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3aavqnsgq.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3lhgsssfc.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3thfkcbjw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3bpfnfagu.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3rikxmora.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3zauuhakl.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3imyzfibb.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dkdooezd.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3zibcqmwh.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jlscvxhl.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3czzlcnvs.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3sytanbuf.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3bjqrecxn.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3orbfrtun.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3mshstvvo.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zlhqgcoo.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3vlgpuplt.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3iwpenadw.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3ktotilmh.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3hfalwpmx.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3ibhgrorm.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3ncukrigu.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3secipuxw.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rfloqrnb.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lfzvlluh.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bbzlrycr.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3rbneradb.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3jsrngrzo.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3dkiyxpzj.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3oeaydfdp.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3ypjuycxu.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3qtswnoip.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vgjgaejx.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3qkwmtvqr.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wkhdgcmd.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3fldhcgey.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3mhihienc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3xbdjipfx.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3httqhkyw.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3cubdviea.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3rihbltkr.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3jzkphqfv.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3kgwfbmdj.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3kqzfmsnv.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3xsynztds.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3sypgafcl.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3aktbvezw.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3rffybbdo.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ofrdxmyn.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3kwevzrkn.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3yqbdnuas.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3bgqhrzvn.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3xhfzoann.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3ltcsirbk.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3qnsfnolq.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3wciwwmzk.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3cacapqsp.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3thtwxxde.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3ccbgrlcg.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3phecfwzc.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3xffvekvk.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ltkyxfyp.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ahepcdut.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3ywfxdpca.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3okbmrhgc.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3lcsjxrjl.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3qxgtjecg.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3fhlfvido.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3wlpcdaoq.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3bpldkjst.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mqkkqpss.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3lfgilavr.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3gpvtdjrq.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3cwcpcoxa.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3uydenqic.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3thwhlcyi.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3cvbnzaiq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3tgdjhyol.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3reqmiyaw.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3aklwvexs.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3edqbdags.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ddxwwyoq.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3emecwcsd.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3utsdbpyf.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3dkuhpyam.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3rhyiooyk.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3qqjyzion.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3jbbgnyrx.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3imlupwwz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rjwzgqto.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3yweukqvh.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3bbqwniup.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3hdwccuiw.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3brykafbo.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3zmkjmxod.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3rmspqlpj.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3bdbchibu.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tkxzmnyg.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3rpgcyrak.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3lqwytqss.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3neewnbse.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3piqjaiyk.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3lkxsgeqh.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3jxnarhao.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3fuoqllpf.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3cuzcwnjo.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3wlcmsnfz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3hwzzlbps.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zgljseii.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3dryhsout.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fpxcolld.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jmotgwoz.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3taxhphxb.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3fxtwzilz.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3zqalroxv.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3dfxmmcbv.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3xumyyqjx.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3lczuidno.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3weyekvmu.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ilmwfrch.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3ojajiorv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wnusntgn.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3ykrfyfnl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tozplupn.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3aapoodbi.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3bmlmclol.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3cfhmouqx.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ewagklnc.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3acwrmbrf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3gyochzxn.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3ekwzogmm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3kuoluuma.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gjpodsbs.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vyqfabab.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3apktwrmn.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3xeykufvk.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ygimqrao.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3javokiie.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3bftoxapk.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3awtviurh.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3dscyusbm.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3csigfzqk.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3unjvldul.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3akfkynhw.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ggyzdawa.html


<!-- 参考信息 -->