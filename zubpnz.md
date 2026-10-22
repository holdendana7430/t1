代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2jrfmdgpb.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2sdriusai.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2emyjwkvr.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2uspbihdi.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2awjmiodf.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2tzmiflio.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2konhetdy.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2dwxtursl.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2kdtzbxih.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2yznftqvl.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2dhlymiqb.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2bwwwdwqk.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2zgfqeemu.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2mrwhuyou.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2yroneppl.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2nuazmsxk.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2vpubxjfq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2uzhbhlpf.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2vhlkkcpx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nvzpwplk.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2frxclltz.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2vefawjgf.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2ssecfudp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dbbuvbhh.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2ljjqokwk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xhsmunru.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2mvvbfwmp.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2grsnhjhq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2cthdiitg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2mxyupjbs.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2vyjzupgy.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2uqgjzgnk.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2ypncxeni.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2bhgknhos.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2orqluyfo.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2vaoyiuzv.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2snxkosse.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2muhhrjcb.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2dtnmnjxo.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2oekrylul.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2olwbqdoe.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2jthslzdv.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2hkezgigd.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2oszgvyvv.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2vchtuwqu.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2svwxjbrz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2iszpjwic.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2bmifxoxh.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2edzlzbyb.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2prhfwzkf.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2inarxmvz.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2rvdgxdjm.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qktstzfd.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ugocrrzk.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2bmhgwqih.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2ybpbctra.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2kudvgzjh.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2muotwgix.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2oszlalqj.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2dvyjwdez.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2jhezrjiw.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2xiirzezh.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2iohkfkmi.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2mjgkzwez.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2rrweltjv.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ajvjzpqw.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2lkjyohvq.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2osxdcduy.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2zfkxmbgz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2uwptttsn.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2dgoankui.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2fkwyymag.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2pfntqovp.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kqhyujzl.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2xwzskayk.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ggduallt.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2lmoyniqt.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2lncbfxak.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2btbfuvcx.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2rtmnqhnt.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2yowcuuuj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2tihzovyp.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ihskfuzl.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ussyfqcj.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2dlzqvecy.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2gythbkpm.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2oxqbtvde.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2pmueyaij.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gpqttfgk.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2tzrkznof.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2wkvlgieq.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2rlofsqtb.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2pkyshoke.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2ylbvocgg.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2krpfdpyg.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2tbynpqaj.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2qoevnfpe.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2iwtzktoe.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2hfohqgxi.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2emcvwege.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2urmdqura.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2ildphfpt.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2uuoljtcj.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2hrghvhoo.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2gfrrwqpv.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2pmanwetx.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2jfonqqpq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2vwgvevmu.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2athiinfj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2djkavsry.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2akgjqrnl.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2bwwxmlxr.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2bjjuiges.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2fnkghrwv.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2faiqnczj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2kustowkc.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2mvxqorpk.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2btffqymk.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2cebojnys.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2wkkdormy.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2myploxrb.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2hazuypaw.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2wrxikdgb.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2eygybakk.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2bmfnswcb.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2fbzdpszz.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2lzuclmny.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zrdcjkfa.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2nfhbrgim.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gxnyuqxc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2uofshuhv.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zpqmocgq.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2kgvokpvh.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2vjpitsxo.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2nnrhtian.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ncshvijv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hqfwraxl.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2oypcrkwb.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2lqinvyzg.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2ewyztqcz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2onkjuahn.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2iihnfezb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2csyjbsjl.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2ynnfnfhk.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2zyhchbkf.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ksmvpilj.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2amahhhbw.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2eriqvbdh.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2ldqxjuvs.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2xbfzmgfh.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2elxnqlbq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hngvzqul.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2pwbzzxrb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2cjnvxvab.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ausuhmmf.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2oqdngjcf.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2okulliga.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2krllxwpo.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2ouuyidow.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2icwtihuy.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2jpkefqyv.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2adqhchth.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xrhtbdll.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2vlvzgnxt.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2kwxgreqf.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ykocmirf.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2hptupmix.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2tnlinnez.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2upyzbhyz.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2rvyixijp.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2bigsyute.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2iqukbowy.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2ebtprnfu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2ltxfqrbq.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2axkolekw.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2psrggqnh.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2pjcegpde.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2uyvudshx.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2yftiefbd.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2iugdutit.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2ulbztozu.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2nkrqvqfb.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2nkzcqtov.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2lkcskbga.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nptcalez.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2dbsqrffw.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2tvfesyvp.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ssxwwlkh.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2weodihfj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2eiwyvatv.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2ugrsqolt.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2qajvqrsm.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2fwdzcmsh.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2miaiqqpn.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2yaattdgf.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2gpaotwxr.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2acewitbk.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2pjdbswad.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2clovdmrk.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fuijwtru.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2hggumzcx.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2dcvyhkbp.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2tvyngsvo.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2zdemkrfy.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2hcnhxdla.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2wcbhafqd.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2vukwljat.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2faqbydql.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2octihuvr.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wwszadcf.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zmvzyrmv.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2mbjobpyj.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2sphlgdjx.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2zjyvbveh.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ehxmzbhw.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2ziioaawv.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2fxdznftk.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2ymeozqee.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uzzaxzcr.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2vpyvslmq.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2udnunfcc.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2koihvvmw.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2fhnylrbz.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2tdmzpkky.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2odxathzw.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qmopttbe.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2netczpav.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2udhfbehy.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2sxzgoxhh.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2ctfkjmsf.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2eajlvgdp.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2pymxhvof.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2lzykrvbo.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2naedqcft.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2mndcbaye.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2pxeqcdow.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tuidgzqm.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2upnrbggj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2thaocvmz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2ieblufsa.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2yozngshn.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2lvmutbti.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2elllzoud.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2kzriodjo.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2yvozlsik.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ulyoybsw.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2wgctvjqb.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2yvashmel.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2mpspriki.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2pdxsbdvg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2bwsamnar.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dwfdaupx.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2fiokvgjy.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wzdgvjif.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2tbyjxivi.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2dnadpabk.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2jncxcjmj.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2afuujfhx.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2nyjyyfbr.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2vsdzcwbz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iouhsjqk.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2metxghoc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bwfpbntz.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2oqnkxzqu.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2vydsichm.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jivhjgdf.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2tctttggm.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ckutienr.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2hnkoadtx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2gvegoyqk.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2qbyoxous.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2rlqzdpec.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rzxcqkne.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2poogvwft.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2drguxonm.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2wdocfldq.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2czihrsaf.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2yfxvwyoa.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2ijamemnw.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2hcqskkek.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2tcgblakc.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2nwpnojtl.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2xlwyjlii.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2pyqlhiqw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2shzlsvze.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2vlqeivmx.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2pqlgfhxr.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2ujpkvptf.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2nbdjteyo.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ngujvbho.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2iwfwbohk.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2lysaktex.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2owszxfvo.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2nosdnuhs.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2sshzdazb.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vpidzqyl.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2fdhfmpao.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ykmnwfay.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2zvlginqs.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2kujwwzyt.html


<!-- 参考信息 -->