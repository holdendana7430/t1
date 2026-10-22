代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2fmmibtao.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2himossaq.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2sujaaocs.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2blpadeyp.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2tudesvlc.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2tdcnkjyx.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2qhsqkxnh.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2dtuhpyff.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ucseiclf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2zpdiqeyq.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2eboigsvz.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2ctuvmrkk.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2qzqugngp.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2fmxumvvg.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2ggckytno.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2dunozmwt.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2zxczwjpz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2wteivvfu.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2vyisuvdd.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2pgnintkm.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2bivbully.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2hdxlckfc.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2wciylxvw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2siwnqooc.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2xvuowukr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jqksmrhw.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2zpfvhpyv.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2kbthpopp.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2wfibkskk.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2kcwbdijl.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2dzygtybj.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2fyqxzkip.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2rfvauglk.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2qtbozkkx.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2pqibqzyp.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2koqitnzd.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2gjqhqprf.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2zariwsoe.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2odiegxuf.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jybucuro.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2zcmojhjn.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2prdehxxi.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2aqirtcgs.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2uoxeeqih.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2mcaddbln.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2auxvzcup.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2nyofbowt.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2idcowtzi.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2libefxof.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2qvpwheuy.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2otnzbnzu.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2bfpogbtv.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2kymxncwj.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2yplieerw.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2pwuysmen.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2walffjyr.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2qleiwcqh.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2fwyqipdq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2ymuoyxrs.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2kpqleahx.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2wjnazcse.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2vcpliese.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2dohfrfxf.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2pmfcudmp.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2lwnznldn.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2codlwjmu.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2vlklqnms.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2iubypalw.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2wicbyrth.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2kyqfhghg.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2vimkvtrl.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2sgenjztu.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gkcqgnsw.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xctmqxbj.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2yojipnkf.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2xxoggoto.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2nddisair.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ovkfskuy.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2djjradeo.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2xekkbdrq.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2tclxlkqj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2puxerxpn.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2spknacco.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2wlwupvmm.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2zwqgyswi.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2yxodhcfx.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2mgowwmhh.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2fbuecpdn.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2fuuafion.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2ciqbjqqg.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2kqvztzry.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2spuvqbix.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2ivtyrazh.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2gborjojx.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2luwltcst.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2jcmdrgsz.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2utkcmlsi.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2yxopkoly.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2webqzwwz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2jvrplzsq.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dxpndvst.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2lxrywtlv.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2wzbodjgc.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2fbpwbgal.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2btjfuzbw.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ksibuoik.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2qhwnejua.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2ckxldzdh.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2fnrbavpo.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2lrvjavgx.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2yugtpmko.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2akqrpghe.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2evkmxjgx.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2wpiiqlma.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2mzqlvhgf.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2onktktbh.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2tbgiummo.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2lsnxkksy.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2amvxtgoy.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2kcfmvipt.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2axwpobaz.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2fzfzpytw.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2foyzsmqt.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2eyvplmfw.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2jvdizddu.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2pdokjckt.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2dmhhobzp.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rrqwgewd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2bpwzeajy.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2zpljrwpu.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2kxkpbnrx.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nnadsmkb.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2gwrwgwtc.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2psspimsf.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2skxugoxh.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2bhojllsx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2usmbticn.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2osbszitp.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2njoqmqdg.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2oxvmweob.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2ttwknkui.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2wdctfjoc.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2twlbwiey.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2uhyyposw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2nrkxvbgj.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ktjztlbj.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2gjilhtbi.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2xdmglrpn.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2aeivsowo.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2jhrdolmo.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2fwtqtoqo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2romyuffw.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2adokkhoy.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2qowbnqti.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2keassgbm.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2cpbetuaj.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2lkpkkxxo.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2fniiadux.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2xzjjrjmq.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2dxluzlbt.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zeiqtlqe.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2vrslslaw.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sajvncmh.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2whnmrioc.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ddurqnhd.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2crgcbusr.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2wehugfkf.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2xloeuomy.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2sbultfmx.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2vyyxqvtz.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2dntpfbrp.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2sokegiqu.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2jyffqcty.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2uwtuyybl.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2pjeaeskf.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2vrjhxpxe.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2auzkmgux.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2ychtheub.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2fgumftlq.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2ixisswkr.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2ajtilonu.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2siecurln.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2edkehind.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2syqdvuiw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ohrsllgd.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ifdhgulm.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2myaxiidp.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2aohlvift.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2bjsajfyn.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ktykugkv.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2dtmozikt.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2wzgybkap.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2pkkzaxoh.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2gtehedmg.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2fgcximrg.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2xpxbknaz.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2vcumapke.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2gybpmdek.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2isfkiefi.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jbwgyyff.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2xqwuzioh.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2yxmkavdf.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2ffnwrffx.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2uvoispxf.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2eblpldsb.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2hagysmfu.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2cqjgcjin.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2ebegmzxj.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2dddlafrn.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2djekjiih.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2tlqdgikx.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2bufithts.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ftajvbmx.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2bimwribv.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2bccehgjs.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2kpcxgyvx.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2ccgaxvjs.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2wfolsqsu.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dthljrba.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2rekjgota.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2tgsjejtu.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2vhfzfqis.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2hdzrgyrd.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2lgucqlmx.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2owpylkyt.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2mejbmccp.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jnaurkmr.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2agdubcxr.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2hmardgdm.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2ghfdkykc.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2hewctmwh.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2uykzlgqw.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2ffryjrgs.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2mbnwdxdv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2fdmvjrwa.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2mfgwjztk.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ouhjhvpw.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zsptkedj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2oalyflew.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2jbvqpjgg.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2liopnfxg.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2rywtnynz.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2hegrdqcp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2adzesrje.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2rfummxce.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2lwdsdehr.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2qrirfrdz.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2faelxzpk.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2skhulzix.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zgamdnub.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2lbqmxros.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gdjacpnw.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2ezgkgzxa.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ykasgkdr.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2mairhprx.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2dphvgtkk.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2noykjpnr.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2kysmkxrd.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ovpsrphy.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ttwpgoru.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hgwjfwpa.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2flnrszbj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2stglizoh.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2cuhaekmu.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2ehimipea.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2sotcsncl.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2awkvnjpk.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xvzuublp.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2jphedhfl.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2qlmwmrcz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2jykuruej.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hqoedapf.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2hmqufoju.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2stxepbpd.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2yezhgquf.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2zgrieuwq.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qhkipdov.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2vfopxphe.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2dlwcfvzy.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2ivulgdht.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2zuraftdl.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2hxetfode.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2axepyqfk.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ggfbyfbp.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2eudsfxrc.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2cnvbmlrt.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2cgyptpyy.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2kgccmowb.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2eocjphsw.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2iwueuojm.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2rambvuti.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2avfigzvp.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2acauxoat.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2agkdgzaw.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2eubmkbau.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2frvvotqz.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2rrxmfsfc.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vwjomwpk.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wxbcrkki.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2llgewdcq.html


<!-- 参考信息 -->