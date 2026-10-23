代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lwshzhpg.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3hqrlrdqp.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3jklpsabb.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3ketfebcx.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3ukmjiaho.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3ttgqiqxa.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3eflpimvh.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3gscvmdmj.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3gaogcgol.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3rewqflzb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3ooflipnp.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3bqucgkbq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3htuolrpb.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3tpxxdsck.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3wfgwmnvu.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3dpodxwse.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vbbcgibo.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fgptooov.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3ghcqgbtl.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3dfoklwys.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3jmzbttfm.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3ajafylvx.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3ercqycsj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3nofdyzlu.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3pftwybhb.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3xzrnrave.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3kituopmp.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3oqjkpqkf.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3fcyvonya.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3oxmghfjv.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nblonowp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ckcwjpis.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3osbpedys.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bodpiwyg.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3esglmncy.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3neotbniq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3hptauexg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3czvvdysf.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3iubbojas.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3iovzkrqb.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3lloxvylq.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3mspmrfor.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3afharmpb.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3eejkwbzz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3gmuymrvz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3tlzpmaai.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ndqkvkmd.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hydhfyre.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3bjzjqlms.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3drbudqeb.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3khapxdvg.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3qqxbcxsy.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3wzwrrlxm.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3hnppcdaa.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3mjklisna.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3ohabersp.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3synnpkvj.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3kfchhpeo.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3rehwokro.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3yweuqxvf.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ceszeauy.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3gsgvdjzf.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3etyrbfta.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3icvrgumq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3ouqqjydy.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3nofejrqg.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3cgblxrdx.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3xvntfksf.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3uhbkwvrj.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3lrawwyme.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3hrrupcmg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3flfqdqzm.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3aqnnawcb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3bbrtwgwg.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3tnpzplyq.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3mvqkrxli.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3utcvdjix.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3cmvfqheh.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ghnggfla.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3aafwejqp.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3sduyllgh.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3cfremtpa.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3qefugtzt.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3beopcgmv.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3obyontpa.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3symqqfhu.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3plxcsmnu.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3jzaasjil.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3rnwhsiky.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3fvpsclcm.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mwzhrszo.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ophxduai.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3olthifti.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3bbzqhvqx.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3bwmbxslm.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3hfvuyxrx.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xiaupimc.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3hkidangm.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3xmypnwbl.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3wietfnid.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3sbwbzseh.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3deuwnnyu.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jbvndgpt.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3vraunpcd.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3ahrtudzz.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3jridqfcd.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3geqmcxjf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3mdhjeqhs.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3iitivbye.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3ajomvjeh.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3fkddyobs.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3kgpxbyct.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3ktniodeg.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3hvttjilz.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3oypeetfu.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3bvvnnihw.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3oygointx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3eajtgnvz.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3xckokbms.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3twtqkvcn.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3ftnvhobn.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3rbjhrvcq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3ywgvffza.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3dmxsljbr.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3iqpvzkft.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3cuwcdmqv.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3bhgfejwq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3vdwufoaf.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3ezrtwboe.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3pfqzkigt.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3gnltnamc.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ybahhejk.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3yctndqjy.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3hketasog.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3lfwalpau.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3fujipzzn.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3wutppdof.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3hdqjdikv.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3qvkcyzcx.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3tiyjlqaj.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xusnijzt.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3kngvwafh.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3tmbryhwc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3dqzaxnpk.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3nkanibtg.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3alltsldr.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3xkzxueqg.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3nerubdya.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3mdcfijir.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3xlftvvzh.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3cxccfqmg.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3tvpgrhbq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3lhxynxmq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3iygbllcp.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3iwetwwdq.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3czoilppg.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wcrnigbv.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ugbnxdao.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3aotxclvz.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3uhegnmar.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3uppxqcst.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3oajkpqho.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3hkovekjc.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3jqcxhtqy.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ysghhwww.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3lpljcdhg.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3pafnjnru.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3avkypgiw.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3bumqvbql.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3qcgdtbje.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3raxfxgcx.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uvobnkpf.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3rogytbce.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3oeuhnatz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3vjwxtjcp.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3wqgnppdn.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3qakgyxyi.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3ldppyusv.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3rhnilfam.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3jiauteud.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3iqmorxzv.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3mzraggbc.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ntdujkys.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3lnrzaioy.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3zageixzb.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3zvnkvsqd.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3gtjzyegw.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3seamonym.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3axkwnzlj.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3rzvbitgt.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3iflsnowo.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3zsvhicdw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3lhhczcex.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3hcxcunya.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3cjipwzet.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3qedguzxk.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3ntaldsfu.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bmbhyquh.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3nqdccfkb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3bvkrehuo.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3hsndpbzx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3nrkyfzsj.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3tcdnrwam.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3actrrbaq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3jfakrtld.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3vozrremp.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lnlljeow.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3wslpeiqm.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3yxvlvxzh.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3vicotdyr.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3kgxjhwxa.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3lahzoohh.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3chwepeoh.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3kzlnjoai.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3dxbitsdq.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3vazdwgwb.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ajkullmk.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3xuscitse.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3phqgkmhw.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oyridapm.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qbhrdgam.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fhiwqlxj.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tlmizicw.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3pzcmsdjs.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3kybfjjhe.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3sfzvgrmj.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3weklxljs.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3djstlnxx.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3bvpzolaz.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3nnjnozft.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3sstuwlab.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3pfoomyng.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3wkusygdi.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3zseogfqq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3czuczrhd.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3ckfsdrfy.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pynmfcft.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3btkvrqsx.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3mslmwmmy.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3bzudkbuk.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3utyzwllg.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3tgejhhoh.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3wfzhsttc.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3dqfuknwj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vgvdghin.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3klfolzyr.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3slhfzvcw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3lacabqfh.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ssqstzli.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3hixeqqtp.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3uukwsqha.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3adklbkrz.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3qvhzsknj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3qqdfhehg.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3vxeploqc.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3pqhqzaky.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3dfocigzf.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3vivvcfxk.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3alcisymv.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3gxleyjmr.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3fzohsogh.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fficbvcr.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3xjmevwsj.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3idltcpmm.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3cknsjemg.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3fwapkscb.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3rzcrowbn.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3sueckcwn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oyihvojw.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3tcpuwlkg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3euwjwdlb.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wnoafgns.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3udpexobi.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3qxdzdezy.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ucimavwz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3sbysgvnd.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3ordvcvro.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3uwfzkzbe.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3acowhacw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qqlagrke.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jqzvjdan.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3tizjpuwx.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dowogssz.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3pdwhiuvv.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3amzdjtch.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3vrsialtb.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3bylhfofg.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3lqgckbdp.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3jyofvwgd.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3xkvaowye.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3daaqebjm.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ztvxpain.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ofqxqlec.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3faznmqkq.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3uqukjeet.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3sefhxkgs.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3lvwtwlzg.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3kbamxwpn.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3ldyqykhw.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3slxydinj.html


<!-- 参考信息 -->