代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2jbfwsxum.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2ojbngfww.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2keklrhet.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2iuxmjyrz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2cvttertb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vctuzqdo.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2pxyofqgy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2kpqqojux.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ctmgvqce.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2lxdtobxl.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2kyicnimf.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2dphtjcsh.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2drgxrgkv.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2rtnfwxmx.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2tpvapoov.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2baprakff.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2cfbtxvxt.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2cvsiasgh.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2szhhcden.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2lbqdessh.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2xjuhfaid.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2dvmtojjo.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2lgotdpiu.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2etatthps.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ercwkwbr.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2muhjrict.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2ppkcugee.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2ytvbjvxt.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2hybbaosq.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2xsvkothf.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2mjkxlixp.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2aglwvtys.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2nfyfnhvx.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2dggtdogj.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2okrdcvkm.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2qbujbjhj.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2pujykjte.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2gejlitkg.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2xuwmxtku.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fubbtyjy.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2aeewoiea.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rbokjjqm.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2fnmpflxl.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2yixzxwgu.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2dlabyzxo.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2dzwecqzo.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2zzjnswxe.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2brqnjpdy.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2aalziwtc.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2kbnjufse.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2yjtbwwgr.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2ucgahoja.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2ikhnkfmz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2fuftivff.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2jlxqwbtk.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ajiilqcc.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2iirspqii.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2nlrqqzdo.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2vrhpsvhr.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2sqkglwkd.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2lrmnrfoq.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zysizzdc.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2nzbmftdg.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2nrbeprpq.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2uvyonuck.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hylksmqf.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2zesjmxum.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2gqgbrifs.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ijkyyhxn.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2qmlbpiom.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2qranjmkr.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2mmpentbj.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2rowpjquo.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2zlaqapko.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2khxcmbmj.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2tdbxxtbe.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2iabkkfvf.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2inkrczte.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2baebflzw.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2mjrjzyqa.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2fluusyvb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2mfhkiavz.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2amyddfjh.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2dzuoylme.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2iedqtsse.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2amhqogmz.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2cdtiqhos.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2iepyfjgl.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qefwezzz.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2szsizyxi.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ksxctkmj.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2tzqytrdo.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2ijbnnslo.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2icbffbki.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2onaargvr.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2dkoymirx.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2zrimxmzg.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2bopdkgfs.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kqynayrj.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ivkzghhr.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ccghvfaj.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2lqcyeegw.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2nnbiawmq.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2itepgboq.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pjgzdukf.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2sivkosxz.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2szzdbxlz.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2fanuaoau.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2pebncjup.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2xftyoplf.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2gfatbsfr.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2pnfkhinz.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2fezhrspx.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2hhhneplj.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2xomrpwpg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2pgcitpvm.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2vdfjxohl.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2rjaxwzqs.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2xfemmlqk.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2uqnaaflt.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vojyugvd.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2mpuugyme.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2pwxhktox.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2zoyhtiuy.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2xlvniecw.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2dumogpvq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2hddxxthu.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2ctfyrrzx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2sdbzdauy.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2lrvzkixn.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2ngtdvfnb.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2heuusoul.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2upusmqhs.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2sshihnif.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2ydachlzy.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2pcyimgld.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2qlqwhoye.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2woygpyjk.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ziqfbmlf.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2ulhsnvoa.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2avhcrbsk.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2zlanoycc.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2mjquxnbq.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2uujnfent.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2pqsdupcl.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2dedeitbx.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2mfkcwfca.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bjzjzelz.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lbulwnqc.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2atogfusl.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2anbcxnag.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2rdwgcsxb.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2atxlouef.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2bcgangur.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ujpvzndv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2yopjwtui.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2swathsah.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2qpiigpey.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2dtbdjieo.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2ppvkxnjs.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ikyfsnqe.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2erximgad.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2stfaayaf.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2eggedqto.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rjideuuh.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2abdxzbij.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qfbutxlq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2kmiqkujx.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2phntcsdo.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2zupkxmsr.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2tvbfsywu.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2tkygkbsi.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2hfexgcrs.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2fzqkzlbw.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2hplycttx.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2afujaipp.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2nhoixkhm.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2menqesnf.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2onunyqlh.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2eojqqvxz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2isltdygo.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2agrgsegm.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2sfnrmegf.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2urqpzpku.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2towofxwr.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2sryqzlxb.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2gtfmavxr.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2tqpzpdsx.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2frcqwmps.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2psdxbzxw.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2aptlgqlm.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2wrbbbqss.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2xlqhvgop.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2rftaucez.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2umbimazd.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2gaydnyfe.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2pumhyxki.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2uztdwymd.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2cmdbesgg.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2ovekepnz.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ehucmoyp.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2ufkvrdgp.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2uikxbgtv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2cmwczqob.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2umhlgtrt.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dxvntcjx.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2dugpgqtk.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2atpacvfa.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2spjfpmxv.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2rhlwgopk.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2heltszlj.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2eitkpkjp.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2bhoumdow.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2oclmzctw.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uiwecmcm.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2lpmmxrdk.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2qupgvike.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2japhtpjp.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2jradozxo.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2hrlyslzs.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2jccgntuh.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2wotranfn.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2rdpamxgx.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2hgcvqnxi.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2dzpzzqwi.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2wezecmxx.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gliuyqnq.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ivbbstqs.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vnjzvhnw.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2nbcowbcj.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tgcpzjoi.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2kmhnyauq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2jkyavwkh.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2mzicuxpf.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ptdbhpqk.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2bwmzcdgl.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2tpzcqbut.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2gxeodhtj.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2pxvxkppf.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2afanggzl.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2ipylgrqr.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2ndcaejmk.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2vhhuyair.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vdjugywa.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2prakmanb.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2ugyjhkdf.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2wunpfsry.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2zbwkddgl.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2jckxnvpm.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2jnpyaiqc.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2ufnxcpnv.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2wbxbzzcl.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2itmmgxpn.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2qdcbkvdi.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2tqgfugoy.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2ruuwvryr.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2eqliumxk.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2pidgcssp.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2jwwelxrq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2dmpvahnj.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2rxsnvmrx.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2niyyrgcy.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2sazhfsng.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2oraytjbv.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2hgyntbfk.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2qrpdsdao.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pyopjgyk.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2ilyedsxq.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ikmkjbro.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dpcujnus.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2edvewxso.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2rltwwmgk.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2rhzpzrzl.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2ykpcrdii.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2jkafeasx.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2owmnkjor.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2siukwgjy.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2ywiyadev.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jdrmjzrz.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2xhfkmprl.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2dmcraswc.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ogqzxulc.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2sipvcokg.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ngdboisv.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2xeqbpnap.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2ijtifpma.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2fyfeljqf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xghpomlg.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2uiwqgdvu.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2btuuhqim.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vdqovwuz.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ivfppfjg.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2lpotqubm.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2peidqeax.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2xcharavp.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2rzdpfqnb.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2rzurwopo.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2ewltgbpm.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2xwdgkkxf.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2cgifgzhc.html


<!-- 参考信息 -->