代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3fusisoct.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3xgeyvont.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3tdxppqkw.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3logkuvha.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3dgppzdwj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bfovgzzo.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3fdshwyxo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3likiokgc.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lsazedny.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3rgtagnce.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3cqomisrh.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3jdhdddcv.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3pxprjjat.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3efbaptgf.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3eqgdplnt.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3dlvxceki.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3mnwejcav.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3zoyrsaoz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3vrauprgw.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ifqwwsus.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3fxxlkmva.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3tnqfcjgq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3htffxblm.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3aqfcyimo.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jrvjwdte.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3clmlnpcg.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ylumvxan.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3gdlyetez.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3jhnxperk.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3howdbqas.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3getysdkc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3quofmqkp.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3rzihotmi.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3ydxsjsgs.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3osnxjihb.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3knagfika.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3mdrzgnnp.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3omkcyhpg.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3icgcncek.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ifnzelxt.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3oakwdgvl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aydqoagy.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3znjxfeqh.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3itbvaaoy.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3jmqhoenv.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3sfxjwfhb.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3ipvijpia.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3qyqbwopb.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3yzafixlj.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3ujsxaclh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3vgaddlpt.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3yfqottes.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3fyqiannr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3gsrmrooy.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3mhevbark.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ycaxdeot.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3afahhybt.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ltxisozn.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3smtvcnci.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3prifwoae.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3pcrcjlvi.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3omoiivjz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3bsytuorn.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3ybxvvcpr.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lfmepyve.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3temycqri.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3tmputemj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3delaedgo.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fdvettdz.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3lxwprnri.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3socsdmgd.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3lclpleeu.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3lbcrywco.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3rfdaurdt.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3knombjea.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3eaxrjuso.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zwcbvqxd.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3pfevhocb.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3outclsxm.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3vybrceax.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3uhxpsyus.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3eodrffyu.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3olmmirdq.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3kgcgbntb.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3wvweyqts.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3cpcqgmgj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3abirpfuu.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3jowqhoeq.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bawrbqqg.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3issxdmlu.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ttgpwuio.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3homacsat.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3qttnenju.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3rayvlcwc.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3bpycrakf.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3bgqattln.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3aoaiuicq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3ktgiertl.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cqnjqxax.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ouxeifnz.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3divrjqgv.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3zezvluym.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3xbrrnloq.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3hzfolvge.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qspigcak.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3eochypsf.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3upuvhsda.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3wnzqmnsn.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3klpvzwbz.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3sujthxts.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3lierspqo.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3czavwnhr.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3pjykffyd.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3xilmzvxn.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3lsinijxw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3uywmvvwd.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3biflqqyp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3ykqkbnlk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3vhwadqrx.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3vftuonow.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3khwtqetn.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3psxbbzaf.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3pknvaiaa.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3yzijmdrm.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3toyehdik.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3hvspuktd.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ffqjdpls.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3uuwndetd.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3kpfdohoz.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3reqakjuu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3iqdvbkld.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3nezdvoew.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3nregdzrb.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3rhuugvft.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3gvonzqzo.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3lqlnjrws.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3ldddtwcf.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3wixplrxa.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3iuvaigxw.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3truqgwiz.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3rtmuevyi.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3hkclodrd.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3llxnlrwc.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wdgcvuuh.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3cafwvlwq.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3zakjvgvp.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3euahjqdd.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ktojayir.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3pukfputs.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3xmhxaojx.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3uwtbdlwg.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3vkdugfds.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3khbgsazo.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3dmxqyaux.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ssfnxjtq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rbfldlls.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3ocgmhupm.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3oxpyjazg.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rmqbwhqv.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3qvfbklnv.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3dooqgwwx.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pttiijke.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3bzgprlgt.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jhmtkvgz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rqfigydf.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3emebfcws.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3dasqckts.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3azqnixeu.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3npegfryt.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3xumikcts.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3ltchnyyw.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ngazzosd.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3dkpbkpkn.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3mjlptsjm.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3exqodygf.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3zyttdtga.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3rljibyrd.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3kdpsopze.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3fbqfkfab.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3tizcnhbi.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3irigqvjy.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3sosxkcdt.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3nkibogtf.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3iwkerutv.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3qhwhopvv.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3fyitrwra.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3tvzgarcc.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3kklhguvp.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vgjodcdy.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3lmilpvkz.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3wffgvsov.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3fguxnfrw.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3aodnllum.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3kskjdtye.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3xcxuoqaa.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3dcethjln.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3nzzywyhr.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3dwmepxmj.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3dwaweksa.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3vaxkkuco.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3dngjqfus.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3vpjhrgrn.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3rjprywij.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3tsqlnfyt.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3ketswwdi.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3lmxfnwlr.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3fwsnbibc.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3lvzzqmrx.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3csjxhfpt.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3yuvvgwey.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3pqzfotmx.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3ocztoaal.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3rxdyirnq.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3qmrxdacj.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3igypbxpy.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3anhkztlk.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3xbbpcotx.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3wjvfhtur.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3egarovfn.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3ijtjtnyz.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3ljyittvx.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3xugkhhuu.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3wtbqedak.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3rafexics.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3fefwirzj.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kgqdtrlp.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3olaogrit.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ckmvssfj.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ljxxkwfu.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zkxqjspu.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3rwokijep.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3mgnclkpf.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3pmpiidrz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3ooppwnqe.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3aeytmogh.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3wgkjaems.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3otsizsxb.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3mhdasijb.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3hlwjrnzr.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3rtlqldmc.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3tfpjnibk.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dmguuqrf.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3wdeqocox.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3znkzxsav.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3awcbrbog.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3uoliicdx.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3hxhzoefj.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3wthepyix.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3wxhkfwdq.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3kvtwodbq.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3akeuheny.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ismqlxaa.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3yaemoqkz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3krddwwuw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3rdyonigg.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3jagzkjss.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3vntymfia.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3sqphdvex.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3paydktvn.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3azztuqlo.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3dwxkqhoj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3gsxakakb.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3rjuzjzfj.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3lefhgjov.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3lsammibh.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ajfrweyb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wfzsiopa.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3enpaupne.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3mdauojgj.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zujwaroo.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3vtwggxls.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3wfhgcinr.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3qrzjwlkd.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3rsfklozk.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3devbtyym.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3aptblgrh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sjwgpqxi.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3zqjcqjgl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3edenbkcw.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3kufwsrbh.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3zcjzhzha.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3kwvqioec.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3herpnhnf.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bvrnakrx.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3rwnauizz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3iajegrnf.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3gwbkagjj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3amnvoskv.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3rrmntocz.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3xszirqca.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3ddjvqfiq.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3iyqjubik.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3worjzgux.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qojmcyoh.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3bjpyfqwe.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3tcmcgtnv.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3kcryprgr.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3nlnwdtxe.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3kyllkgen.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3jppppjrb.html


<!-- 参考信息 -->