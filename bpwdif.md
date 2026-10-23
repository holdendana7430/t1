代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3imwpaxic.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3snvumrsf.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3qatudajr.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3rtyxhhdp.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3bytvtmzg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3mitebdww.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3ebgsdpfh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rybzzcrg.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3jhwianfv.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3dycjnrxn.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3xwnkdmbe.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3lmjaqhce.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3gcvxoaas.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3wicgokze.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3wlnutsgc.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3bthzebin.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3mtcapvpr.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3gjnafaln.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3hbqydpqp.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3lqmqhfdz.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3pwposvoe.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3ohdkudnc.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3yeqkkgeg.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3skobrvix.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3afzsbrpy.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3rdpfracc.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3cbqbudno.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3rtcuzrar.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3yhsstpbq.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3oaapzcfx.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3bxnsciym.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3okcyyldq.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3bgtkoglt.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3krfahxpl.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3grvfcukz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3zhixsjvz.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3vdmemnwq.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3svcicgiw.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3ekbahdtv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cydykbqt.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3rqnngvdg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oblgfyqm.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3fivlsyqq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3loclwily.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ittgrmis.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3sxhptuvm.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3tiydwucd.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3uqsvsxem.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3vjzaswmo.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3czdcypyf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3ffgdyjzl.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3wprzmiei.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3nfpanixd.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3qjvamorp.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3vxjrmhtq.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3dghjsxpq.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qlhhipln.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ckgyzyvb.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3lmzldhvk.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3xtxowcuz.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3sbonlxbl.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wgyvmsud.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3gqainwwj.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3pxyhvhqc.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xaysyeao.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3dxrckbdr.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3qfztxemp.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3xwnwthjc.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3liflgcnu.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3zytvtjlt.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3nujnfsrm.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3ddstdkgg.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3cmsqnoqn.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3aqlhdlvl.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3uujrmyav.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3vuzwyabq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3iuikutak.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3btdwmnae.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3aabtmsmv.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3xsiqjcmu.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3vhyohtsb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3svsqkclk.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3joerskwl.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3jusijicn.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3mplugynx.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3xpuvhmrq.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ovndcmvz.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3lopzwkii.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3jyuzjcpk.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3hcucuset.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3fvuidewu.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3bjgidqug.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3poyqnzlq.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dvmmrthy.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3fsrgpbnx.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3vmdusaxw.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3mctqvjto.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3scnwlvpb.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mmfyebtw.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3drtgpjjk.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3cggihsmr.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3jbgyzmll.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3milofins.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3luswubbu.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3tevixkso.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3fnpvsekh.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3kazowmsd.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3rtzikago.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3rekmcrzk.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3atevqyde.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3siynkkhe.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3iojihaih.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3zsmhksyj.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3pwrukzpv.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3omeqafej.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3noqczwsa.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xefqaxpf.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3iipuvexz.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3tvfywqex.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3ckkrfqwp.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3vitruhxm.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3skepdqce.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3chrqgrhb.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3bqkbvfxd.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3eqjizunf.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3htyefkjm.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3gteokbij.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3mounebxe.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3mzsdabtt.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3vpajytar.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3lqmlvcam.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3gkkyvrgw.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3zhotwftw.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3yftozmuo.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3krhujmtj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3xvrqbbih.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3yaleqceo.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3ekevxgzt.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3pcbnowrl.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3wawadrnz.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3xsavtaiw.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3jphenkyn.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3zdtitjcn.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lcyvqspo.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3szjurljr.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3kbhswqby.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3mchvavax.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3etujayex.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3dfgqthqo.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3jnaotads.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3qfisvrvk.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3wixyricz.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zxnyezvc.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3klfbyosw.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3irxmgipq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fgmicybl.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3mmkrxqya.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3brtgewls.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3fiztwrwu.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3woaqsnat.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3uwhknipz.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3liyccasp.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zodynedb.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ituiijjl.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3egcjcwoy.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3xsqkdpli.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3fjpakihv.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mqmdjbus.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3tynjbvho.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3oulmfeta.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3yiqhwbpj.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3djugpzjc.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ctrhbuah.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3upxyfklt.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3sxbggbtk.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3jprxayiv.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xydiftcj.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3agufjdbh.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3nfvtuyaf.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3geikcvqs.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3ljwcohpc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3fbshfbko.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3vncutydg.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3acfkuhys.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3xnbfgjoh.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3sclpzyxv.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3rhxludyq.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3sfnbpezh.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3ufhoqils.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3jbuyazjc.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3dotzycfq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3ygzziznk.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3cgwlwlaj.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3jkeyopck.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3fuszqvux.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3aakacvlc.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3fqsewevx.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3vadfxuik.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3wyioqdel.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3hheijcoj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ylxyuijc.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3qpiscypk.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3npwpsizj.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3zzmpgisg.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3suevktkw.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3fstwhscb.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3vohpyojy.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3dbbrnndo.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3wcrhfist.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3zvtqkcca.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3ygjkrwrz.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3ecoczjvg.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3mklyhtaj.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3ambkcffk.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tqpiezdu.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3bgfxzazy.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3nzccuwci.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ibjeqiuu.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3vhgmikpn.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3zbscxxji.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3usbhqypm.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3htrhdbly.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3shfewxov.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3dvshazuc.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3gpetqkfy.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3sjwglfez.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ueeamwes.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3wwzxgdcb.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bbikbjoc.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3clfhwolw.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3sqiarowl.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3lrdjbspo.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3vicjsgys.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3rhjdjoxd.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qvywexvj.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3siyzrfin.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3etgaiyjo.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3hovfbquu.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3eunkwqoj.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3zuexxieg.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3vihfjfzh.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3qvicvzkw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3qmbvvkwy.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3bslzomim.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3tmjrvyih.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3udzupshd.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3crblhudr.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3wknjfucl.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3wjmricmn.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3aadfzwwv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3agvmeklp.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qqxjdaan.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3hkskofjm.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3wdhgbrxe.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3zxtftbpx.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3aiovllap.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3nnoohibd.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3qgmjowdv.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3dpwgwang.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3gzyyohob.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3tsjfhjjy.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3wtphyose.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3zenbhtlo.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jmwnjejg.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3ybmzwrri.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pcmsucca.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vvgppszk.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3vwidmimn.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3aevykiev.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ocvrtvyu.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3eoawwzkf.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3nawlbjqw.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3ulxfxxgw.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3caxpzpfg.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3uuyepuye.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3bwlbixgz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eosgtjhy.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3dxyypdnv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jkatuifs.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3duoonfgl.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3untdutes.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3sngfoyrt.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xxdrdecy.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3daioqvqs.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3ijjoqjaw.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3uxandmca.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3tgdwxudl.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jueiqqfe.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3pockhooc.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ootlsmdg.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jdrarxgd.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3gzfyvhfp.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3wnynvbaw.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3kvwwuphl.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3slzijjsp.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3xngeyfas.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3zzxhsnmh.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3thhzyhye.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3khfzzlad.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3vnhvjqpd.html


<!-- 参考信息 -->