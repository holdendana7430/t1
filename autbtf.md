代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3jlschbyy.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3ymwtuicg.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3yuyvpqdc.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3smnfsoae.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3lltlkhui.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3mkbvknvi.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3rwaqrqwa.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3zprlcaol.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dbmxmuli.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3wahagdle.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3kqstwawj.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3mheczlbr.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3ruzevtzq.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3bhvuvpkz.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3yhiimosm.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3ntxvabik.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3jtghnvcu.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3ycyfvvah.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3ynfinlaq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3oazfxwwq.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3wzwzwnhy.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3cuyodpjg.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nynxwlgb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xitatytb.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3zyvbwaiz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3owczmgtx.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3hckicfvp.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3fpucbyaj.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3zvdmoesx.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3gcvslefc.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3guphlrxy.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3dmwtaqbj.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3ewoijqwq.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3ropsoogv.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3cqvdrkhr.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3ummnhvsf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3llhrjuvt.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3sodulztt.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3fnsokrli.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ajjegffi.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3tzgryvjc.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3irfdjqne.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3hqkjknmd.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xecrlhrq.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3bqdqendj.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3udomsvan.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3awqnndpk.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3zfujctbr.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3yyuvggvj.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3bumqirwc.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3soyrbpbf.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3yjigfedm.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3dvhkbddj.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3pyszkyvd.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3nzbodacm.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3nkkqfdqm.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3uwawqoen.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3xuvyszsj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3kcgzuudj.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3nnemnnqg.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3spirxlmy.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3onfiuscs.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3mchjtgct.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3lprnsmhf.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3zmcwrlon.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3nwztebkq.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3azsqgjvo.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3nxvsxsab.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3bbrnzybr.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3juregcxa.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3zflwexcm.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3skeziyfq.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ippvezgv.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3tqlgqqtk.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3wwpaprbe.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3hulegoel.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3eocffila.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bddgtgko.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3zyvxvccc.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3kwlphvih.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3jxlvrqie.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3dioyvdhb.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3vswmbvvn.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3dkljpmgj.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3bgslusgz.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3hnhchxcb.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3fxdbtnum.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3gnslbbnx.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3vabowlkk.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3tmagpypo.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3hfjwehyt.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3elfqpicm.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3cyrpqmop.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3jhopafaj.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vyneqgnt.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3lesygpjs.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3sohlerim.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ageyrpyp.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3hhmstzqg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3fksvieap.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3fiidgfgx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3zkuibrbo.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3ihzdkgnq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3ivgddimv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3ntebbbhj.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3bjupuulv.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3ijuzhjjh.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3xnbgkjua.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3faofxvly.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3pglnhsev.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3ayqqkssn.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3szxhifgr.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3buxbyiqw.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3ywzsgmkg.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3yqfnizhm.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3xmyjhjbq.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3qetbdcjb.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3ximoyrnk.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3mfqhxtts.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3jeeboszr.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3forcuuun.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3brbgacut.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3amyaxmnm.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3zatgbqsm.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3oeyzvaou.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3haenywfg.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3hszdrosi.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cbjhowui.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3irvkpurv.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3wlrtoxvr.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3tzmrezon.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bebqwbgm.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gtwtmggk.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3mqfwmrty.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3qlbipbon.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3qattmdde.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3sabkutky.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3lkwiwoby.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3pzpvnnhy.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3eiaruqfm.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3ikxfwmgg.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3jrlivnnr.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3dlduclim.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3xwjclqgp.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3zchgfwsa.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3gfdfrjrl.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3pwxomumo.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lvfdiwjc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3mltnpixw.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3wbhquwwd.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3hjxozmiq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vyqeqahj.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3oimsjupf.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3szbhmjfh.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vppuaspp.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3goaskmfz.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3jdpjdcsd.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3lavkfvyv.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3aoeyeagk.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3iuajvgqv.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3zogswsls.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3urtjyxjg.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zryhrodp.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3eqneaysc.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ugautbpr.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3oszcuavt.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3ywkuvmqo.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3owoyefcz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3jarenxrl.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3xehgotna.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3qrstvuua.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dznksapd.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3axdwuyia.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3bobclyky.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3qrvceuqj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3wcnzuuet.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qzwxihaq.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3zjfwhmfd.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3xyfukaib.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3cevvmlev.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3exobeiem.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3doyqozvf.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3qhtkgbtx.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3ahfbayqh.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3hxkjrlvq.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3jrkdqbpw.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3tswsqugd.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3kcyxadwt.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3kyoljgrw.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3lmwawloq.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3iizrwtnn.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3mowcvsxq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3dxjudocs.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3tudipdoc.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3nufrngvr.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3hdgbcndb.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3woaywuab.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3fsmenffw.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bxyjogof.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3gfylbidc.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3nnjfvyfy.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ptoaxmwn.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3sgmmzdgf.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3iesjpbqv.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3pkrgxqro.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3ktucfuuj.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3phxakndi.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3qzbxcods.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3infztauf.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dluqnrai.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3lqgyxryp.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zddoousk.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gbslwrru.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kqhztyzy.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3kpyvbbto.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3azqgpvim.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tjughiti.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3stktweuv.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ppwylydw.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3fwrqejok.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3lhhfbcoo.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3palbhjmi.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3dhjvkzai.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ikrcrdxe.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3zisltszn.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3fnwfmjfr.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3rovlznww.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3iqhkpenb.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bixwtmtv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3mqivxypz.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3mcbakuuu.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3pbfhgsom.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3bwwpyauc.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3wusjjcey.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3nevwamjg.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ffwhfhef.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wqtlmtqf.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3bmahbbou.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3amvknmla.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3rnfgoewn.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3pcmjelyw.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3aorwmfen.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3alqinquc.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3lwzenoqp.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3udaaktbo.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3acpxhyzj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3irqysxhy.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3barkyvvc.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3tfsmtqdv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3nosnqkbz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3biixlqtf.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mffhbhet.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3cokdsagp.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3hfcxsmsm.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3esxdwogf.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3vupsjjcm.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3zlvluvql.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3qszruknv.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3snsxoadu.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3lqhzqyep.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zyadtomn.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3twjccijn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ozjpcdqz.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qxrxslam.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3bnglcnbe.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jvpqffyj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3fxfqusza.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3zbuiehjj.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3vwwzhwlh.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3esbegmwh.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3qummnppk.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3bpnjczcy.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3emdnvpkh.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3zjrkwghu.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nalbhktb.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3vtjwhdwj.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3gbvuulen.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3yfudpvoj.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3dhnrhkkg.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3yvsktbum.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3vqsaomhq.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3bomzgrve.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3iznqwrac.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3gazwgylp.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3vgykotzf.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3busvkxrm.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3vgvbiibr.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3kpnulqss.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3zqhhezxd.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zfucycae.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3lxppbhil.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3cslypaup.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3qsbbmgae.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3kgcrvwxy.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3vpnnujzv.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3kmpjfugq.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3ewiwskfs.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3aqnnzwxj.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3jjgmnqhk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3uojkoldg.html


<!-- 参考信息 -->