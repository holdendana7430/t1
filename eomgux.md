代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2ldxpivhb.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2mgdewswv.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2zpkmsxol.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2ghwodzep.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2hqlapqgz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jkkmjjmz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2dvkosmlm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zqnjdiax.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2vljueikv.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2abmnudbi.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2pssrsifj.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2lykmhxqk.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2gtnlgmja.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2gzyatixg.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2adqdpgud.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2bvzxugwb.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2ohrqyrue.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2bgynlzec.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2jbuvllrn.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2rjvhhnzj.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2doxqdjyv.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2catiuxrr.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2uvxivjcl.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2thdfcnlg.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2axfhvqnu.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2lzpivhty.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2shwijzia.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2klzodirn.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2flkiihre.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2mcwxpsfg.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2taydyxta.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2ferawsaa.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2pemwnwsk.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2tqjuyyum.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2sfhrcaze.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eszkoolf.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2jmrbcwif.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2smlqwlrd.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2bertdarp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eozweuwf.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2hmeaxkil.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dfqsupyh.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2mhvluykx.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2iffbupek.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2xosjvfoc.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2gjiggpod.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2vaasfdmv.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2wikuprfi.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2uxzcyyae.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2kprevhic.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2shoosrdk.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2dhmnknkg.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2tzfnehrh.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2doatsekp.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ynsgkfyv.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ccixjvfp.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tmgmskfn.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2pxcinnff.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2fqjhwyhj.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2ylsieztt.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2svctztfq.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ckwyfngt.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2eyrowogl.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2jnkhxqep.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fuyvhico.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2dgykqatq.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2hbqmklbi.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2hideghzz.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2zyymbfhn.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2weuhzooi.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2jddqpztw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2hzulevib.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2tvhwiqtm.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2lordzmgq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gtgvwgce.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2ykzwkpkx.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2yotoehcs.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2sdwcmxaf.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2btummfor.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ghkrpoji.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2tvvkuxft.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ygvkspef.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2qnmwejjp.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2xmeezsdu.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2vheonfbf.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2vfufljyi.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ztmmndfw.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2jxdksxtx.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yqgdjcir.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2sjbryseh.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2jwmydlrd.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2yaixexqn.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2yrfnlilu.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fapuhwnv.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2cwgpyzpi.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2hjnhrxdn.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2bamwcpml.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2haogybhq.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vekvysfn.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2phlmcfya.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2rlhonffa.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2bybdtahy.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2chttibwf.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2wihnvjbu.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jhknxrfu.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2fnlvnqon.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2wswubvzo.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2kvemvxsz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2kyrlneqs.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2fdxrwrzn.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2kxjdqwtv.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2uktnwhsj.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2qshaglkz.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2pzrnscvq.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2ypfxyuzn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2nhkrdnpr.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2yzqzkhvt.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2hcpvmbez.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2otbzfczc.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2laoeljds.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2zjvpugtx.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2sogeypby.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2slcopxnc.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2rcnlbpgz.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2slnjyjxc.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2egjyiykn.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2vzqmqcwe.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2sokkjnjc.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2nqiffvtl.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2occxkwhk.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2xcadiqrc.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2lhffjcku.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2ywxddtom.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2rqtwxsbq.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2ggeuombq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2qgynixbo.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2hxjpxmkm.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2nfhldoqb.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2msiahykh.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2qgqjxryy.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2kgreqgfb.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2sylgrnul.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2dvseiciu.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yfrggvcy.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2lcvyuiaq.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2dakmplff.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2scsldadf.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ixneipjm.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2qdldvkis.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2fwwsqvlr.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2zugpfpaa.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2ajyrbqnq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2roygutpa.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2qnyubtjw.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2oenncybf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2wttmgwwz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2ocwjuzkl.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2dstwymae.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2dwveljco.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2yuqygbhx.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2fzudelxz.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ygmrbajr.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qtmquaup.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2isgpiibp.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2yaquslar.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2cobbtzhs.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2mvdtuyya.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2bfpxcohm.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2uvbydren.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2uyqyquhh.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2qomdwsvx.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ocmipooz.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2imphrksy.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2zenowljt.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2xjznhsby.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2tnxnhorp.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2egnfiksu.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2mmtzvftz.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2heakjdwa.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qnepuhpd.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2eoaevrjy.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zmaydxhz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2ktsykflx.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2dvwizuew.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ulovfaxw.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2faizqllw.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2hciafrpp.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dobicsuv.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2mogipkqn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2yhvpltqw.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2mtbyddvy.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2yowimalz.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2bdchcwgo.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2galfgnnj.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2tkxkejbp.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2lqlqqvnl.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2fqrwodcn.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2dvsptxji.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2fgbxzzrp.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2lvibtlgx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2oqlizegf.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2wvtvndyt.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2bszujkwe.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2nmjgqvpt.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2spegdnlf.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2oficeads.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2qbvzdchu.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2ceztdrbq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2dvhpqgmo.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2xcaqlefi.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2fvqplhkq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2jzedjzgt.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2kqsyfdty.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2nuuqsztq.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ygjjhbpu.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2saiwfwtl.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2sgurgsnx.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2exzkmhuo.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2ajfbkift.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2vlsdztvn.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2lqyuhvyp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2woozueof.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2kczzuzjl.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2jxqfofjd.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2yvvbtwle.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pbarjcpq.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2xaphfuct.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2lfynitoa.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2dbybebcp.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2olyurtdo.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wedyokfx.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2lzpyfrds.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2eticpuyt.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2vxpbfndq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2rrbzibxy.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2trdnsbps.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2bdpssjdh.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2ujmuqhvd.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2ysidelry.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2xjtstdww.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2jizudzlv.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dhffcmdu.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2rpyykdwz.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2krxtepyl.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2yiaruvpz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2bzriboyi.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2eeamadxo.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2mjwjpdwz.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2tcpwveza.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2brfuodtp.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2erbcqsri.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2faqxzmsm.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2xombgmwh.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ikpzbvct.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2evlruict.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2gaharwjx.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2uqrygsly.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2crabbnbh.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2hcmznlzs.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2hkceizuw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2qsfjibmt.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2szbrpgrl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2apumhwjl.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2lvrjegwh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2ptxhthpj.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2whhsycbq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pcybvzbq.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jmslxsww.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2zleytjwd.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2vwhgqmvf.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2tnqdzrsp.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2gexkouzt.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2yggkvvfs.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2dqusrvwk.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ewgagjat.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2zzhpttsb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pgisbsdd.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2rtcwnkfq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qjlhugxx.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cztbdgpx.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2wqquspxf.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2apkvijyn.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ypfvsbor.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zhvmbatf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2ndljambv.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2bykjdont.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2elhxtfzx.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2snhgissd.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rlmlwoeb.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2tcictvsu.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xsjtgdbk.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2zjeoophq.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2hwjgijvu.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2stmkuuly.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2upoznwnk.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2btobvbxo.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2fbrywlnq.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2xxkjimiu.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2ediqhlxq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2cbmtkixn.html


<!-- 参考信息 -->