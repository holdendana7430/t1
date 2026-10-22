代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2syubhzus.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2rbdtuvsg.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2rlniarzh.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2zmwmxcdu.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2xhkbpkbh.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2khlqenif.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ncudvyie.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2xtestpid.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2rdvalpse.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2vysuzvdx.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2mqozkqtd.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2qwuillgu.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2hrfetzex.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jgpoaykw.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2ojnvplre.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xgqknrag.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vxtzajov.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2yhiodzwd.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2ykiikfou.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2ppvurtua.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2bwrqemuc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2bllyykrd.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2bzofdjlb.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ejlhjeex.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2uyewcypq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2vwfohsom.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2tyolvoqt.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2iomawlcw.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2qsslpudk.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2vdujegty.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2nsguvvxn.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2exlwrkgy.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vazbrkbg.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2xekllyyr.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2rejaeycv.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2xfeptkyt.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2boxeapmd.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2aoawppks.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2prtudraa.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2jwyqxfbt.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2nhgraxcy.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2nyuhbrdb.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2pmfquini.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kuyscnbv.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2loxhwdeh.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2jalsyhya.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2fupdrity.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lcseytol.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2ipjsjmyw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2opltpvvw.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2qiecbjdh.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2tpsgxcyp.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ulhliexa.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2eueuycoz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2hsyjcupe.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2nrzhjxgu.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2ovgizrto.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2cquqjuvy.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2nlofvkzk.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2oysjtbxv.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2frvqlmyy.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2yvkgddxw.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2gnlmvncp.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ullrppgs.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2qtokxzpw.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ugongutv.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2hlnvgjde.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2lskggosm.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2ijhzyxcf.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2woniluuh.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2bukzgtxd.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2roplnovb.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2opgawebz.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2oohsbzbw.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2yiuxegxd.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2kktswtff.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2grilnajl.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2trludctv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2rrncblbh.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eqizpiha.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2qakpmewu.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2rwafpvki.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2qdxinkco.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2jbiemdye.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2kxontphb.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2specboaz.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2oysvdaev.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2qeehayjh.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2qsffxsjz.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2smqfsurr.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2oxujoona.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2ybghwhcu.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ltulpzhi.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ygdeahxi.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2gkjnvoau.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2kjfhpgox.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ndxfpcey.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dytgrtig.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ryudzukc.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2nzthgigy.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2neitcwhe.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kxvddgow.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2albrmdbf.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2odqctleq.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2dfoyzbti.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2pvwqmpyt.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2hpwpifmy.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2kwbfpetw.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2zvejmyfu.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2vcjpjprz.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2bceasxyl.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2aenbzpdr.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gxejvnpo.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2cvlvtoxd.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ggoezaml.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2tqmmfsxf.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2rmfkkfsi.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2aawoktip.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2mlncmmbx.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2mrhnjzvy.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2jommbrwa.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2lcuqpwnk.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2ileaifgx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2liirhjjd.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2veoirkob.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2nydkwyje.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2turcnhez.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2jkkjdlsk.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2rpductac.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ruouklnn.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2dqtwekgp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2lnsjlfeu.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2viuxswtt.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2gpzestep.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2kzvliucq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2zpvjeimq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2mgfandqh.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2wyoqcbyo.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2vosxrlsz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2qrupwcfx.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2mxyouxed.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2ikurjsiq.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2iertfleq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2ypwbzymg.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2ogmctyjz.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2gwohicas.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2fygvhwpk.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2jpmypppp.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2jlnteznp.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2xgkpdwqf.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2qhjhhvfs.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lmdbjkcw.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2tawsmwie.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2xcdupsvu.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2qufmwrjr.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2amcgsrcv.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2phgwsbbw.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2jysvsadg.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2rkziznqp.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2nktsrker.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2cubqrhuz.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2nqaogagm.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gkdnhsdo.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2nlpictvw.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2vtzfdlif.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2zcpngljz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zkinwizd.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2cldpisnt.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2uskvpuft.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2qsndaxwv.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2lfgkmmbe.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2oxeclejs.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2excyfgij.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2bydygibx.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2guhqdtjf.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2annqytwx.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2ujabjnae.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jvhcleiq.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gbogqkcf.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2oqedagsm.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2nvnobxrc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2msxsfcdt.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2cfsgtckn.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2yvxripya.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2vherenvh.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2tzowhkyc.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rzdbmwth.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2uxgdmmmp.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2dmsopqqw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2eauokptm.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2dfpkstne.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2cfiogyvo.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2qfdqloqv.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2obrqsjcu.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2erzloihn.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2axzjyady.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2weiqjswd.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2irmxtycl.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2xoasaxvg.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2rpniecaj.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lfcyfdds.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2rrnpisxh.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2dshkcdjn.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2asjbdcrb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2yalcskdd.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2qgliqbut.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2umruukkt.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2bmzbkwvr.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2yzvuplfv.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2razzozzu.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2pdgnvkfa.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2qraavkji.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2trwddmxp.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nbwtmfbp.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2hedpyktt.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2hfoozizt.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2eazbidug.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2hqvejhjt.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2ckrjslpw.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2tnpnlyfo.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2eplzrwrv.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2gchbrhdr.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2brxzsauf.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2nqwzbati.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2kbyzylix.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2lenwowep.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2jyxrihib.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2pcpwhtxt.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2qrslygvw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2ofowgcgw.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2opmshcay.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2cmagfxpq.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2vgoexmex.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2eucddvtn.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jjfwjavh.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2qqrqjtlc.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vyipfefk.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2akpcpnti.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2psauwrgg.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2bbtpgmjw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2tkhbqlrl.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2jnkbqpra.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2rnkjfags.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2syhpijlt.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2pqukbjqw.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2thfbents.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2sgepbter.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2kzjxugek.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2irllthmh.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qihnmbsr.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xjficgwi.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rqxzjpyp.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2thzdonme.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2ebeyades.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2kfugltby.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2bsiwbuqt.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2bznamido.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2zsjyakjk.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2vfqsjlww.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vlrqehgz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2raxzirww.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2trjyzlrp.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2hcyoisgq.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2jsbhegtp.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2huoygdhz.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2aoegxagb.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2kigpwtsk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2bwzzbyzo.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2myhvsgqw.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2ssobfjna.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2qrqlglbs.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mlvptjut.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2yzguphnn.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2izkjlbiw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2fqilzqbj.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2nogaaixz.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2fuuckwpo.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qndixjgt.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2igglidlh.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2qgartpmp.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2adttoryz.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2roquohya.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2bwufvdhq.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2undijnyi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ivglrree.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2lgjdmkxg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bbwpdcmx.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cngazumt.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2ovyaccii.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2dkmsrsal.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ctiwgaqx.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2fyqcdbby.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2zbanxbws.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2muibxdgk.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2zgteyugp.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2oiomjokd.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bjauwsrn.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2bvzniikm.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hltkgscu.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fqvftbvo.html


<!-- 参考信息 -->