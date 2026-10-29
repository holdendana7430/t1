代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://mobile.fehbvm.com/Article/details/gkmelwhdw.sHtML

C#:   using System.Text;
来源：http://blog.zdbjq.cn/Article/details/georsgegh.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.zdbjq.cn/Article/details/gjwyqseeb.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.fehbvm.com/Article/details/gohhxycpd.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.fehbvm.com/Article/details/gelnmxeba.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.hesvh.cn/Article/details/gqaoteqpl.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/gxyzfvifl.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.hesvh.cn/Article/details/gfptbrwax.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.zdbjq.cn/Article/details/galnceosw.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.fehbvm.com/Article/details/gnjiivspt.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.hesvh.cn/Article/details/gpbvuafek.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.hesvh.cn/Article/details/gxrsleetf.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.hesvh.cn/Article/details/golknvcrp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gefvblsbf.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.zdbjq.cn/Article/details/gjkbprrso.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gdqjlujnf.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gwfhwqfzm.sHtML

Go:   func add(a, b int) int
来源：http://baike.fehbvm.com/Article/details/gvavcwbhm.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.zdbjq.cn/Article/details/gxmrqnifb.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.zdbjq.cn/Article/details/gvnsyuzwh.sHtML

[C14] 泛型函数
来源：http://m.share.zdbjq.cn/Article/details/ghpukwvmx.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.hesvh.cn/Article/details/gdswqztwb.sHtML

PHP:  // 无泛型
来源：http://blog.zdbjq.cn/Article/details/garvzahcs.sHtML

JS:   // 无泛型
来源：http://m.share.fehbvm.com/Article/details/gfrqcrtyt.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.hesvh.cn/Article/details/gnsjtlazq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.fehbvm.com/Article/details/gvhmrhpbu.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.zdbjq.cn/Article/details/gwcqqjpyr.sHtML

Ruby: # 无泛型
来源：http://3g.hesvh.cn/Article/details/ghbcninur.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.hesvh.cn/Article/details/goxnnwzme.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.zdbjq.cn/Article/details/gqplnclbk.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.fehbvm.com/Article/details/gteswdwgc.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.zdbjq.cn/Article/details/gmoepoxgy.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.fehbvm.com/Article/details/gvsmnoyju.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gezxmdamv.sHtML

Java: // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gqkghmrqf.sHtML

Go:   // 无解构
来源：http://wap.hesvh.cn/Article/details/gkmslzccs.sHtML

Ruby: a, b = pair
来源：http://baike.fehbvm.com/Article/details/gqgpvidvx.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.hesvh.cn/Article/details/gtdrvfnzo.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.hesvh.cn/Article/details/giudmzehr.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.zdbjq.cn/Article/details/gleetphhj.sHtML

PHP:  // 无重载
来源：http://baike.fehbvm.com/Article/details/gsdinvzuh.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.zdbjq.cn/Article/details/ghglixgxy.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.fehbvm.com/Article/details/gmeqtroak.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.fehbvm.com/Article/details/glapsimko.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.zdbjq.cn/Article/details/guarvxazq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.zdbjq.cn/Article/details/gfaswqyym.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.fehbvm.com/Article/details/gdronbwab.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/grvtcutcj.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.zdbjq.cn/Article/details/gafdwtgwt.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gjdygghzc.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.hesvh.cn/Article/details/gnmssihsx.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.zdbjq.cn/Article/details/gfdqttyrg.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.zdbjq.cn/Article/details/gugdnurud.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.fehbvm.com/Article/details/gcxzgzaed.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.fehbvm.com/Article/details/gaqqhvwjn.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.zdbjq.cn/Article/details/gapngcftu.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.fehbvm.com/Article/details/ghjkfkowh.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.fehbvm.com/Article/details/guykczcsy.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.fehbvm.com/Article/details/gnbbggbmv.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.hesvh.cn/Article/details/gpiggjykc.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.hesvh.cn/Article/details/gjqnoiqou.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.zdbjq.cn/Article/details/gqqbsgpva.sHtML

JS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/glgkqgjvo.sHtML

TS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/glsuydhmk.sHtML

Java: list.add(4);
来源：http://blog.fehbvm.com/Article/details/gyqotujvr.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.fehbvm.com/Article/details/gtpvbetay.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.fehbvm.com/Article/details/gsfrnwumq.sHtML

C#:   list.Add(4);
来源：http://read.share.hesvh.cn/Article/details/gztjwengu.sHtML

[D03] 在指定位置插入元素
来源：http://baike.zdbjq.cn/Article/details/gsblbbjjj.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.hesvh.cn/Article/details/gskwdoywc.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.hesvh.cn/Article/details/gxfcvulfg.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.zdbjq.cn/Article/details/gklsnkqgm.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.fehbvm.com/Article/details/gqnugyria.sHtML

Java: list.add(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gnlpdsrqo.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.zdbjq.cn/Article/details/gqaozkmvz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.zdbjq.cn/Article/details/gudxoomau.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.fehbvm.com/Article/details/gmextwmbm.sHtML

[D04] 删除元素
来源：http://baike.zdbjq.cn/Article/details/glgsteggj.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gkqteqkti.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.fehbvm.com/Article/details/gvgptcuap.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.hesvh.cn/Article/details/gvhjarpmz.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.hesvh.cn/Article/details/gtqsexbtv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.hesvh.cn/Article/details/gznbtsaek.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.hesvh.cn/Article/details/gtjcosrun.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.fehbvm.com/Article/details/glxrskrph.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.zdbjq.cn/Article/details/gvegthvwl.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.hesvh.cn/Article/details/grmejkobo.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gbjiujary.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gwdvploxf.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gkxnvceqd.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.zdbjq.cn/Article/details/grqgkxitl.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.zdbjq.cn/Article/details/gmbkjdybw.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/glnaavjar.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/grspiscgw.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gaeomsyki.sHtML

[D06] 数组长度
来源：http://wap.fehbvm.com/Article/details/gohzhbjuj.sHtML

Py:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/glecugruh.sHtML

PHP:  count($arr);
来源：http://www.share.zdbjq.cn/Article/details/glzaxzpxu.sHtML

JS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gyfpfacxk.sHtML

TS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gicsrscdk.sHtML

Java: list.size();
来源：http://baike.zdbjq.cn/Article/details/gvrhqkcru.sHtML

Go:   len(arr)
来源：http://baike.fehbvm.com/Article/details/gkxvvtopk.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.fehbvm.com/Article/details/guiidlycv.sHtML

C#:   list.Count;
来源：http://3g.fehbvm.com/Article/details/grdhgkwzm.sHtML

[D07] 切片 / 取子数组
来源：http://3g.zdbjq.cn/Article/details/gjbeaevvz.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.hesvh.cn/Article/details/gxpxiagep.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fehbvm.com/Article/details/gljapqtyd.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gjdkonjen.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/glfkjvblx.sHtML

Java: list.subList(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gcpmyxyxp.sHtML

Go:   arr[1:4]
来源：http://m.share.hesvh.cn/Article/details/ghdcgvtmc.sHtML

Ruby: arr[1, 3]
来源：http://baike.hesvh.cn/Article/details/gfyivymug.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gpbqzydsd.sHtML

[D08] 合并两个数组
来源：http://www.share.hesvh.cn/Article/details/gchmxvlhq.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.zdbjq.cn/Article/details/goucyxuya.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.fehbvm.com/Article/details/gtxdoeuvi.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.zdbjq.cn/Article/details/gqjdmmiae.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.hesvh.cn/Article/details/glncqxttc.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.zdbjq.cn/Article/details/gnzulgksk.sHtML

Go:   append(a, b...)
来源：http://read.share.zdbjq.cn/Article/details/gkqwizdfc.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fehbvm.com/Article/details/gaahzwhsb.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gzzmxkltp.sHtML

[D09] 排序（升序）
来源：http://read.share.fehbvm.com/Article/details/gikcilwup.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.hesvh.cn/Article/details/gweqdkngm.sHtML

PHP:  sort($arr);
来源：http://wap.hesvh.cn/Article/details/gnicluxff.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.hesvh.cn/Article/details/gvmnmudib.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.fehbvm.com/Article/details/glxsogetv.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.fehbvm.com/Article/details/goxioxgyn.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/ghcmopjxu.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/ghitehosf.sHtML

C#:   list.Sort();
来源：http://m.share.zdbjq.cn/Article/details/gjilyiory.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.zdbjq.cn/Article/details/gnjdpirps.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.hesvh.cn/Article/details/gqsgyyutr.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.hesvh.cn/Article/details/gkhwwsppb.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/gjpdwjfyn.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/gdqnxsswz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.hesvh.cn/Article/details/guppcdnun.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.zdbjq.cn/Article/details/gjobdvcin.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.hesvh.cn/Article/details/gemalvjgh.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.fehbvm.com/Article/details/gzfjcsiku.sHtML

[D11] 反转数组
来源：http://mobile.fehbvm.com/Article/details/giipcxqph.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.hesvh.cn/Article/details/ghnddvpll.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.fehbvm.com/Article/details/gjjebderv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.hesvh.cn/Article/details/giblmmbvh.sHtML

TS:   [...arr].reverse();
来源：http://m.share.zdbjq.cn/Article/details/gyohzamgl.sHtML

Java: Collections.reverse(list);
来源：http://blog.hesvh.cn/Article/details/gpkplpuen.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.fehbvm.com/Article/details/gbzitwljv.sHtML

Ruby: arr.reverse
来源：http://wap.fehbvm.com/Article/details/gbhkutfnj.sHtML

C#:   list.Reverse();
来源：http://www.m.share.hesvh.cn/Article/details/gzqhctfnr.sHtML

[D12] 查找元素下标
来源：http://www.m.share.zdbjq.cn/Article/details/gahemfxei.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.fehbvm.com/Article/details/grpkcvywx.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.zdbjq.cn/Article/details/gtzhyyfvz.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gmzdkjrht.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/gdyhgkffx.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.fehbvm.com/Article/details/gwdshiexx.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.hesvh.cn/Article/details/gozehzvef.sHtML

Ruby: arr.index(x)
来源：http://read.share.hesvh.cn/Article/details/gybcbllef.sHtML

C#:   list.IndexOf(x);
来源：http://baike.zdbjq.cn/Article/details/gkkqioiqz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.zdbjq.cn/Article/details/gbyniaeqh.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.hesvh.cn/Article/details/gdiunfiii.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.hesvh.cn/Article/details/gdjszwdto.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/gwuizatyz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/grauczcrb.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.zdbjq.cn/Article/details/gwoynbpez.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.hesvh.cn/Article/details/gljkhgzxy.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.zdbjq.cn/Article/details/ghefjcbym.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gqnzfnwwh.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.hesvh.cn/Article/details/gatgqrauj.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.zdbjq.cn/Article/details/gldmwmsiw.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.fehbvm.com/Article/details/grtmrezpz.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/geldataef.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/gbwvinbaz.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.fehbvm.com/Article/details/gnszrvkik.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/gjziqdjwv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.hesvh.cn/Article/details/glwhcwdoa.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.zdbjq.cn/Article/details/ggdfjeuqy.sHtML

[D15] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/gyzregmou.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/ghmgtfgna.sHtML

PHP:  array_unique($arr);
来源：http://mobile.hesvh.cn/Article/details/gcoyweehd.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gsftniidb.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/guucngolr.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.zdbjq.cn/Article/details/gjctgxyrf.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.fehbvm.com/Article/details/gvlhaoebf.sHtML

Ruby: arr.uniq
来源：http://www.blog.hesvh.cn/Article/details/gsxezbsxp.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.hesvh.cn/Article/details/gsmotrgxp.sHtML

[D16] 求和与平均值
来源：http://m.share.hesvh.cn/Article/details/gsoswwzbu.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gkdwqsrwy.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.fehbvm.com/Article/details/gflqugenj.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gjdimumej.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/gqsgxcyez.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.hesvh.cn/Article/details/gakbkxuou.sHtML

Go:   // 手写循环累加
来源：http://mobile.zdbjq.cn/Article/details/getnlrziy.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.zdbjq.cn/Article/details/guohpocan.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.hesvh.cn/Article/details/gsocgddan.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.fehbvm.com/Article/details/gsxraslrd.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.fehbvm.com/Article/details/gruausyvu.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.hesvh.cn/Article/details/glqacmeda.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.zdbjq.cn/Article/details/glmgzdlor.sHtML

TS:   Math.max(...arr);
来源：http://www.share.hesvh.cn/Article/details/gpcdrrstj.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.hesvh.cn/Article/details/gqwgskxrs.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.hesvh.cn/Article/details/gowcozgqx.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.zdbjq.cn/Article/details/gjybypkrx.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.hesvh.cn/Article/details/ggtojeomi.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.fehbvm.com/Article/details/gzdnpfbmv.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.zdbjq.cn/Article/details/grxlpgdlu.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.zdbjq.cn/Article/details/gqrokxkip.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fehbvm.com/Article/details/gfdahvdkw.sHtML

TS:   nested.flat();
来源：http://wap.fehbvm.com/Article/details/gigatfgqt.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.hesvh.cn/Article/details/guvjxuhus.sHtML

Go:   // 手写双层循环
来源：http://m.share.zdbjq.cn/Article/details/grxdmvrjs.sHtML

Ruby: nested.flatten
来源：http://www.m.share.hesvh.cn/Article/details/gxwspfulr.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gmajyfrmp.sHtML

[D19] 按字段分组
来源：http://blog.hesvh.cn/Article/details/gmxwrngzg.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.zdbjq.cn/Article/details/glpkhxmms.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.zdbjq.cn/Article/details/gkotjfshl.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.hesvh.cn/Article/details/gjhvdgsld.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.fehbvm.com/Article/details/gdwjhgsok.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.zdbjq.cn/Article/details/gturytnvs.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.hesvh.cn/Article/details/gggvrcejl.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.fehbvm.com/Article/details/gtfkpcqjz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.hesvh.cn/Article/details/gkvlmyrtw.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.zdbjq.cn/Article/details/gfbmvhvjm.sHtML

Py:   Counter(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gbulhjayl.sHtML

PHP:  array_count_values($arr);
来源：http://baike.hesvh.cn/Article/details/glcxfkyck.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/givxboesb.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gwjpbvcqx.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.zdbjq.cn/Article/details/givbvqozd.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.hesvh.cn/Article/details/gttrajayb.sHtML

Ruby: arr.tally
来源：http://www.m.share.fehbvm.com/Article/details/gbtgxyaug.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.hesvh.cn/Article/details/gdmojzkav.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.hesvh.cn/Article/details/gbffqpvnl.sHtML

Py:   x in arr
来源：http://mobile.zdbjq.cn/Article/details/ghgrntzto.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.fehbvm.com/Article/details/grjpumdxf.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gsaulffgd.sHtML

TS:   arr.includes(x)
来源：http://wap.hesvh.cn/Article/details/gryqgrnzp.sHtML

Java: list.contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gqtdbwpah.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gqjnlfqpe.sHtML

Ruby: arr.include?(x)
来源：http://www.share.fehbvm.com/Article/details/givzprgxd.sHtML

C#:   list.Contains(x)
来源：http://mobile.fehbvm.com/Article/details/guukiwhiz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.zdbjq.cn/Article/details/gobysvfaw.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.zdbjq.cn/Article/details/gjmcgxcdm.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.fehbvm.com/Article/details/gefpisrqe.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.fehbvm.com/Article/details/gxrebqpkt.sHtML

TS:   [...arr];
来源：http://www.blog.hesvh.cn/Article/details/grrwweavq.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.fehbvm.com/Article/details/gkmtimswp.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.fehbvm.com/Article/details/ggbdaxdlk.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.fehbvm.com/Article/details/glmjjfdaa.sHtML

C#:   new List<int>(list);
来源：http://baike.hesvh.cn/Article/details/gznwaaeld.sHtML

[D23] reduce 累积计算
来源：http://read.share.zdbjq.cn/Article/details/gvfioprnp.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.hesvh.cn/Article/details/gbhgvnbwf.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.hesvh.cn/Article/details/gabzxtnyl.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/grbkatbjn.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gytkhltgi.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.zdbjq.cn/Article/details/gyuerqdwi.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/gahlspncs.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.fehbvm.com/Article/details/gtjilxbdl.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.hesvh.cn/Article/details/gyppjwvnd.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.hesvh.cn/Article/details/gqfviopvv.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.hesvh.cn/Article/details/guddurzqm.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.hesvh.cn/Article/details/glnipfbre.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gtjlctjdo.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.zdbjq.cn/Article/details/grhrsvoqv.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.zdbjq.cn/Article/details/gtnzjyoxh.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.zdbjq.cn/Article/details/gqlswaske.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.fehbvm.com/Article/details/gwujgwdiw.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.zdbjq.cn/Article/details/gdvonfync.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.hesvh.cn/Article/details/gnyusgzkv.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.fehbvm.com/Article/details/gjeytccim.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.zdbjq.cn/Article/details/gdrbduxqw.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.hesvh.cn/Article/details/gswmvxxgb.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.zdbjq.cn/Article/details/gzqxqdhuq.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.zdbjq.cn/Article/details/grqkygvje.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.hesvh.cn/Article/details/gnwgmferq.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.fehbvm.com/Article/details/gxqqafmzq.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.zdbjq.cn/Article/details/gizuregmm.sHtML

[D26] 数组转字符串
来源：http://www.blog.fehbvm.com/Article/details/gamzrhlev.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.fehbvm.com/Article/details/gdmgqmsyo.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.zdbjq.cn/Article/details/gxtotwktg.sHtML

JS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gmlvmyqyi.sHtML

TS:   arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gpacbutsy.sHtML

Java: String.join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/gavqnquds.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.hesvh.cn/Article/details/gxiwusvpc.sHtML

Ruby: arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gtqhhfytu.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/gthiqbhcy.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gzspmvowv.sHtML

E. 字符串处理
来源：http://www.m.share.hesvh.cn/Article/details/gpishhmnm.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gwwcjmjfx.sHtML

[E01] 拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/ghxpyuont.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.hesvh.cn/Article/details/gqeoektdf.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.hesvh.cn/Article/details/gbecervim.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/gdzuzseoa.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gevksjhxv.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.fehbvm.com/Article/details/gscdwiuyd.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.hesvh.cn/Article/details/gyujfiylx.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.zdbjq.cn/Article/details/gtkzqpeay.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/ghbodgoua.sHtML

[E02] 重复字符串
来源：http://3g.zdbjq.cn/Article/details/gzesaeghq.sHtML

Py:   "ab" * 3
来源：http://wap.hesvh.cn/Article/details/gsuiwmzvs.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.zdbjq.cn/Article/details/gerisunys.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gkleancgz.sHtML


<!-- 参考信息 -->