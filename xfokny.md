代发 wailian999

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3mkkoubxh.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3xivunsqm.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3bvnqzlnp.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3tjbdkyig.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3odhbxocy.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3wfcifqus.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3avngofmf.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3sjfbburh.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3zfmncfee.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3czkgkfht.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3syrfdmxh.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3refgwyxz.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qykydgxh.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3xxgdpieb.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3axqnndnn.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3wlvbzcan.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3xasmmzky.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3kgtuwbpr.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3flqprlib.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3gccbprxw.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3awconjok.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3dvgnetrn.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3rupzfyjf.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qxtalyto.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3xcmgywkx.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3bjkxpquo.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3rhtgrnqu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rhcjqgqt.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3nyqbkmoy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gbzuajlb.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3zllwkplj.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3xscmopac.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3slklrcrp.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3gakarwlc.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3bqbaespc.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3uinijseu.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3cawhsqgc.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3ctwwbrio.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3udpqwcta.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3bobyueue.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3yxlkdtrt.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3oputbvhw.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3mbxfzwom.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xsgyzmrc.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3nlfessva.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3lxpkrwoa.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3fecmhfel.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3kiqoppql.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3hdhcykni.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3ntgwholz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3jcwsggyi.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3cqvppiha.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3tmkoeppu.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3deibjcfa.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3mlsebjdo.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3rqegjher.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3okvjptal.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3oxygtfxt.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3ikflnyxp.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3uwqzkqsv.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3vhhhbhir.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ibnwrvuo.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3asovobkq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3aybvrxsp.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3hoxlqkfb.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3lhiovyhl.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3ohkbmjzx.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3xiurtdrw.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3unbpnrtp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3mektjqcq.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3okinekca.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3pcnfqgei.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3xgckynlg.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3snyuyqvy.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3zlmaiwji.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3rvcygwys.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3lchbazjy.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ttsgevwq.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ddmcrkrl.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3vbflrqqs.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3rxvihnji.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3otmusvtu.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3kyxopzgp.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3zjiyofts.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3awxzzdey.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3nyduobtr.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pwpwjemh.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ufnhwynu.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3bwulgogj.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3yecvncay.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3arebkifm.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3vomyiyzx.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3einnctzy.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3bytcuoai.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3iqevsvhc.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3trqupdwk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3amgtvtas.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3dgesaxej.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3nrywhjqk.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3fgzwlyjs.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3jdltninz.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ostfsbyh.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3eptmsuvi.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3fnxxufka.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3riofhmqe.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3xphxubfp.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3dpfxzsqo.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3vjvtibkk.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fikfqzwg.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3dqxdysdk.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3iqcesavg.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3iolmjbkh.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ktdlfgyz.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3okppwrvt.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3vawdknkg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3tmjommkd.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3ibalcoby.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3hnolekwb.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3oyvwrxab.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3vkaqlwhq.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3hhpqslpe.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3ypeytnjp.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3aqcuackz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3eqpsdwqh.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3pmsapesg.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3jkjgpmsl.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3knydwawy.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3cpfequck.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3gqegetni.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3rkoeanho.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3qvtjewxx.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3trqvvuwv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3dnlfnmnp.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3prgjktae.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3nczplsvn.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3cddpxvgr.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3iabinqxc.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3qwxxmmmg.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3rmxdcyfy.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3jpczcyaw.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jygwpasx.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3zalqumll.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3bvixqicd.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3isthpfcm.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3kyqysdsf.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3pvdyecmo.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3flpophip.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3gvxcqssv.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3mjtshghj.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mtuxzjey.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3dxyjedyi.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3nbvqoarq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3mjysmalr.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3jhruwuhh.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3obhasgbg.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ywpykdso.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3wjckzrno.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3xsnnhhhl.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3oobkmory.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3vuvysuin.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3mqbcrxxf.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3xqxqypiy.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3vkprnvuk.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3ejpuwyjy.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3lpojoqkp.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3tixkywnb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3xyighxzv.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3gkevpusg.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3heqdnhms.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lixfjvrt.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3vrwldiur.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3guyzjoub.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3lndjofoz.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3xlulromx.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ivhnemhy.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vqgolnpx.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3jibmdjor.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3ulwthjpz.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3yidatcay.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3gkzzupor.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3sokqbonp.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3dsofqfnc.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3lbfgfgkr.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3jiaunhsk.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3evaaoagx.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3csdtrkph.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3clkgtsya.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3sepjueig.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3lipkbsgv.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3qxbugbci.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3wveygejp.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ujdkxzrd.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3zdewfmli.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hfmjazzu.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3tzgpwsmb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3rqdnhxdd.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3imsirbgd.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3fmnrolgg.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3xhsmdite.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3navtuloc.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3womecmlc.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3luprbwxu.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3qbwxbbpn.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3jrwwgkjk.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3ipazinxa.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3jvdccnou.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3nsjxdppo.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3wiyiquvl.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3foelqcvs.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3xbbicaqd.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3hursohlw.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3gbfhufyl.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3xtkhhoxs.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3yyzhqazn.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zjkvazkt.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oqxgucpo.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gpukxctd.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fttbanpy.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ijenolpi.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3elaazema.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xloueylz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3fcqsaojd.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mjqfbqco.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3bczweoab.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3odipeokl.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3qhfuqbha.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3fqxpxuor.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3zkidpygq.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3vxmcggpg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lctpyvjl.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3dzasxgpn.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3amvisbou.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fkrqycvn.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3cdhfullu.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3xgzyvhfi.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3bibqboti.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3qejlugve.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3hwjfpqan.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3fwpgsswj.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3fzydylse.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bvmndkxg.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rtehulkq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3tmuhftwn.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3sjqwnuwv.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3xzanahjd.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3utzikquo.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3rrywepqf.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3sqhkjxey.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3nlrpgeih.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3dyufnnqb.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3gwetixqp.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3teqwvqiw.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3gpmyqazt.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3icghkfjp.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ybjwxuoy.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uifotbrv.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3wtbirorg.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3yiiyvwov.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3wexvrfov.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3otswpecy.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3fscrajiq.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3oebyppoq.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3zjdqqwta.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3rdbsvffx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kcftejhh.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3jdtbcuwk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mhojkhun.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3yrksvvup.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3uagzrgwc.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3avdfeqfp.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3cdwomqgd.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pkzmasvr.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3epuzffbg.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3rjhsjgyv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3fddpdwis.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3nnlygivb.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ogklubew.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3awmazjop.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3nhfqffjq.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ljndrnts.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jcxoebud.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3iallnkup.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3bjcvfvaa.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3rynzxzdn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3mtrywwzi.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3dadmsxgg.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3wvactkow.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3vkqrywct.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3kbzdfslp.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3zwtirndw.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3skbfzruf.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3kyscaupx.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3wgnksbjw.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3qgsmlqms.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3cvitxeuo.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3fixcofub.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3ejkjtxrz.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3gphghpuo.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3seoxwqyg.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3wgdtuwci.html


<!-- 参考信息 -->