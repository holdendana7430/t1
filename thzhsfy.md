代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://baike.fehbvm.com/Article/details/gonnayjed.sHtML

C#:   using System.Text;
来源：http://baike.zdbjq.cn/Article/details/gtazrakfv.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.zdbjq.cn/Article/details/gicueuzpw.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.fehbvm.com/Article/details/gasygnjhw.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.fehbvm.com/Article/details/gxeqaquht.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.zdbjq.cn/Article/details/gpeslenye.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.zdbjq.cn/Article/details/gmvrtvilt.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.hesvh.cn/Article/details/gwyhbhiso.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.fehbvm.com/Article/details/gqczbqviz.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.hesvh.cn/Article/details/giepaneso.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.fehbvm.com/Article/details/gdtfoxoqm.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.hesvh.cn/Article/details/gagkixpwv.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.hesvh.cn/Article/details/gkvqjumxh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/glpikcwpt.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.zdbjq.cn/Article/details/gemfwqtgy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gvgwpocax.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gzxywsrny.sHtML

Go:   func add(a, b int) int
来源：http://read.share.hesvh.cn/Article/details/githyzpmh.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.fehbvm.com/Article/details/gmkmeuuxu.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.fehbvm.com/Article/details/gsarnayiq.sHtML

[C14] 泛型函数
来源：http://www.share.zdbjq.cn/Article/details/glzuunhhk.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.fehbvm.com/Article/details/gyhtldeft.sHtML

PHP:  // 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gvdnsvkif.sHtML

JS:   // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gpufkxtln.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.fehbvm.com/Article/details/goqdziroi.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.fehbvm.com/Article/details/gooitehlv.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.zdbjq.cn/Article/details/gvmgkkazd.sHtML

Ruby: # 无泛型
来源：http://3g.zdbjq.cn/Article/details/gdvbnebac.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.fehbvm.com/Article/details/gbjrzvotx.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.fehbvm.com/Article/details/gsziyzhof.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.fehbvm.com/Article/details/gbkcnnrfh.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.zdbjq.cn/Article/details/gbtpfgpun.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/gadhvamzq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.fehbvm.com/Article/details/ggnhcdmup.sHtML

Java: // 无解构
来源：http://wap.hesvh.cn/Article/details/gnkwrtcnn.sHtML

Go:   // 无解构
来源：http://wap.zdbjq.cn/Article/details/gwewsumpl.sHtML

Ruby: a, b = pair
来源：http://www.blog.hesvh.cn/Article/details/ggxrchfbv.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.fehbvm.com/Article/details/gyrgesree.sHtML

[C16] 函数 / 方法重载
来源：http://blog.fehbvm.com/Article/details/gpndklwkg.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.zdbjq.cn/Article/details/gjztdwpub.sHtML

PHP:  // 无重载
来源：http://baike.fehbvm.com/Article/details/gfemaqxur.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.hesvh.cn/Article/details/ghuhaaoug.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.hesvh.cn/Article/details/ghorurnat.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.hesvh.cn/Article/details/ghxjwmjvb.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.zdbjq.cn/Article/details/gqcoevtan.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.zdbjq.cn/Article/details/gureslwom.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.fehbvm.com/Article/details/gkebnhtnb.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gzadtuknz.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.fehbvm.com/Article/details/gvllqjsow.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/godahqdov.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.hesvh.cn/Article/details/gnxlyxaxt.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.zdbjq.cn/Article/details/gzqvbmsbj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.fehbvm.com/Article/details/gxkboczxi.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.hesvh.cn/Article/details/gethemcug.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.zdbjq.cn/Article/details/giayqwsux.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.fehbvm.com/Article/details/gtrbqypcf.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.hesvh.cn/Article/details/gijkahfou.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.fehbvm.com/Article/details/gmxijoybx.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.hesvh.cn/Article/details/grnguzhys.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.zdbjq.cn/Article/details/gtscqirma.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.fehbvm.com/Article/details/gaxolobob.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.zdbjq.cn/Article/details/gdgfpupzv.sHtML

JS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/gxhrztkva.sHtML

TS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/gqlvfiplc.sHtML

Java: list.add(4);
来源：http://baike.fehbvm.com/Article/details/gmtkpahez.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.hesvh.cn/Article/details/gimnxdnmc.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.fehbvm.com/Article/details/gbolsacry.sHtML

C#:   list.Add(4);
来源：http://read.share.fehbvm.com/Article/details/gftwovywi.sHtML

[D03] 在指定位置插入元素
来源：http://baike.hesvh.cn/Article/details/gmdkcfaqm.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.zdbjq.cn/Article/details/grxhuciep.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.zdbjq.cn/Article/details/gsmvgzneb.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.hesvh.cn/Article/details/gmerqqqpd.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.fehbvm.com/Article/details/gogybrrpd.sHtML

Java: list.add(0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gvyhxktfv.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gyydmsfei.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.fehbvm.com/Article/details/gmufzywuv.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.fehbvm.com/Article/details/gdwgpomci.sHtML

[D04] 删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gyywssjzx.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.hesvh.cn/Article/details/gtzpujnbc.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gapptywmy.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.fehbvm.com/Article/details/gxvzzlori.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.fehbvm.com/Article/details/ggxkjqnui.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.zdbjq.cn/Article/details/galypjwnx.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.hesvh.cn/Article/details/gauzmzwwx.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.fehbvm.com/Article/details/gnvulkipi.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.hesvh.cn/Article/details/gbjuchdqm.sHtML

[D05] 访问与修改元素
来源：http://m.share.fehbvm.com/Article/details/geydverbb.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gtdgnqhrs.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gvzpzsyyy.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/glnruwncs.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.fehbvm.com/Article/details/gsivjxbmw.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.zdbjq.cn/Article/details/grndwgfvs.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/grfwmwfnp.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gruvuyhxb.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gchswhzfd.sHtML

[D06] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/gyukwflch.sHtML

Py:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/ggmjmultx.sHtML

PHP:  count($arr);
来源：http://mobile.zdbjq.cn/Article/details/gftmejxya.sHtML

JS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/gynuzvxcz.sHtML

TS:   arr.length
来源：http://wap.hesvh.cn/Article/details/gopqoykdq.sHtML

Java: list.size();
来源：http://baike.fehbvm.com/Article/details/gbeenseot.sHtML

Go:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gwvqywsry.sHtML

Ruby: arr.length; arr.size
来源：http://3g.fehbvm.com/Article/details/glhftzwxj.sHtML

C#:   list.Count;
来源：http://mobile.zdbjq.cn/Article/details/gvpbwprpu.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.hesvh.cn/Article/details/gdtmtgqbg.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.fehbvm.com/Article/details/geoxvivng.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.fehbvm.com/Article/details/gqktyxvst.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gabwdwzqo.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gbowuxczy.sHtML

Java: list.subList(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gzuukyyeb.sHtML

Go:   arr[1:4]
来源：http://www.blog.hesvh.cn/Article/details/gsjwmkoru.sHtML

Ruby: arr[1, 3]
来源：http://www.share.zdbjq.cn/Article/details/gtnlkkbnx.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.hesvh.cn/Article/details/gzyssnoce.sHtML

[D08] 合并两个数组
来源：http://wap.fehbvm.com/Article/details/gheabtamd.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.fehbvm.com/Article/details/gnkethych.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.fehbvm.com/Article/details/gedasnrbs.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.zdbjq.cn/Article/details/gamjbagar.sHtML

TS:   [...a, ...b];
来源：http://wap.zdbjq.cn/Article/details/ghusouivz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.hesvh.cn/Article/details/gntzkbtdt.sHtML

Go:   append(a, b...)
来源：http://baike.hesvh.cn/Article/details/gdofzhqvo.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.hesvh.cn/Article/details/glqtktdjr.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.fehbvm.com/Article/details/gpvfebdha.sHtML

[D09] 排序（升序）
来源：http://www.share.fehbvm.com/Article/details/gjbbejvft.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/gelcrkmdu.sHtML

PHP:  sort($arr);
来源：http://wap.zdbjq.cn/Article/details/goafpuetr.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.hesvh.cn/Article/details/gmgwfphni.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.hesvh.cn/Article/details/gggeyyjhk.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.zdbjq.cn/Article/details/gxuuhywvr.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/giocsrczq.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/gpgszajrq.sHtML

C#:   list.Sort();
来源：http://read.share.zdbjq.cn/Article/details/gvqcurqem.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.zdbjq.cn/Article/details/gbuvvqlyi.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.hesvh.cn/Article/details/gyuwfhmin.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fehbvm.com/Article/details/ggrftvcfu.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/gvwdedvpw.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/gicujbigb.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.fehbvm.com/Article/details/gfkmgopik.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.hesvh.cn/Article/details/ggqojokig.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.hesvh.cn/Article/details/gwmcnhlhc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.zdbjq.cn/Article/details/goyvtwpev.sHtML

[D11] 反转数组
来源：http://read.share.fehbvm.com/Article/details/gvogiuxca.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.fehbvm.com/Article/details/gkotncfwy.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.zdbjq.cn/Article/details/gsfecsdot.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.zdbjq.cn/Article/details/gkrxmurvf.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.hesvh.cn/Article/details/gjjmhcxic.sHtML

Java: Collections.reverse(list);
来源：http://wap.zdbjq.cn/Article/details/gpdkedxmy.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.fehbvm.com/Article/details/gidvkknbh.sHtML

Ruby: arr.reverse
来源：http://www.share.zdbjq.cn/Article/details/ghoccrtvv.sHtML

C#:   list.Reverse();
来源：http://www.share.fehbvm.com/Article/details/gxivergsd.sHtML

[D12] 查找元素下标
来源：http://blog.hesvh.cn/Article/details/gnqcpwslz.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.zdbjq.cn/Article/details/gkrjujygi.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.zdbjq.cn/Article/details/gytowusnl.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/grfhfidqj.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/ggmrscggo.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.hesvh.cn/Article/details/gmwssxrwy.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.fehbvm.com/Article/details/gjvemdaoz.sHtML

Ruby: arr.index(x)
来源：http://m.share.zdbjq.cn/Article/details/gmnipmvxj.sHtML

C#:   list.IndexOf(x);
来源：http://3g.hesvh.cn/Article/details/gkfmpddjy.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.hesvh.cn/Article/details/giqjijbgy.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.hesvh.cn/Article/details/gyitbmeij.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.zdbjq.cn/Article/details/grvnjlwnb.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/gylpxahbh.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.fehbvm.com/Article/details/gyffhaxuy.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.hesvh.cn/Article/details/gchzwgfld.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.fehbvm.com/Article/details/gwgnbpxdh.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.zdbjq.cn/Article/details/gizzpqbuo.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.zdbjq.cn/Article/details/ghizrijnq.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.fehbvm.com/Article/details/grcepazdq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gpetbncai.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.zdbjq.cn/Article/details/gcfmeiacb.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/gtdovlxba.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/gtxsfqiaz.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.fehbvm.com/Article/details/gwnfmhldo.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/gmpbuidte.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gzszljwte.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.fehbvm.com/Article/details/gfkebcavo.sHtML

[D15] 去重
来源：http://read.share.zdbjq.cn/Article/details/gakfvjhrj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/gctmvdnwd.sHtML

PHP:  array_unique($arr);
来源：http://blog.hesvh.cn/Article/details/gxwteeyzg.sHtML

JS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/glqyvjosp.sHtML

TS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/geufshpfe.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.hesvh.cn/Article/details/guvgktuyg.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.zdbjq.cn/Article/details/gysgmhhwo.sHtML

Ruby: arr.uniq
来源：http://www.share.fehbvm.com/Article/details/gbdogzobo.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.fehbvm.com/Article/details/gomxhlcgr.sHtML

[D16] 求和与平均值
来源：http://www.blog.zdbjq.cn/Article/details/gmwkfumwz.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.fehbvm.com/Article/details/gpxxlripg.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.hesvh.cn/Article/details/gviqjozud.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gyljjziut.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gnjpibvne.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.hesvh.cn/Article/details/gbbnooyno.sHtML

Go:   // 手写循环累加
来源：http://read.share.zdbjq.cn/Article/details/gwbqwlrbv.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.zdbjq.cn/Article/details/gbbspllwe.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.fehbvm.com/Article/details/gjubfiluw.sHtML

[D17] 最大值与最小值
来源：http://3g.zdbjq.cn/Article/details/grzahwrrt.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.zdbjq.cn/Article/details/gzloronvn.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.zdbjq.cn/Article/details/gylmzjhgu.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.zdbjq.cn/Article/details/gljwqophp.sHtML

TS:   Math.max(...arr);
来源：http://www.share.hesvh.cn/Article/details/gesxbqtpi.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.hesvh.cn/Article/details/gvblsfydc.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.fehbvm.com/Article/details/gaysaozgr.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.hesvh.cn/Article/details/gdeuvzapd.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.zdbjq.cn/Article/details/gyqtjdgcv.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.hesvh.cn/Article/details/gpsrqjqqq.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.zdbjq.cn/Article/details/gscxexxzu.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.hesvh.cn/Article/details/gtskmwzcr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.zdbjq.cn/Article/details/gycjmsmts.sHtML

TS:   nested.flat();
来源：http://wap.hesvh.cn/Article/details/gtxehmttr.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.fehbvm.com/Article/details/gdwvwslns.sHtML

Go:   // 手写双层循环
来源：http://baike.zdbjq.cn/Article/details/gzkyexvxk.sHtML

Ruby: nested.flatten
来源：http://www.blog.hesvh.cn/Article/details/gkkqmxtdm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.fehbvm.com/Article/details/grvlmxhpa.sHtML

[D19] 按字段分组
来源：http://www.blog.zdbjq.cn/Article/details/gsidkqple.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.hesvh.cn/Article/details/gdqoypdov.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.hesvh.cn/Article/details/gsmvwilff.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.hesvh.cn/Article/details/gmlponygj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/gyrcaynda.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.hesvh.cn/Article/details/gxbjaplhh.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.hesvh.cn/Article/details/gveotjrwh.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.hesvh.cn/Article/details/ggtixvjia.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.hesvh.cn/Article/details/gmxtyxjyq.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.zdbjq.cn/Article/details/gefmbrxgh.sHtML

Py:   Counter(arr)
来源：http://read.share.hesvh.cn/Article/details/grxpzzgad.sHtML

PHP:  array_count_values($arr);
来源：http://baike.fehbvm.com/Article/details/gbmdrsqvs.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/gvfbximux.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/gbhcqpmvy.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.hesvh.cn/Article/details/gborzcbnz.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.fehbvm.com/Article/details/gxfcopuzo.sHtML

Ruby: arr.tally
来源：http://wap.zdbjq.cn/Article/details/gsimaxscg.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.fehbvm.com/Article/details/gpheaijdj.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.hesvh.cn/Article/details/gmejhqpjd.sHtML

Py:   x in arr
来源：http://www.share.fehbvm.com/Article/details/gxdsxfqxn.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.hesvh.cn/Article/details/gaxviptch.sHtML

JS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/gxpspaluw.sHtML

TS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gorloavsw.sHtML

Java: list.contains(x)
来源：http://baike.zdbjq.cn/Article/details/gllqwuzac.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.fehbvm.com/Article/details/ggwbquibx.sHtML

Ruby: arr.include?(x)
来源：http://read.share.hesvh.cn/Article/details/gkyckrlnz.sHtML

C#:   list.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gsoqlljwt.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.hesvh.cn/Article/details/gbasjrhqr.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gggnwogxr.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.zdbjq.cn/Article/details/gzgovvsgf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.zdbjq.cn/Article/details/gecphohhy.sHtML

TS:   [...arr];
来源：http://m.share.hesvh.cn/Article/details/gomrocixj.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.hesvh.cn/Article/details/gbbjrmuua.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.hesvh.cn/Article/details/gmpuhtevl.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.fehbvm.com/Article/details/geuwqhtaa.sHtML

C#:   new List<int>(list);
来源：http://m.share.zdbjq.cn/Article/details/gcaimfnwj.sHtML

[D23] reduce 累积计算
来源：http://www.share.hesvh.cn/Article/details/gzwfwbiav.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.fehbvm.com/Article/details/gqbsiqtnp.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.hesvh.cn/Article/details/gevryusqp.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/gentjxrii.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/gbizabbfu.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.hesvh.cn/Article/details/gzjpaqzon.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/glstyggpt.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.zdbjq.cn/Article/details/gqexehllu.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.hesvh.cn/Article/details/gwokxaorv.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.zdbjq.cn/Article/details/gmehfuzpa.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.fehbvm.com/Article/details/gxsfwerct.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.hesvh.cn/Article/details/gxtswmhea.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.fehbvm.com/Article/details/gtpllffgd.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gfwpngpyw.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.hesvh.cn/Article/details/gdfhazoej.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.zdbjq.cn/Article/details/ghpjekwnt.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.fehbvm.com/Article/details/gxmnujwfq.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.hesvh.cn/Article/details/golrqhnki.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.fehbvm.com/Article/details/gvsacugil.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.hesvh.cn/Article/details/gilchpgts.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.hesvh.cn/Article/details/gmkzknblf.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.hesvh.cn/Article/details/gmpbjkvpv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.zdbjq.cn/Article/details/gwyhpgjul.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.zdbjq.cn/Article/details/gpbtbiegi.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.hesvh.cn/Article/details/gprspgbia.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.fehbvm.com/Article/details/gkblqasdc.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.zdbjq.cn/Article/details/gbetktckw.sHtML

[D26] 数组转字符串
来源：http://mobile.fehbvm.com/Article/details/gwedawlay.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.fehbvm.com/Article/details/gaatotayi.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.zdbjq.cn/Article/details/gefoujrzn.sHtML

JS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gnucithiy.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gdigjfebg.sHtML

Java: String.join(", ", list)
来源：http://blog.zdbjq.cn/Article/details/giuvwgmet.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.fehbvm.com/Article/details/gzoylwzyn.sHtML

Ruby: arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gfhrqrpfk.sHtML

C#:   string.Join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gacidngul.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gecvplruf.sHtML

E. 字符串处理
来源：http://3g.fehbvm.com/Article/details/gecghjuac.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gvwzwerbm.sHtML

[E01] 拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gundopaok.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.fehbvm.com/Article/details/gekmqjfdd.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.fehbvm.com/Article/details/guqzpvqhl.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fehbvm.com/Article/details/glbrncrqd.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/gnedlquht.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.fehbvm.com/Article/details/gbuwibzfn.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.fehbvm.com/Article/details/gxlodjjcf.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.fehbvm.com/Article/details/gjarlcqob.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.hesvh.cn/Article/details/goibpezly.sHtML

[E02] 重复字符串
来源：http://www.blog.zdbjq.cn/Article/details/gyxlefmeh.sHtML

Py:   "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gknolhzkg.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.zdbjq.cn/Article/details/gajzgoqmg.sHtML

JS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gcnorvsnb.sHtML


<!-- 参考信息 -->