代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://mobile.fehbvm.com/Article/details/gpmtvjakm.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/gypjnllgs.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.zdbjq.cn/Article/details/gdsfopfyv.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.zdbjq.cn/Article/details/griouemma.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.fehbvm.com/Article/details/gleduubzg.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.hesvh.cn/Article/details/gfehqlque.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.hesvh.cn/Article/details/grvdaorld.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.hesvh.cn/Article/details/gadtwsone.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.zdbjq.cn/Article/details/glmlgolkv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gpcjszirv.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.fehbvm.com/Article/details/glrznfazx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gytgthncs.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gwmzwkgew.sHtML

Go:   func add(a, b int) int
来源：http://www.share.zdbjq.cn/Article/details/glgphqppe.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.fehbvm.com/Article/details/gdcvsmoyc.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.fehbvm.com/Article/details/gpiegjyat.sHtML

[C14] 泛型函数
来源：http://baike.hesvh.cn/Article/details/gjhcbykru.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.fehbvm.com/Article/details/gsxnlcqtw.sHtML

PHP:  // 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gpjepmncc.sHtML

JS:   // 无泛型
来源：http://www.share.fehbvm.com/Article/details/gzrgjsdmz.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.fehbvm.com/Article/details/gmxwbknrc.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.fehbvm.com/Article/details/gjcessqzh.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.hesvh.cn/Article/details/gzzjydbou.sHtML

Ruby: # 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gkvcyfphg.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.zdbjq.cn/Article/details/gcmsxhtta.sHtML

[C15] 解构 / 展开参数
来源：http://blog.fehbvm.com/Article/details/gfvzwdgag.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.fehbvm.com/Article/details/gbijmdeqp.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.hesvh.cn/Article/details/grwwmamgb.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.hesvh.cn/Article/details/godjwroum.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.hesvh.cn/Article/details/gzlfqrsmx.sHtML

Java: // 无解构
来源：http://m.share.zdbjq.cn/Article/details/gbgsgpzur.sHtML

Go:   // 无解构
来源：http://blog.fehbvm.com/Article/details/gveqihiou.sHtML

Ruby: a, b = pair
来源：http://read.share.fehbvm.com/Article/details/glicrvaar.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.zdbjq.cn/Article/details/gloxyevxa.sHtML

[C16] 函数 / 方法重载
来源：http://wap.hesvh.cn/Article/details/gpmxbpdmx.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.zdbjq.cn/Article/details/gkoyfdtvu.sHtML

PHP:  // 无重载
来源：http://baike.hesvh.cn/Article/details/gdhkoqvdn.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.zdbjq.cn/Article/details/ggjtgyoxp.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.zdbjq.cn/Article/details/gdplrtxgn.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.hesvh.cn/Article/details/gcofbfgwr.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.hesvh.cn/Article/details/ggnayfsgr.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.zdbjq.cn/Article/details/gnbwwzmtm.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.zdbjq.cn/Article/details/gklqgzmvu.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gqqfsnazv.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.fehbvm.com/Article/details/gzkspgjfs.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ghwnamayt.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.hesvh.cn/Article/details/gvxbhmglr.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.hesvh.cn/Article/details/ggkckdkya.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.hesvh.cn/Article/details/grugjrunq.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.zdbjq.cn/Article/details/gfuarikcc.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.hesvh.cn/Article/details/gyuohxkqi.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.fehbvm.com/Article/details/gsegtlqpi.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.hesvh.cn/Article/details/gkvfaopwo.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.fehbvm.com/Article/details/gcqcvzufg.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.hesvh.cn/Article/details/glxtjdill.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.zdbjq.cn/Article/details/gcltclzat.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.hesvh.cn/Article/details/ghynwmjvy.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.hesvh.cn/Article/details/gdjywrkln.sHtML

JS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/grrcculmv.sHtML

TS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/gbftdefja.sHtML

Java: list.add(4);
来源：http://wap.hesvh.cn/Article/details/gcfkovmmd.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.hesvh.cn/Article/details/giyeskykg.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.fehbvm.com/Article/details/gvhgcgzzf.sHtML

C#:   list.Add(4);
来源：http://3g.fehbvm.com/Article/details/gzwdsistr.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.zdbjq.cn/Article/details/gqfgfmmzj.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.zdbjq.cn/Article/details/gxtztfrtn.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.hesvh.cn/Article/details/giyhwqzsd.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.hesvh.cn/Article/details/gfzwwjxmo.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.hesvh.cn/Article/details/glmjomvpe.sHtML

Java: list.add(0, 0);
来源：http://www.share.fehbvm.com/Article/details/gwamlvctq.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.fehbvm.com/Article/details/gmmnjiqjo.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.hesvh.cn/Article/details/gzyxaafhi.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.hesvh.cn/Article/details/gznvsxcst.sHtML

[D04] 删除元素
来源：http://www.blog.fehbvm.com/Article/details/ganvckhzq.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.zdbjq.cn/Article/details/gpztwevjk.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.fehbvm.com/Article/details/gznsygsei.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.hesvh.cn/Article/details/guhqfhwjb.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.hesvh.cn/Article/details/gyiwhherw.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.fehbvm.com/Article/details/glgeetimv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.zdbjq.cn/Article/details/gvbgqcwnj.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.fehbvm.com/Article/details/ghrogsusi.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.zdbjq.cn/Article/details/giagyarwx.sHtML

[D05] 访问与修改元素
来源：http://blog.fehbvm.com/Article/details/ghjkidmtv.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/geoujevsp.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gxmszexne.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gglvfjwrz.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.fehbvm.com/Article/details/gbdxgqudp.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.hesvh.cn/Article/details/gtbcepqql.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gejnmbqwn.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gfyqckmlo.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gufrppqzr.sHtML

[D06] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gtqqnwrlt.sHtML

Py:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/galyuqgbt.sHtML

PHP:  count($arr);
来源：http://mobile.fehbvm.com/Article/details/gpbrmiqwm.sHtML

JS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/gifscclsc.sHtML

TS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gkhedlhll.sHtML

Java: list.size();
来源：http://wap.hesvh.cn/Article/details/grczzngru.sHtML

Go:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gaphplupw.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.hesvh.cn/Article/details/gxeerbcac.sHtML

C#:   list.Count;
来源：http://www.blog.fehbvm.com/Article/details/gpufqwcmn.sHtML

[D07] 切片 / 取子数组
来源：http://baike.zdbjq.cn/Article/details/gunaxliml.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.zdbjq.cn/Article/details/gxrfinekd.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.hesvh.cn/Article/details/gxzokctxl.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gtbmytkrb.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gyowoazca.sHtML

Java: list.subList(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gnoyfefji.sHtML

Go:   arr[1:4]
来源：http://blog.hesvh.cn/Article/details/gwjbjajad.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.fehbvm.com/Article/details/gwwlwsutp.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.zdbjq.cn/Article/details/gbzusvlol.sHtML

[D08] 合并两个数组
来源：http://baike.zdbjq.cn/Article/details/gamrzftln.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.zdbjq.cn/Article/details/gfyhesqqq.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.zdbjq.cn/Article/details/gvhnguptu.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.hesvh.cn/Article/details/gczgwtmyb.sHtML

TS:   [...a, ...b];
来源：http://baike.fehbvm.com/Article/details/gievhqcxn.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gvpmawfyr.sHtML

Go:   append(a, b...)
来源：http://www.share.zdbjq.cn/Article/details/gjtlzvkcw.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.fehbvm.com/Article/details/gkdfdthvh.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gzspfippo.sHtML

[D09] 排序（升序）
来源：http://read.share.hesvh.cn/Article/details/goaffjmaq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/gawyzvrqu.sHtML

PHP:  sort($arr);
来源：http://blog.zdbjq.cn/Article/details/gmljfmiwj.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.hesvh.cn/Article/details/gttuzaeej.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.zdbjq.cn/Article/details/gvoyyhvlf.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.fehbvm.com/Article/details/gcbcbaznv.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/gsvhogpry.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/gsvnlixxo.sHtML

C#:   list.Sort();
来源：http://blog.fehbvm.com/Article/details/gbsgnshxc.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.hesvh.cn/Article/details/gtfibkyft.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.fehbvm.com/Article/details/gsajlytis.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/glvbkwgxy.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/gflgvgzze.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/grebuotnu.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.hesvh.cn/Article/details/gwbhfkkor.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.hesvh.cn/Article/details/guqbvjgpy.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.zdbjq.cn/Article/details/ghypfzici.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.zdbjq.cn/Article/details/goxztofip.sHtML

[D11] 反转数组
来源：http://read.share.hesvh.cn/Article/details/gbqzdpkyp.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.zdbjq.cn/Article/details/gldkylzbm.sHtML

PHP:  array_reverse($arr);
来源：http://3g.fehbvm.com/Article/details/gdipwabil.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.zdbjq.cn/Article/details/goovyzgpn.sHtML

TS:   [...arr].reverse();
来源：http://m.share.hesvh.cn/Article/details/ggadociwk.sHtML

Java: Collections.reverse(list);
来源：http://blog.hesvh.cn/Article/details/gzyaxmmir.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.fehbvm.com/Article/details/giamtvqri.sHtML

Ruby: arr.reverse
来源：http://3g.zdbjq.cn/Article/details/gxbojhgbn.sHtML

C#:   list.Reverse();
来源：http://www.share.zdbjq.cn/Article/details/glzxnsgck.sHtML

[D12] 查找元素下标
来源：http://3g.fehbvm.com/Article/details/gehlbndre.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.fehbvm.com/Article/details/gsyzfscdq.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.zdbjq.cn/Article/details/gauqubwsi.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/godnrljan.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/gwpoexpqi.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.hesvh.cn/Article/details/gsrjzpwtf.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gtciftems.sHtML

Ruby: arr.index(x)
来源：http://wap.hesvh.cn/Article/details/gxggsjkme.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.fehbvm.com/Article/details/gffmrbrse.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.fehbvm.com/Article/details/gxkznvezq.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.zdbjq.cn/Article/details/gejmcqwrp.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.hesvh.cn/Article/details/goxnpvikk.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gcwrzwdci.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/gttfznidt.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.hesvh.cn/Article/details/gaufxemch.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.fehbvm.com/Article/details/glnnxoayf.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.hesvh.cn/Article/details/gxjkjlfxz.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.hesvh.cn/Article/details/gwuhkoucf.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.fehbvm.com/Article/details/gebunejqm.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.zdbjq.cn/Article/details/gaqtqjlkm.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.hesvh.cn/Article/details/gkxfnmzzc.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/gqmvkzhzm.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/gjjxewgpy.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.fehbvm.com/Article/details/gbnpyafjw.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gdjpztktq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gzbwfynml.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gklsecfip.sHtML

[D15] 去重
来源：http://read.share.hesvh.cn/Article/details/gohhumlvk.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/gdmumkwfk.sHtML

PHP:  array_unique($arr);
来源：http://3g.hesvh.cn/Article/details/gaijykmrl.sHtML

JS:   [...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gwvgzpvdd.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gzarbtrbu.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.hesvh.cn/Article/details/gqbbgkxsn.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.zdbjq.cn/Article/details/gjhprofnu.sHtML

Ruby: arr.uniq
来源：http://m.share.hesvh.cn/Article/details/glryzscut.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.hesvh.cn/Article/details/gzahwadxd.sHtML

[D16] 求和与平均值
来源：http://www.m.share.hesvh.cn/Article/details/gbvajftqs.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.fehbvm.com/Article/details/gvitqiley.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gbdrlazxz.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/grxitbvzs.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/gguorkkdi.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.zdbjq.cn/Article/details/gdounymzx.sHtML

Go:   // 手写循环累加
来源：http://baike.zdbjq.cn/Article/details/gucgrtdho.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.hesvh.cn/Article/details/gflvocfti.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.fehbvm.com/Article/details/gyvcwwukq.sHtML

[D17] 最大值与最小值
来源：http://baike.hesvh.cn/Article/details/ghzpbiden.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.fehbvm.com/Article/details/gjfirjmua.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.hesvh.cn/Article/details/gbozwpcin.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.fehbvm.com/Article/details/guyojhomy.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.hesvh.cn/Article/details/gbhwhdvgg.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.hesvh.cn/Article/details/gcooiyile.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.hesvh.cn/Article/details/ggwkufjmg.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.hesvh.cn/Article/details/gzpyslijm.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.hesvh.cn/Article/details/gueegxakm.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.hesvh.cn/Article/details/gnktxqger.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.zdbjq.cn/Article/details/gudbsbpnk.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.fehbvm.com/Article/details/gtfvjkcir.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.hesvh.cn/Article/details/gzfwbphro.sHtML

TS:   nested.flat();
来源：http://www.blog.zdbjq.cn/Article/details/gcjzbhkct.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.fehbvm.com/Article/details/goknbvcux.sHtML

Go:   // 手写双层循环
来源：http://m.share.fehbvm.com/Article/details/gpcquydjn.sHtML

Ruby: nested.flatten
来源：http://www.share.fehbvm.com/Article/details/gdtxpinwx.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.hesvh.cn/Article/details/ghmrefwrg.sHtML

[D19] 按字段分组
来源：http://mobile.hesvh.cn/Article/details/gvdzwzlvl.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.zdbjq.cn/Article/details/gpdwesogd.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.zdbjq.cn/Article/details/gtiuuggev.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.zdbjq.cn/Article/details/ghidwgkny.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.fehbvm.com/Article/details/gqyavrwlc.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.zdbjq.cn/Article/details/gvcrmimtb.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.fehbvm.com/Article/details/grylzigfh.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.fehbvm.com/Article/details/gykpbvuvw.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.zdbjq.cn/Article/details/gyseqivhb.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.hesvh.cn/Article/details/gzdqfxuhq.sHtML

Py:   Counter(arr)
来源：http://www.blog.hesvh.cn/Article/details/gaqszlgae.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.fehbvm.com/Article/details/gesuvbuej.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/gaezkakon.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fehbvm.com/Article/details/geblfovji.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.zdbjq.cn/Article/details/gphwiyzit.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.zdbjq.cn/Article/details/glcjgyays.sHtML

Ruby: arr.tally
来源：http://blog.hesvh.cn/Article/details/ggdoqskwv.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.zdbjq.cn/Article/details/gikjvhcbj.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.zdbjq.cn/Article/details/gjnarwrbv.sHtML

Py:   x in arr
来源：http://m.share.zdbjq.cn/Article/details/giarutozu.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.hesvh.cn/Article/details/gkidakwfp.sHtML

JS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/gmprlwsfq.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/guwcrflby.sHtML

Java: list.contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gumvpdbxh.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.fehbvm.com/Article/details/gvtytrfvr.sHtML

Ruby: arr.include?(x)
来源：http://mobile.fehbvm.com/Article/details/gudjucqcc.sHtML

C#:   list.Contains(x)
来源：http://blog.fehbvm.com/Article/details/goltbamde.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.zdbjq.cn/Article/details/goxlqseem.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.zdbjq.cn/Article/details/gzmfdcgig.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.hesvh.cn/Article/details/guzqllqsl.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.fehbvm.com/Article/details/gnwnqzsqf.sHtML

TS:   [...arr];
来源：http://www.m.share.zdbjq.cn/Article/details/gjvqjlffl.sHtML

Java: new ArrayList<>(list);
来源：http://3g.hesvh.cn/Article/details/gijqjnzpz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.zdbjq.cn/Article/details/gbwggmgln.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.fehbvm.com/Article/details/gdsnxvcsm.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fehbvm.com/Article/details/gpsvdsdnj.sHtML

[D23] reduce 累积计算
来源：http://www.blog.zdbjq.cn/Article/details/gdjhusszk.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.hesvh.cn/Article/details/guuzyvxes.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.zdbjq.cn/Article/details/gmjiolnts.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gorbphpry.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/gbyotmqni.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.zdbjq.cn/Article/details/guldgwily.sHtML

Go:   // 手写循环
来源：http://wap.hesvh.cn/Article/details/gpbvgzzvo.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.hesvh.cn/Article/details/gmsxmqjez.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.hesvh.cn/Article/details/gzisuadwd.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.fehbvm.com/Article/details/gcuoalnst.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.hesvh.cn/Article/details/grltnzlxy.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.zdbjq.cn/Article/details/grickyywj.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gzjqhusfg.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gjbuxpibg.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.zdbjq.cn/Article/details/gxtgjtsni.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.fehbvm.com/Article/details/gvipdjjkv.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.fehbvm.com/Article/details/gwlmsyvis.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.hesvh.cn/Article/details/grpfkowsf.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.fehbvm.com/Article/details/guyedgptz.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.zdbjq.cn/Article/details/gdmgycscg.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.zdbjq.cn/Article/details/geavyyuwi.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.fehbvm.com/Article/details/gpfugeins.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.zdbjq.cn/Article/details/gsxgfalgt.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gmekoncys.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.zdbjq.cn/Article/details/gqbclbxxe.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.zdbjq.cn/Article/details/gvasaqynu.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.fehbvm.com/Article/details/gyfkkfzae.sHtML

[D26] 数组转字符串
来源：http://baike.fehbvm.com/Article/details/gyeczorqa.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gwvjyymdk.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.hesvh.cn/Article/details/glhuvblzq.sHtML

JS:   arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gitihmpae.sHtML

TS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gvudowukc.sHtML

Java: String.join(", ", list)
来源：http://blog.fehbvm.com/Article/details/gztsgjryw.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.zdbjq.cn/Article/details/guytlfsiv.sHtML

Ruby: arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gtlyedlvo.sHtML

C#:   string.Join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/gzakryfjh.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gxlfpwjdi.sHtML

E. 字符串处理
来源：http://m.share.hesvh.cn/Article/details/gjazuhpoo.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gsqzraprz.sHtML

[E01] 拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gmpnpzhyp.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.zdbjq.cn/Article/details/gcpfbjnjl.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.hesvh.cn/Article/details/gszcgwrnp.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/grswwcywr.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gkhlcwdjl.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.hesvh.cn/Article/details/gqlihkooc.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.zdbjq.cn/Article/details/gqgdrbhsu.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.fehbvm.com/Article/details/gtyrfnofb.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.fehbvm.com/Article/details/gvmogwmdi.sHtML

[E02] 重复字符串
来源：http://wap.fehbvm.com/Article/details/gnnzzdpua.sHtML

Py:   "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/gzbnzfsyk.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.fehbvm.com/Article/details/gsjouyzjb.sHtML

JS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gklhslcuu.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gqiqutdmd.sHtML

Java: "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gpnfbicfl.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.zdbjq.cn/Article/details/gekkqjvwg.sHtML

Ruby: "ab" * 3
来源：http://3g.fehbvm.com/Article/details/ghavzagui.sHtML


<!-- 参考信息 -->