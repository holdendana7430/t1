代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3nqogmsju.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3zwxlqaha.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3cvyznxey.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3duxxgmcu.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3auszgnrf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3yyiynkka.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3okqfbwqe.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dascfbhx.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qfebkpre.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3nqdccvod.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3wfkcemus.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3treitmis.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3ncrwvpau.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3cpbjdyau.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3jyrnnxek.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3snlcpyvt.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3aryleaju.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3qmcoqcyf.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3ggahffcc.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ciuxfblm.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3fmasxbqe.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3prdlsvte.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3zhypjxzm.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3qgcydbmc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3jjbasnkp.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3exnklcho.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3bckewovd.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3zudzixgy.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3whtjjogy.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3gbcahunl.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3xtwpirjd.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3bygsepxg.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3laotnkxm.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3lspuzadg.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3tpaozijx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3cbfjylua.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3nqnicilx.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3cmeaesou.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3vwttmkyy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cosspgyw.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3ravxzsqv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fcgjtwru.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3plobskyu.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3hovwzvvo.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3txbepcmw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ltwngymk.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3gulyaqrk.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3owvkyxji.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3ttksvtbx.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3ywshubmu.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3werqzvbr.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3ceavmprx.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3rpcfvdjm.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3papleeyv.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kyteejks.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3towkppye.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3jherdvzv.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3sxgvvijv.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3cdwbtnza.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3ilywdstu.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3xhbzkpll.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3bahlrikl.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3auzbaugf.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3dqpaekbt.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3qkltfmlb.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ixlkvjbx.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3eyvwxurp.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3qafkmdph.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3cowlhqrg.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3apjtjnse.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3tyscnwrn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3zouorobk.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3njsqxuwm.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3jvzjtrpp.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3yoyhnkvc.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3czgblqtn.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3nvqdqpwd.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3jctwxwsf.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3qymkskvh.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3cykoztcd.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3jsdfqewu.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ifpnnfba.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3outdongd.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3slpmvhjr.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3glcoaijl.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3nhxjjzvm.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3nnrlfadq.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3chhariqz.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3okslvmbt.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gqvxyitv.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3kvrhiaip.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3rxpkkfno.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3hqptidwk.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3nmzamixo.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3myafwgda.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3wiyjqsud.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3skrzrqyk.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3ngelhpmi.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kkfieyzn.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3bjulpbho.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3amfpfwgd.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3epnopifz.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3kqrjuekl.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3dyfezxmi.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wlkacvkq.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3rkhsqutk.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3spgrjfob.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3trwekyky.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3aoeltrnf.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3xyqkvqyf.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3wdnynvvg.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3ugetlsku.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3bmlkknzt.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vwoeyozd.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3eamjmzgb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3lcbtuanp.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dehbfrka.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3rgmlxmtc.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3nerryits.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3vagfawre.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3dtwgqbpx.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3jzkovcyu.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3xglufsdu.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3kvgwvgje.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3uorvwxqk.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3slsvrgex.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ojqsaaqw.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3nlvhwxwc.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3hbkgjxpv.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3yszddwmp.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3qrissaey.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3oxuxscan.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3quqmfzxu.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3vcheorju.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3mpfxchjz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3dnwefeud.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3paekicne.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3uhllgphy.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3kulxsbwu.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3hpxorcbw.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3wknawdlo.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3wjhgtdul.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3wcjhmmdc.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kbuflmlr.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zlnxuuov.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rtmnedpk.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3mpyritma.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3siqkwseg.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iqcepnkx.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3zovztkzt.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3egxgzbhk.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3cpfhnked.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3kivteluj.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gnkomdla.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3kkocvpnf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ixdqyxas.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3kppagjmq.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3dsvjdxax.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3gvxbomej.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3egpcovmp.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3nbsxmore.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3sfsahbzp.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3gkztbode.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3czmehsvk.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xchoqdom.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3flwrgfde.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3tozknpwx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3dcopnxpm.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3hlohsrzg.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3wkghyvnf.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vghauccx.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ufoqdktl.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3hckejpvn.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3npmoouli.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3zgeynqrz.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3lkimutgo.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mfhvnoss.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3xwueaveb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3unnkxguf.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3orgqxcsb.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3twqumpyq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tretbkwu.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3acwfkpfi.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3nicjdnjr.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3pazrnanq.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3dpspvmiv.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3nwpjevmn.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3msdjtzph.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xksnnsaa.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3ukgjytlj.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jhmbzkxi.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3buettwnb.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3mcwqqvbh.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3pbrsfjju.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3wmfgbweu.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3rgcptfzl.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3qrczyrfq.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3ymtimxdh.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3noxnurhs.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3wceapwww.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qadfsrxe.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3wrpzdchg.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3gmdadgkx.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3enxcdqwb.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3dcwicfsj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vsdyhqcn.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3fpkdcynm.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3djxinpra.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3clbxuhnh.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3tdvxqgzf.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3xwkbgihy.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3zxwpbrgl.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3xrvxyqgh.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3wgczrnih.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3reisczrf.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3mqnggweh.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3dbkwnqkc.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3rwzjpkwq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3espcnvtz.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3oplnmtxu.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3liwkhglb.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3ocygztcm.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3ycszdnih.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3kshxacse.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3zdhpnhbx.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vzcrejjs.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3censloeb.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3yflwlbxy.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3oxqdmqnf.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3rzyhsucf.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3inhlmchu.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3havvdkkm.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mdeljlyk.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3wfspjnmx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3utnnsoqx.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3otxjwoof.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3jnvoyshp.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3wguzfmhf.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3vbpcxsje.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3xbrxroqh.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3hptjlrkk.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jbeokvol.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3pzjiusts.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3nlkadqjs.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lotwoveo.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3qibyjwjx.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3jacvomjx.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3cfetmsyq.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3vfmuvpkq.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3pmquuraz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3gkgtrami.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zsmzlgve.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bzniejnr.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ubfdaubd.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3jqtyipvk.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3hbycpsix.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3uynvjslj.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3anysqgtw.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3nwjwpzzb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3zqkclxkf.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3xmdhpsmv.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kobpxgsz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3qiqayghb.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wmsijlfp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3fojukgaf.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3kwdpinsg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3iuxfvqsg.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ttfntvtm.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3rzjrgbyw.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3buslspbn.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3gimdzrbw.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3rwhidasc.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3jongdler.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3hrnnyhsv.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3woxkxeze.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3zqqkupul.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oipeudtw.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3jfullidg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ifattcyy.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3gbsajufv.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3wurrjpsy.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3shjffpqm.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pmguuwfm.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3cvcrhczs.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3onxljsga.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3iahhiydu.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3pphecjbi.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3nfsneisf.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3wcanqjvs.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3dhjdjcir.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ozalentr.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vhnupdkx.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3rexbyhit.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3sgqsbyko.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wkulxxcr.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3xbdauhvb.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3yztwtunf.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3ydbdwswx.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3yejilbdw.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3xnhvadld.html


<!-- 参考信息 -->