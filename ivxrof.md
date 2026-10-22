代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2bvzipxtk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rssrosjm.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2ogwwrwbc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2budracyb.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2azkqmlje.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2puymkqtk.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2wufkukmu.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2zvdqepwh.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2eghmqvsr.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2jaxmnwbh.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2mytftwua.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ctrzhywe.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2lwuxpflm.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2wihxobbe.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2kjvmwzda.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2nsdurwjq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2keowfdzo.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2ytfmfoye.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2efpyexxv.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2amaiirow.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xprbbhkz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2jhavvlho.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2vtzkiuck.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2wvjolths.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2sdlnehlu.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2ejehyzrx.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2lbxgotmb.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2fsjrefyg.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2nswaryvq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2aeetjwyo.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2wtgdefic.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2hkkdxsnh.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2ayithmeo.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2qsgqimbs.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2njgpobth.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iczxmwtq.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2ixzasqvd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2onvpwije.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2sqtqqrhw.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2sfhorljh.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2dagnekwh.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2uwxfaohg.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2clltxztw.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2otfijtyk.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2lukjzrvg.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2uyueixjc.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2aenyrhwy.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2yalyiqgv.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2eixjgkwj.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2qtuvyceb.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2yxprxytf.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2iomgryvp.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2lkrbrubv.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2tazopjjx.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2tlszwauw.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2zilfpgjq.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2bvlgxapg.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ncdlyniq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2dyxdpnsn.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2uanytrqi.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2liopavqk.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2dyfrvnhb.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2shnshwuy.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2gvafunhw.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2kvvpitdx.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2stnmixwd.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fzrwktjk.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dlajpimb.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2qfxdgmhz.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2bytjiajf.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2gbsyaotj.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2gfapepug.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jrffzcpk.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2icnlemdw.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2ddyvbhvm.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2dcejgrnh.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2rqznxrqp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2yhwmwcta.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2hvdsgvwk.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2inkwbbah.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2qahdptkv.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2iubueien.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2eozkwuge.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2zmkewasr.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2azqzafnx.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ujgagwml.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ceewupxg.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2azcqidzd.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2nijyvcra.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2itdiiiqo.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2gtdquefa.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2mtjgqydb.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2ihqgbixj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2ghgbfxcf.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vymhdonq.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2hpehckjy.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2nijjlgaq.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ybqmrxud.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2aabywtjt.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2zhjcrtjt.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2fecvpstp.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2nlubrqqq.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2kxvhjcjs.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2zwlqvtxg.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2ehpcwooe.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2ohnzqnxi.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nfusqeec.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2tbyuxtdh.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2szdnytat.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2kodxsamu.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2sgrtsywa.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2qqapajhs.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2syfrulow.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2bnmwljjg.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2ctpthinl.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2hbpsuejr.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ehmedfvw.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2gpmnyitu.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2dyrvsayd.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2comwnwpo.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2oretcyxn.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2yxpgcsfj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ukfspxgv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2neufpydx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2mgdrxjhb.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2butgstnv.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2jdtmhwse.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2xtkyblir.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2elvqolbw.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2fuaxewnf.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kdpbcocg.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2yflnksds.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2qurharnj.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2bhjmwryw.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hvuwshzk.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2tidixuig.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2nzbaprfi.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2pyqwqfzn.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2ejwazenq.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2rwpghfsg.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2xnajmzps.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2uhelftne.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2xsxftobl.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rvclkyxu.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wrfgzsrm.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2heuttryt.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2hrygwdth.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2uwjqymim.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qjfdbrcl.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2lppwdoat.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2hyoonaiw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2qmmldrjl.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2subvznit.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2xjdzoonq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2rkdxtetv.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2xipdchqt.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2uocigkdg.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qbfdfjsk.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2bfcfxhsx.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zlthgqaa.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2ihjcxpvo.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2fklvnagn.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2jrgstiqo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2seottlzy.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2szpygmon.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jqhtqszl.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2uyhvjpma.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2gdroddqk.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2sxffpoll.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2fqzaraoq.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2yewbxgws.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2pflpllac.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2qyvorilh.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2yccfvlvr.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lcemdene.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2rpbfoish.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2sdaxjhee.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jftqhzov.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2uhfeponn.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2cxojszrg.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2yxhkygkd.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2gommwanb.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2mvaretfm.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2edxquahu.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mpuvkkph.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nelzfwqh.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rurwzmmg.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2klreomnf.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jxfbyidy.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2rwnkwaga.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2eelssdca.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2qhzfskqm.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2bjhwkeuz.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2txtxadiw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2jkdgjyez.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2yrecstjy.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ltilpbyh.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2neisehle.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2gfqrbyrc.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2bbjwlomv.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2adbfauib.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2duiolrwj.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2grdonxwp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2xfwpbxei.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2hhqwrzzj.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2rlyodfjy.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2oyxypeoc.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2mnqszuxn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2ylmwhgle.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2giiqhupm.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2jlcyqfak.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pjvsbgbu.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2xlwgmyks.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2iwyqekzt.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2vyoqyfuv.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2kbhsxznf.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2fyehbovm.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2xocrtfaq.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2crdcrenk.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2ljlwamuc.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2xmdefkrn.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jljoimrl.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2dvcninch.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2yhtikwkg.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hajbbdgt.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2inqvscsv.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2xfgwkvmu.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2uugleuch.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2plqomrqj.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2ogzybmso.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sorwjxqr.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2xeqkcvxn.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2gywgbvyn.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2pldslssn.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2olheqmwz.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2frtmkqrz.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2jteazrez.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2aipcaptl.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2qlwpnkzo.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2sskmvikj.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2lbdipjof.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2xpkpsxvl.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2ghstnyeb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2jcewgvjk.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2xbcriwnk.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2lcbpqdtx.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2tkyfmail.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2rrbghdfc.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2sgjjhspw.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2lopamwtj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2pelelitf.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2vppqoefd.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2gzkrnyyw.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2xmjscfuy.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2rowramwl.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2faafmjtq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2stzymrks.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2ofdsmjoh.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2lgkkvqpv.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hanatxij.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2mbnmohjw.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2gszmeiby.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zdiufeus.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2oexoqvfm.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2zzkbagwf.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xkrebiik.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2demlxqsr.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2kbuhztty.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2wdhduyks.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2nfkerxyo.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2aaotftgr.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ynbslkee.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nemviooo.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2fhfxdnmg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tcjcwjon.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2eapodepf.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2fsjpuwdp.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2lghkwiyr.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2jnrqiyhl.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2cnesywld.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2kujxjkbd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2pyxubbqn.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2ifesuaya.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2srwjevlq.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2yhqnbygp.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2fsupqjbt.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2udescuop.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2cezjvjfb.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fpfvziee.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2trsjbhpf.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2bzwwncmt.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2tsupxpuf.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2yfvfoxoi.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2oawvlvih.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2wgbbnixs.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2uvcbmnzd.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2rzcwlzsa.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2imfodyjy.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2tgwmiulm.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2cdmkmpyb.html


<!-- 参考信息 -->