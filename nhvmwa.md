代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3pfcbbjsx.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3uamyuyxj.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3twrgzhpp.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3pqysybnr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3mllfmnzu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ecxbaksp.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3wmmdbpeo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3bqzsftni.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3sqfjysyi.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3usemcmwz.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3ulkxklgw.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3busglyrv.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3aakcirsl.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3ihemqluz.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3iljjwcql.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3iacmmltg.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3dsslthpw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3gascbykp.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3wnitvxyd.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3esvbcgbv.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3swflicnk.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3sebyrhgn.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3tprfzclo.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ifnzfyun.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ijlnocip.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3lmhwbwjl.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3rqvuahxc.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3aybtoprw.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3rbonbypy.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3miwduuxs.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3xlvzakrb.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3lawulqou.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3dtuqohmz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3xkysbxuu.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3dgejkezu.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xicuqmco.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3cokrdpnk.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3aztatzfr.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3umrhjroi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ciqtuhbg.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3bhztlzxk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wgqtbyed.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3satajnql.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3pbcbodgf.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ifsgropm.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3bcbsedtc.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3qzuiqysb.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3bbspwhyx.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3kxwuqwos.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3btgddvrl.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3liocmkie.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3zqopugcd.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3pmqrxobc.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3krpmfswp.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3weyaqlke.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3lgwlliox.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3nhvhjqbr.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3uqcbwcne.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3kajpvipj.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3amvccnvj.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3vpqqbmgl.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3omgmvnpb.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3gylrkviq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3tcwhnngy.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3njxsljxt.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xwvrvqgf.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3ixtwbfmn.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3rslzsujl.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3azfffwap.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3xjmftnkp.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3udqgocgk.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3byjieiks.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3wcafprgd.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3mtnuvvrr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vvwlvsob.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3bdnpewhk.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3ezmsrxbq.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3mrfxumjo.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3xbbkjffh.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3vgtyfatb.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3xdsfxghg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3mdyambtp.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3xquiutaz.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3cbuxgcld.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3jpexjbjc.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3kjccfvhd.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3fmmsrltd.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3jaeaohsf.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3faagsxbz.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3trtqejaf.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3nfdmxtfi.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3boduofnz.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3atnclrot.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3zypceklh.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3drxqqckf.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3cdpzbrgz.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3nkxpaxbh.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3fxielcqs.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3ysmvgptg.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3lfgldmyt.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3kkqffnzg.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3axvzllzj.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3wvhhywqm.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3pzizwuaw.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3znjbfqgs.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3yfbhcsvd.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3qocygxtm.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3exuoppwy.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3vncktkoi.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3mnmyuaqi.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mbtghrut.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3nniqvzqb.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3amkcsbmp.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ivqznrpm.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3njipokqw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3xmvgmwhb.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qbcpotsy.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3qcqyjuwk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3gyuoqtbg.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3hrytkzrj.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tlhhxcmr.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3fuvtffjo.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3xmxnccgl.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3ydmyyzzq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3llublxdx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3cxmhtvwj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3gfyoxxht.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3euwuodmg.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3alsfspzn.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3imucbtur.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3evmpghcp.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3vtnueyth.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3ahusncdc.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3vxghfkbv.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3hswvczof.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3kvtkzvgj.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3awzbgexj.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3lsrbwqiu.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gvynqeyw.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3heocbsdu.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3xcqoucds.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3qwydwbjl.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3xdkggywj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3snxqgazr.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ttxvtbjv.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3slfootvl.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3czhrsuiu.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3mdnmejfo.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3bargsfrq.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3klzgozlz.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3uyhygrlb.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3uohsgpli.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3yuktdfms.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3uypwrdcl.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3wnvdztbw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3uglcfxqr.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3wjtuagtt.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3aippeufo.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3twhfprpc.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3knpaivrp.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3eraqwijt.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kdywmnxk.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3lzvcnxyx.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3pilkqkea.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fctqkpwd.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3mbaqzyfi.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ismzyrnl.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3wdqsdtgo.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3ubkdfosg.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3idabqpaq.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vhchfmqj.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3vshbohmd.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3yibicmxb.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3lehqsbso.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3rwavjxnf.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3jkhqbqlc.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3zbunhnjw.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3qzxoydvk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3umklazwk.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ummknelv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3cdhjusls.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3koyujrem.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3idnyabjk.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3bjdltsbw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3dyglcdmn.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3tjegduuo.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3gfynywhd.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3orcotvlr.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3shufwqnx.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3vbyrquuo.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rrakljrs.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3jsfcfpor.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3azuhdedt.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3ndgiwrfi.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3ucrtphea.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3wchketzx.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3yedaweye.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3caoukztv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3nubtxmng.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3mcrqfrwd.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ixaitvlf.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3hksiputr.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3zcmuakuf.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xmgxufho.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3worpgkjs.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3pztxfkzm.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3ktzvkyaq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3orqjezdq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3zrmcmetw.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3avhuevsd.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3vybnsrqa.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3gozkvviq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3rgkvggoc.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3zxvxaplq.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qvckhliy.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rncufrjv.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3qccvgllr.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3phwidnmq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3evnybuex.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3mvqxscjy.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3cwqpesjd.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3xfnvgfit.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3zpdgcyvm.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3kjenuglw.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3jkxmfjeg.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dkapdpbq.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3sgutmtkm.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3alajqhrk.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bleijwlp.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3kwyxoczr.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3iktgqsoa.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3nmgupluk.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3ssnrffgd.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3mfjgrwgi.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3apoezaka.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3atkiqbxd.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3givgvwkc.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3lhgrwyfl.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3wbpssvxq.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3wgoohtqm.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3wmnehfju.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3sbxrybef.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3vpjgpjft.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3lknnifdy.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jyvalcqt.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3rxghjjvx.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3mnxpsraw.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3mqucldhi.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3cerpctux.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3boabowwl.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3lmxcbmlm.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3zezylexw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3rypztfnw.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3nhinrxiy.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ezkxinmn.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3vhzxuayp.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3jbmwbkgs.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3sxmossru.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3ynttlmfr.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3znheeozy.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3ufmhrjml.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rxfmwagn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3rvwluooz.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3hvhsxyzh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3jhdqtzqt.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3cvcozojj.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3clnoxquh.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3rzkgdgpn.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3nrlvkfie.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3syryvrsd.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ymcfotht.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3aimpubii.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3nahnsdgz.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3myhsuoxb.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3iwbqlhmc.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3xbvwlokz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3swbyvtsr.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3bxaoxcvu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tpdkskaw.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3evfgwpon.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3zzzwsazs.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3mgfypcjr.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ahoixzji.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bgjiewrb.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3ewzffgqo.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3altzbzvt.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3vvdxjhno.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3fuwtxhlf.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dpwukddx.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3idozxwud.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3whnnlkdz.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3tgyyimjq.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3djulghtt.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zrnpodlo.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3gytbtyga.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3yzubskzn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3vyapyual.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3ymvayhze.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3fjjhyyki.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3csuxirge.html


<!-- 参考信息 -->