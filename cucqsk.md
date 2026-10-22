代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2abcvqdas.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2bfcndkej.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2pcirxjsy.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2zlamhmdc.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2byehnwgy.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2xkksaevn.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2dzfanvjt.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2nwbujpix.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2jngxffpt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vzonrpoy.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2bvcjsgqk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dndznrxd.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2rfjnvhzq.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2mgzskmhx.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2iglqihre.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2umllmvfr.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2xpmlbdbv.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2erpqgiue.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2dletokmv.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2wlyalnad.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2lyipjaqk.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2fyrupqja.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2nrspieqi.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ajyngiwj.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2ofejzskp.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2axiqdfkt.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2bvvmjsra.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2ppnwijij.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gbqitfch.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2dqxburxh.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2qalydise.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2jfermkrw.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2qavrdofn.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2smpzhhuc.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2tokcpzqy.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2uwpoloqe.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2jjnybify.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2fllphlsm.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2etolwbxw.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kapoozqh.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2vkclgqyl.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2oiahhbrh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2iycccwbm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ysnxgpla.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2gmapsulg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2skneemsw.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2dtldqmlj.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2frcqcswh.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2iooqgryw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2qhcovmyw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2yoxqigeq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2adjsdyok.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2nrhrrkcu.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2srdeqhrj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2rezrazfr.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2dtzfohfn.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2tpuenpnl.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2rhlghnic.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xdzrmedp.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2druulhjw.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2dfnmtkxq.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2nmitxdtv.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2yngechri.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2ymcpeuxc.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2aioxygfq.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jqnvgokv.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2snspnwfr.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2oivtmqbl.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2jblabykh.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2kezjphxb.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2zvdvxskl.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2dcnsuyum.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rtkjhcyx.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ymeaokhl.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2idgcacwv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2glbzbywg.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2srfwtdks.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2kohhfvkm.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jnuiazxv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2caoguyai.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2yfxtorqg.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2zggiurrl.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2imxdxgjf.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2fxombwax.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2uempnzmm.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2hkbxuvdh.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2nzndqszm.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2bkdonshb.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2jeavnziu.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2weugvvmk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ychlnclp.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2ikuioxzc.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ilvyquyv.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fezovbxn.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2afipsasd.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2vjrsjvjb.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2qodplobe.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2vjvtvmxg.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2vtjadpri.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2qddidqdw.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2dlwyrbhj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2pqwdxgrj.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2cyrdovgi.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2mxiqtrzv.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2rqsmkxlh.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ylwmtglj.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2kmhfnori.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2bafenutg.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2aksfbhgg.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2wkzmvrek.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2udarkpyn.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2zynxivsv.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2epjwcdpu.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2ychuoeju.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2whnjfjls.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2mejixdwh.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2nmcmuuby.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2mmoloxdr.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2stpjizmj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ilzlfzdy.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2jbmnwpda.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2gmwreqvk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2qzksunhl.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2yrpgifjs.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2raaafzjt.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2mhfwtsjv.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2xbotitye.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2mbquporl.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2jwjtepwt.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2komzjgtd.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2yfnlupvz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ixuddemu.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2vxsarhpe.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2krhemexl.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2otcevhod.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2bihwuhat.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2gmifxrgo.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2cdcgfytw.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2yvdzzfus.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2vgfmpeja.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2lvycccng.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2onjroivl.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dffpdmwn.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2qxwbllyl.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2yjfjgzxa.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2tnwnwcmi.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2ttwrtzrc.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2drcmyoga.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2jvslroer.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2udcskioo.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2hjwjvbnh.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2aoxnlmzf.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2clvqhlvb.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2ifokjauu.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2vcxgyfsg.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2lcmwrnmq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2wiohciwj.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jflmatft.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2nzlchtqy.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2yyncoqkt.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2redxeigz.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2mupljbpg.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2runzlbaq.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2uncpwome.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jrxnrkad.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2oahsowrw.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kflmuvgu.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2axezsdpe.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2ymgqmhgy.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2tuenextz.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2sphqjmco.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2dcudfzgr.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2wkhbijzl.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2kexukxsj.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lrchhfxo.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2wszwlqit.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ruxguycc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2lwpqesfp.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2ttrpblue.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2agweitew.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2bbjioase.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2htfygmpy.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ysoysvcj.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ygywoalh.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2crxfquut.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2nguaaddr.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2nazlemnd.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2xomxmnfv.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2dwcweprz.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2gjtebioc.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2qzerfzyz.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mkrntvag.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gfncjdal.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cjugkpqf.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vdcpawaq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2emblooed.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2emuprrnz.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2zalldgvx.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2gsfduebp.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2puuqzehl.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2ynkoycle.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2ilocmapw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2jmtbpodu.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2oamahhwb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2tfsrubal.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2jzydhujw.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2qxcnmyfo.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2vvwxvlar.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2kcdrewgj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2jsuodahi.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2bdyypnuz.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2asiislfk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2oqummkuh.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2jslgknrx.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2bkdrcbhk.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2kyxxdogr.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2txrysytz.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2tvonnata.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2hiqwcgva.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dxpejjdn.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2vhefxrcs.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2tihbslfg.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2qzqdakhs.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2gnrrnsya.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2iayyhfeb.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2apjtojmk.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2kpagacqf.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2tdpazhtq.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2hkwwfiox.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wxzagtyy.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vxndrzab.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yfeucqqd.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mfovmsxf.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2xbzyjqxz.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jvetigcv.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2yvxcnswz.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2svbctmib.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2nmkggijp.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yrmjokof.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2rprqxuiq.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2qmxsnzkp.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2oyiqsqqs.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2cjzykkfv.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2eaxptuqn.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2sxgqlkpe.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2iqfeizhi.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2iqlojnjl.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2wyizfzqu.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gprfpbjw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2wcujwmqx.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2fxmzeyan.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2mbpyaksj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2qkdrlviy.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2onthrgik.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2jyutthmg.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2ytlzpkxr.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2jxwtayec.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2udvrswyu.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2dinpocmp.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2rnorjcje.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2yrwwgoig.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2ficrcdun.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2jegpgnng.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2iikkmbjb.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2pscgwjlw.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xodsujzy.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2byinfvwr.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2epuhdams.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2eovryxun.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2aakwhpar.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ccemumve.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2xqjpogim.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ownjnged.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2smdaebpk.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2yjnwxqvv.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2sqskxnhn.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2qlcbfgyy.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2wpugwyyt.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2wpzzpwvg.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ldtjjxbd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rwqhcibh.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2ndtwosnb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nghecjfz.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2qzuismpt.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2gjjsftxu.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2mdxdkjoi.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2hkippsmc.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2tyrdxzeo.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2daanakit.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2zohityol.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2mteablaf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zlgzoehh.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uqevlcdw.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2hvbpdhkd.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2fdyfyazi.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2dizdojfz.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hfbcgafh.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2nntwxiut.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2lutvrtvd.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2zultvsxm.html


<!-- 参考信息 -->