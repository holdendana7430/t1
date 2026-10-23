代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3shrprvvd.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3sojhofqb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3kydsohjx.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3hiotdize.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3mpwwyqjd.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3wisztepu.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3rfnnauxu.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3swrvlacw.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3eersihlp.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3qmgtidey.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3pyczvuup.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3vjagzbpb.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3qmebwboc.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3fgdoaxpo.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3gjxgzxsf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3wgkpbdco.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3nvbazmbq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3ujcvpxoe.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3pljetypa.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3rmzejrty.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3jnfnpajl.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3wljxmiwk.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ypuvxaxb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rhcfrsae.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3vgohibdl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dfsjxwmq.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3mibhkkrn.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3kvobetkz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3dwiyinzv.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3nbdiufal.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3yrfacfor.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3lizzrxwq.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3mkllvpuc.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3yvzisibl.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3suubujuw.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3pufjlbzw.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3nlhnyofz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3wplaotrn.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3pzpmdiel.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dkwplxqo.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hbeuyfui.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3svmpjhqg.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3qbaytqla.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3stxmarik.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3rrpjrycu.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3hxssppcl.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3amplmbvk.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3msbidrki.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fnbaimat.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3vnecfdso.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3recynsfk.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3wognqmci.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3upualeyt.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3sqotsqrg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3pjwbqjgm.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3oxqcwqqa.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3ukrxmwlj.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3bdzjkrya.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3caavdhvv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3htgdsesy.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3mlqjmdaq.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3wdxpjfdr.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3ptknmxye.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3pvhefoci.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3qckkplac.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3wygiwxsg.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3qgijomkk.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3kbzhnizp.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3itdjatny.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3wgomtnfv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ayohrkao.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3agotcjvt.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dcnymuwy.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3twpjcjyd.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3vxcxlquf.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3fqmoezxo.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3kbfomxfj.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rgkdcgbw.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3wybdlome.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3xwruyjxn.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3bzbjknvg.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3nesjobbf.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3rdjxsyyw.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3idcewffk.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3cheehvwe.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ggdtptrf.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3qnpbhhpf.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3mhiwgcpv.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3vpoqvlay.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3mvokrkjc.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3dcevtgmx.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3gvvpitxr.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3dpsspclq.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3elxcivxx.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3frqsywzp.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3owikmsev.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3ralumrvj.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vcibsjpa.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3indkzwyr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3hqbzicha.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3vgpkxvha.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3ozlrfkcw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3wwhbbbml.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3vygrapfp.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dlxzgjgr.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3bxemctub.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3fyneagfa.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3eyehdlrg.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3fiedgdao.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3phlftrit.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3uyfgaxjc.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3eyqmbtqe.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3mxhpalsg.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3tkkxyiqo.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3kvxsejss.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3mvyheunk.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3dguqsabo.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3edzkweej.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wioebwms.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3krdxbntc.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3atshzasf.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3cjigyrhe.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3zaewdkxe.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3ktfqbvbt.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3quzocejj.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3cxmgjptu.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3mastimrt.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kuzhoufv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3iyfmurep.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xmelpygp.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3pcanjzxa.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ieqtediv.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fnoqyogs.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3gxhspfdw.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3olqayzio.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3dwjtxmmf.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3xouzptsd.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3nzdqpsgt.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3vaxpywgq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3svqowvao.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3enxtsitg.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3fynyfdge.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3pcanrdzo.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3tkmteeyt.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3xikrpymw.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3usjwmkxe.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zacruciu.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3xobwitac.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dwuxzxxs.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3fghzbhml.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3gjjzelnx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hflusvtt.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3cnnrmxdj.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3kuoxuxch.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qyimoggs.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3smntuwiu.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3qlhevzsw.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3brxavimb.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3wnjraaxh.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3vgwayvmc.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3xrdiyfjl.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3fcqwgfwe.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3bqobsfrf.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3mwswgohs.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3bkhgvyxd.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3nbdmkags.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3ivonbwhx.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3cqpkwbrc.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3iolxneto.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3wezhtvpw.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3jzmgahwe.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ibpcudyi.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3sdzgnbkq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3geejrlpo.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3athbaxqc.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3kditiwnz.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jfajdjnt.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3lanldmph.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3chlutshx.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3czppzact.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3qsyssotf.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3cssfocbx.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3gkfxaemf.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3qvxbfkjx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3vjvsgtol.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3qodbdgfs.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3evjcigek.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3npbsiiym.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3zlhsrabw.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3sedebkxs.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3vmsdaymg.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3vdxeavop.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3kbwvzlts.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3gghxvhkw.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3gxtunhpw.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3avbebopu.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3htckocha.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3hbuvrxxn.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3ydkkivug.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3olpxafbr.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3yqbeipyw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3jsimszrh.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3nxbvuyws.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3neqsfree.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3qozfadtx.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3qwigkhki.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3vovsflhu.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3rbzyhphj.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3gihovnod.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3wanofurh.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3lylsdoab.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3tvejlrra.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wmtrlfzd.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gekyfydx.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3zkcbzuhg.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3couqdwnd.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nsmdimdi.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3fszakyjj.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3esyvkaxs.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3npzudlze.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3dxhtrdxw.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3tvadtaky.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3fdrtkfpb.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3varvjghd.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3vdthiwjv.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bebskoic.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3tixzuruy.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jliznkfm.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rhqtburn.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3whifonjt.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3rlcgzvvt.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3mbolcxkg.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3opwmudnj.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3ltajliix.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3tmxwzsak.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qgwpptwk.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3wcysgmkp.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3fnkjrnmw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3oynqlvht.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3ldfrobig.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3dzrmilde.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3cgcmjutc.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3fjboicwe.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3rxdiuahx.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3etrtkkhd.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tjmokkjj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3cybsxkhu.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vpvgwrnh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3vhdnuqwu.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3gzaqbxtm.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zpkisrbe.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gfcevrzf.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3fvhnalvm.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3thtdjpeq.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3bmpmlozb.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3hplttbzl.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3brnerqqk.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3sfaxdgpq.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3rtzhqyvz.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3kdmeobsu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xudzrnhx.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3bixqidxz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3efvnulkj.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3bqkhfhao.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3nqqveugy.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3mfsbnydd.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zqeuiokk.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hqfefvnm.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3xissrvts.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3emetkxxt.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3autespnq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vpipgeql.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3bbvxcfbc.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3iyqpfklr.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3oqifmaur.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3aefnppmz.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3fbfryovg.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xmpsrfsg.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3khywuixv.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3lyknjfft.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3fuazmxos.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3bgdointm.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3hsxiyagy.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3doknzmja.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3xdgtlfbj.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ixantmts.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3tyitrxbe.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3qxraxvrc.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3qtuzsetl.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3zjwsupqn.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3fcgwniuq.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3sdpqlcvi.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3dqzirvmj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3trvvvdgh.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3nkqpavca.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3dagnaeeh.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3pnlmyesb.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3badnjrih.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3cfqzeceu.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3cqgfmbqm.html


<!-- 参考信息 -->