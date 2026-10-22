代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2agmvqaac.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2cerwnyut.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2romhsejj.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2eeafhxou.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2xntmsyol.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2mritpekg.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2hnwzcimz.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2sojalrnp.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2hldkztbb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yagratyj.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2zjgvanyj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mjqpgomz.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2svhewotz.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2vssyiuvi.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2pdgipdvh.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2dbfbzyrv.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2qoqmgarv.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2dreaawdv.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2vpcfppyu.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2zbdwkxbz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2hdlrvhnc.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2ncdayntd.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2rvennwlb.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2flpwzywr.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2vvwlpche.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2njmtvudf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2eagrgupf.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2tancjhnr.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2byppbrbq.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2uquwofmk.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2jxndoslu.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2yfjzyflz.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2sidcldyl.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2hmwnejbl.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2aymvlqyd.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2mpxdpwiu.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2xxdoncrn.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2nrjwdcxc.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2dpqlhtdp.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2kbomirif.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2mciaxunt.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2eqfckvci.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2hnmyklnc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2txbdlacg.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2fejoppkw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xsxfjnlh.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2dposjzho.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2ewsbppmh.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ghnzldnm.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2vjndqkir.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2wmifsxpz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2opmmfspx.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2khqpnelb.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2pahbcxlj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2pjphjdhi.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2xfuwpkpm.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2wyhmeboa.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2nwggahfk.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2pjadbvpw.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2kjvymzli.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2melsvgdw.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2hnhvgygf.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2oqindqhf.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2iyoywbon.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2kmgbartl.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2qanystch.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2ynvgowyl.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2rzqevfdh.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bzqtqylt.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wkyutluv.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2bysezjba.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2fawbjwol.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2jmatqala.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2sfadolbp.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fubqhwbl.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bpqsclnc.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2khmzapxq.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ejajffmq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2uxtgmyvq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2iplkogvg.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2rmvoxivz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2ffbhnszx.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2rlplmfsx.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2zyloydzr.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2fndrcwgi.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2qvimvfvy.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2wkfeufhp.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2thrhgxuf.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2xwkofvoo.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2bfqkpmyv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2swidhnkd.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2wwqtizpp.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2fxieqmss.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uouwwpcf.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2nsakzwpv.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2zmmlzfik.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2upghmzrd.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zndrjzwr.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2rpngpsig.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2rchorptu.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2tcaqxzjf.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2kupliuyn.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cqelsaxc.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2pvonhkch.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2efhqrbcf.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2dluydtkk.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2qkvxkvot.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2crehyjps.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hjuhlbfx.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2efqmpent.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2wcstejzl.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2atoknnjn.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2mdcgzigr.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2aasxfips.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wtmhxscy.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2vpzmlfoj.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2gmxqflia.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2diozxdtt.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2souairuz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2eagqahnw.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2advbhekd.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2nicgcxqz.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2rqykssgg.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2vkdzluno.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vycocdmq.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2kcvjmicv.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2lxficrop.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2gmmlskph.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2ychbzvdu.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2orkairks.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2zrnssxzi.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2snakzajy.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2kbbjbztt.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2oksykrnj.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2dniwkyoz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2oqzglfhh.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2suedxepd.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2ybxxvuga.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vhucizff.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2asshujpc.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2ldbmxczo.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2ngfbraok.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2rpnqxkuz.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2aahyrylx.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2wefzstaw.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2mvgiambh.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2bzmylelo.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2ixvmjkgm.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2kxuujqdp.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2nwuyopym.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2oobubqej.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xzoouefc.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tinacgwf.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2psqygsdt.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2farzstjp.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2oegcswfn.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2ljmwqxbj.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2qwgjnehv.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2hebjdsjb.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mbrrrejg.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2ddktuqvw.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2qsytnttc.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ahjoufsu.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2nxopewvu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2wibkrumz.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2earrsgju.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ekicspcf.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2jruhiuru.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2onesebnz.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2kokkodbg.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2vjnfpaye.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ikbvzvbb.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2ldkeysmk.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2ajuzrjog.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2uzikxblv.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2fjctftnr.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2dwrdnrou.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2otoyeups.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2zatdrqzp.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2apncxqul.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2rofuypwe.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2ddtfyjnt.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2relpukwr.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2himpzdmr.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vhrvakvo.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xucjtwyg.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2adecgxrk.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2kxblayul.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2eduadhwe.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2ohaotchk.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2vlboejhj.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2npmsybnn.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2mkdwkbsj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tzitggsj.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xwfdqphe.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2ifmueejj.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2kdmhdmco.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2xamtxrkn.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2xlgreqjx.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2mwycnzmi.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2cbhjyujt.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2kkrzubsr.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2hqwlnalg.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2loovmbht.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2catmbdud.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2lurjgweu.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2cuokbczr.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2scpuvrlx.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2dezurcpl.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2khuozuxj.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2ubywahvb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2djyidsea.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2nxjhdvmh.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2fguxmxfo.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2wnislbld.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2psykqelb.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2alfavtfz.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2uiblzrgf.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jcrbkmde.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2mjgembno.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2kdiswfzn.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2cmdjrrww.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2uwevhplu.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2mygorpmp.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2djrziezn.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2dxgzmsju.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2fruzytxu.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2uloseavi.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2vkfdydef.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ssllpwcu.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2jtrijmen.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ddndmdia.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vomowfbm.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wmwukpnm.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wsjhvjvu.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2tswyltgq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cbixqxuj.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2bokdiral.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2gueakowa.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2wmjlyzom.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2njhzqphe.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2qhegqmte.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2rppemaet.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2mvoijnbj.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2yevzmajw.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2kxsvbrqo.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2yapetoyo.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2yvdcchbv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qwzwujkr.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2vqgjvgzf.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2olpfzbre.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2kprwkvqq.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2rfzsstmn.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2srhffmuk.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2kwruemhn.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2yevzojwt.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2rmqafxrv.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2strhrskx.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2bxrrnqcs.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2hzebqong.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2mhefzqbb.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2ceypznub.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2hbyhjrcd.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2yqazsbfn.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2xvsyfavb.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2edrgyykd.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2idmgnaiw.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jahrkety.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2tfprcuit.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2hrvlwziq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2caretamo.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xuwlgcnx.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2khmnjggt.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2tkiblsba.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ksyswacq.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2bnskntsl.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2xfqpqrvt.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2xniszuiz.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2sioipqcv.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2bblfymew.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2owwhhwxp.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2xxkpjnkn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hqqfqtiw.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2uyescmew.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2knxhpkug.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2eycnevhc.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2maqdqsyt.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wtytjvlp.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2bxsdoenu.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2dclinoit.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2wkxmsztx.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2nnfeuzcy.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2jczfymvz.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2pxyuvgcz.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2itnulsod.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2hjoscehh.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2lpvzkauz.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2hodfuejg.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2sbxvkgol.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2duzluzon.html


<!-- 参考信息 -->