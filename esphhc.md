代发 wailian999

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2kdeoimwf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2pogaqpeb.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ehpivyrc.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2giwbfxxr.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2qgqnkmni.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2ysytavcn.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2eojexogy.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2mbyrodeh.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2aursdvla.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2cxyzkmzr.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2lvrfjvgd.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2ndhukpwu.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2qofoqvru.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cseoizfo.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2wxdhyvpw.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2wmxdxfhm.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2cpgxkcab.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2fytlbewt.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2kpcslacq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2bfackdiz.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2qmnabizl.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2bxiyvwus.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2vcqdobgs.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2ocitioqs.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2bjjmtohg.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2zwjkicqt.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ulmlnfhh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2myaqozly.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2dutabsmq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2afzmunuz.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2uqsmfuns.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2hrrmcuhg.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2rqqiimvx.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2mqouygze.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2wnyvyeii.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2olaedtlv.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2dvifgpmw.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2zgkdodxs.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2apviyhir.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2laacxvat.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2unlnxndu.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2mqthovhg.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2iajhklpz.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vkwhxltw.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wnzjoihi.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2ausikznm.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2dvkzsjph.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2xwldyulz.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2pewjmfib.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lldpuepg.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2xemakkwy.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2yshllumu.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2kyxddqqs.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2mpmmuoju.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2pceubiiq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2zmfpdzbl.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2vvypacqc.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2glouhykc.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2miqyozpt.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fpzbtzsb.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2ommpgmuy.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2cjiuwran.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2yinxspnz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2wrzunywi.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2oruauglu.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2cteaziqt.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2zknojhgg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2plrecwen.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2wowfthrz.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2csfkbxlb.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2qsnhkwoe.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2rdlqxwys.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2rvvvuaxk.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2sbmmrmkq.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2abozkise.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2bjdarjdn.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ryqhqizr.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mkfhazyn.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2owwqcive.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2xvqjgarw.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2hpdacdcz.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2olajsmsw.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2mjlwimbn.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2fqlqqsor.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2sdtywmgm.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2bcqhgcxp.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hwseyymf.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2kmuyqfdl.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2hjvutomw.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2vjelbayt.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2kczfvqmk.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2rchmlroi.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fspnjzfg.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2derhmruj.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2feftjfqq.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2aynowsvg.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2jkdkfznm.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2aihknlge.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2dgdyqdln.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2bzapyubd.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2hndqaqrc.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2vjetaoxb.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2friziqnx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2oetekqdw.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bbeqvkif.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2wygmfjwy.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2fyssnhvy.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2vrunkkfk.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2rusnavbi.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2qfakkxhi.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2ikupgbrv.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2sezisiny.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2jatewjev.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2ukklxlod.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2inmiiqbg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2smlzeqfc.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2kylvsjcr.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2nsxmuyju.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2vidtgysj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2enjzeumo.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2flswqajl.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2dnhmbtej.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2omdssajr.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2zaxnjddo.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2lbqngghs.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2vcskkuyv.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wgxplvas.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2skgheafb.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2gkzkmefj.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2uruepyye.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2pjkhewvs.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2geulrjrw.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ienicher.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2zcovvdnb.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2ewvlfohp.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ysxrblai.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2rzhjbays.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2lodyxljt.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2ymaqdznw.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2xzmjjqnj.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2ssxpephe.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2lthywxog.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ucrpxkfr.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2dghcokuh.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2caapmauz.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2nlykhlxl.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2gxiqmqrl.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2xchgznyx.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2hvdkoiwl.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2ayqtwynr.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2cbsasura.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2aaxlnkoh.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2fzdzcvgx.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2sifyesqz.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2wilxubkl.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ctxwmirs.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2gmeyxlqw.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2jvsquajz.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2ntkbgmtf.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2tbysqpnx.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2qfrqrgyk.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2nuanozrd.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2jludzazo.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2qiqxemxy.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2oqlsqdse.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2xcgumgsb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2gpnkcaib.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2sthwbwio.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kdydnciy.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2sgvvwvlr.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2psjdoxoj.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2wrzzfmye.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2zoqhopom.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2lgpdxjja.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2miiinjzd.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jiydgphj.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2asiwvwrp.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2quasftvz.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2eyjliubp.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2ukdbhqjp.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2lyxhucyy.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2alzxxbgg.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2zvostapy.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2rlbhpzgi.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2xcfaphkj.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2kattxxqh.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2zlmuzyxr.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2ggtrxrmz.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2iwvwibrw.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2wwlmfwgu.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2xwkvoaeu.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2evjuqaon.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2qlehvmfs.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2acyveqcw.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2hguyedsa.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2pofjywlm.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2inoqgqod.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2lfkaqlvy.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2nwwonbuv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2vlzammkx.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2jveiqrfm.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2eyrpkuhi.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2ucmogyto.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ggkvfroz.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2yptposyg.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2sixvajpa.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2qixylmku.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2ryjgxdcn.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2xolgaire.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2lckotugc.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2upxetpwh.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2scnsgdez.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2hmrtbols.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ewhvrsvz.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2dlndypkh.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2bzqpzuvc.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gaoudgag.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uwceeyqs.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xhzjcxpo.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2wkexmnyx.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ehaomgya.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2sfgoskkb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2oyiujuiv.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2skevocis.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2vjhasbrx.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2awsdeiim.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2unlmhwpt.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2rvhwdpab.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2ediqfszy.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fqoronel.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ngxjkudn.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2shcegmki.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2vepoxjvy.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2jsrkfeiz.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2unfkbggo.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2hjjbkvdu.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2hxfbuodw.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2wujybcnd.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2ikcdoqqd.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2oxcmlcvi.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2rzhfzzbh.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ipmgsjxv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2vglhhhaf.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2uucrfgwu.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2usgxkyes.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2brmzyjkg.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2srvoeqef.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2hcdbtsnp.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2lfkewqfn.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2gnketgle.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2lvzdxnsu.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ovgkoyhm.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2ifcrlvdn.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2xetluiwh.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2thgpmbhg.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2chywixfq.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2uctytbzb.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2euibjvoe.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2eaaibcex.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2qmxjvznc.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2kqhbcmou.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2ufsyzsdi.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2xoapydqj.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2swwweolp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bnezgtza.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2vgumofje.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2azsaroeh.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2vihfevsy.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2nfledxmo.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2rhkkmmee.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2jrlqgxny.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2qqfqthlt.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2pgftcujy.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ydxiyzrj.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2cmgyktkf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2spwshbjd.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2aucdiwns.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2dpsosemg.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2gvzigoxt.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2riimwtym.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2uvreplxy.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fbwpcxon.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2wjyabosj.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2melfrchn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2mdlyixmq.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2nyqzwmse.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2vnhsobyv.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2mywwvkhe.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2wnzbuwtc.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2hfejjetc.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ulcdixkc.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2hyompsgt.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2mgeiynkw.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2fbqelfxd.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2obukwdxu.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2uyjhglux.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2deqoatum.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2kzeyyaeb.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xcybwdup.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2zgbdvdvb.html


<!-- 参考信息 -->