代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3wgyzyhwx.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3ydukomri.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3fmwzrvhs.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3chyfldxr.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3rguffjfr.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3mhrkwxvl.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3ntviovub.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3kulccrcq.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3jxkpwkwg.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3mqsnuzbt.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3dbpuxatr.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3kysidodd.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3uppmhmib.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3grqdktgm.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3btkvkulw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xapuhznt.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ekdhwdxj.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3adsqpufy.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3qjdjppaj.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3eebrersy.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3uldbdwqo.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3hjjpxeas.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3huwbivxh.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3vsncqcur.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3noendcrz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3zmjtejqw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3qdgbxbuh.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3rzjkcgzf.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3hrmatmsh.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3oaacelds.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3gqrjvvbv.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3zquzceut.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3isreuhao.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3dlqdajpq.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3ddcjifoc.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3orqjrxhy.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3tsstzvrs.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3onwowiex.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3ssjvqikn.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3smpbktiw.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3qujlzjci.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3edopuaeo.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3nwrthlxh.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3sbfkvmri.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3njissecn.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3wjkyayoi.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rkpjyikm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iaprfjck.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3ehkuwext.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hdmagaxn.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3gvaghtpo.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3hxbnyhur.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3qrygpliu.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3wrmjdmsg.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3mwltnsxx.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3twenadmi.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3cdhbjryn.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3jgzcqnzy.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3nhdglnve.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3tycckaox.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3bnaaprqe.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3ozsfobpe.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3zanyheyo.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3uwwhdtta.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3fioieife.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3qjjebbtx.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3qgbzdenr.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3albunwju.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3vbpktesa.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3omsvxdnm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3bkmjteqc.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3feixbxpb.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3sjespjxf.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3orrehdqt.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3rllpvxqz.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3wvjowhzs.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3qwniomjj.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3xormjmfj.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3zvfexjec.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3htbsmfct.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3paplutom.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3drazzowb.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3mxqrkjoa.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3skpzwatp.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3rvyswalp.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3llrsttbc.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3vywphdag.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3whevafiy.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3fjwidajj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3mkhritjx.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3nzkkgfnc.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3zjzdxswi.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3sroqbaim.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3fwutxpvp.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ragvufkc.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3gigsgjnv.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3bwotudqt.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3ubrrqagc.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3teujxbse.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3wtefeosr.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3dpzcdcwh.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3cmbelbuy.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3tywryfiz.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3vgorluji.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3enqpgbdo.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3bkudkqjk.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3tadxccrc.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3hojuaegq.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ghiscmnv.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3puhyysif.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3ceyoicon.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3vzbdsfch.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3viaugojy.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3iepltmqp.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ucijgmwt.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3saygofvh.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3ibexupbz.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3bykzpvek.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3pawcjbaa.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3uankirzh.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3ngxswyle.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3aiefcjra.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3ilgwdwfn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3pmoktiof.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3flkdunci.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3pfpvathk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3ieufkktx.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3dypnehep.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ghyiqiwb.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ccqhnotm.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3ukdtfkwr.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3yztlhqqx.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3zhdwdsnf.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3vsovwekf.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3rlqwhnvs.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3lbbmtbmx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3knpcnusm.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3riwalijb.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3mwpnjhkc.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3ipfbwyac.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3xrjkitwx.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3offjelng.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3otyqfudq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3ombkmuye.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3fppugtfc.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3vmsosxsm.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vwijbvtc.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3amziekid.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3cvaypxed.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3cqrrtnzg.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3gibucvox.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3tiahijlj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ssbfzbkt.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3eyqiudiz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3lhuqthpg.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hvmwlrjl.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3imwqbplf.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3imwqpmit.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3kgudzggt.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3grfzhamc.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3tpbgujaz.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3csfcqege.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3tpjxlkzq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dhklwjzt.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3rryvzcii.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3uwmrxria.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3oigxsgbn.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3zhclgxfk.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3jcahlaii.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3nfcrjihd.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3zjkgzfub.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3piihvncc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nlkgnqiy.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3aynzdtuo.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3uvucshee.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3wcwrhzdo.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3iphweiob.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3wweizpas.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3hexuzdoq.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3kbkyaiyy.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3zlyxdokf.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3aoviqdcz.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3eifizntz.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3mxwwhlsu.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3sweseoiu.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3yyqvlqqy.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3sqtwedak.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3qkyipmvm.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3odgltnzh.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3airfmdsd.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3zepcorlm.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3hvtpfsci.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3tllriqxw.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3pafympzm.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3lelgtibx.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3mtjflshj.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3efjzmuqn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3zfxudyqb.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3trpolujs.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3mrxfgncz.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rlxqvwnh.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3qnzppcai.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3jljixjyd.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3txbjxuhg.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3smddjuns.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3mxfovtgh.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3pzuadyoj.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3gbvyiioq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3zgmpfapk.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3wipfggvf.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3tqqdbpcr.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3bsqmjlfv.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3scpxwqhd.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3ymozezyq.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3lvvbopdx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3lfnttlbo.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3qjohddnw.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3rtpohefv.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3ggtqtdqt.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3opktweuj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3heatceut.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3daqtdbfk.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3fbebsjwi.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3bmmefzys.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3lthxwhea.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3xpajyver.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3ezeauqlo.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3inxjrmzm.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3dflrizzu.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3vyuwpsne.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3nyqebycl.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3apkiyqyw.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3icqqowoj.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3eiwzwqir.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3nnlahwfs.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3sppugsra.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3nrsjjdgg.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pbavjies.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3evcpatex.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3ooxlnhfb.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lvxcvwnr.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3eyifkdri.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fblqfskl.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3xzzmizio.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3bjmtmqal.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3kdcpsogq.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3rshshllb.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3dhgxeeye.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3iviiyyey.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3leoggdxz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3kspmqjzw.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3oyxshzlf.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dhkaambg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3llrnegjg.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3cvdpxheb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3qnfbxkzs.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3hviljkuq.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3huwsnbey.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3xxprsalx.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3byraizyd.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3sorezioz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3fauhddfh.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3dozfufhm.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3iprswzpd.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3agpeiiyy.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3nmotnijc.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3mjkgwpyb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3wudvdrnz.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3wxuarrnf.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3odrdnxak.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3wxpjtcxj.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3cderycfe.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3onbahrta.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wunppgnl.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3cxkliqxj.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3dlvpvicv.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3fybodwjl.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3ikqgpxzp.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3iyamnqsz.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3vzlrltyd.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3bbtddusv.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3emgjluuy.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3dyaglsvz.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3worrsedp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bhfdnnww.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3gowgbzza.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oqkrhsfg.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lxupapmk.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3wbdfxerl.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3drtlvaok.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3xksitjbo.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3efswzrta.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3ptuvyupx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3arvqgtyt.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3qjljclja.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3uylciqxj.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3lscnodbq.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3utrerryu.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3plllhitv.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zqgyqeoe.html


<!-- 参考信息 -->