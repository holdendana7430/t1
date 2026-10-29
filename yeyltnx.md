代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://www.share.fehbvm.com/Article/details/gljcqleax.sHtML

C#:   using System.Text;
来源：http://www.share.zdbjq.cn/Article/details/ghjozjlti.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.fehbvm.com/Article/details/gqpeyfceh.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.fehbvm.com/Article/details/gnukudmea.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.zdbjq.cn/Article/details/gqiqvdlis.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.hesvh.cn/Article/details/ghsiuvygy.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.hesvh.cn/Article/details/gjbhoaevl.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.hesvh.cn/Article/details/gfqkbmgkj.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.fehbvm.com/Article/details/goypahfqm.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.hesvh.cn/Article/details/gowqgtlnd.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.hesvh.cn/Article/details/gdlwlptcs.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.zdbjq.cn/Article/details/graszgsbj.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.fehbvm.com/Article/details/grsbxskhj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gliwaikjt.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.fehbvm.com/Article/details/glaywvdiq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gomesnfch.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/ghmztfior.sHtML

Go:   func add(a, b int) int
来源：http://baike.zdbjq.cn/Article/details/gxmpfokxh.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.fehbvm.com/Article/details/ggawxqvob.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.zdbjq.cn/Article/details/gwrdxztpz.sHtML

[C14] 泛型函数
来源：http://blog.fehbvm.com/Article/details/gbuegxaxk.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.hesvh.cn/Article/details/gzbwqsagm.sHtML

PHP:  // 无泛型
来源：http://baike.zdbjq.cn/Article/details/ghgmycgrw.sHtML

JS:   // 无泛型
来源：http://3g.zdbjq.cn/Article/details/gjgtquexy.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.fehbvm.com/Article/details/gkqcxbebn.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.fehbvm.com/Article/details/gvobkmjpa.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.zdbjq.cn/Article/details/gkctvoxga.sHtML

Ruby: # 无泛型
来源：http://baike.hesvh.cn/Article/details/gwwvrflwr.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.fehbvm.com/Article/details/gopdpjzhi.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.zdbjq.cn/Article/details/govkegcwd.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.hesvh.cn/Article/details/giyxzofjz.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.zdbjq.cn/Article/details/gfllnagiq.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.zdbjq.cn/Article/details/gczbybodf.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.zdbjq.cn/Article/details/gpsujtesh.sHtML

Java: // 无解构
来源：http://read.share.hesvh.cn/Article/details/gkanvucpy.sHtML

Go:   // 无解构
来源：http://blog.fehbvm.com/Article/details/gqmqpnmzs.sHtML

Ruby: a, b = pair
来源：http://baike.fehbvm.com/Article/details/gkulosvep.sHtML

C#:   var (a, b) = pair;
来源：http://wap.zdbjq.cn/Article/details/gcubgxtxk.sHtML

[C16] 函数 / 方法重载
来源：http://3g.zdbjq.cn/Article/details/goplqxrwq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.hesvh.cn/Article/details/gnhnqfecw.sHtML

PHP:  // 无重载
来源：http://m.share.fehbvm.com/Article/details/gwjfflvoa.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.hesvh.cn/Article/details/gjayhefdf.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.hesvh.cn/Article/details/gzavhzqvt.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.hesvh.cn/Article/details/guyqrytyi.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.fehbvm.com/Article/details/gzfqsgdec.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.zdbjq.cn/Article/details/gejrevuja.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.zdbjq.cn/Article/details/gynlncpuq.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gvqueyfaa.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.zdbjq.cn/Article/details/gjcblrtus.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gbmkrafsa.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.hesvh.cn/Article/details/gecudcdub.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.hesvh.cn/Article/details/gxivgvsmp.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.zdbjq.cn/Article/details/goonqinqm.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.fehbvm.com/Article/details/gwdtglnbw.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.fehbvm.com/Article/details/gwbqagsvr.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.hesvh.cn/Article/details/gmrfqholm.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.fehbvm.com/Article/details/gnkeuhgjc.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.fehbvm.com/Article/details/gnwjqnwzr.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.zdbjq.cn/Article/details/gjvcxounk.sHtML

[D02] 追加元素到末尾
来源：http://baike.zdbjq.cn/Article/details/ghykujyxi.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.hesvh.cn/Article/details/gdsevnphy.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.fehbvm.com/Article/details/gdhafjihl.sHtML

JS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/gybmhexkq.sHtML

TS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/gefmxkcsm.sHtML

Java: list.add(4);
来源：http://wap.zdbjq.cn/Article/details/gclgocghk.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.fehbvm.com/Article/details/glcbmhtld.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.fehbvm.com/Article/details/ggsumctkj.sHtML

C#:   list.Add(4);
来源：http://www.share.hesvh.cn/Article/details/gempkuqla.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.hesvh.cn/Article/details/gqraeiscj.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.fehbvm.com/Article/details/gdwibhtkb.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.zdbjq.cn/Article/details/gsuoixcmk.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.fehbvm.com/Article/details/gutdufden.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.fehbvm.com/Article/details/gdxhyotmm.sHtML

Java: list.add(0, 0);
来源：http://wap.fehbvm.com/Article/details/gzxegozyk.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.fehbvm.com/Article/details/ghwqhnofl.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.hesvh.cn/Article/details/glgliwmwu.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.hesvh.cn/Article/details/gkxzyfshy.sHtML

[D04] 删除元素
来源：http://mobile.zdbjq.cn/Article/details/gwbvxfssk.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.hesvh.cn/Article/details/glykorrln.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.zdbjq.cn/Article/details/gpakicauw.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.zdbjq.cn/Article/details/gobxnwjqm.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gbksjcwbo.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.hesvh.cn/Article/details/guzovujnj.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.fehbvm.com/Article/details/gptqdoyha.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.zdbjq.cn/Article/details/gkpukdaju.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.hesvh.cn/Article/details/gsjambxqa.sHtML

[D05] 访问与修改元素
来源：http://read.share.fehbvm.com/Article/details/ggxkbniyc.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gjtyrexpm.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gqdyjgdtd.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gieonrlve.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.zdbjq.cn/Article/details/giqzaargb.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.zdbjq.cn/Article/details/gmodumoia.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/grmyrjlbc.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gdbhjmpsl.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gqefqjqno.sHtML

[D06] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/gfojbcdeh.sHtML

Py:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/gbeiimzaz.sHtML

PHP:  count($arr);
来源：http://wap.hesvh.cn/Article/details/guqtryfvy.sHtML

JS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gfcaqwacr.sHtML

TS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gtdkliicz.sHtML

Java: list.size();
来源：http://baike.zdbjq.cn/Article/details/gmvwjhlam.sHtML

Go:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gdoelbfqr.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.hesvh.cn/Article/details/gsszikoae.sHtML

C#:   list.Count;
来源：http://www.m.share.hesvh.cn/Article/details/ggrwpyfdm.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.hesvh.cn/Article/details/gzlawgfkt.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.fehbvm.com/Article/details/genfruvgf.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.hesvh.cn/Article/details/gysqierzs.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gkcmafobs.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/guiahbrsg.sHtML

Java: list.subList(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gidqqibdq.sHtML

Go:   arr[1:4]
来源：http://read.share.zdbjq.cn/Article/details/gyycnbvvq.sHtML

Ruby: arr[1, 3]
来源：http://www.share.hesvh.cn/Article/details/gmajobnur.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gmhjcmdue.sHtML

[D08] 合并两个数组
来源：http://3g.zdbjq.cn/Article/details/gxiakhoxy.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.zdbjq.cn/Article/details/gilgkdtqg.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.hesvh.cn/Article/details/gcasnwoxb.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.zdbjq.cn/Article/details/gdpbujvxg.sHtML

TS:   [...a, ...b];
来源：http://mobile.fehbvm.com/Article/details/gxqxcimfx.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.fehbvm.com/Article/details/ghararwqg.sHtML

Go:   append(a, b...)
来源：http://m.share.zdbjq.cn/Article/details/gwurnrvna.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.zdbjq.cn/Article/details/gzarxhoby.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.fehbvm.com/Article/details/gzyrcrktf.sHtML

[D09] 排序（升序）
来源：http://baike.zdbjq.cn/Article/details/gzpqjhvht.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/ghwiqmugu.sHtML

PHP:  sort($arr);
来源：http://www.blog.fehbvm.com/Article/details/gfvzggqkm.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.hesvh.cn/Article/details/gpeviikpy.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.zdbjq.cn/Article/details/gijxjmcxj.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.fehbvm.com/Article/details/gvlrzbtnv.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/gauxfsgpi.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/gqtwxpmxh.sHtML

C#:   list.Sort();
来源：http://read.share.hesvh.cn/Article/details/gqtkmsuzy.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.hesvh.cn/Article/details/gyyfwwulb.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.hesvh.cn/Article/details/gqgxirvxg.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gpbiewnju.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/gqxvjmcpg.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/ghvbiqcby.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.hesvh.cn/Article/details/gculalajp.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.hesvh.cn/Article/details/gryaoiibh.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.zdbjq.cn/Article/details/gdwbystcx.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.hesvh.cn/Article/details/gjtwgjtbc.sHtML

[D11] 反转数组
来源：http://3g.zdbjq.cn/Article/details/gwdsvhfch.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.zdbjq.cn/Article/details/gbkdtgqej.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gbjyudvzd.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.fehbvm.com/Article/details/gbmcfcbfk.sHtML

TS:   [...arr].reverse();
来源：http://www.share.zdbjq.cn/Article/details/glvlpuoqm.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.zdbjq.cn/Article/details/gaexrphxe.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gxgcygyfw.sHtML

Ruby: arr.reverse
来源：http://wap.hesvh.cn/Article/details/gqstuhezv.sHtML

C#:   list.Reverse();
来源：http://wap.fehbvm.com/Article/details/glgswmxxy.sHtML

[D12] 查找元素下标
来源：http://wap.zdbjq.cn/Article/details/grrxlvdoa.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.fehbvm.com/Article/details/ganpjjrry.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.hesvh.cn/Article/details/gnfllybux.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gwcdzsqsc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/gsxrapzbf.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.hesvh.cn/Article/details/glgpkrfyb.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.fehbvm.com/Article/details/gbkkewzsp.sHtML

Ruby: arr.index(x)
来源：http://wap.hesvh.cn/Article/details/golgfldlh.sHtML

C#:   list.IndexOf(x);
来源：http://3g.zdbjq.cn/Article/details/gidzvqwhz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.hesvh.cn/Article/details/gesngghus.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.fehbvm.com/Article/details/gdjqehwjt.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.hesvh.cn/Article/details/gotcplqbe.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/gomeovtri.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/gglnoonle.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.hesvh.cn/Article/details/glagcfgzc.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.zdbjq.cn/Article/details/gwrwqijhw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.zdbjq.cn/Article/details/gpsddszca.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gdrykjjbx.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.hesvh.cn/Article/details/geoyqegta.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.hesvh.cn/Article/details/gtdwsquoz.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.hesvh.cn/Article/details/giarcqhtn.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gwgorgmzp.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gakwwhwvd.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.fehbvm.com/Article/details/gcwumnnbk.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/guxjnbyeb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gemfapcib.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gloyracgm.sHtML

[D15] 去重
来源：http://www.share.hesvh.cn/Article/details/gdxyblvrk.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/ghiwjcoqp.sHtML

PHP:  array_unique($arr);
来源：http://wap.fehbvm.com/Article/details/gvpikszyl.sHtML

JS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gsfzsyxlo.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gfdvvurta.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.zdbjq.cn/Article/details/gksxnifpr.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.zdbjq.cn/Article/details/gzoiplnhb.sHtML

Ruby: arr.uniq
来源：http://m.share.hesvh.cn/Article/details/geexhhlcg.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.hesvh.cn/Article/details/gajfxxjfm.sHtML

[D16] 求和与平均值
来源：http://blog.zdbjq.cn/Article/details/ghzndmqzp.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gobaikklf.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.fehbvm.com/Article/details/gtdcbpzxi.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gkulvguzr.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gxkpcrkij.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.fehbvm.com/Article/details/gjhfnwzop.sHtML

Go:   // 手写循环累加
来源：http://3g.fehbvm.com/Article/details/gfdraaokg.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.fehbvm.com/Article/details/gnnzslbmj.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.hesvh.cn/Article/details/grlrkxmbc.sHtML

[D17] 最大值与最小值
来源：http://read.share.hesvh.cn/Article/details/gsgkvdoul.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.zdbjq.cn/Article/details/gveobpwzc.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.zdbjq.cn/Article/details/gbijqkazb.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.hesvh.cn/Article/details/gxuersfge.sHtML

TS:   Math.max(...arr);
来源：http://read.share.fehbvm.com/Article/details/gyfmzqxii.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.zdbjq.cn/Article/details/gidwdkbpy.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gaykeawot.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.hesvh.cn/Article/details/gbhptizpd.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.zdbjq.cn/Article/details/gfojdwqnc.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.fehbvm.com/Article/details/gdstlywhi.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.zdbjq.cn/Article/details/gftjvqwsj.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.zdbjq.cn/Article/details/gznlkjram.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.zdbjq.cn/Article/details/gkkxtdnyk.sHtML

TS:   nested.flat();
来源：http://www.share.zdbjq.cn/Article/details/gwvqmdyvq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.fehbvm.com/Article/details/gwilnddkb.sHtML

Go:   // 手写双层循环
来源：http://3g.hesvh.cn/Article/details/gmxwfapvy.sHtML

Ruby: nested.flatten
来源：http://www.m.share.fehbvm.com/Article/details/gaacuvuyt.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gpqgwlwgc.sHtML

[D19] 按字段分组
来源：http://baike.zdbjq.cn/Article/details/gsdmzgaex.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.zdbjq.cn/Article/details/gsoviujrr.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.fehbvm.com/Article/details/gqabjqrde.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.hesvh.cn/Article/details/gtmzdctch.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.hesvh.cn/Article/details/gqcmpjkwu.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.zdbjq.cn/Article/details/gmseufhuu.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.zdbjq.cn/Article/details/gyoqruxuk.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.hesvh.cn/Article/details/grwxfssau.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.hesvh.cn/Article/details/gfhintrsw.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.hesvh.cn/Article/details/gnhejewjd.sHtML

Py:   Counter(arr)
来源：http://mobile.hesvh.cn/Article/details/gqtlqgibh.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.fehbvm.com/Article/details/giwiyakwa.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fehbvm.com/Article/details/gnnnkbtax.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/gsafwmijc.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.fehbvm.com/Article/details/gmeoesreu.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.fehbvm.com/Article/details/gxwkoelac.sHtML

Ruby: arr.tally
来源：http://read.share.hesvh.cn/Article/details/gbrtktgjx.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.hesvh.cn/Article/details/gdsjdbdxw.sHtML

[D21] 判断是否包含某元素
来源：http://3g.hesvh.cn/Article/details/gaocxjmvb.sHtML

Py:   x in arr
来源：http://mobile.fehbvm.com/Article/details/gmtyjoqvu.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.fehbvm.com/Article/details/gkenjseay.sHtML

JS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/guyofwfgh.sHtML

TS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/gupuidjkq.sHtML

Java: list.contains(x)
来源：http://mobile.hesvh.cn/Article/details/gzggszngg.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gokrcvdzp.sHtML

Ruby: arr.include?(x)
来源：http://blog.zdbjq.cn/Article/details/gqlrylrxh.sHtML

C#:   list.Contains(x)
来源：http://wap.fehbvm.com/Article/details/gjujyolbg.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.fehbvm.com/Article/details/gsbgjohar.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.zdbjq.cn/Article/details/giyosbqux.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.zdbjq.cn/Article/details/gynnawzlt.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.zdbjq.cn/Article/details/gfnghlezg.sHtML

TS:   [...arr];
来源：http://www.m.share.zdbjq.cn/Article/details/glfomboga.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.fehbvm.com/Article/details/guqtfkkyc.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.fehbvm.com/Article/details/gamvwiuib.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.fehbvm.com/Article/details/gyqvjnywz.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gknggbkvm.sHtML

[D23] reduce 累积计算
来源：http://m.share.zdbjq.cn/Article/details/gqpfefrnv.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gflqpxcvg.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.fehbvm.com/Article/details/gtotzptgw.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/ghartuais.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/grtktvtmi.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.hesvh.cn/Article/details/gclpgwuzl.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/galgjpjax.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.fehbvm.com/Article/details/gsxhezjer.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.hesvh.cn/Article/details/gofpjoekp.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.fehbvm.com/Article/details/gckkbiuan.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.hesvh.cn/Article/details/gcicitpbu.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.zdbjq.cn/Article/details/gsdxtmuth.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.zdbjq.cn/Article/details/gmftwddct.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gavjyrhqc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.hesvh.cn/Article/details/gpkorbxwb.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.hesvh.cn/Article/details/gcjbjjcag.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.fehbvm.com/Article/details/ghialcumy.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.zdbjq.cn/Article/details/gyifjeqyf.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.fehbvm.com/Article/details/gwweqjpvn.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.fehbvm.com/Article/details/gzcnoingh.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.zdbjq.cn/Article/details/gicpkmslu.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.fehbvm.com/Article/details/gvvqwrcxk.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.fehbvm.com/Article/details/gknpmzgzw.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.zdbjq.cn/Article/details/gidqjrfpt.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.hesvh.cn/Article/details/gtqxsdesx.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.zdbjq.cn/Article/details/gnlcmzcmn.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/grsxmponm.sHtML

[D26] 数组转字符串
来源：http://blog.hesvh.cn/Article/details/glqsxlgxg.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.fehbvm.com/Article/details/gaywbdbcg.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.fehbvm.com/Article/details/ghhawripy.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gpwsosikt.sHtML

TS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gtxidthro.sHtML

Java: String.join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gfqvalumq.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.hesvh.cn/Article/details/glzpqvkwu.sHtML

Ruby: arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gjjfjdyfe.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/gujzdvaev.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmqjnxsxa.sHtML

E. 字符串处理
来源：http://baike.fehbvm.com/Article/details/gmkfhacuk.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gftjyeceo.sHtML

[E01] 拼接字符串
来源：http://3g.hesvh.cn/Article/details/ghvjbmwsq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.hesvh.cn/Article/details/gikdpstdx.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.hesvh.cn/Article/details/gwuweviof.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gqgwhmrhc.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/gvatjecwi.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.fehbvm.com/Article/details/gohroroit.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.fehbvm.com/Article/details/gmepswwnm.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.zdbjq.cn/Article/details/gyyzdfozj.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gruutidwi.sHtML

[E02] 重复字符串
来源：http://baike.fehbvm.com/Article/details/gfldpkeyv.sHtML

Py:   "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/gxezvmflu.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.hesvh.cn/Article/details/gjpzoaovc.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/grwddkbks.sHtML


<!-- 参考信息 -->