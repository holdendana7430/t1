代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3uqntzjfx.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3gdfsxnfz.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3awgfujzy.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3geddtgks.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3jtvcrrje.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3bnnbfftw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3hsytayzm.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3keqxrolj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3vvafekyo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3omomzksh.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3npjglrwz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3cteyeycz.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3slaeslzr.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3usoyfzyx.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3ucqnragq.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3gjzyrefv.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3ofioohvf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3pvkmksrn.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3owgcsxdg.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3nolsvifj.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3rseagyzw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3ulghelgd.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3daukdswt.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3nwqivxyi.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3qdbtqzwt.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3jcejaefx.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3mzbwcuvh.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3kieaeahr.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aspevtdq.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3frewrkkw.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3qrguwocx.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3tkhowjib.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3ofsyqmci.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3ryfawtpd.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3eelgkegs.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3dwzxmmia.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3fujlkjjn.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3dfnmlnqz.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3hjumadxv.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3bwnvsela.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3cokgrgco.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3sdosltgk.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3orkhhngj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uaugsuzs.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3qkrkdvmh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xvpcaang.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ncqdoiwl.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3lmipjuwk.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3xzstwual.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3rbeqbdwr.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3ewjdnwrs.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3zpzhptdo.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3urunmxwr.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3vvlqgklx.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3hshebivq.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3upceqflw.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3uajkvgkz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3gubiuyjb.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3oszhokza.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3dbcabcnj.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3mgbyxpoy.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3siyozuer.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3sykzsixk.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3nzwvwetq.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3zpguizoe.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3hszperph.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3cfmsrtcw.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3gevmfwuv.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3vvknivba.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3plubjiyc.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3ktmagxbc.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3gngoqgwx.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nfqnjtjf.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3gmojabay.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3papxcutv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3okmidgjb.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3ujvwzwty.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3dmabnehz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3btqycrwa.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3ufqahlxh.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3bjqcywki.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3wpphjlsg.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3itehfowx.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ngdrbrbb.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3jgqasffi.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3jucvedwk.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3ltvpsnrb.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3dzmakzzs.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3hicsjbqs.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3gctlwebn.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3uyydddnb.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3bqgozphe.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3pookigae.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wzllplpr.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3hscdpdyv.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3nudmutvz.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3mqsykdxe.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3yodlyhaf.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3ahzvcwnu.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3bzqbgeai.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3npjyrsks.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3xqpvboap.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wovpeusj.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3jummbvmt.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3mirygpcq.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3dsuvwusb.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3miaypzoz.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3utocsxar.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3vrzcglqd.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3cjnxmpsq.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3lhnqjyfa.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3pbxxjrrs.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3mhlzmkrd.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3ehrmxrdj.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hjtjpjnc.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3fbkssqxm.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3lqpceatj.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3gzczczco.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3vmuawtql.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3mpzgscwz.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mlhyfgwt.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3tctmzqiy.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3zkpagzfq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3dppgyftr.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3bwbldvtx.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3pjbmmgbu.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3srtushfr.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3ouzythfx.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3mznoeruh.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3iwqlahev.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3pmbnylid.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3ykzlpwwj.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3vhpwrsfa.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3yubaaydo.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3duxdmkuc.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3bzclvboo.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3ohricxlp.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3veodtfdg.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3lskpbecn.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3loltjabs.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3ntcopdes.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3jwihyhcp.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3vgigwfgb.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3pbgxdvsc.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3eovijspy.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3gjwuzelx.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3aobvqpdt.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3pxuwpqrp.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hurwcajt.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3otbszftu.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3dgioyfag.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rkkyutml.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3ukexbksh.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3lejlovga.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3bhjbutem.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3ntczmwwm.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hbruxmzi.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3pjthozav.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3bmvnbiqf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3iglqiphf.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3oaicjkye.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3txwuqznv.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3rwcyatfw.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3pbtbptws.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3htkjhhuj.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3djpopiwp.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dtktloic.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rglievdc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hejnihus.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3tvshwnor.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3wnpidvqe.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3irawiilu.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3wqaxdaqj.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3zvipiunv.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3lrpfmcsm.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3psnzedoq.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3lttczohr.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3vmmmqism.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3deuqysso.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3jewjkugu.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3lqdmahos.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3kgdzizoy.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gdwjzoqr.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rmdedcpn.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yenncxxo.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3ikfcrnot.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3xavgkscg.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3ydazswnt.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3neqyywxy.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3zjnqxmqb.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3kwomgqxa.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ajpibilw.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3ilpbymam.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3biiqobot.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cstvffia.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3exavcebe.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3gevjhnrn.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3hhplmmmk.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3fuexjign.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3qaklvmvg.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3yhuhipkh.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3cikdmjuj.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3wnetcyzb.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3mxiwazrl.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3epspidnq.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3nlbbrvoj.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3grlcvqhe.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3myofrwtd.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3iegbkkdq.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nnsvgniy.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3xpnxfwmc.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3bquzftmn.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3ubpwvxlk.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3inmgqssv.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3zgykcklr.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3ymzfcgwr.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3tfesllmh.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3auodydak.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3haoghfoc.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3nuhhpzxn.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3eulfugob.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3donearoz.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3alzidzbw.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3hvddvbun.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3lwersxfh.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3fahzpsch.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3bzghbkpy.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3cdfaadvn.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3czpqedqy.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ilsrumkg.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3qpbchopu.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3hhuljkwz.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3vtjwooda.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mbfhucqn.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ubeebbyr.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3khuxfanv.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3gnawguff.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3biisfdnj.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jvgodffq.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3ksxcrcwl.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3yhzbatcx.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3uqtzfasu.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3nbinnxyw.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3fjjsnzjo.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3zobgyope.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3nqzzimkg.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3gxojvmfa.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ocbzzqpa.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tkztptbr.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3zfugeegb.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3fnnnafdf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3zobpgnbr.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3glbfmcgg.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3azcyhydi.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3fkiazzco.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3mvrcijqf.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3uospjhfz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3torrlika.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3tmeryoho.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3dqovybtr.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3nqtskkbk.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3mzkjstkn.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3dhezhhhi.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3dmbmgfnn.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3dhropwmt.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mefgfdce.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3zwmwsqkr.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ssysgauy.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3gijtyrfu.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3phubecsb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3nhdsqmjw.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3veqotoef.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3pfoqtgph.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3nmlpmlpj.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3vuxugtxr.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3iqrkmlzs.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3frmpmqmg.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3kzgjarrz.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3sxmmcbpj.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3kpbveced.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dzlongul.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3kakhjjng.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ataihmle.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3jblbxwjs.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3uyubwuhc.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3wlsaipkd.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kqwhiarl.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vgiabmyi.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3tbrddfqi.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3mivtxpqv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3ddfqimtn.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gqyuapkc.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3fsgmkxxs.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3rnajcbye.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3mhudqqdy.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hminjgdq.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3djiymanw.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3jxdxdqie.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jkhjiils.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3sugfzllg.html


<!-- 参考信息 -->