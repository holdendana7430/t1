代发 wailian999

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3hifpyvxn.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3ftsqoruw.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3dpxohrzz.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3wpciuyxo.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3yukidtzm.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3asfmlxxc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3fvdbnaxw.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3phnzugdc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3kiywmnen.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3zfqpwpsx.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3dfhipxnz.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3gfsicqft.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tojuuuen.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wclnxfvg.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3xorvusev.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3vqawifzf.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3dzbathgc.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3vqwyrccx.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3mxmabcky.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3ihrkcuvo.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3rvaqqcrz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3ndfnywnz.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3zojyfntb.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3rdsbewto.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3kuywzpei.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3pmeycypv.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zihfbzbe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vqqmrvsx.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3dczqlajq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ofsrwojy.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3hsilcdws.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3typfkonu.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3vegqycfu.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3kdypfnoa.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3avwhpwtc.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3vsdscryh.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3itkvbygl.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3pugiqxlw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3wigyvjkt.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3bukxecwc.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3pozwzydy.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3hgluirhr.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3sodxtnas.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3kqequhtc.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3nizbrnjp.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3dulbzjes.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3qajatryi.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ygpoetfw.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3lzksvytx.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3rdqsrvur.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3gvzpwtsv.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3abxllqzx.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tawbgney.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3agsholno.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3idqitbyl.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3kwkovaqc.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3pccbznma.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3ternmvch.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3lwuofrde.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cegjsxts.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3vgvowhwn.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3pioflpnc.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3emyhysyi.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3yczkeyek.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3oxvbgdkg.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3rezhuqrg.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3cmnmgyva.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3lxhavznw.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3rpbdvjqw.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ovnkqzwh.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3ibqmxnag.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3zickggjp.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3itffonbw.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3zcmzjspt.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3uylimyyd.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3lotkrvmh.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3yehlevjr.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mbexnmbt.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3xbkdaxbl.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3zmanwzrj.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3iiwqlwke.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rhqwqzto.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3qpwrfxeh.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3zvbtofik.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3zkcxnawp.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3btghvnut.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3zgsrkzeh.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3mmlykrpo.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3nsjjzooo.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3pslekehl.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3xaluagdm.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3mbtyhfcz.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3mdppvfpw.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3wqjbqwpb.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3khnqyhcq.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3nrtucntl.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3fchyqcxq.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3sowbctqb.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bcqbexsq.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3tcjirxuv.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3egbvizbk.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3shugexai.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3cthsgbdv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3asvenkxo.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3ppnyajcm.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3vqoytjbl.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3pgqrfjnn.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3urtvtshc.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3zornnlgz.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3lpiiyeax.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3nnoorolh.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3gcfywxyp.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3ejxawjld.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jmbxnbfm.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3amkoxppj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3kdjhjzuu.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3esrdjawa.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3zjbdojzm.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3mbwmltxo.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3whtyupnj.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3mtvbjovx.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3ogbvbbsc.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3ovmpzikf.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3heaxsken.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3jxhqzpko.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3sndqquub.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3zseskmvj.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3reaklxhj.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3brwwcbnx.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3obbjrpuw.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3qoozrang.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qljlqbhd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zjagugyn.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3byaczoji.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3pemmlosv.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ugkwxltw.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3ripolsby.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3jwegkxve.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3nwyrjauz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3pwbhneeh.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3tjutgump.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rulpvsqg.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3pcacaqsp.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3asmrllyv.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3icpwxjxw.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3pfyyhgjr.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3adiijvoe.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3wbzsqvjz.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3hlsohfzz.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nqdsrgkq.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3sjuzbidj.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gfwtvodm.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3iyvmdart.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3nzvlzmro.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3cocfwtei.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3snfpekbj.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3bfjasyvs.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3yfdsljnh.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3adeyadxy.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3fxlpegno.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3mjdkyygj.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3ydcmvmam.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3xlwarpho.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3ziugpqfh.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3yjtrcrqe.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3okmxxsjv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dekxgyav.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ykaxwhgw.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3aeahsscl.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jbqxybjw.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3yukdqqep.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3ygchmqtb.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3svzddhap.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3dyanalep.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3gzzyfhmt.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cceoxigd.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3iftboiqw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kpklbwyk.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3stbjnghr.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3agdmanzp.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ihqcoeqv.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3qtnoyxre.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3shmyqpfq.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3evhtmpxc.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3sphgsdon.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3klyzxegj.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3lzfdhdbn.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3aqgvrhww.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3luuwutkj.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3fjnkgksq.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3qsqinjji.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3bzomikgc.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3gejdpvtv.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3nqhvuwix.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3rrasaibx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3cwkrzomc.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3kggkdwmd.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3faxhvqpf.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3jfrtvbde.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3pgpkynbm.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3hsctdyaa.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3uvudqroo.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3snkbuakl.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3mpuwfjql.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3wiinjzjv.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3eecdvsbo.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3zozhxvjn.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3yulmgjek.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3poynpvkm.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3aqlxtkbc.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3iooasznv.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3ajgcahsp.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3cadehshx.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3iauibnyj.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3jkikdcfv.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3kzlaadrv.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zmgfgivo.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nnccysor.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tnexqdfk.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3nflxutma.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3gxsxiejg.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3rfitjnqo.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3uiosdxud.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3ovpkwvwy.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3zlmqmooc.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3rchtuxus.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3ergeiujo.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3owxwrutw.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3czseyxun.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ormnnuwg.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3cymrkwqx.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3fmrlcaty.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3kaodsuwr.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3khufnbwx.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3awilftiy.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3pkmsnnhf.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3gkuvrwym.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3jehcjbap.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3oftqqxca.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3fdnjpjai.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mlgmqbse.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3exdkgqlm.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3mvyjvszy.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3rngahzyx.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3giakqiug.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3qypmsmoz.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3vldxymxz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3uoxobanv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3puxbuelk.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3rbovmzbn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3sdfjbphb.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3aidiafid.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3hciitqqo.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3thzhcnyo.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3evyqmswc.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3stikevxc.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3mysridtl.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3revuftrz.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3dxnnlwdb.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3yfbwlijl.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3jgruhims.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3bovsduin.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3wtzqzehg.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3zocxaatd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hdrgtjwu.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3xhdtakue.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jjdtziuv.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3toxgwcsa.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3pfxgxydm.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3yloatfcc.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3drkejnmp.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3zvfjkolp.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3qeqokeiy.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3lwpwvtge.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3bqgyrbcu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3iboavrxl.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3iibtpihn.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3ikpjtdvf.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3zbefunpa.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3wpvmepvc.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3kianaixo.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ddkzamph.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3tyzofvmz.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3llynqvtv.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3tolnhnop.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3blwxfyya.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3njzkqzdi.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3kjdblqqf.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3mjfcrwgo.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3fqxcryaz.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3jeqpoecc.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3fhcupnec.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3omlgnyrx.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3teypelia.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3cqvitumc.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ijzpnrzj.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3kwtzkpwy.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3opbvtgcl.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3pevueeog.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3woeveqhp.html


<!-- 参考信息 -->