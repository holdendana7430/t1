代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2civuezeq.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2qglyikwf.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2pjdquvum.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2kmaywjmc.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2ossciole.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2omdoengg.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2wdvcaouk.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2yistvnmb.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2bjvhpsni.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2lotgxqqc.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2splvkvhi.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2epqytcmt.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2nambyepe.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2zpbfazyt.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2jdrxpsyu.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2mgylhxgi.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2oiqqloux.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2kqkbcwio.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2dockvyin.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2gctynoys.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2godugkbz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2pqwgzvcl.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2fvnqtzoi.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2zjwdzvkf.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2cfzaxqya.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2mkspmucy.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2lgoovrli.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2kinhqubl.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2fqmwlofp.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lfojlnhx.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2ztzytivn.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2gksaznif.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2iqxaijdr.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2rdnpcgfq.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2cwechqlq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2ppkqngji.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2rqrxbhdj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2ckdsgbym.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2kuhowhqc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fuvtsqbm.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2pxsvxuth.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2ijujpujd.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2ngeimrjs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iwefjcpd.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2jwbpwkkr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vmwdzzvu.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2qotyynbw.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2jljwdxqy.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ppdgcoqd.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2zezznwhg.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2kwqlrxwl.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2lokxefta.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2yroxwryh.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2zxsdrrma.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2axqcwpic.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2zmrdcuwt.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2flosedqs.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2yeajprxq.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2kqxchbtv.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2endmotmx.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2kbmxycyj.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2kkuqsfxx.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2iyfgdlpx.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jlmyhgln.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2qgrpgnko.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ugcgjehx.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2vodkgpbd.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2fntssmkd.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2qwhdfowr.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2kyilirsi.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2lskvvtky.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2zlqcnrww.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2lhyjwygm.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2ymziacao.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qcfthqft.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wjbqcwbw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2ouyhlgmd.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2qqyafutr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2kbggotsn.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2ktebavzw.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2nggcefid.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2qaqrbxsz.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2nqdjsrda.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2dbzexavf.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ncwjbzzf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2qfrrkmdl.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2symtprsa.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2acvjisfd.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2uqofgqzh.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2jybbapai.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2eeckfcad.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2psmlpnvq.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tlszmxlp.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2qfwkddae.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2ofibswmj.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2jdnkiqqh.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2mvpddsxj.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2qukbpset.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2rdlwnkat.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2szfbumvm.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2ygjbyijx.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2majtnvin.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2dtaujrhm.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2wmarccvi.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2mvuzecak.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2uwrmpqhb.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2bcklewiy.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2hzzrmbns.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hygpfxry.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2hiyvmqvy.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2yjurtytm.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2mhnxjnxq.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2zuqhdkrz.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2orypkada.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2ntzaviqf.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2iblroixh.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2pnzsgbru.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xabjpnnm.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2zjknkbhs.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2dkmthmkn.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2ibgkhnvf.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2lfthswzr.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2xquseszd.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2uczcpvoz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yfxhzltl.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2krlbbpai.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2vcpyyddm.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2ctqcakgp.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2ejpvhfpt.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2nawdknvs.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2qindsomi.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2ksdunlzm.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2iihvcxiz.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2iwpvkicl.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2jywnvpke.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2xsrfuqvg.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2ggbfwgbt.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2gfoirvdy.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fpvcbuog.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2jjyauprh.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2zimpqhpj.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2fygapbqu.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2nkdjchha.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2ycweitfp.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2mxseellx.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2mowkztoy.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2lbvbedqr.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gczextsh.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2acxdwlpr.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jjzduntm.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2ksispyun.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2pncfgbov.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2jyhnqjnr.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2spfpofeh.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2fsgoqtuj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2bpnpuevb.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2dtgugwrq.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gsjykzmz.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2qooiyizu.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2emruqkyx.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2ikgimbxu.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2sjaijawd.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2mlqwpuae.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2pcodtftc.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2xsfdpfms.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2affhwyah.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zebslbkt.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pjlhnnde.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2jmuguygf.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2stetensi.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2lbalqmbx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2koczfryz.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2qskjhgbo.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2ryfumjyl.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fpuibgyd.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2xcmrzfiw.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2bthklejv.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2abuccrna.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2msosfzuo.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2jagdnywj.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2kiovpusy.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2chvcqyve.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2eiantkzw.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2lmxttuhi.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2urnarywd.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2dfirqpfj.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2xojekgwa.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2vyepdrtq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2kdvwifsh.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2fgrpmhwi.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2yejwtbro.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2owcbenpd.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pvwmcolr.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2ubmojeug.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2vlgsgruc.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2kzbdxryq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2bckjprwq.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2bvdorbkp.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2sppeifts.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2pzmvirlq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2gqrzlsbj.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2goqgxhgk.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2ghsaoipm.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2euffupjj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2krqvljrj.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2chowxhhp.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2lwcklmkx.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zdhygwux.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2rrpailkx.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2tgntnnrg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2vfoblska.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2ypdhgzwk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2xxkerngi.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2ixxtpndl.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2qmkfejuf.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2lwdvqnrx.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2ulbwtdfg.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2ppqzzymn.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2bsgmewdc.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2glileikp.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2wyzvpstm.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2aarkuqnk.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2hariqrwj.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2ezoiabgi.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2arxjioqa.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2ngcqaace.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2wglguytj.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2vkziatza.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2gmhbvnbu.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ospjwvbf.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2chiysvpc.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2xkqnazgb.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2nvkuqcoe.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2pjkkgggr.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2rhaqbaff.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2suedapmr.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2criyfagq.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2hbnunjim.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2fvipqlgz.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2qtkuqvbi.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2xtjyuwcz.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2khrotvyx.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2aacqjstx.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2eihdidzx.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2xafxfhrr.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2alwagwxe.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tlymccqd.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fgwrimcd.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2jcstdppc.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2jcbcgxwu.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2abkdyxlg.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2akdgsukl.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2dlmcyhlz.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2lcyustoa.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2iigopsgn.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2qhjfxevl.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gqsqdqco.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qjtjbwxb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2xccogpjc.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2trjueefw.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2hdixfxgb.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2gdhpmapi.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2rjhmqgti.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2zkcwzgdp.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2mapkrmhs.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2olrsijui.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2fakmzbsz.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mspsxbft.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2yhqubznm.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2wjhwothx.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2czqcrvov.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2xevczcbh.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2mhcgfzgj.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nnxgrdlg.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2zedmkzyb.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2imkziimn.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2afctznqo.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2lvbbtvhk.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ubvwrzij.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2arwetyek.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2memkazgd.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2rifknpfs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ppwftfxc.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2cilmlrap.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2jxveddjv.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jzenxzcu.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dmazmhqv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vazsbrhi.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2nzjswctq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2bukjsymn.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2bwvmxxid.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2pjsuiaez.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2loqzswmc.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2kenrargu.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2ekwfhteg.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2xyfxllvh.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qkapryxa.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2skgstkxd.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2mrzgnfcq.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2dpqnnmnk.html


<!-- 参考信息 -->