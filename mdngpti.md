代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwlbjkdbf.sHtML

C#:   using System.Text;
来源：http://3g.fanxiaobao.xyz/Article/details/gworqxzid.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.fanxiaobao.xyz/Article/details/ghlfkxiuc.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.fanxiaobao.xyz/Article/details/gcvfglqkp.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.fanxiaobao.xyz/Article/details/gsxzjekfn.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.fanxiaobao.xyz/Article/details/gercuuiml.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.fanxiaobao.xyz/Article/details/gekznqsrn.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.fanxiaobao.xyz/Article/details/girfqkvmj.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glnhqqxbc.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.fanxiaobao.xyz/Article/details/grqaeqgwl.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofnbgvwv.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gacquvbdl.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.fanxiaobao.xyz/Article/details/gtzvzcirz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdgtdaep.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.fanxiaobao.xyz/Article/details/gwuokhqix.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geayyumlc.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gtcotnbne.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwrguciq.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.fanxiaobao.xyz/Article/details/gytwfmrlp.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxbpyikc.sHtML

[C14] 泛型函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjfebisg.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.fanxiaobao.xyz/Article/details/geqqymnvv.sHtML

PHP:  // 无泛型
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmiovoam.sHtML

JS:   // 无泛型
来源：http://read.share.fanxiaobao.xyz/Article/details/ggobqjxyq.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwrorqwxz.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjusaukt.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpujxoyot.sHtML

Ruby: # 无泛型
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqsvlote.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.fanxiaobao.xyz/Article/details/gkzgmfjhc.sHtML

[C15] 解构 / 展开参数
来源：http://blog.fanxiaobao.xyz/Article/details/gcivnkrzf.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjompnvvs.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fanxiaobao.xyz/Article/details/gphsdugdc.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gtpoqrsqz.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/giuxubsto.sHtML

Java: // 无解构
来源：http://m.share.fanxiaobao.xyz/Article/details/gokmjebzm.sHtML

Go:   // 无解构
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guyuufajz.sHtML

Ruby: a, b = pair
来源：http://read.share.fanxiaobao.xyz/Article/details/gaakoevsn.sHtML

C#:   var (a, b) = pair;
来源：http://wap.fanxiaobao.xyz/Article/details/gajrstkxq.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqmvigdr.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.fanxiaobao.xyz/Article/details/guyrulutm.sHtML

PHP:  // 无重载
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbsrddyq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.fanxiaobao.xyz/Article/details/gypvbkgsc.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.fanxiaobao.xyz/Article/details/gwtciawxd.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gvuwjmrlo.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.fanxiaobao.xyz/Article/details/gyjwkdlaa.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.fanxiaobao.xyz/Article/details/gqiomutpy.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gxeleyuxr.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gokrxcmre.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.fanxiaobao.xyz/Article/details/gafeutdhz.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfogkjsmp.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.fanxiaobao.xyz/Article/details/guvpjaisa.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.fanxiaobao.xyz/Article/details/ghnrrdkzo.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.fanxiaobao.xyz/Article/details/glrayaprl.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggosdnjbf.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyljhazyx.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwagklex.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxdkxwra.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.fanxiaobao.xyz/Article/details/gccppvxab.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.fanxiaobao.xyz/Article/details/gowjmccbi.sHtML

[D02] 追加元素到末尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gctspuabl.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.fanxiaobao.xyz/Article/details/glueqenyw.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gulfygbei.sHtML

JS:   arr.push(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gldinvhxy.sHtML

TS:   arr.push(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxnnoyyoq.sHtML

Java: list.add(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gllvsgyuc.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjpynyoqr.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.fanxiaobao.xyz/Article/details/gfjajzmuq.sHtML

C#:   list.Add(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gncndfjfm.sHtML

[D03] 在指定位置插入元素
来源：http://wap.fanxiaobao.xyz/Article/details/gfkckmako.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.fanxiaobao.xyz/Article/details/gorgfpmdi.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.fanxiaobao.xyz/Article/details/gfxgwktqa.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzhprxjh.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfpyyrwxe.sHtML

Java: list.add(0, 0);
来源：http://3g.fanxiaobao.xyz/Article/details/gugoqhyhm.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjnctkzmq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkabbfcpd.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqdxhqpab.sHtML

[D04] 删除元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gubuuqksk.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.fanxiaobao.xyz/Article/details/gortgkwre.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvqdqldb.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.fanxiaobao.xyz/Article/details/glyhlblbn.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqdmbovgl.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.fanxiaobao.xyz/Article/details/girximwia.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbzwkbcg.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.fanxiaobao.xyz/Article/details/gspzyrprj.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzimqbphx.sHtML

[D05] 访问与修改元素
来源：http://wap.fanxiaobao.xyz/Article/details/gsrkcoxvn.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmkriqey.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gegnsvbjw.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.fanxiaobao.xyz/Article/details/gzlhdtkin.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.fanxiaobao.xyz/Article/details/gmihsqnsd.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvprovqc.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.fanxiaobao.xyz/Article/details/gdjwqtzpp.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fanxiaobao.xyz/Article/details/gghjzsxel.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.fanxiaobao.xyz/Article/details/gngivzljx.sHtML

[D06] 数组长度
来源：http://3g.fanxiaobao.xyz/Article/details/glvkpqiqu.sHtML

Py:   len(arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gfiejtabw.sHtML

PHP:  count($arr);
来源：http://3g.fanxiaobao.xyz/Article/details/gpgiqmtmg.sHtML

JS:   arr.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwvanlsy.sHtML

TS:   arr.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavkipvgw.sHtML

Java: list.size();
来源：http://wap.fanxiaobao.xyz/Article/details/gpcuerdzr.sHtML

Go:   len(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gtgywxriq.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.fanxiaobao.xyz/Article/details/gktdqqldh.sHtML

C#:   list.Count;
来源：http://3g.fanxiaobao.xyz/Article/details/gbxnebvbn.sHtML

[D07] 切片 / 取子数组
来源：http://3g.fanxiaobao.xyz/Article/details/grlyzykmi.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.fanxiaobao.xyz/Article/details/gaddtefuc.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqmqrhqvd.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghteqqzzt.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrfybtds.sHtML

Java: list.subList(1, 4);
来源：http://baike.fanxiaobao.xyz/Article/details/gtxcidirz.sHtML

Go:   arr[1:4]
来源：http://blog.fanxiaobao.xyz/Article/details/gbtyfrzsi.sHtML

Ruby: arr[1, 3]
来源：http://blog.fanxiaobao.xyz/Article/details/gttatgtgy.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gorfsabms.sHtML

[D08] 合并两个数组
来源：http://baike.fanxiaobao.xyz/Article/details/gnmuuzxoc.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdsfmjofs.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndslfyui.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbyegtigv.sHtML

TS:   [...a, ...b];
来源：http://www.blog.fanxiaobao.xyz/Article/details/goipevmqk.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.fanxiaobao.xyz/Article/details/gsnahqpmb.sHtML

Go:   append(a, b...)
来源：http://wap.fanxiaobao.xyz/Article/details/gqstqphtp.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.fanxiaobao.xyz/Article/details/grhnarpga.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.fanxiaobao.xyz/Article/details/gnnaovztd.sHtML

[D09] 排序（升序）
来源：http://mobile.fanxiaobao.xyz/Article/details/gykdptecy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fanxiaobao.xyz/Article/details/gvatvrgkp.sHtML

PHP:  sort($arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpexhssjl.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdurmutf.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.fanxiaobao.xyz/Article/details/geigakzcz.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.fanxiaobao.xyz/Article/details/gowgabjsq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjenwawr.sHtML

Ruby: arr.sort
来源：http://blog.fanxiaobao.xyz/Article/details/gkedcwogy.sHtML

C#:   list.Sort();
来源：http://mobile.fanxiaobao.xyz/Article/details/gobvjhmtj.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbarjewr.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.fanxiaobao.xyz/Article/details/gmfjtnwmw.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfflgeoef.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fanxiaobao.xyz/Article/details/gbpvwivvm.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzkswhbts.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.fanxiaobao.xyz/Article/details/gugwpqfez.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.fanxiaobao.xyz/Article/details/ghtrowmkd.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.fanxiaobao.xyz/Article/details/gcqrdmqfc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.fanxiaobao.xyz/Article/details/gfhlqheeo.sHtML

[D11] 反转数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gobjzbpex.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmbbhrvk.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvydgiqly.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.fanxiaobao.xyz/Article/details/gylmgstvn.sHtML

TS:   [...arr].reverse();
来源：http://m.share.fanxiaobao.xyz/Article/details/grfsqsjzb.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtdilkakk.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gwfqczkhe.sHtML

Ruby: arr.reverse
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmexwijw.sHtML

C#:   list.Reverse();
来源：http://3g.fanxiaobao.xyz/Article/details/gxbbnjdyl.sHtML

[D12] 查找元素下标
来源：http://www.share.fanxiaobao.xyz/Article/details/gpuowxqnu.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.fanxiaobao.xyz/Article/details/gimcuxmlr.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gaoixilnd.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gviqunktt.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fanxiaobao.xyz/Article/details/gzdfqqhph.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.fanxiaobao.xyz/Article/details/gdyvqrmgy.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpnrzvrpg.sHtML

Ruby: arr.index(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gywlvczpd.sHtML

C#:   list.IndexOf(x);
来源：http://blog.fanxiaobao.xyz/Article/details/gjxpdllmj.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.fanxiaobao.xyz/Article/details/gizgrtesp.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.fanxiaobao.xyz/Article/details/glppkibqo.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gbdxanque.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggrxicdah.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.fanxiaobao.xyz/Article/details/gtnxpnnav.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.fanxiaobao.xyz/Article/details/gkqvkwlvw.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.fanxiaobao.xyz/Article/details/gedjpdxon.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.fanxiaobao.xyz/Article/details/gsmplyitt.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.fanxiaobao.xyz/Article/details/gcohxompm.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.fanxiaobao.xyz/Article/details/gcuwhwnfc.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwpprsgc.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzgwndvbl.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.fanxiaobao.xyz/Article/details/ggfdisrxi.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjzemgcho.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.fanxiaobao.xyz/Article/details/gorspepoh.sHtML

Go:   // 手写循环
来源：http://m.share.fanxiaobao.xyz/Article/details/grsmbbkem.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/gkdnnqpsw.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.fanxiaobao.xyz/Article/details/gjovelrfc.sHtML

[D15] 去重
来源：http://m.share.fanxiaobao.xyz/Article/details/gnenfrhmb.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fanxiaobao.xyz/Article/details/grwsalzvi.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gphiwknil.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.fanxiaobao.xyz/Article/details/gmcuhbppf.sHtML

TS:   [...new Set(arr)]
来源：http://wap.fanxiaobao.xyz/Article/details/grrkedaro.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.fanxiaobao.xyz/Article/details/grtheasnf.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.fanxiaobao.xyz/Article/details/grzukcnzc.sHtML

Ruby: arr.uniq
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvcjpelv.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjzlxtij.sHtML

[D16] 求和与平均值
来源：http://wap.fanxiaobao.xyz/Article/details/gydnvyhvg.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggrunlkhk.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.fanxiaobao.xyz/Article/details/gcyawmeif.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fanxiaobao.xyz/Article/details/gyqvzdxku.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzycfdlaw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geinknysu.sHtML

Go:   // 手写循环累加
来源：http://blog.fanxiaobao.xyz/Article/details/gukyrcrzz.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.fanxiaobao.xyz/Article/details/glsmunbki.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grljmhyjs.sHtML

[D17] 最大值与最小值
来源：http://blog.fanxiaobao.xyz/Article/details/gqyerdwif.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpglouhid.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gruglvmrv.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbkezyitm.sHtML

TS:   Math.max(...arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdeuufogn.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.fanxiaobao.xyz/Article/details/gzaubobmj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcfvdwmne.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfqazklce.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.fanxiaobao.xyz/Article/details/gbryvtzmk.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.fanxiaobao.xyz/Article/details/grgfwhkfc.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqudvfhwx.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.fanxiaobao.xyz/Article/details/geotqyfxe.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geocieius.sHtML

TS:   nested.flat();
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvnoydyf.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.fanxiaobao.xyz/Article/details/gpslrgdqf.sHtML

Go:   // 手写双层循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxwxwuev.sHtML

Ruby: nested.flatten
来源：http://www.blog.fanxiaobao.xyz/Article/details/gootcpxaq.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.fanxiaobao.xyz/Article/details/gmacaiozr.sHtML

[D19] 按字段分组
来源：http://www.share.fanxiaobao.xyz/Article/details/gujfsxtnu.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.fanxiaobao.xyz/Article/details/grqykckki.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.fanxiaobao.xyz/Article/details/gawmiwcfv.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.fanxiaobao.xyz/Article/details/gqdegxgjv.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.fanxiaobao.xyz/Article/details/gdbtkthkh.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzpbjgfff.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.fanxiaobao.xyz/Article/details/gchiqeybi.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.fanxiaobao.xyz/Article/details/gvcxccddz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.fanxiaobao.xyz/Article/details/ggllbgikk.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpzibtxua.sHtML

Py:   Counter(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gusspezre.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gyrmexnrz.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fanxiaobao.xyz/Article/details/gmrkmvuqq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbdxgjzet.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnvemlbaq.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxtlfxhu.sHtML

Ruby: arr.tally
来源：http://baike.fanxiaobao.xyz/Article/details/ggjxumtln.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.fanxiaobao.xyz/Article/details/gfzosurmk.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gasfcedjc.sHtML

Py:   x in arr
来源：http://read.share.fanxiaobao.xyz/Article/details/gjpwkqlnz.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkdokkmkk.sHtML

JS:   arr.includes(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdyvtwzm.sHtML

TS:   arr.includes(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gdknaabtj.sHtML

Java: list.contains(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gqyrfowse.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.fanxiaobao.xyz/Article/details/guibcnsda.sHtML

Ruby: arr.include?(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvcpgbju.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfctjeveh.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzsbfzir.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gklbhyjha.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.fanxiaobao.xyz/Article/details/gjiznmqkd.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/glrihbmbe.sHtML

TS:   [...arr];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrgfojwc.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmnafeicw.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.fanxiaobao.xyz/Article/details/gndtsnkrb.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.fanxiaobao.xyz/Article/details/guitjwyge.sHtML

C#:   new List<int>(list);
来源：http://blog.fanxiaobao.xyz/Article/details/gyzvdcyte.sHtML

[D23] reduce 累积计算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdafnusyd.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkghizckb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/geehbvwlx.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fanxiaobao.xyz/Article/details/gmlntjqps.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjpokcepz.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggaehhsll.sHtML

Go:   // 手写循环
来源：http://3g.fanxiaobao.xyz/Article/details/gyszacdkt.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.fanxiaobao.xyz/Article/details/gckqwypbv.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.fanxiaobao.xyz/Article/details/gzmiwitbp.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gwfmccync.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.fanxiaobao.xyz/Article/details/gqbvhaqwd.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdugnvsjt.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gcevodcng.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbdjnnjue.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.fanxiaobao.xyz/Article/details/gjwhthxej.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.fanxiaobao.xyz/Article/details/guxgfrgve.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.fanxiaobao.xyz/Article/details/gghvvuzzu.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.fanxiaobao.xyz/Article/details/gfosvwgrc.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.fanxiaobao.xyz/Article/details/gcyuzhyag.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.fanxiaobao.xyz/Article/details/gqqzklyfz.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.fanxiaobao.xyz/Article/details/goibblwiw.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gguyzuadu.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.fanxiaobao.xyz/Article/details/gptfswbjt.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmqkjqto.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.fanxiaobao.xyz/Article/details/gqdvlveco.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.fanxiaobao.xyz/Article/details/gxczafurw.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwpyfeiz.sHtML

[D26] 数组转字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvjvpmlp.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.fanxiaobao.xyz/Article/details/gsaihgwpz.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gdzdzodar.sHtML

JS:   arr.join(", ")
来源：http://baike.fanxiaobao.xyz/Article/details/gfpylyyef.sHtML

TS:   arr.join(", ")
来源：http://3g.fanxiaobao.xyz/Article/details/gvuneejre.sHtML

Java: String.join(", ", list)
来源：http://blog.fanxiaobao.xyz/Article/details/ginkghbxo.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.fanxiaobao.xyz/Article/details/gsbafrdsg.sHtML

Ruby: arr.join(", ")
来源：http://mobile.fanxiaobao.xyz/Article/details/garvubbhv.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glognitgo.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gbbausinu.sHtML

E. 字符串处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gderedosx.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gqdclssyr.sHtML

[E01] 拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gvzybjalp.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.fanxiaobao.xyz/Article/details/gvzymtrxw.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/geqcfhnuu.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fanxiaobao.xyz/Article/details/glftrlyrb.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxdoxwjg.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.fanxiaobao.xyz/Article/details/gnkgajzzc.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.fanxiaobao.xyz/Article/details/gtllszmsl.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.fanxiaobao.xyz/Article/details/gfthfpwbx.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.fanxiaobao.xyz/Article/details/gklvszztz.sHtML

[E02] 重复字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqkdalds.sHtML

Py:   "ab" * 3
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqwkniyt.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gbduwxywq.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfcdwtqrd.sHtML


<!-- 参考信息 -->