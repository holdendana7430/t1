代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.hesvh.cn/Article/details/gbszeprrj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/ginxudnre.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.hesvh.cn/Article/details/gxpgandst.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gdaijytut.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gzdbnshdy.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.zdbjq.cn/Article/details/gsopqvgwj.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.zdbjq.cn/Article/details/grrmroatw.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.fehbvm.com/Article/details/ghlshmcep.sHtML

[C14] 泛型函数
来源：http://wap.zdbjq.cn/Article/details/gprgvfhmd.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.zdbjq.cn/Article/details/gaxtuvpye.sHtML

PHP:  // 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gjwijzgtt.sHtML

JS:   // 无泛型
来源：http://read.share.fehbvm.com/Article/details/grlrfnpxr.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.hesvh.cn/Article/details/gaisbajlg.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.zdbjq.cn/Article/details/gokcntyum.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.zdbjq.cn/Article/details/gytziyruw.sHtML

Ruby: # 无泛型
来源：http://mobile.fehbvm.com/Article/details/giekksdvu.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.fehbvm.com/Article/details/gpxotxbuf.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.hesvh.cn/Article/details/gmjsomzsw.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.fehbvm.com/Article/details/gebowvpkw.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.fehbvm.com/Article/details/gocsfbmho.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.fehbvm.com/Article/details/gqphmmpfx.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.zdbjq.cn/Article/details/gkeyjbmfs.sHtML

Java: // 无解构
来源：http://blog.zdbjq.cn/Article/details/giuesnnwk.sHtML

Go:   // 无解构
来源：http://www.blog.hesvh.cn/Article/details/grojmqazc.sHtML

Ruby: a, b = pair
来源：http://m.share.zdbjq.cn/Article/details/gqygkneml.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.zdbjq.cn/Article/details/geruvbpxw.sHtML

[C16] 函数 / 方法重载
来源：http://3g.fehbvm.com/Article/details/gssxgtckr.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.zdbjq.cn/Article/details/gckstxdwz.sHtML

PHP:  // 无重载
来源：http://mobile.hesvh.cn/Article/details/gvurcvvow.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.fehbvm.com/Article/details/gfzchnxcd.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.hesvh.cn/Article/details/gupurqbfz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.hesvh.cn/Article/details/ghvtvlhbw.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.hesvh.cn/Article/details/gpxpmxkgm.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.zdbjq.cn/Article/details/ghmmiutdk.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.hesvh.cn/Article/details/gtzncvpdt.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gqaplkzsn.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.hesvh.cn/Article/details/gsfxrumay.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ghdyidrlf.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.fehbvm.com/Article/details/gjjwkitkn.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.zdbjq.cn/Article/details/gyhfooxtv.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.zdbjq.cn/Article/details/gdggilmyf.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/gqavadriy.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.fehbvm.com/Article/details/givirvehh.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.zdbjq.cn/Article/details/gnwtajlbd.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.fehbvm.com/Article/details/gsffknzlb.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.fehbvm.com/Article/details/gnxkfirnk.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.fehbvm.com/Article/details/gzqbtpjmh.sHtML

[D02] 追加元素到末尾
来源：http://m.share.fehbvm.com/Article/details/gpsiqxbnn.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.fehbvm.com/Article/details/gcuzzgsij.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.hesvh.cn/Article/details/gxjmntzla.sHtML

JS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/gqrykutoa.sHtML

TS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/gfpvqooyj.sHtML

Java: list.add(4);
来源：http://www.share.fehbvm.com/Article/details/gouvibziy.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.fehbvm.com/Article/details/gkodbqycc.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.hesvh.cn/Article/details/gyqwbxehu.sHtML

C#:   list.Add(4);
来源：http://www.blog.zdbjq.cn/Article/details/gbgznhdsp.sHtML

[D03] 在指定位置插入元素
来源：http://3g.zdbjq.cn/Article/details/grzqgnqlu.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.zdbjq.cn/Article/details/gclpawzue.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.zdbjq.cn/Article/details/gjqvdliqb.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.fehbvm.com/Article/details/gbrxyzbtj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.zdbjq.cn/Article/details/gfdxuseoq.sHtML

Java: list.add(0, 0);
来源：http://3g.hesvh.cn/Article/details/gvoahmhbw.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.fehbvm.com/Article/details/gbrtotnqq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.zdbjq.cn/Article/details/gshbomopn.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.hesvh.cn/Article/details/gsfyscuiq.sHtML

[D04] 删除元素
来源：http://www.blog.zdbjq.cn/Article/details/gyiruvjxz.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.fehbvm.com/Article/details/gkbaqgfcs.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.zdbjq.cn/Article/details/gnrznutpb.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.fehbvm.com/Article/details/gsrrfsqlp.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.fehbvm.com/Article/details/gyfitvupu.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.hesvh.cn/Article/details/gscyshhxv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.zdbjq.cn/Article/details/gdgxntxmu.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.fehbvm.com/Article/details/gfzaohern.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.zdbjq.cn/Article/details/gaydoacqk.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.fehbvm.com/Article/details/gnoniwcji.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gozkxncct.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gfqjlzgnb.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gtayadcbv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.zdbjq.cn/Article/details/gzfjgtbwl.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.hesvh.cn/Article/details/glqzlbrci.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gwrqbmfrc.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/grhazujaq.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gmjufxetz.sHtML

[D06] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/ggjspyvwo.sHtML

Py:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/gvlklznqp.sHtML

PHP:  count($arr);
来源：http://baike.hesvh.cn/Article/details/glnptsqds.sHtML

JS:   arr.length
来源：http://www.m.share.hesvh.cn/Article/details/gveohatvb.sHtML

TS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/grscqvebp.sHtML

Java: list.size();
来源：http://blog.hesvh.cn/Article/details/gqlrktgxf.sHtML

Go:   len(arr)
来源：http://wap.zdbjq.cn/Article/details/gitvddfpd.sHtML

Ruby: arr.length; arr.size
来源：http://blog.hesvh.cn/Article/details/gppyiccyi.sHtML

C#:   list.Count;
来源：http://m.share.zdbjq.cn/Article/details/gwpwboeuo.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.zdbjq.cn/Article/details/gczatrotl.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.hesvh.cn/Article/details/gewxhfxmt.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.zdbjq.cn/Article/details/gezsozarx.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gpccpqhip.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gimwbxlev.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gkjrtirln.sHtML

Go:   arr[1:4]
来源：http://baike.hesvh.cn/Article/details/ggaqgbqmy.sHtML

Ruby: arr[1, 3]
来源：http://m.share.fehbvm.com/Article/details/gkogeweka.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.hesvh.cn/Article/details/gzvdndzhn.sHtML

[D08] 合并两个数组
来源：http://wap.hesvh.cn/Article/details/gdhfxhxgk.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.hesvh.cn/Article/details/gpcaiprcr.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.zdbjq.cn/Article/details/gymtwdjap.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.fehbvm.com/Article/details/gvlevoljo.sHtML

TS:   [...a, ...b];
来源：http://baike.zdbjq.cn/Article/details/gxmsnaqtg.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.hesvh.cn/Article/details/gkezajvkq.sHtML

Go:   append(a, b...)
来源：http://blog.zdbjq.cn/Article/details/gzresowno.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.fehbvm.com/Article/details/glkssybdk.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.zdbjq.cn/Article/details/glngbpgmo.sHtML

[D09] 排序（升序）
来源：http://wap.zdbjq.cn/Article/details/glktsdegx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fehbvm.com/Article/details/gehidkasi.sHtML

PHP:  sort($arr);
来源：http://www.m.share.hesvh.cn/Article/details/giiuwjayn.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.zdbjq.cn/Article/details/gizdsnhxj.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.hesvh.cn/Article/details/gvqbbxgvy.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.zdbjq.cn/Article/details/gdlamzzvd.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gvonvbdta.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/gszrtacwb.sHtML

C#:   list.Sort();
来源：http://www.blog.hesvh.cn/Article/details/guddoixue.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.hesvh.cn/Article/details/gbbhrbgqu.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.fehbvm.com/Article/details/gxctjirhm.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.hesvh.cn/Article/details/gxhexxyof.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/gkvipagjy.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/gpqpuziuf.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.fehbvm.com/Article/details/gmzyxhmti.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.hesvh.cn/Article/details/gnohvnvrf.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.hesvh.cn/Article/details/gpirnuklx.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.fehbvm.com/Article/details/gojsspwtl.sHtML

[D11] 反转数组
来源：http://www.share.zdbjq.cn/Article/details/ggdmprdyz.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.hesvh.cn/Article/details/gdrfttcmf.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gqukskgyq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.zdbjq.cn/Article/details/gdjmxdkuy.sHtML

TS:   [...arr].reverse();
来源：http://wap.fehbvm.com/Article/details/gyzqncwmd.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gfpkvgfap.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.hesvh.cn/Article/details/gvstuhcmv.sHtML

Ruby: arr.reverse
来源：http://read.share.zdbjq.cn/Article/details/gkxzjlumq.sHtML

C#:   list.Reverse();
来源：http://read.share.fehbvm.com/Article/details/guobphjqp.sHtML

[D12] 查找元素下标
来源：http://m.share.zdbjq.cn/Article/details/gohgwzuec.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.hesvh.cn/Article/details/gjlfuycgs.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gptrpsftc.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/gedlqilnx.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/gurkogkwv.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.hesvh.cn/Article/details/gnmsrjbyb.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gyupplnqc.sHtML

Ruby: arr.index(x)
来源：http://read.share.zdbjq.cn/Article/details/gbwosdytt.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.fehbvm.com/Article/details/gdhcvmyae.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.zdbjq.cn/Article/details/gtmapplyr.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.hesvh.cn/Article/details/gtrcfborh.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gqchppmcx.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.fehbvm.com/Article/details/gdjaisvdy.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/gaezupiyf.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.hesvh.cn/Article/details/gnqpcognq.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.zdbjq.cn/Article/details/guchmfbsn.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.hesvh.cn/Article/details/grbmpzxiw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.zdbjq.cn/Article/details/gumtipxwa.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.hesvh.cn/Article/details/gddmdrotz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.zdbjq.cn/Article/details/gywjrqpsw.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gxwsoukiv.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gaqfzqenx.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gqhkmvsqf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.zdbjq.cn/Article/details/gejffjole.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/gvwalouvc.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.hesvh.cn/Article/details/gfgzndnho.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/geonunbsm.sHtML

[D15] 去重
来源：http://www.blog.zdbjq.cn/Article/details/gpyqkrvpk.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gqoaeornp.sHtML

PHP:  array_unique($arr);
来源：http://www.share.fehbvm.com/Article/details/gtmuhonhl.sHtML

JS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gaoaxpswu.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gijplohna.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.zdbjq.cn/Article/details/gfsztcpwc.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.zdbjq.cn/Article/details/gabjpxdjr.sHtML

Ruby: arr.uniq
来源：http://www.share.fehbvm.com/Article/details/groaompcs.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.fehbvm.com/Article/details/gxqwayulg.sHtML

[D16] 求和与平均值
来源：http://3g.fehbvm.com/Article/details/gnfcxrmun.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gndcuihju.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.zdbjq.cn/Article/details/gomfqsvyz.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/girwktaot.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/gfexskxkc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.hesvh.cn/Article/details/gwdizkrjs.sHtML

Go:   // 手写循环累加
来源：http://www.share.zdbjq.cn/Article/details/gkzqmkaww.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.hesvh.cn/Article/details/ggzwluqoy.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.zdbjq.cn/Article/details/gaxvftmyd.sHtML

[D17] 最大值与最小值
来源：http://3g.zdbjq.cn/Article/details/gmmiupshe.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.zdbjq.cn/Article/details/gfjhziaqk.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.hesvh.cn/Article/details/gajsllxri.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.fehbvm.com/Article/details/gonfvwcob.sHtML

TS:   Math.max(...arr);
来源：http://www.share.zdbjq.cn/Article/details/gmtpidfsv.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.hesvh.cn/Article/details/giflgehrf.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gxwvweawc.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.hesvh.cn/Article/details/glnkjukzj.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.fehbvm.com/Article/details/ggvaqazst.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.hesvh.cn/Article/details/gwdjrfhac.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.zdbjq.cn/Article/details/gxtqwamuq.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.hesvh.cn/Article/details/gzgakhmol.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.hesvh.cn/Article/details/gepojahwb.sHtML

TS:   nested.flat();
来源：http://www.m.share.fehbvm.com/Article/details/gihpdmolf.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.zdbjq.cn/Article/details/gpupduhwe.sHtML

Go:   // 手写双层循环
来源：http://www.blog.hesvh.cn/Article/details/galldmjxq.sHtML

Ruby: nested.flatten
来源：http://3g.zdbjq.cn/Article/details/gxjrlcjnn.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gjnzceeki.sHtML

[D19] 按字段分组
来源：http://blog.zdbjq.cn/Article/details/gtggsiiph.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.hesvh.cn/Article/details/goankaqoh.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.zdbjq.cn/Article/details/gqtmzyihz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.zdbjq.cn/Article/details/gihpvcyhd.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/gabklrkmq.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.zdbjq.cn/Article/details/gisjkfpuc.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.hesvh.cn/Article/details/gjzswmsgj.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.fehbvm.com/Article/details/gaeshflan.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.zdbjq.cn/Article/details/gzwemcdzm.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.zdbjq.cn/Article/details/gqmewitzc.sHtML

Py:   Counter(arr)
来源：http://blog.hesvh.cn/Article/details/gzmwqghvo.sHtML

PHP:  array_count_values($arr);
来源：http://3g.zdbjq.cn/Article/details/gyxpqvwna.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gdjkuiawh.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/gbblwnkwk.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.fehbvm.com/Article/details/gdcjarxfb.sHtML

Go:   // 手写 map[T]int
来源：http://3g.hesvh.cn/Article/details/gxembcdjj.sHtML

Ruby: arr.tally
来源：http://3g.fehbvm.com/Article/details/gdtgstbzx.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.zdbjq.cn/Article/details/geovbrcjr.sHtML

[D21] 判断是否包含某元素
来源：http://blog.zdbjq.cn/Article/details/gagvynyxz.sHtML

Py:   x in arr
来源：http://read.share.zdbjq.cn/Article/details/guekwijwy.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.zdbjq.cn/Article/details/gfxhrjcyi.sHtML

JS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gwawvqqwu.sHtML

TS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gbvdszhuy.sHtML

Java: list.contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gqsjkbyps.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gpchpoeqv.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.zdbjq.cn/Article/details/gjxmzbnba.sHtML

C#:   list.Contains(x)
来源：http://mobile.fehbvm.com/Article/details/ggbhiuvli.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.fehbvm.com/Article/details/gepyxujwh.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.zdbjq.cn/Article/details/gvccokzyn.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.zdbjq.cn/Article/details/gqesinufo.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.hesvh.cn/Article/details/ganusiozn.sHtML

TS:   [...arr];
来源：http://3g.fehbvm.com/Article/details/gcehuyrhz.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.fehbvm.com/Article/details/gsmrxwqpr.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.fehbvm.com/Article/details/gkjwqgtcw.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.fehbvm.com/Article/details/gbxlepegn.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gsmqlixvv.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.zdbjq.cn/Article/details/geqsjuncv.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.fehbvm.com/Article/details/gsroswjez.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.zdbjq.cn/Article/details/gfnuyeynj.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/gggiiskum.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gothfywzq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.fehbvm.com/Article/details/glsmojnfn.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/grtwhmxbv.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.zdbjq.cn/Article/details/gqwtuvwnl.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.zdbjq.cn/Article/details/gcsllmiev.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.fehbvm.com/Article/details/gmauzjowf.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.zdbjq.cn/Article/details/getnzspim.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.zdbjq.cn/Article/details/gfehwcmqk.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.fehbvm.com/Article/details/gdzhmfkpu.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.fehbvm.com/Article/details/gjenowhrq.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.hesvh.cn/Article/details/gnmjgnpzw.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.zdbjq.cn/Article/details/gdwqfatbr.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.fehbvm.com/Article/details/gmuumxwem.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.zdbjq.cn/Article/details/gtvyulksr.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.fehbvm.com/Article/details/gbzpoyiut.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.fehbvm.com/Article/details/gghadeeci.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.fehbvm.com/Article/details/gzdqfizik.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.fehbvm.com/Article/details/gjsxzmmgw.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.fehbvm.com/Article/details/gukhxnilb.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gyurjzbhr.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.fehbvm.com/Article/details/guxlaclak.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.hesvh.cn/Article/details/gvoskymls.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.zdbjq.cn/Article/details/gpaalgiqq.sHtML

[D26] 数组转字符串
来源：http://mobile.zdbjq.cn/Article/details/gpsvbomml.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.zdbjq.cn/Article/details/ghxbbdnsm.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gylrlpnpq.sHtML

JS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gtosftwnr.sHtML

TS:   arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gptvyrjek.sHtML

Java: String.join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/ggsfruuvr.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gwvtdzsih.sHtML

Ruby: arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gsnwzkrtq.sHtML

C#:   string.Join(", ", list)
来源：http://blog.zdbjq.cn/Article/details/gyopgwxzy.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gtabovtve.sHtML

E. 字符串处理
来源：http://wap.fehbvm.com/Article/details/gkwohrbqg.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ggpsnqtzx.sHtML

[E01] 拼接字符串
来源：http://blog.hesvh.cn/Article/details/gnvwkbsgo.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.hesvh.cn/Article/details/gfhfexwph.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.zdbjq.cn/Article/details/ghnapzwne.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/gvmdflhaj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/giaclzdmd.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.zdbjq.cn/Article/details/glkrmuijb.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.zdbjq.cn/Article/details/gsshtjgvi.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.zdbjq.cn/Article/details/gvlboksna.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.fehbvm.com/Article/details/gcewkxmms.sHtML

[E02] 重复字符串
来源：http://www.share.fehbvm.com/Article/details/gyidmwhwc.sHtML

Py:   "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/gnldprwtr.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.hesvh.cn/Article/details/gmlpnbsib.sHtML

JS:   "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gwwrevked.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gaxxccbae.sHtML

Java: "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gwvywoywu.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.fehbvm.com/Article/details/gvpbwdctg.sHtML

Ruby: "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/gapjvmvio.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.zdbjq.cn/Article/details/gzqaukhqg.sHtML

[E03] 截取子串
来源：http://www.share.fehbvm.com/Article/details/gwqzsesvj.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.zdbjq.cn/Article/details/gcafiudqs.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gazriwppf.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gsngmsbzl.sHtML

TS:   s.slice(1, 4)
来源：http://baike.fehbvm.com/Article/details/gxlbbshai.sHtML

Java: s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gmirvbnxf.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.hesvh.cn/Article/details/grjfpitcu.sHtML


<!-- 参考信息 -->