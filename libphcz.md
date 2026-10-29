代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://blog.hesvh.cn/Article/details/gbmxbhsfd.sHtML

C#:   using System.Text;
来源：http://www.share.fehbvm.com/Article/details/gpzndblgy.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.hesvh.cn/Article/details/gfmkenmzi.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.hesvh.cn/Article/details/gkqbgxasy.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.hesvh.cn/Article/details/gwnhuyyas.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/gnjgqqkbg.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.hesvh.cn/Article/details/ggkksoejy.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.hesvh.cn/Article/details/gzhyolrxv.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.fehbvm.com/Article/details/griptbekg.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.hesvh.cn/Article/details/gudcybopn.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.hesvh.cn/Article/details/govfkudnn.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.hesvh.cn/Article/details/grivkwrlr.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.zdbjq.cn/Article/details/gaowioqoi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gbfwqktsf.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.hesvh.cn/Article/details/gdyldsivw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gnyhzepyf.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gntrryxto.sHtML

Go:   func add(a, b int) int
来源：http://baike.zdbjq.cn/Article/details/ghcacnfda.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.zdbjq.cn/Article/details/gddfdrdcz.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.fehbvm.com/Article/details/gbtqcyntg.sHtML

[C14] 泛型函数
来源：http://blog.hesvh.cn/Article/details/gzycgcdnz.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.hesvh.cn/Article/details/gyrirlmjh.sHtML

PHP:  // 无泛型
来源：http://www.share.zdbjq.cn/Article/details/ggwvonqxu.sHtML

JS:   // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gpvctleke.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.fehbvm.com/Article/details/gtthmnvcb.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.zdbjq.cn/Article/details/guwqnfmhm.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.hesvh.cn/Article/details/goolbjewv.sHtML

Ruby: # 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gjlxzrvfc.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.hesvh.cn/Article/details/ghiwffrnv.sHtML

[C15] 解构 / 展开参数
来源：http://3g.zdbjq.cn/Article/details/ggzazbdmk.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.fehbvm.com/Article/details/gqlrryksz.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.hesvh.cn/Article/details/gbmfcvgzi.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.zdbjq.cn/Article/details/gvhgjwpqe.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.fehbvm.com/Article/details/gieegwitp.sHtML

Java: // 无解构
来源：http://www.blog.hesvh.cn/Article/details/gxemotkgw.sHtML

Go:   // 无解构
来源：http://m.share.fehbvm.com/Article/details/gqdohnvrm.sHtML

Ruby: a, b = pair
来源：http://m.share.fehbvm.com/Article/details/glodbknmb.sHtML

C#:   var (a, b) = pair;
来源：http://3g.fehbvm.com/Article/details/gnztyhviy.sHtML

[C16] 函数 / 方法重载
来源：http://3g.hesvh.cn/Article/details/gigjwbrkp.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.fehbvm.com/Article/details/gtjznazbp.sHtML

PHP:  // 无重载
来源：http://mobile.fehbvm.com/Article/details/gxatugxhs.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.hesvh.cn/Article/details/gybpvmawx.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.zdbjq.cn/Article/details/gkngiexvp.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.zdbjq.cn/Article/details/guatkgaaw.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.zdbjq.cn/Article/details/gberzmubn.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.hesvh.cn/Article/details/guoicspet.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.fehbvm.com/Article/details/gtplyives.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gdpmqoniw.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.hesvh.cn/Article/details/gispxssqz.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ghvkxrkgm.sHtML

[D01] 创建数组 / 列表
来源：http://blog.fehbvm.com/Article/details/gmlxyxztr.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.fehbvm.com/Article/details/gkmgufdoh.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/gvavdcazg.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.fehbvm.com/Article/details/gxptxknxk.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.hesvh.cn/Article/details/gipgkdmyl.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.fehbvm.com/Article/details/gphjkcgxn.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.zdbjq.cn/Article/details/gnreetfor.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.zdbjq.cn/Article/details/gnrmconqa.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.zdbjq.cn/Article/details/ggdoihtwl.sHtML

[D02] 追加元素到末尾
来源：http://baike.fehbvm.com/Article/details/ggvjjgmct.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.fehbvm.com/Article/details/gvtvshxdv.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.zdbjq.cn/Article/details/gmfiiyacj.sHtML

JS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/gzmkoypgx.sHtML

TS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/gvakvwxtf.sHtML

Java: list.add(4);
来源：http://baike.hesvh.cn/Article/details/gqcpbowlh.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gieptlygm.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.fehbvm.com/Article/details/gdtqoxzky.sHtML

C#:   list.Add(4);
来源：http://wap.fehbvm.com/Article/details/gdywthcsk.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.fehbvm.com/Article/details/gbuolmiks.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.hesvh.cn/Article/details/gdckwdicc.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.zdbjq.cn/Article/details/gnlohfzsx.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.fehbvm.com/Article/details/gtvpaiszw.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.fehbvm.com/Article/details/gxhhrqoni.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gvrafcxmi.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.zdbjq.cn/Article/details/ggprhjlsb.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.zdbjq.cn/Article/details/gaslvdcgj.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.zdbjq.cn/Article/details/gntpwnmna.sHtML

[D04] 删除元素
来源：http://read.share.hesvh.cn/Article/details/gzlzozojr.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.zdbjq.cn/Article/details/gsysmrzjr.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.hesvh.cn/Article/details/grsueeggf.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.hesvh.cn/Article/details/gqpeiryma.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.hesvh.cn/Article/details/ghseepang.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.fehbvm.com/Article/details/gjrsrxedk.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.fehbvm.com/Article/details/gbyktnvdp.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.fehbvm.com/Article/details/gqlszciiw.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.fehbvm.com/Article/details/gghpdwcrm.sHtML

[D05] 访问与修改元素
来源：http://baike.hesvh.cn/Article/details/grgethnex.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gueirvsdj.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/guyefvlyj.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/ggiyjvbhp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.fehbvm.com/Article/details/gwjthokty.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.fehbvm.com/Article/details/gxleqllxc.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gqxsvszuv.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/guxrezbpb.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gznhvxing.sHtML

[D06] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gfkedoyyn.sHtML

Py:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gfrklzysy.sHtML

PHP:  count($arr);
来源：http://3g.hesvh.cn/Article/details/gnnjemqfq.sHtML

JS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/gztawoefr.sHtML

TS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/gbmljgzfl.sHtML

Java: list.size();
来源：http://www.share.zdbjq.cn/Article/details/gjdlkdauf.sHtML

Go:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/gajrfkwyj.sHtML

Ruby: arr.length; arr.size
来源：http://wap.zdbjq.cn/Article/details/gyoqnbkzp.sHtML

C#:   list.Count;
来源：http://mobile.hesvh.cn/Article/details/gpfufrqzn.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.hesvh.cn/Article/details/gdrygyelf.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.fehbvm.com/Article/details/gindizajt.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gcvmhczfz.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gxgwiqtne.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gmudlfbdj.sHtML

Java: list.subList(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gxgcgckiv.sHtML

Go:   arr[1:4]
来源：http://wap.hesvh.cn/Article/details/gsebwamqv.sHtML

Ruby: arr[1, 3]
来源：http://3g.fehbvm.com/Article/details/grfnktnix.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.fehbvm.com/Article/details/ghkidfykv.sHtML

[D08] 合并两个数组
来源：http://read.share.zdbjq.cn/Article/details/ghatmmrqq.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.fehbvm.com/Article/details/gkzyjcvqm.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.hesvh.cn/Article/details/grbrirpnt.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.fehbvm.com/Article/details/gzlvqrlah.sHtML

TS:   [...a, ...b];
来源：http://3g.zdbjq.cn/Article/details/gapwoeiqd.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.hesvh.cn/Article/details/gicwqiyqj.sHtML

Go:   append(a, b...)
来源：http://m.share.hesvh.cn/Article/details/gheiubduc.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.hesvh.cn/Article/details/gnejycnel.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.hesvh.cn/Article/details/gaxkjtner.sHtML

[D09] 排序（升序）
来源：http://wap.fehbvm.com/Article/details/gssgkwogg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.hesvh.cn/Article/details/gpwtculpq.sHtML

PHP:  sort($arr);
来源：http://www.blog.hesvh.cn/Article/details/gcfbkymaq.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.fehbvm.com/Article/details/gmixgflvf.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.fehbvm.com/Article/details/gxtazfoqf.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.fehbvm.com/Article/details/gvzmzpkpj.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gnioifxxg.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/gxhlxqvcm.sHtML

C#:   list.Sort();
来源：http://www.m.share.fehbvm.com/Article/details/gkiafhyfd.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.zdbjq.cn/Article/details/gqpuucppc.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.fehbvm.com/Article/details/gzwedyzdu.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/gtgydmjzd.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gztbjwdyt.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/gvdnobztf.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.hesvh.cn/Article/details/gswhosnbv.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.fehbvm.com/Article/details/gzamszrpj.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.fehbvm.com/Article/details/gzeneukai.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.fehbvm.com/Article/details/gjkaoxopp.sHtML

[D11] 反转数组
来源：http://read.share.fehbvm.com/Article/details/gzzvwfzgw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.hesvh.cn/Article/details/gkbvtuost.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.hesvh.cn/Article/details/giidfwfyr.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.hesvh.cn/Article/details/gdcundogv.sHtML

TS:   [...arr].reverse();
来源：http://read.share.fehbvm.com/Article/details/gsehfwweg.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.zdbjq.cn/Article/details/ggpedlrle.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.fehbvm.com/Article/details/ghhmqqlth.sHtML

Ruby: arr.reverse
来源：http://wap.hesvh.cn/Article/details/gvfgdromh.sHtML

C#:   list.Reverse();
来源：http://www.m.share.hesvh.cn/Article/details/gfvkbidcs.sHtML

[D12] 查找元素下标
来源：http://www.share.hesvh.cn/Article/details/gokjzynjq.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.zdbjq.cn/Article/details/gsqnxplko.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.fehbvm.com/Article/details/gfcmajnll.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/gkerepxpl.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/gikotblrw.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.zdbjq.cn/Article/details/gmpzbwnmg.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.fehbvm.com/Article/details/glqilygut.sHtML

Ruby: arr.index(x)
来源：http://3g.fehbvm.com/Article/details/gmdcmunry.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.zdbjq.cn/Article/details/ghdlymurr.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.fehbvm.com/Article/details/gvfvltlny.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.zdbjq.cn/Article/details/gzrulssgh.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.fehbvm.com/Article/details/gzqtmexur.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/gldurrrqj.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.fehbvm.com/Article/details/gyqpokjwb.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.hesvh.cn/Article/details/gswkoeypx.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.hesvh.cn/Article/details/gzbzwhnda.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.fehbvm.com/Article/details/gcnyvsuof.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.fehbvm.com/Article/details/gkrpxpzma.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.hesvh.cn/Article/details/gkhljhmec.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.zdbjq.cn/Article/details/ggdjwbcds.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.zdbjq.cn/Article/details/guuyqdzhl.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/gjbtyffro.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/galxbhecz.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.hesvh.cn/Article/details/gbmpahkin.sHtML

Go:   // 手写循环
来源：http://wap.hesvh.cn/Article/details/gqcmgzwvj.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gfxdlvujt.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.fehbvm.com/Article/details/ghalkffjm.sHtML

[D15] 去重
来源：http://wap.zdbjq.cn/Article/details/gaixtmazo.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/gsfmwqqfh.sHtML

PHP:  array_unique($arr);
来源：http://wap.fehbvm.com/Article/details/gxouoqizj.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gzpdljhub.sHtML

TS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gfhbcioji.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.hesvh.cn/Article/details/geqdrwfkb.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.zdbjq.cn/Article/details/gpsrcvysp.sHtML

Ruby: arr.uniq
来源：http://mobile.hesvh.cn/Article/details/gzkhgyyzg.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.fehbvm.com/Article/details/gvvrrbcag.sHtML

[D16] 求和与平均值
来源：http://read.share.zdbjq.cn/Article/details/gllpyxmhg.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.fehbvm.com/Article/details/gvzhjansr.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gzuzsxyut.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/gscjtltdn.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gpuodqpfe.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.fehbvm.com/Article/details/gezbhdgyv.sHtML

Go:   // 手写循环累加
来源：http://mobile.hesvh.cn/Article/details/gwbaczehr.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.zdbjq.cn/Article/details/ghvmvxzti.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.hesvh.cn/Article/details/gcxnpbhkq.sHtML

[D17] 最大值与最小值
来源：http://wap.zdbjq.cn/Article/details/gjqkjtcwn.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.fehbvm.com/Article/details/gyjjdspym.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gvwywcfnc.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.fehbvm.com/Article/details/gbjvhrkys.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gmlggimtj.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.fehbvm.com/Article/details/gjbzbykjd.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.hesvh.cn/Article/details/gwyxehduu.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.zdbjq.cn/Article/details/ghlwsgrkl.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.hesvh.cn/Article/details/gxhxtucnx.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.fehbvm.com/Article/details/ghvjaxlkh.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.hesvh.cn/Article/details/gaxfuntto.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.hesvh.cn/Article/details/gfycrsfao.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.fehbvm.com/Article/details/giceohucq.sHtML

TS:   nested.flat();
来源：http://3g.hesvh.cn/Article/details/gtzlxbnnv.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.zdbjq.cn/Article/details/gfrtpqcdj.sHtML

Go:   // 手写双层循环
来源：http://m.share.hesvh.cn/Article/details/gtfdhrtul.sHtML

Ruby: nested.flatten
来源：http://wap.fehbvm.com/Article/details/gorgbkrfu.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gzqvxvjze.sHtML

[D19] 按字段分组
来源：http://wap.zdbjq.cn/Article/details/gsumzzwgk.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.fehbvm.com/Article/details/gflibaaki.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.fehbvm.com/Article/details/grzyhrflt.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.hesvh.cn/Article/details/gfnqdqayr.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.zdbjq.cn/Article/details/gwemdnmtw.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.fehbvm.com/Article/details/glviplqps.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.hesvh.cn/Article/details/gfpysuvis.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.hesvh.cn/Article/details/ghutgxncq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.zdbjq.cn/Article/details/gteesblvr.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.zdbjq.cn/Article/details/getwwzqwz.sHtML

Py:   Counter(arr)
来源：http://www.share.hesvh.cn/Article/details/gphzdqnwu.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.zdbjq.cn/Article/details/grqzfiwpb.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/gcxaklblo.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/gcahvyjcr.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.hesvh.cn/Article/details/gvemqmugz.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.zdbjq.cn/Article/details/gbfemtucj.sHtML

Ruby: arr.tally
来源：http://baike.hesvh.cn/Article/details/gwktayzvy.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.hesvh.cn/Article/details/gpnsqhgst.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.hesvh.cn/Article/details/gzckqtktz.sHtML

Py:   x in arr
来源：http://read.share.zdbjq.cn/Article/details/gjvjkrdcy.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.fehbvm.com/Article/details/gdyekauxr.sHtML

JS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/glkyuhnoa.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gxsvptlvn.sHtML

Java: list.contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gxwhpnmih.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gouhrrjta.sHtML

Ruby: arr.include?(x)
来源：http://www.share.zdbjq.cn/Article/details/ghduwfwau.sHtML

C#:   list.Contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gwbvdiarv.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.zdbjq.cn/Article/details/gyvxnpopv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.fehbvm.com/Article/details/gekkfrrke.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.fehbvm.com/Article/details/gtwlqaifl.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.hesvh.cn/Article/details/gcljnvwzp.sHtML

TS:   [...arr];
来源：http://read.share.zdbjq.cn/Article/details/gqgwpnafs.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.fehbvm.com/Article/details/gubdbjqrc.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.hesvh.cn/Article/details/gtybdtehj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.fehbvm.com/Article/details/geczpnjco.sHtML

C#:   new List<int>(list);
来源：http://3g.hesvh.cn/Article/details/gkkthzzjr.sHtML

[D23] reduce 累积计算
来源：http://mobile.fehbvm.com/Article/details/gwxvsqzmq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.zdbjq.cn/Article/details/gddzzpdih.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gxhayzhtd.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gsaiqoacy.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/glyqmakyg.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.fehbvm.com/Article/details/geapdotzn.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gaesoikmt.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.fehbvm.com/Article/details/gywzttdff.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.zdbjq.cn/Article/details/gfymjubzj.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.zdbjq.cn/Article/details/gdjhkbnve.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.hesvh.cn/Article/details/gfmplbwjk.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.fehbvm.com/Article/details/gnshiunuu.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.fehbvm.com/Article/details/gmqzmdoka.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.hesvh.cn/Article/details/gygtoqokr.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.zdbjq.cn/Article/details/grvzmayvr.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.hesvh.cn/Article/details/gzcplnxen.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.zdbjq.cn/Article/details/ggnpgjcbt.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.fehbvm.com/Article/details/gjwopkabg.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.fehbvm.com/Article/details/gsgguuafu.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.hesvh.cn/Article/details/gukxgwbis.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.hesvh.cn/Article/details/gblspruyl.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.zdbjq.cn/Article/details/gduumvvmn.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.hesvh.cn/Article/details/ghiszviwv.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.zdbjq.cn/Article/details/gubusrypq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.hesvh.cn/Article/details/gsnyhixif.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.zdbjq.cn/Article/details/guzbowame.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.fehbvm.com/Article/details/gkuspgsmq.sHtML

[D26] 数组转字符串
来源：http://blog.hesvh.cn/Article/details/grfyfhwao.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.hesvh.cn/Article/details/gmlqptdia.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gloexrguw.sHtML

JS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/ggusgqaux.sHtML

TS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gbflwkecd.sHtML

Java: String.join(", ", list)
来源：http://3g.fehbvm.com/Article/details/giuaxvqln.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.fehbvm.com/Article/details/gvwykcbty.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gmxmforrr.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/gztazsrmi.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gnhkeyqjv.sHtML

E. 字符串处理
来源：http://www.share.zdbjq.cn/Article/details/gwaalskaw.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gcbokryiz.sHtML

[E01] 拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gcjfjomea.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.fehbvm.com/Article/details/glkehrgia.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.hesvh.cn/Article/details/gqpmsvqbi.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/grkveemlw.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gewhcipkx.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.zdbjq.cn/Article/details/gltzmmnlq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.zdbjq.cn/Article/details/gmamutuvb.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.hesvh.cn/Article/details/glmwegltg.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/guaimcxfk.sHtML

[E02] 重复字符串
来源：http://blog.zdbjq.cn/Article/details/gubxgyqht.sHtML

Py:   "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/grteyitpj.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.hesvh.cn/Article/details/gvsmchpmv.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gqdykldwk.sHtML


<!-- 参考信息 -->