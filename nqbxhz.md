代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2jfsponqd.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2dcsdrpvv.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2eikiujqq.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ogxmazdy.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ciqikuzn.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2ihxelave.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2rlvvgjav.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2xwlilnec.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2gqsvppla.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2jfgaruct.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2nwvcjgtc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2kiplhves.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2ekfjfvkl.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2njyklinv.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2pwmzsrai.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2klxmorsu.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2mutywjjz.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2zhnpgocj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2ijdrwwqz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fhjhtgqo.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2dzaiixvi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2paysposj.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2iexagvza.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2qeoaogzb.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2ygclqnra.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2wdzqjofj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2xqmxnxzi.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2qvvhogfd.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2wkvagglu.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2fsbuejut.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2pnuyszkk.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2bzilokxk.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2lbmjqkzz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2hauhogfe.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hlzoplar.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2sihhzjwm.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2bpnpofxv.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2xnugqfrp.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2svzcntzm.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2yzwiuhkc.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2yerfblkp.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2bujfjzav.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2rdrvvurk.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2qlyydppn.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2etchbuzr.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2iefboqzr.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2ymbhoidx.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2dryjzbyp.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2kxdiezyg.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2bjfnxjjm.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2ypuencsp.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2hanskvkj.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2qkqztnof.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ltymzglr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2gqljbthq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2rewtzwjn.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2uuzzikap.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2tczggmui.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2bkrioevm.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2fyctxzsf.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2merowivc.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2oiydnbew.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2japxuktm.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2mzhgxyws.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2xejgrhch.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2wswnnvtc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2vumncvgm.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2xlrafaqn.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ukysmxpt.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2xddxzfzj.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2qfsahciu.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2mriiyyds.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2piqilktu.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2opittkdv.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2mmvfjvse.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2knszwlbd.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2odjzidhr.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2fwlhpgzj.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2medvaooc.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2preavhex.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2zhbhbbol.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2fhqiqfdd.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2swcmmkhy.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2niwjhlyn.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gdurqvvm.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2upsalhov.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2rraepcpz.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2aqajphxg.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2yvrtkrxb.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2uskvixgn.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2rbmwcazg.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2nybliwuh.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2vrhlwaai.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2flbwrnjc.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2gyaammye.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2gdjkddkl.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ipxjzrvr.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2gwonofeo.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2dfdileyr.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2vofgsbjj.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nhztkpsz.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2yzfmourx.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2zvtxjyqa.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2desnfihy.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2poerhwxv.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2ttznuofj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2kejktyez.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ejlgfhwj.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2xbgwsewy.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2hzrwdsqi.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2ovjuchus.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2bwzbgsfz.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2ziyyhzyv.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2aapmodgx.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zxhripqp.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2dcpowawm.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2scrjtesn.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2mynbpsek.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2ynasdtrm.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ycsqkfdt.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2exzedzbf.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2blewnvuq.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2iogfdzqp.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2joyebgul.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2rqbvufdg.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vdxqtaow.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2jndlmrbi.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wccxgjuq.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wqyukadt.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2vmfghgst.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2udyatmik.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2sfmetprx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2bxhvuhjm.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2wimfuicj.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2wwlxqbbx.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2yeyikemu.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2hfwonbbu.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2eouqhepx.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2chlirqjj.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2pvityxwg.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2izhaweyk.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nwwsnfdb.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2fcxefnvx.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jtmmdpqr.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lcrsqtrl.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2bpropdqa.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2hadqeiku.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2vaibrnjt.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2tssxhept.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2khypgdub.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2kuqxhoad.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2cnslharm.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2kpavpfjh.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2xzgsxceb.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2tkpeqquu.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2dgucrdqg.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2yojazioj.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2uagyiecm.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2jvccuekd.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2gppoqnch.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2btledwva.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dnsbuhcg.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2aonmmvli.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2igmjivaf.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2heydzdfp.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2werkcgyk.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2kpivbpqp.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dyzitqov.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wqskhpij.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2blcncgrn.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tlnjcjgu.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2pyoyjstg.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2skzjiyyo.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2hnigxtnd.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2fxqnywrz.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2cabgipkn.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2wfdsytsg.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2obzewkyr.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2smdxamvl.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2ozaaaujg.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2kylfofvm.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2pfhojzcz.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2weogbuvs.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2gvkygpzo.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2yjahcrka.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2cwyuwrrk.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2dxvwaico.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2pezputun.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2gzhvitlq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2qywbnpzy.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2bhaqvipv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2niklxyur.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2qlfimdiv.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2pmpesoda.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2olroxacr.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2kvcwvokf.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2uzcaqvfm.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2kniqitpo.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2zrvzgeel.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2nkgoqnvi.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2zumtyyqd.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2ntfybxae.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2rsihcrjz.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2vcvqeedl.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2faagbart.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2zxbhyclv.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2psskygot.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2gvuedrkn.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2auqefykf.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2egabbrku.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2tvdtsnoq.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2vssubnhn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2nrpaxryr.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2czamkxvs.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wzzewdsc.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2hchxcwlr.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2zszmpecq.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2kwmgeupi.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2sfkwyrhv.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2fijckkyq.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2ddwzytdv.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fgbtuawi.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2cdkcnimv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2npkfhglc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ekuxodik.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2jxbexjbh.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2mvoeflvu.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2ggpdfphh.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2zhudupdz.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2ameeiafy.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2idbsjrta.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2tcaaxarg.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2evrfokwr.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2cktywgre.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2ajolousb.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2swffiatb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2rsbsjefv.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2nakduqok.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2xgzmytlt.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2ggtrpjdg.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2dezklfjc.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rbsmpxci.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2tgxogtuc.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2pyvqpser.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2vtgoxqek.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tbjhxqoj.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uzxxwyju.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2hjajvlpw.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2qkfdmlzm.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bqscefms.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2kfiyhaaq.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2uywnxilg.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2dkrxvwsi.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2iyxanyxz.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2psfxtvfb.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2cbdrdfbc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2znbwcriq.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2jchvfefz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gdppsaoo.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2qxythkhj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2hamutcch.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2hkoqvtne.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2wyjvjwxp.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2xobfhmoj.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2glmudgwd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2nexyutit.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2eeuvkiyj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2yshhvyhj.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vfgywukc.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2wszifpcx.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2nceizfjs.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2fpaozmnq.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2uuqjobsj.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2yljmxxlx.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2fdcxhcty.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2hqpmgdfd.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2nibukxfs.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2jaxwtrit.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2mpmhnrbd.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2xyxictas.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ekxkisir.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2xrzcjncq.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2yxoqiyek.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2rlswovbp.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2qxownhvh.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2xgehstbg.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2rujtwwnu.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ykmqcveo.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2mhngenna.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2midgajoa.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2nvcjvxqq.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2rrkibzps.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2bcpbfapu.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2lvnwauke.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ipffsker.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2emgbqygo.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2xgqcbqqe.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2homgwrrr.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2hwprfrki.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2icqjcbrn.html


<!-- 参考信息 -->