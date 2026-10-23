代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3zqahdngv.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3swhdbbyw.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3uhrvdzkf.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3ppjhcwfe.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3ptoraqoq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3oibxfsop.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3goflejqo.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3cyeswkec.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3rhdttajx.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3kypfniij.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3pvlitrky.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3wkmnwtwb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3lcznglpd.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3fxlrmnek.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3ypjeqoni.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3gjdppflj.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3kftvmiru.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3esureqxn.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3qlojbmsv.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3adverfuj.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3bdeekqdy.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3sqoyufks.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3zoaznjtn.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3mjxksdqr.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3lrqtbugk.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3mdeeqkal.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3oyviifbh.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3tjcubloh.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3ipdododv.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3bsmtwcuk.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3acxrkauu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xwbxvzoj.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3lodbtqir.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gktmmaus.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3dtdehsmz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3xgktkohg.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3trvwcuxv.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3hbbhknmb.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3colguloo.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3pmjyuhrm.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3cxhqjvuu.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3rxfizdpi.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3smgzzmgy.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3axagzfhi.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3ozxyskhb.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3ugfjnwyw.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3abgzyopn.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3icidlwmx.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3qguzxktz.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3jqcktdvu.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3fhsbbwud.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3gxspybqa.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3wszswwwc.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3qutunujz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3vmyslved.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3wgraxpwf.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3krzhncol.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rgecoptx.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3nczkwmbz.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3efdrcodh.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ejrblmkb.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3bpjhnckf.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3oqoedlgs.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3texueqjk.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3sxfjlecz.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3toucaidc.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3nncknjzc.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3ubzfxzls.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3shgcdzwj.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3acgsiusg.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3qwqrmokm.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3yctbcxxj.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3jqgmjsub.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3wrghcumt.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3obafmcij.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3knmsoocn.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3txbydiou.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3lspvbjwe.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3gflhgagf.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3izpuxvox.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3svejtzfu.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3cfjtrkvf.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3plrkllkn.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ttifxdyp.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3wbbkucmr.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3pofidzaa.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3qrcuuwil.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3vapqvybb.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3tngwehqg.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3nqvvnctr.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hjiftzoi.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3fusdjajf.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3avjlvmwc.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3rhbmufur.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3qnuyxxwm.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3uufsenrz.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qouodfij.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3wrbozwgx.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3plkhzdkp.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3ugspoxuq.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3xwtoplrj.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3zchwszpk.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jizcveen.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3ugngnrfp.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3pryjfgga.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hugelfnc.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3twmwmtbv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3vbfmybsj.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3njhgpdxl.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3rhoomttn.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3wcwxntlp.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3foddwxhx.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3trwelqar.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3dmsrxmjq.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3trbwosze.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3wutoeglq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3rixgimvj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qwedqqjo.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3wbefrdnx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3hfyjhpuk.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3hvqegioj.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3xnkdgssn.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3xbyporsv.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3fclkqyug.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3omycyfnw.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3tkqnckyr.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3sazrgkab.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3ujwciosn.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3goqhusry.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3lbsarrnq.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3epaxjbag.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3xcfpqetw.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3oznaqrme.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3cvnyvngo.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3xzpjcepm.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3wpldiavk.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3emsnljpx.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wolmixhm.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3pfznteyo.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3sdosfsgm.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3lsktaznp.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3gxlprzyc.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3gawywyvv.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3tdamaroj.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3pximvngy.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3vsyzqtze.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3dzblkahu.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rivyxtne.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3jtqysuad.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3xewsmekl.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3wmhqfyob.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3qlxcoerr.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3unjfhyns.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tynmaapq.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3bwdhjicj.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hxagspgx.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3taecxumk.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ukraoakv.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3dkukmnsf.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3lwoigozl.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3pbqwpyef.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3oahpnwev.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3xjwcpwwm.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3uzsewwgb.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3magcwrxd.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3epaffijt.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3hkksrtqv.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3zcjwbslk.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3cwrgqnmf.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3vhhetjbi.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3oadrwqoy.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3rukfcohp.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3rsddmted.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3zyvsewqr.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3xwzeoqug.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3amxjphxd.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3tucevcgv.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3pnjlwnmr.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3nqkpdlui.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3kkpzgqyu.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vywvwmzd.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3fpxdhugw.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jkobbved.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3ixztqrke.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bnutumhp.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3irrwcnla.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3ahhqmmlo.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3oblfbmgv.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3napqisoq.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3wsugcbep.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3ctgtikys.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3dzjlhcek.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3kbouturi.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3qvnujmuy.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3nyovjrpk.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3mvdicpgl.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3lcehlajv.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3lpfusbdg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3bdeikyhr.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3wkzrufzl.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3wtqqprww.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3axyphyjm.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3lymcmzlj.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3trsktqpk.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3esaillxq.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3uhymwoay.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3xpcsvqzc.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yacwsqdt.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3qrissnst.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3tzfeucem.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3mzkyfwqh.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3gxsxlwyh.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3euzhepen.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3rvazkzdb.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3zpyykyit.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3smrqssyt.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3wtflbcji.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iwficnfi.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gvblsird.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3znmvslgn.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wydzplxq.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hnrjnjzo.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mobsgasg.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3zdvrvshh.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xulhxxob.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3oidwpxld.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jdccfvkp.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3qluwfale.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3gntetipv.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3uyippexj.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3ejdfuuur.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3chnceudl.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3jcmqiyrt.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3ijthvpts.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3mfgbrche.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3indjodmz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3xlergjkf.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3mekqldqx.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3akrpqbyo.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3unijacqe.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3szyekhxv.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3evtxvaea.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3agrkrmpi.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3dqawhqcs.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3axgvuxml.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3tmtnuelb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3kacetuux.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3uevncvqa.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3brmqvjsu.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3nlqrjuko.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3pistbrnf.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3nykxsoeg.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3hueaiicn.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jfeknjyi.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3jgclgfnq.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3asdjrnxx.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3sevymqri.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hdsvncua.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3lbmbipim.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3siswmduj.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3esxfhxrj.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wqyhnjeq.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3zoxrdpqr.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3wemxwgfm.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3wjaobgyg.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3crprziok.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3kmachntz.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3jltlkxgp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dkkbrylm.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3qsvlbbtl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cqrrtotv.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xjzrtavr.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3xnkypmxf.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3bwomjpan.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ydvntnod.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3srhylsij.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3xcmpdkdr.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3soetnhzq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3wirmzawv.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3cgxqgxua.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jlnspuhg.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ejcgxagt.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3gwstpxtd.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3owsofftd.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3tkwdcwqc.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3jladxymi.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ieimoust.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3kzupkoph.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3ujzdxvyp.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3ysvkhjyx.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3bmzyxldn.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3phztrwbo.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3lvnruabn.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3gxverelt.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3hljajfnq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3cssqxtrd.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3oobkulmn.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3dzxdhqlt.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3uxhxxrkq.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3tuucbmki.html


<!-- 参考信息 -->