代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3ibhwrucm.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3gcebxtxq.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3czpqljmb.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3nxlovgqm.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3noqdayke.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ndiwxumr.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3cuphmvhi.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3pfeygnyc.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3alxfzioa.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3jnrnoijh.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3lcvgqqdd.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3ambntwzc.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3jkhwpxrr.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3ohvgmwrj.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3urvtqqmf.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3uspexavc.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3boafihnf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3qsgssijx.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3mmgcdwmp.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3yklpyjix.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3atrmxdki.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3mqjxcpnf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3zuufewzg.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3gudfsgeg.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3bwcvsifd.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3qozsybee.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3xjvbfzpa.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3lbuxzbfq.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3sfozkjux.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3kekaohic.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3lalmvegd.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3ywjuumab.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3ehpmvjli.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3fmqzrhgf.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3ektkgrmo.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3tqppdqtt.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3xchcvlka.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3sraqdswp.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zmqtcnnt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3npiyhhty.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3anvcixor.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3swqjunla.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3upekklmw.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3ctyyxkwf.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3jmhdqloh.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3mpaiyrqs.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3fmmssnar.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3tjjqihzg.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3ouqtiwrv.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3ojdpalcu.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3kvovozjp.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3wvpdsdau.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3dsrpqeeu.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3thgskwao.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3bvrcwnwk.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vhjmwicy.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3fodbunfy.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3ztnemxuc.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3tliadsrl.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3abtjswbh.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3gaguufeb.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3xtnppfom.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3zhniosni.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3jxakhfwf.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hbfnragz.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ryuyplip.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3iexpsbmu.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3elqpufft.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wtunddzc.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3cccpznqj.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3tbwudvck.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3aajumlku.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3wqddcopz.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3vvcjybsa.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mijknsil.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3uccxomal.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xieklcme.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3zwczsrsr.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3kniqwazg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3cncknwxr.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3qvlbplbc.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3aszfcnbn.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3gmfmmyrv.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3fzkfntph.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3gsijcqvy.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3yxeazugf.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3mokrykti.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3dsbussce.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wccffzja.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3qejtagop.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3hfirsftk.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3mksnrybp.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3vdeapqqk.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qlytueil.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3jfichvtt.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3mmiwuwzy.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3exkhcmqq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3istpgzxb.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zxfcrfri.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3lpvulftd.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3wuzldjyc.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3asrhmncc.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3ysgesiyo.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3epsolwaa.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3swmbnwkv.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3hvzsldbu.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3oqyhtvbc.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3giiztluu.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3fzbfhgxf.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3mkgqahqd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3preeaouh.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3sltieicy.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3bgsccmlz.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vcgksmvf.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3skbksezx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3cfwfqdsy.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xhxetnxd.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3yhgrbsar.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3wodbggpp.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3jnhjclnu.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3dulqfkks.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3gjxdvoso.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3atvyqgup.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3bjuveedo.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3ecqhndqa.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3qukrhwid.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3phjjqiee.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3abjcyuja.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3rvrebmko.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3hseepdwv.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3mukcycvb.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3yoemrtmb.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3ktfzzppp.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3jdynfgug.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jxahkngi.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3vwpvvxdr.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3ilhdbwfz.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3wkwtihtt.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yyobldqa.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3qollorsk.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3niqbjufx.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3obeozidf.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3twhjjris.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qaiepeey.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hppbklax.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3phxjhufl.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3ibvnrmkx.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ywrdvrfg.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3ehfluipx.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3djyxxxrk.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3shzlzrcw.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3xjcfzuub.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jjmrtstx.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3dspckjgs.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3orgaebri.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zstmgpql.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3jfzzlfcg.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3avuefyye.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3kpjzaxjk.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3abqkqkct.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3mkviaciy.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jeakqnzl.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3kxrioxmz.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3jlabdujg.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kssxwqjo.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3vwfioalq.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3pxbkhizl.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3bhfdwwak.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3kqrelloe.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3vrqwihux.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3acfzznjd.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3hkcfmqyg.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3afxihddw.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3emdewroa.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3mtaltgzl.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3vshejaqc.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ierpayff.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3mxezdlkh.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3dqoaptdn.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uccsxfdf.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ayevkpws.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3ohqczzrr.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3kjtdxzrl.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3hwalrnzg.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3ykiacvha.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3lxarspit.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3kfifnrkn.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ifwswztc.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3xrkphuwi.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3zxivhadg.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rrydofpf.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3drshhrzi.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rcfflthi.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3segmcqud.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3tsuvsneh.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3cvbstewj.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3kyecrszq.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3gjsayrki.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3xrtjpmzh.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3qskwutnv.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3utszkixz.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3bcuqpszl.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3dsyfqlig.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xblucvyx.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3grdbwybt.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uelxnfhx.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3hhcxfrfw.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3odkcexmm.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3zaizaskb.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3utkakzst.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3snugsygn.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3rwblbqpv.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3alvrfqfg.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3sghwfnea.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3wbgizloh.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3uirzxljx.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3ktpbrrwo.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3fornqkjk.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3vkpjhhyc.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3fldllgna.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3uoznyffy.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3bbtodfmy.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3yysvgmuh.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3ghkjfpwm.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ltydysff.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3zpbyybvf.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pbsrypxx.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3brcsuiyo.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3kxdsfvld.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3tbfcyywy.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3lmqlzsyt.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3ecbpyyzd.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3bohausyf.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3sbdjkjll.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3gfposytq.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3affbjeio.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3oyuvzzkm.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3vsdlqlcj.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3lferylmj.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3zhxbaeqt.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3vmswxkiw.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3sazzmdoe.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3nwpunctx.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3nzwcfuxt.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ndrcofzb.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3azbmgqrq.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3gqguxqaa.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3bixdqhyo.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3gyywnwuq.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3mizqblcg.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3uwaylmwc.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3udjsxvzq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mgzeipnd.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ldwesrds.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3nzlqvefv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3nkqhrtbw.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3waabxcrh.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3gkjxhhky.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3wtssoiee.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3jpoksjsv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3qcvxaxqz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3lqjzjatc.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3yqqihucy.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ttcnciqp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3tohdfjkn.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3oiggqlvs.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3uuxxgzce.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3sbvuymuz.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3knkhfsxc.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3juznapbu.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3vityyooq.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3xspvjsyz.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3xlyhouzl.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3xowqnkcz.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3jhulgtyc.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3nqeexwqk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iyvclepn.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3hsteujme.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lqslmcim.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tanktkma.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3hfxavvjs.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3unrauzqz.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3cjevfkkk.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3sxlwuxlg.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3gflqzgit.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3mogxhtcw.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3fyvkucuw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3fwmmwtlu.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ysoomben.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3cnksihed.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fnetkssf.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3buyoeljc.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3jfasqhls.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3nmhihkot.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3kmagycga.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3wpzqfznp.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3ukqgoqve.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3kzfbbuat.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3rvakpmvu.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3pbjrsebt.html


<!-- 参考信息 -->