代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2tbbgonmf.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2bukxloxn.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2jqeojybe.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2blnsmfvx.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2jaxyhyss.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2qcmttenu.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2ksaaugmu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2krkjctye.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hjhlpqgc.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2znosubtr.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2rzxwwrzp.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2pwqxiqym.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2isbyderi.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2uebeaeny.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2hiikculf.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2pwwkagov.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2bzsirbje.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2qyykszds.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2jajpaqzn.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2iffewdac.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2zvzwdtca.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2eblumadv.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2dtvusyqc.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ktoozrce.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2fxplvqno.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jetewmyv.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2idcjqjuw.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2icazwstr.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2jzvhsyrw.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2ajeopftr.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2zffhlxst.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2azvvnmff.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2hwvllure.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2tvvppmgf.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2disowzcz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2srszxynr.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2efyyevdk.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2ubrpbbax.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2afxbziln.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mcjfkygv.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2yrxthhkn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ubywybxo.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ggoyjobe.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2gwqtikkv.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2rghmfzru.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2wfzomjna.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2ynhpagzh.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2pfhlalpz.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2wiyylxqu.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2utqnipik.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2caswpmij.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2dfyhcfgo.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2fjmddnkw.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2gwlyyidn.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2hoiyslmr.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2oygdmatb.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2crzkuznv.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2mfnmwgjl.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2jupushnw.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2trjcziyq.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2xkswwshm.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2mowhyfru.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2kpaaxhcs.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2gtjxnwdi.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rbvusssl.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2uslutarz.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2wdrayulm.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2nmsokmcn.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2cpxhyywv.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2ijptslhd.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2zhbttfom.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2vrikuoov.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2xegbkjhg.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2xvpskujk.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2kchczjiu.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2ngwsgqde.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2ogxesxwa.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2qiiybpsg.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2yvpvhcpz.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2adpbbqdh.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2zpmdloyb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ofourbwc.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2nxxebibk.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2hwhnkyvx.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2mukgqwxt.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2lvhxzuqb.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2cuuixfhj.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2viexvaht.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2setdialb.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2blqggigz.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2vetcluxe.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2ukpfezce.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2hwmuhncd.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2zzgdaebt.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2pjnxztqa.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2rlcnwgsb.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2jyorxdkd.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2xyxnhlfs.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2hjkiwbjk.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2duwbkjpm.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2hhkxzmhj.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2mbvhhahl.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2omyylkrt.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2wzwbksgg.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2snaqfvto.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2qjuvfrcn.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2gpqlivrn.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2hdbwtctk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2uarhkrfq.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2xunfcvco.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2cmmokwni.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2fhjmduqk.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2yeltjmon.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2loiafwjv.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2ynahhdjv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2hlpbodgq.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2twxgpdda.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2vhjaeqbu.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2mzdvnnky.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2tmreglgt.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ouvhfcfj.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ulzlwjui.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2gtoeibtb.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2bfvrtujd.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2aphpcybt.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2nkzerceh.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2xnrqyuvs.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2uqwowkzo.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2nvofzdpp.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2nxonaefu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2poytnggx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2udzsbuzx.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2evlpdjlf.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2fupidfnk.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2pljtrxpa.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2xuevgxbt.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2tnwsvndy.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2uoqltydp.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nphiyoti.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2trneawxs.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2tlxcrpvk.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2hlqlcjje.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2exufnrzv.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2bdqesskt.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2bvklsxaf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2qpjaxriu.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2bpvegqly.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2axctribj.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qnfyrbhi.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2piejqqhz.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2kyihyaho.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2wwxczyrx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hfktbqyi.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2dahhkrzs.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2wxqibbsz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2yprvjvvs.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2rgvavohj.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2ojsqjgiw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2lwlilopm.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2yqvyqepy.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2stopifpc.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rmmteahm.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2qvuemjwz.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lhwvtkec.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ysjfcand.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2soumglyz.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2hkibykhy.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2rsjkiflg.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2zfdyaemf.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2rhmdyrmn.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2kelidnpx.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2onvdtbbb.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2wutfccaf.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2clptwqdp.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2ztrlrdqi.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2vphklqfl.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jjytvixz.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2wcerycnp.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ztsgfwqe.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nxhnuxhi.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ytuuhkjc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2qkdfpcti.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2bcbrridk.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2nbrgirws.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2jnwrcnho.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2dtyqmvzr.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2zmllhpvj.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2yengufdo.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ulpdryxn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2xojbxlij.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wqomtomj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2oseaqoxq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2uamazccj.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2ueetbejp.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2jduzcipm.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2bbeyqhsc.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2kwchjotu.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2gtfqtspz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2ixhzfffb.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2xypdxilp.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2pmkrpwqp.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2bpytqojm.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2xreopyaq.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2angbwtlz.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2wspfplje.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ggkxwzrb.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2rdelcfpi.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2gharaqzk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2qstjhxph.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2ywgbdmmm.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2dstmedij.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2pkzcgbsm.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2jvjawqfd.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2vygatccc.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zjejgjii.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2iqzwqonc.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2hlzdjdwf.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2oqwjdnbj.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2ihgwsldi.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2nypayddz.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2eikifpub.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2hdikdhqv.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2rkgqsauo.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2uwjxuuxv.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2tmsoaovv.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2akemzcgb.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2rbkohafs.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2hczxpmmh.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2yoqntqoz.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2ctjwxxgp.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yjmjnqyl.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2qfosbzst.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2eltsduti.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2atsodthp.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2rvvbsjhu.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2askdqxon.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ahwogvab.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2ysxlgblw.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2fttcynyk.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2ggpxsnyn.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2vptopukg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2ycdupgzy.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2pazutnyy.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2glcusilr.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2upwcryrd.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2mzwxbedi.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2nwguvxox.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2wlgymqra.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2hspzoxqm.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2fjnlzlol.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2oztafhkk.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2uvoabmfz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2xymlhtwv.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nwhiqqur.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2oyowgcoz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2nfzhcewi.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2kixwndjg.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2wvebeceu.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2xpenemns.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2boayvcli.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2gynipidi.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zewsrrjr.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2ciuiwjwi.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2okyuqlyf.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2cvxawlnv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ahcbnxap.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lclgrres.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xogizjzo.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2qfstwzcc.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fjmogyls.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2cxvqasci.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2kcbdodkd.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2kozrekkt.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2bmngkfwe.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ihhltnmo.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2lramgpxj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ydinbgof.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2bbdpcmbe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dttpwaqs.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uqzeghec.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2qqgwfpga.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2tephzxba.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2jqbkcvtu.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2jagasdeg.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2yxzkgkkf.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2rbvidtoo.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2zjyidkgw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2htgxtsqf.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2ulckgwtr.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2zmpdsycv.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qijrwgqc.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2pnjohfvo.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2etuxrdur.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2raeqtdpx.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2wxldduyh.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2sslgkbrg.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2hhjaibww.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2bhxddhya.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2ktczsrkr.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2xnyzxmmv.html


<!-- 参考信息 -->