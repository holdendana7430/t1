代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ffewtxcm.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2nalhmiwm.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2cohseisf.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2wrbuzcmh.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2qjizwnpp.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2elyvmlhl.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2bqevsffr.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2hbbchysw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2uhsyscaa.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2phsebsmh.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2ssvzpmeq.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2wmmftppx.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2laiydlvl.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2drbosakj.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2nsogscma.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2xfkejbpr.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lsthdder.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nqewmzyx.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2ergqiaoi.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2mspxgsee.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2nrrmnfsm.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2lzdcqujx.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2cylyilcx.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2pzlwtvjm.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2exlcdutt.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2knrcuhlu.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2dknlmbun.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bwdxkpdm.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2hpihsvsi.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2xfhfyitv.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mdlsabih.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ojuqnymb.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2nulqizce.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bmdiwvby.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2aiantfbq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2gcyyicoy.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2kcsyivph.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2mwdoxnui.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2nxlfxvyy.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2ojyadipz.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2ekayjunr.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2fszvcmkv.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2ksnwbrcg.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2anobxefr.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2fnjoazhy.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2vkvpldkq.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xbkubabk.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2pzrlkhtu.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mzocyjur.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ynxmdktf.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2bvjrgojz.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2aexvizbx.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2hdvzaejj.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2otoykftj.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2pagfbcoa.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2xsetvuod.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zsyaxvrc.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qsmrirzv.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2hexfwbyh.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2kbrtnizl.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2fuhakuca.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2nmmnkwje.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xqscklzy.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2wnqkaoyq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2rmrwujpw.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2yuuxrgbo.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2uwhcolbf.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2aobjqxod.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qziiymrb.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2llsqirem.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2xprvohil.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2yopacmdh.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2wnrrljrs.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2wcekkisz.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2zmbikpce.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2okzlklih.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2qkjakrwr.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2iwaoswtj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2jylqdmsu.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2csvbdogu.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ypvmbibi.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2qqoahicg.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2bnkdgwbt.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2mvwdbltr.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2swunmzye.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2hpdcxypk.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2oakdgbqp.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2xgomqdqu.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2jwuurimi.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2ddfdtfzu.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ksleklui.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2mppkyrxt.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2rwvjcsxm.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2fxxwylwm.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2jbmzjtrf.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2dwpmmakn.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2qnfujuyj.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2vzzzuwui.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2gjqkwzqf.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2pzahwkze.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2leybfnna.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2xhqzdgav.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2hqssoyez.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2jevlqzro.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2dkpzmhql.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2rjfcigce.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2vbusfrny.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2uuzqopsa.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2wwspehky.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2etpwublx.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2kcdfixyi.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2iajcyycm.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2pidvpryk.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2pmevfsyv.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2xbfsvyaj.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2nhsrbvoc.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2qeawitet.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2hjgycztf.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2jyhukzak.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2pcxeudau.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2zmpsojde.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2kefhdddf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2zfyjxklf.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2nckiyjyt.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2drrwwsba.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2cfzwuapj.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2igekbjyl.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2oolafuci.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2mwpwgcro.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2petmchvf.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2rysycuss.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2oapmaawy.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2nlofngsj.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2ftrkvvba.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2dkdobgxx.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2hlikubtg.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rrcxebvu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2mwtnqfuy.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2notflwmh.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dbgvovml.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2dmbyvirr.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2hxdnriei.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2plqqxsvh.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2lultszkh.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2nynrtznb.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2wbtmvalz.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2bomstvkm.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2vberqskw.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2wyzuefnt.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2qeglnzxu.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2mklfdxzo.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2qdizbsui.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2imcplcuo.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ngyenhmt.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lobwbqfm.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2uskpktdv.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2ldghyjqn.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2ocgalwfb.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2kmmduokv.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2cnjzhwlt.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2hofbnkcz.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2rnnjzumh.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jjwfcnda.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2gzxqbuox.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2opsvqloi.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2jvtuqxav.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2ntvwpmnt.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2giijtaqx.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2gsgvgkgg.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2mjnuhbnj.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2uqowdend.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cuxttltn.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rweyctqf.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2yypilxdw.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2sxypvwyj.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2rkcoesai.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2muwerocy.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2htvxvzcn.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2ezqaphzk.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xwlasuvi.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2njrcbbxu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2suxnqgsi.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2jtoiocpf.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2yaysnbhq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2enofigje.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2jcczramo.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2srciyhaq.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2yzkkgdab.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2ugnofzqt.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2vvublbuq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2wlqfbegy.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2bcxpmkrg.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dpwefhdl.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2zlzrsfbk.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2wpcuxskk.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2llvzbnjo.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2fvgbhhpx.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ztuygmif.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2lqqkclad.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2qxaksckm.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2mkmzoilq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2wfsxhlos.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2dqvkklcz.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2ujjqlmch.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2wyhsdqal.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2komemigu.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2vtunicnc.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bjpsfwtk.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2jzshugch.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2arnxxbus.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2npkysocj.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2zxcogbfd.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2ubnyykwe.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2twujwyhs.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2kdiiefzh.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2ljeszolw.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2qmtnktkk.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lmjijtie.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2pikelrxl.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2jzjjkacm.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ygwujrzo.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2ougtxqpq.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zkuelfkg.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2tyqssvya.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fwduoctf.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2jhhwxvtt.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2aoxlldvn.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2wsbkfskd.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2hyedhmyg.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2oexingfk.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2ergpygvp.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2ruyoduhv.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2utlhjsjy.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zrpxrbca.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2luypofkx.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rlgtppre.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zljswpwz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2iatxqfzl.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2msmktpii.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2frwnafyn.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2hdsfsxoa.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2kfpeidqd.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2lidxvolx.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2lmruppfe.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2pxdzxxob.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2slxmpiwh.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2hhcmurqi.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2gmjupzoe.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2bejbaiqm.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2nzfwvkpr.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2ulztxhvz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2picvtlyb.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2pzmaklwq.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cryefpfx.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2ldrcvptr.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2zinpfawo.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2rwhplhpc.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yikwflcd.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2wlgusafu.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hmfweuru.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2tizvfceq.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vgacasty.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2rcljrogi.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2vyoiuvpy.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2usjgkxto.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2oavcobzw.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2grcjrloh.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2zmfgfyei.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jxfnhcwz.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2wevalanr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ihngirnl.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2jbazbauy.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2scxpxedv.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2agmajtnw.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ojqahyiq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2fgskiesl.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2pswrwkyh.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2yidzxzzk.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2hckiuueq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2robhyzos.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2oqxnenjf.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2silrqrbu.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2giecwlrq.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2fpgoeold.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2etxnrqmq.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2iawpnhdv.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2iyajsehj.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2uwrtdhnb.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2eenlpttd.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2wcbnwsix.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2bawfbaya.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ynsxydwd.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2lpjdrgmc.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2lnvlfcnx.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2arfcfhqi.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2yhookrpm.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2fxwzlkop.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2tpnmozyt.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2huvibpxi.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2wnprbhnv.html


<!-- 参考信息 -->