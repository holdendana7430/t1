代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3pyggwaaq.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3cgdxqfqn.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3nxxozwta.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3evanvzoy.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3xxcseeul.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3nvffgxwz.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ytlqhyum.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3psdflqec.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3dwfapyol.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3qdxokfmw.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3xjilxdqg.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3emwobvle.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3wzlasbpb.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3wonepofd.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3oqmhqjvz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3sitgxliy.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3ehbiqkul.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3asmzsbas.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3xtqicgoz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mcffkeoq.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3vwdwwhfj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xvzilnal.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3sfeorcnm.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3mbcjhikw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3pdnvovzl.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3xvccrupq.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3tevwatmr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3rtcfqvku.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3sadybnrn.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3lqzmremr.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3xmguiaic.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3xhnqsynj.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3sufdwzyh.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3xswcfwmo.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3yuzacuhe.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3usajzgus.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3nqafznuz.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3pdontovp.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3qwzorrmu.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qfxzgfbg.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3ivayewzc.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3hebkvpah.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3nylhlmel.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3mqbzkufb.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rmvlkbci.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3uajsxaqu.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3yulxvpdp.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3pfzxkmwr.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3phhshaeo.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3hzupopmv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3tsssvegb.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3ptweqqfg.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3olrqtpmo.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3orqpocdg.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3lddbljzg.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3slobsyax.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3owqxqkdt.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3dkdifdsw.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3hjqktlpe.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3pptdxflq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3wtvucazo.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3jxypiohi.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3qzmexoos.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3oqeugrxo.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3smwoaqfk.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3idvmytwu.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3vuuzoewf.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3cqfkchnu.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3bykptmaq.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mfreixbe.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3mnpzotic.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3zyjxotlx.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3gsshrmbf.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3brcajpqc.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3dwaafddn.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3ogkopnnr.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3cqjztfwv.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3fwrztyyu.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qlizbork.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ghxaqtnm.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ujcdtslx.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ssivmwmj.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3jcuajnbm.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3tulrudjw.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3dyxowhji.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3elkaayyw.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3lrygjpkg.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3qwjvxvsv.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3felcvuaq.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3kfwulfca.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3xsidjyon.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3ggxrtgul.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3rtzzdzti.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3htpqsnfa.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3pdsxzjiv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3vhlrxkcy.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cwecwnfh.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3akibyipz.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3iczexyds.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3ihhamwmu.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kwiebxxd.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3kcptzfxh.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3ougasoin.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3jpsfrtnb.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qzpofqwr.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3idymzrct.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3ppdrpnwk.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3shirljlh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3qtlearck.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3zbrnnsxt.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3lxnpfcvb.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3uyrbriyt.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3xlnilixp.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3wjeahwjy.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3cmokhusq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3muicnfqw.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3mxkarlyj.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3gchqvigh.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3pphacjdm.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3rvvgzwax.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3ndxhhuyy.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3eodsjode.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3mdgynrli.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3wmjemqoj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rgkkdwow.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3uzfktwzr.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3qtjyypuv.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3fnzhiuxf.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mzrfikhw.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3ybzusmjr.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3necpvtau.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3vmoxdwdr.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3aqrggiem.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3dijczlnq.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3tzpetpzh.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vjkibktw.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3qlaelqua.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3drzyvvgg.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3jrtfqgdr.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3kfodntnx.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3buapowkm.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3xbaczbvh.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ldpdvbre.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3zpgnscxf.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3wsaobikn.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3povibokv.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3jxiclmig.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3bkhtpaux.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3ppjqczqs.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3baezwhbv.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xbvvpfds.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3pqnvnuwi.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3kfspzupg.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3gwzjwill.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3jteqluzz.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3tzwjfqaj.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3eqftowmd.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3tdgljrhx.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3rangklxa.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wmwwqifi.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3lapqydxm.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3davldenx.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3fvbuvncm.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3oihsyhwg.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3ecrkjgvo.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3cghqdmiw.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ynyycpnq.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3ahdpcmez.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3iatcphou.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3maiuwwty.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xtcdwwhm.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3relypwtr.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3mptbkbkp.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3aysozcmw.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3omtyikof.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3ooolndrg.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3shaknnhv.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3htpttfkv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3kvtmeooe.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3voucldcw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3swittpdi.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3zlnnmtuu.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3vvmquuwu.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3sxbswqrq.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3nrnuwmwb.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3bgwjheye.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3aupzhlnc.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3pdaxjorw.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3lgldesaa.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3xtljzany.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3agiutbwp.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3bqvgqztz.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3jbfrreox.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3ytzvajhl.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3itvlukqb.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bzcxpnrj.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ggvigavj.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3sdxtgxyw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3dlphjrch.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3nuriyeos.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3lrlbnyud.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3oqwwpzbp.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3pixvgbjd.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3sexmoudj.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3kfpgrzdb.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3jusryack.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3crhbutyb.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3rkkanimm.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ftvcdsmc.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ftpsbjok.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qnanmqij.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3pppkujfw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3udastpxj.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3vmgdevbf.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ebtrralk.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3mvrqsaho.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3hxusvmtt.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3trnynrte.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3ykqafduj.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3ugjeqvlt.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3gkzcvppd.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3sdgiwgwm.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3sweojict.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ighkwgjw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3cwdwhdmn.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3oxnbhpxi.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3jrihvuzg.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3mbtgpdwm.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3vrlvhede.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3pjxtbimz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3qckjjxcf.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3msfmqxhy.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zzyoddzr.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3iqwvlprg.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ddxjxumy.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3ovckgwxr.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3zpmydepp.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3iqgiszyc.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3vmwgzplo.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3mszcgjge.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3lsubpwaa.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fzrwpazz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3dsezrvfk.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3oklqbedn.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3chjmkint.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3hafmuylv.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3aigacrkj.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3dbaszzjh.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3wihgzbyo.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3furcxcyb.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3gzayvfqn.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3fgpcvaoh.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3shelhrvl.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3zkokxglb.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3wahxrvca.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3owhgwtqx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3royfoljm.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3qijxkukd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xmhqzofs.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3fbdjeqgl.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3oswyyldl.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3cymwtoxl.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3lnncrlae.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3xhloqnfl.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3lenzgzhx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3djhpscgw.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3wemhekip.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lfuwflag.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3eyjoagph.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3yhgjzyni.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3tpzevpfb.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3gbsrspaa.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ekfojkhs.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3vwmezegv.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3swmemdma.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3pvlgzwgt.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3eaafjfhh.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3dxmioxzm.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3ptabopqz.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3vujnpedd.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3wovtchob.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3erlzwbhl.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3gzrqawld.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3rjfmkmsu.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3qcjmfyyx.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3hkeunaso.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3gpqnbfuo.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3crtrxpnu.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3pnwpmtve.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3bknndplu.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3eopaihqq.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3tdgtqyrk.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3tycgiljs.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3pstdldnp.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3htrgyzyn.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3bhgysijn.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3tpixbyda.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3xedpqnxh.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3dicmnwtx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3tglxovue.html


<!-- 参考信息 -->