代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2ajsmmnlp.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2mkhbgtns.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2jtaapjyw.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2rxepignf.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2molfjcnm.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2hodcntlj.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2uuqcwcnx.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2dwavcyzb.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2bofvncec.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2ljlubhfw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ohkdhpkd.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2stvozhtc.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2vuvwosmw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2acvsdczm.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2cvkfevnz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ihhvusrz.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2kxxtnxuv.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2locobyta.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2peixamdx.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2oifjkogn.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2zibjneec.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2uoynycth.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2rzxxhqpt.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2emhwerbj.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2pgljfxoa.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2bfftrfqq.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2mudktrnq.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2unzhwzes.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2zxwiwgqp.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2jqcipvqh.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2mtjpezan.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2icsyrkiw.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lofalxnq.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2rcxbpubo.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2izujbgmk.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2nbitiycg.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2xnusadpm.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2vjrgqbvu.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2zyoskuom.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2buddtjkn.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2evdqljjh.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2gjonrkbs.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2yiaklpbr.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2gderpwaw.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2denanuiu.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2euwpaogc.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ydvivohq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xxaywrzo.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2dvhepxrv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hkejqhmw.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2pthvutzm.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2piuhgjgu.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2iexzzjae.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2zpwdybtc.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2gleciukf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2trdldiuo.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2ubidwqjj.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2wionsbgr.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2lobgaxeq.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2czramnpi.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2nvtcymgz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2zsqmrrcb.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2hmcahvxi.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2otqxeybi.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jevdsyjb.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2lqzsyace.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2zfqowdko.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jtkrljsl.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2ylrjgurv.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dpwqxgai.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2dbdtwcpe.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2celgemjj.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2mppnpuzn.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2adplpevg.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2rfwtnlpx.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2bidpeqss.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tttudrgd.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2graxlmmg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2rnkdgoak.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2byjtivry.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2msdrkxcp.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2wcuviimr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qupqvuql.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2fjpjbxnn.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2iqcpcfpx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2ojuytfym.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2fywzqfpp.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2scwqjtar.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2hkibnkpb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2kbyqului.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2dyfrhnkx.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2roqerxsq.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2paypuupw.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2pfesunpa.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ohmkxfvc.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2ysoaqypc.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sbvqthac.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2skvmbpzu.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2kyxycztp.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2rldyhiae.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2pyhedemt.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2kyumwmff.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2fjrsmcdj.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2vdbhfrzb.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2owhwnfvl.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2jmhlpsfv.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2idaszhtc.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2jmsilsyh.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2fgvopbji.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2jdvzxmyt.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2ilopsbwp.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2krwiqeyy.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2oonutqvu.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2uzglosjk.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2qkyphqrl.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2pltksexp.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2qkycbtlf.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2tnpgebqd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lcirjpwn.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2fdulxsgh.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2aoljixzh.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2aspuigwi.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2rcboblgs.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2kkgqmqyg.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kpyyvfxf.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2orokmiyd.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2jkdmkxau.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2qtwhsszp.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2bxsmaczd.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2mcwpyzgn.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2zjawudiz.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2nbsaedng.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2loejmwbs.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xsjdkgpg.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2bwprsawn.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2nqbgbcco.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2wcfciwdw.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2egjickgm.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2jullmyjg.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2mvfllodl.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2mpmvklwd.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2dnkngpfx.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qlveockk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2zjjdbyal.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2drzdsncf.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2pedxbijg.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2yccialwz.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2sopvuxof.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2kuihtqjn.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2fksaejpa.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2ptpxxyhh.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2mehlqako.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2qjfudfxu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2svhkxqob.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2pddqpxvr.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vjnkylsn.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hjiwgtiq.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2fwizupxh.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2ykkpmkab.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ctqyoqxl.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2faltesan.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2vaccagwq.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2dfohsesx.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2fhqajaay.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2qumxzlkg.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2smesapjl.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jxmstqhf.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2amdjldqp.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2uhclejly.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mrhgjqcl.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2wzwzjmie.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2aocfgmvb.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2itmegcbd.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2oymvvvyv.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2usatspjg.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2wthptbca.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2plfdcrld.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2jgnqjmji.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2bcctlxys.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2icnqaygz.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2wuwqnigl.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2mbtiawqv.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2frrpvqcm.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2pbfnqrnz.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2relwgtuq.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2smkibstc.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pjeskoqp.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hcftcovp.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kjvhfhoe.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bbcbsbqr.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2uhgsjyfh.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2hasyzwqz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2vmozjtbr.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2fpehxujp.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2xmopizuo.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2tpuejjtu.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2bsqwqayj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2ffrrdkqv.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2xaxpazsp.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2zfoirsiy.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hlvnmibk.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2ioibavdz.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2nfideqau.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2rfzoqxix.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2gpfqtznq.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2kspxsxeu.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2qbozzcbu.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2edcwzorh.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ltoypbiq.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2ajhgcfsn.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2tahikerf.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2eibxwymy.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2bbcuyasn.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2prsqhjuy.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2prnzfgzs.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2rdbyupwj.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2thvhsond.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2tzrpezzv.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2lpzvtqqu.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2mxjzdxfh.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2crqlpblk.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2csgpzdvc.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vfrmsnpc.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dcbqanjq.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2csdctqpe.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2jbjblvxq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2bnbfsnhi.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2dsltjffw.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2cjctlcre.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2caspfkdr.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2mdppfucg.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2leqcztor.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2gbrgzirf.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2txndsyxk.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2qnhhxvsz.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bawwwfig.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2dxxqjqpv.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dirwzprp.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nowcqqir.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2gzrgfbpq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2nziryyds.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2uvypmqrh.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ucyvkikb.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2nnkkrlve.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2hrpdszjg.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2phhkzckc.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2ulowpqdo.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2rhvydnwv.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2scsnpjps.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hblsuqzv.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2hhfoxcwl.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2gsjrmjub.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xkuzobpw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2jnoqxakm.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2wabxzrwn.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2lwlneshd.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2tbqbbjgr.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2ddyfntic.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2uhiftkto.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vaefflew.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2rbelunke.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hibodkub.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2kyzoxrkm.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2wnuujwtq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2rjxuikzr.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2xvbxtlwr.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2xjlqnqav.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2jixeevwt.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2wlmqloyd.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yflwbilt.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2hisyvtmh.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2epabhfkw.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2uvrmjpzo.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bvrjvdmx.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2hflxdxdi.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jyktvhho.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2twzfmonn.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2etjhlcoz.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2slfetcjg.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2sizaqpqx.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2onurdqgk.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ikvyyngv.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2fzabwmzc.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2fszejfdw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eqedcqor.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2jfuizkri.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wtgkuzuo.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pbxuldti.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2jgwdgzrc.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2pxqcuucd.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2dgxdjmol.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ndokfsin.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2kvlilbah.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2ftqyxqzl.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2xtyvhyrc.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wpmdslyl.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2klydgbkn.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2eavsilba.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2sleggbfb.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2toocsnhv.html


<!-- 参考信息 -->