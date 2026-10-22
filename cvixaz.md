代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2mmasqrsf.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2pknhagmd.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2avadvxzr.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2dzbgqflm.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2ccbxwsma.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2iqpaedrg.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2pcjhsbug.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2dgpixwgd.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2flethbce.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2tqkwujst.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2jfiyuyfd.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2tevdbsjb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2zjwgtrjy.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2pknnpxhu.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2aqzfoeub.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2hrqpssfh.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zpsdhzii.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2crlxrewg.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2sggwumul.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2pdxuwukm.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2qwyhfytn.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2wsaarnfe.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2xlcnzver.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2rhvknytl.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2wblqnmup.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2zodrfsqg.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2vrjssxxo.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2uhiddwrh.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2anihezhg.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2vhtnyjju.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2mrmtmonl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uoviffmx.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2zpepeycv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2efeizrpk.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2jaayednc.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2conlztny.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2tkuflvbk.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2dxnzildt.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2ywnssxvq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2xqhazxzv.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2jrytdgid.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2sxkxtzsv.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2goeixcis.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2qfswxrwb.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2iygofdlu.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2tacojsou.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2pfmarwuw.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wbdusmnv.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2pdvxwowo.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2vgyaoieb.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2unhellme.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hoduuxrm.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2hovfgngg.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2lummsnls.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2iunmvmsv.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2jvraxrph.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2kdbzbqmb.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wozaxenw.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2smleviji.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2vmfsjubc.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2giafbzat.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2pyohtkbp.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2pqyndids.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nyxxxnkg.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2elcyuxju.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2lzanipex.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ncjyubsv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2giesxeft.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2hlosyyaz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2lfoabzya.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2gckmkkme.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ycbogufv.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2mkltgisf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2vpjvydig.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2owllbscp.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2bkxyxxhx.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2fadkhwit.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2hukmqtzd.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2vaijtpty.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2mrfrhbad.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qpzyjntr.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ksoggwnp.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2vkpxvftv.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2balxwirv.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2adedlcag.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2iabgtomm.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2lfolifpo.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2umjesnin.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2emqbncrt.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2bcvxwzvg.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zffnfxfq.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2acsvqkhf.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2agxzoopc.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2wtlwfyuu.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2naahtfks.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2zejjipgd.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vuopfgqy.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2qikylkgf.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2lnxgsjfb.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2paojqryv.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2ghoortwu.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2lawgfaoc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2ytvxwmze.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2luhbdmkp.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2kcginucg.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2lwgyljou.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2pcjvlsij.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2wxkkxmki.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2ohpysile.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2bpqcbxbj.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2qbdmzhtz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2vhutinkh.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2zreiyqjw.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2khachqsh.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2immikuqw.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2bfmdrrop.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2vjckictj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2qedpklsf.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2pssinevr.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2iedxcsin.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2trtdxcvh.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2nanavwnj.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2rnmjbzzq.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2lcgcjjpw.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2dptskfxf.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2msvusltn.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2hzpcfncu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2mudclvpr.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2ywpfdtny.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2errihkvq.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yrqqvmve.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2euaimjfc.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2cbstqyct.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2rtupcfvh.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2mbpcqnev.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2pqodykjk.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2lunuoork.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2uiehisii.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2abyinmjd.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kyzcmjtw.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lonmnubb.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2qqirdzfl.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2mrndehfp.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2zgosytjx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2gqqhyvnf.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2vzjubgij.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2qyfrtzji.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2cuqtdhkz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2cmauyusr.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2objjzvyp.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ajnxxcjn.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2ksshfhnb.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2ihsdsvnd.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eqrcsdce.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2iefmysio.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tkaoqfxz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jfbdbfrp.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2hmrikvzy.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2gdobxfry.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hvllglkv.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2wjjdhigv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2kkogkdqm.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2lhygrgse.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2wsdpsixo.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2igtvdatq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2vcydjrdy.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2whrwnhni.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2twswsnuc.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2yuwvvumj.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2lfwcjzup.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2upsvfssr.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rwtfvdfj.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2sdpcqxoe.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rtgfqvmt.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2rvkcmlqz.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2idmruocb.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2gohztfsq.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2qksqlspa.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2dezirgbo.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2eooiupdp.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2ntlrgdny.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2ajthptyj.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2sofmcalu.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2fbnqfhsa.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2makdjiqu.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2rbdogfji.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2uhdnppzs.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2odwsscld.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2lqgfkqiv.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2bsrhyksd.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2ouzmdtbx.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2ocorrtuq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2lzgqxaqu.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2qtkeivdj.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2ssgqxfar.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ispqwibb.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2nvnusoai.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ubrginka.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2bbjedwzc.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2nbqrtxhj.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2wbezolyh.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2nfwzrjyi.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2fxuvfaxz.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2lteamery.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2qgirwaga.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2qdwyqizc.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2fphstwls.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2ggnuumit.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2pevriowc.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2hyytbrcq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2fedhhaoq.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2etsdkmqc.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2hsxkzlgn.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2nxpvpffa.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2qqrklfkk.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2kdomhajb.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2nuaxwnjg.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2kpyrjxbn.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2vprtczof.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2nbjxoyqw.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nabimsbe.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2tzartjkt.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mpccyfxx.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2qqflppdf.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2pbqfxkki.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2umhnqzew.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gstciegm.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2ojquixcb.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2tvzexiqz.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2rccjuqjw.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2onavpxec.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2xopubvrh.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2jxumoltm.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fnanehpb.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tpapkvet.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vbjnnsqq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2dsovromw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2zgqwqwde.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2tojerzrl.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2izpntrwm.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2mfufgqan.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2rtjdayaj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ulhbtjsl.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2usdvpfcm.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2tilfrkfn.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2epzaqngw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2vbekcjdd.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2plwgsbng.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2pbceqdbq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2lwxmbcvb.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2mgykdnpz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2ufrybymr.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2crmaqxkd.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2cvudgqzs.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2fmllosmz.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2betxhgua.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2ccuebchk.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2paipeaft.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ahldmesa.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2yairoizd.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2dhtqlmqb.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2efcbmjho.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2zgoqzdbz.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2sjtcxvqw.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2voluvrim.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2cmqrmmcw.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2vaokqgnj.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2aamacmnh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qcdqotug.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2lsumkbtk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jytccacl.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2xalqexxa.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2uzdcloly.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2nvtxwdgb.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2uynzmyqp.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dnnlzcha.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2fkwqvxhk.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2dpbwuxmn.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2ezfamdci.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ftzcazzj.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ahvipahz.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2hmsytild.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dlgytqhq.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2opddrdik.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2eqdaloml.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2momwyyhh.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2fovaaovt.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2hyrpjxik.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2rhnjdtfz.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2liyteojt.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2yayjcvyy.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2exrodqga.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2muatpssn.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2wusyixxm.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2loyqxeww.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2xhxnwknk.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2tlqecfrr.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2eyklprik.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2reslgzla.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2rsctlmmu.html


<!-- 参考信息 -->