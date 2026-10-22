代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hbcnlhma.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2bhgagtfe.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2conrlwts.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2gewvnwvn.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2zcwfiwog.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2kxexhwto.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2mfozzjjw.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ctukenda.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2onkvlezw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2rvjodehh.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2jemevjvo.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2yybfjlbw.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2islwkaoc.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2dvgblqlz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2cttrnvhb.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2wpeccsxg.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mkeqvqem.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2wcpjwfvx.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2mezrsxgh.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2ajnwglce.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2ftkpsrpw.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2apbjpojk.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2jwhdgsgk.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2ioxkuhzo.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2cjxaobbd.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2rwqslpcg.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2pkisvqhf.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2sghrrvgg.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2dtbklrzp.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2gsfiqnir.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2eqcmgxij.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vdcpwjrs.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2dctiyupo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fpkgapec.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2zkqsupek.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2ncgnpqri.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2yhfekscn.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2wkieuzyu.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2pzhqmzjk.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2weynwzqo.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2pqjzmzln.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2bncdvckf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2nryukhto.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2xmtjfvag.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2dmkxbjaq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2ysmmfyce.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2qnhvwqmy.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rcvyliik.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2imzsoovk.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2jbfdhbcw.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2zchhxcsl.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2kkglgqro.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2twnmadcw.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2hvrhidvq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2kvvuafkk.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2orhfexwp.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2cesrarhm.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2jgwcvcmo.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2qobuchvk.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2umarowpa.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wcvtzajj.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2najarcfx.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2wnspaglb.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jwvvceyh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2egcefgng.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ctxvhbjv.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2xjwvlhoo.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2ctkbrpfg.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ttibamfj.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2rgsfxeel.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2lfqchddp.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2dlphouca.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2avllkueb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ivzqedjq.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2mdivjkpi.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2sclcveel.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ujfsvjsh.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2qztbjfct.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2pomhqldz.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2yworqwqy.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lcynaxql.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nddvygqz.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2zwrxeoid.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2hmpfpenk.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2bdpjshtj.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xjfjnasa.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2zlaswhbj.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2frdamylm.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2uhkkiyhh.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2qnwakxqq.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2xzzovqdo.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2grgzykjd.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2jypxooxc.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2tdrbjgax.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2ewwdbjpt.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2vimsjmze.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2adgookky.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2qeidlyjj.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2henonxwk.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2afdwguuj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2rviahzbp.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2oyklltnr.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ccamwljj.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2zfifpcmj.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2iskwzfnq.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2nhbkkyar.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2wbgtxxim.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2brssffnl.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2ibcpdvib.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2pvvlglfd.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2bjxsqjxw.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2tqvdsylu.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2opqvlgvm.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2nwgujbxm.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2wahsluiv.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2ohhboxks.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2lzveaqmx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2lzvrklkd.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2vxbwhkao.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2xvdmfxzu.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2qhixgoks.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2wjzwymgy.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2jtdjqcmj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2rahjpniu.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2ssnsycel.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2ewonqwqk.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2kezrtipi.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2oqvgztec.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2cfyyusra.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2wxcysdyl.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zfhrjwct.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2yztedpod.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2bfhesgun.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2tjtejpcf.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2apvtifqo.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zhrkxmhd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2thowxdmx.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2cjhecpus.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2fapapmgc.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2aakwuzbv.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nqdulgta.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2xrkabcpy.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2hrchhbqe.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2lkvqhmts.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2dqcxandb.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2seepyovr.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ztehlunw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2teucoxnv.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2ssxsxvxo.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2gevtydca.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2mcfbgjia.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2xmvxrxxe.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2lmflanse.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2voglfick.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tyjlfwfi.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mxfpylzk.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2acrczfmd.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2cghuhywk.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2zsekznhj.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2kruldzrc.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2bfjcpgdf.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2sxtsqvdd.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pmcaeybw.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2aaextobb.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2eddgefgd.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2iflxdhrw.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2mpefadbl.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2mzktvejo.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2xyqbctnr.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2nsgyxwrw.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ktgqhiyb.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2dmconxod.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2swaquauk.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2enqhdpzz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2skmmsuhv.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2kviofzhg.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2clpetxzf.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2vknnxsah.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2fgiyvmyp.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2wmbytrjr.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jlchtebj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vinkpema.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2oqljwflh.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2pmlukxed.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dunvgqyk.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2cizskjhk.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2vsbqtjvm.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2fxjmxgjd.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2raxdclsf.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2tkdzrgna.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2ypzybrco.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2znojchyz.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2khztnxyv.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2exruzdqy.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2fzfmoont.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xpnuvaux.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2hfgzvhya.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2imstfqbg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2ueaeyqct.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2yeelymux.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2cajohver.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2adazkvnr.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2iwevfevg.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2ckzacjop.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2qrcafxxa.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2pfubcurn.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2litqtktv.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2nytdbbkk.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2mpmlxdhf.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2chjoafsc.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2eatatkpe.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2qgigqahb.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2mrbeofmn.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2itmjvdoz.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2rpbfemwu.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2lmegblyg.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2epojavvt.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2qodpltar.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2drvzzwyp.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fjzzeuey.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2syomsonb.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2nqchasab.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2bgwscczf.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2gixjtgxi.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2hqmsozys.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2rcstzziu.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2dwsdddmp.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2aemuwveq.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2hitzlkcy.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2dlxucntw.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2enthbubr.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2yzxjmhmq.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2syspkdfl.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fuflypsz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2kskkyvbl.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2uwuenmgj.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2sjikagzn.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2fvjvcnzn.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2cfvqaneq.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2kkmsbmib.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2kyvwxnsw.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2evtqzopy.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2jrbawkjj.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2gsndtmkd.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2nrvysgzs.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2hodacein.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2jekiiqxb.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2zyscrmjt.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2cvtoommh.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2oerrvfgh.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2hyedkeqa.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2olmndxgo.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2ufcjjtou.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vhjojakv.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2rvalzrfs.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gzenketm.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2qsiqytjq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2rgjeainc.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2kbvsljrm.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2rpwzzrce.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2srqxyrrq.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kyvuaxrg.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2lmtqhsmt.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2plzpetln.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2urelgcdp.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2mpcecsnm.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2dmcsllij.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2nuirebvs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wmmvfvmy.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2ybidkiuf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hedlkkpd.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2xngocxfp.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2phkhffuh.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2okfeuyum.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vavkucbb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2irxjfhev.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2rcmpucye.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2heegmnmz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2fuigobit.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hiurobsi.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2sydhbrvh.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2pfjxmthf.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lkprjczf.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2udheaciy.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2cnjbemss.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2boabphvd.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2prxhjqbh.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2haquydai.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2jirsxbpx.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2zrolmqug.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2iyrggglc.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2qiecmctw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2zvkwdrue.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2lfujopaz.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2khbwmemi.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2ztladhsq.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2tfsgtjmw.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2ctjvdmct.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2bgbutpff.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2osvytgis.html


<!-- 参考信息 -->