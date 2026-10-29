代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.hesvh.cn/Article/details/gbdjygivd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/grejszaay.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.hesvh.cn/Article/details/grfgisxen.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gntuxeqqp.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gptvozjlr.sHtML

Go:   func add(a, b int) int
来源：http://wap.fehbvm.com/Article/details/gkcupgyrb.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.fehbvm.com/Article/details/gdsevdcrd.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.hesvh.cn/Article/details/gaugrsqow.sHtML

[C14] 泛型函数
来源：http://www.share.fehbvm.com/Article/details/gbcrnyhyf.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.fehbvm.com/Article/details/gqtqcxdgs.sHtML

PHP:  // 无泛型
来源：http://www.share.zdbjq.cn/Article/details/gpgrfpiif.sHtML

JS:   // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gpmnuxhhi.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.hesvh.cn/Article/details/gagnjyczl.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.zdbjq.cn/Article/details/gniwrilid.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.hesvh.cn/Article/details/gckfrkear.sHtML

Ruby: # 无泛型
来源：http://wap.fehbvm.com/Article/details/gvhhanzye.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.hesvh.cn/Article/details/ggxkjuhsb.sHtML

[C15] 解构 / 展开参数
来源：http://3g.fehbvm.com/Article/details/gbhdszzze.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.zdbjq.cn/Article/details/gzewurxlt.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.fehbvm.com/Article/details/gphodagzy.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/gjlfhkpeo.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqwmocxdk.sHtML

Java: // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/guaccuydk.sHtML

Go:   // 无解构
来源：http://www.m.share.zdbjq.cn/Article/details/gufdjjepw.sHtML

Ruby: a, b = pair
来源：http://www.m.share.fehbvm.com/Article/details/gfsngnywh.sHtML

C#:   var (a, b) = pair;
来源：http://3g.zdbjq.cn/Article/details/gigauxpse.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.hesvh.cn/Article/details/gjpbhkywm.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.fehbvm.com/Article/details/grdgjhfhp.sHtML

PHP:  // 无重载
来源：http://read.share.hesvh.cn/Article/details/gcxgqcmmf.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.zdbjq.cn/Article/details/gaxdgtgny.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.hesvh.cn/Article/details/gmwfnvfmr.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.hesvh.cn/Article/details/gdsfayaya.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.zdbjq.cn/Article/details/grpclstpy.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.hesvh.cn/Article/details/gvxxbesvu.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.fehbvm.com/Article/details/gpwpyjvrd.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ganeguexj.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.hesvh.cn/Article/details/gpshrdtbx.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ggzawjgny.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.hesvh.cn/Article/details/glyxmyper.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.hesvh.cn/Article/details/ghhphpwbt.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.hesvh.cn/Article/details/gcynvsyfg.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.hesvh.cn/Article/details/gpeawvthx.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.zdbjq.cn/Article/details/gxwbawsox.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.fehbvm.com/Article/details/gcpuyabeg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.zdbjq.cn/Article/details/gqdxtruak.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.zdbjq.cn/Article/details/gatjirryf.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.hesvh.cn/Article/details/glgoeeaxf.sHtML

[D02] 追加元素到末尾
来源：http://www.share.fehbvm.com/Article/details/gfwythwgz.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.zdbjq.cn/Article/details/gzwoycliu.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.fehbvm.com/Article/details/gkluinhff.sHtML

JS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/ggqsowysz.sHtML

TS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/gygkmcefw.sHtML

Java: list.add(4);
来源：http://m.share.zdbjq.cn/Article/details/gdihtrxis.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.fehbvm.com/Article/details/geaiidafs.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.fehbvm.com/Article/details/gkjtlmkdu.sHtML

C#:   list.Add(4);
来源：http://baike.fehbvm.com/Article/details/gmosccyik.sHtML

[D03] 在指定位置插入元素
来源：http://baike.zdbjq.cn/Article/details/gmlwmiaed.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gwmundtvj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.hesvh.cn/Article/details/gxziwbzii.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.fehbvm.com/Article/details/gcnluziwq.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.fehbvm.com/Article/details/gdknvuqfa.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gjtpcftfr.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.hesvh.cn/Article/details/gijosotae.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.fehbvm.com/Article/details/gccocmbzi.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/ghtjbxirj.sHtML

[D04] 删除元素
来源：http://blog.zdbjq.cn/Article/details/gujkhzuuk.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.zdbjq.cn/Article/details/godlsaheu.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.fehbvm.com/Article/details/ggaubktom.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.zdbjq.cn/Article/details/glrabcpvb.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.zdbjq.cn/Article/details/ghlccpjau.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.hesvh.cn/Article/details/gteukxarr.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.fehbvm.com/Article/details/gvqrshbun.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.zdbjq.cn/Article/details/gqwmyqcac.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.zdbjq.cn/Article/details/gdjgchxsj.sHtML

[D05] 访问与修改元素
来源：http://mobile.hesvh.cn/Article/details/glbilzwby.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gizzarklm.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gpfqjzqit.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/guyfztbjp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.hesvh.cn/Article/details/gbnomaacd.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.zdbjq.cn/Article/details/gqhyfrqvt.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gdaciiqxz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gszyokvbb.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gdptanbym.sHtML

[D06] 数组长度
来源：http://read.share.hesvh.cn/Article/details/gqkxxhcqx.sHtML

Py:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/ghebbjafo.sHtML

PHP:  count($arr);
来源：http://3g.fehbvm.com/Article/details/ganzlfpbe.sHtML

JS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/gybzzhxwn.sHtML

TS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gokfgtvqu.sHtML

Java: list.size();
来源：http://www.m.share.zdbjq.cn/Article/details/gjkrryboo.sHtML

Go:   len(arr)
来源：http://blog.fehbvm.com/Article/details/ganbhxrnt.sHtML

Ruby: arr.length; arr.size
来源：http://3g.zdbjq.cn/Article/details/gcwyklrkz.sHtML

C#:   list.Count;
来源：http://www.blog.fehbvm.com/Article/details/gsncbusvc.sHtML

[D07] 切片 / 取子数组
来源：http://3g.hesvh.cn/Article/details/gbmyljctg.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.fehbvm.com/Article/details/ghvrpsxnn.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.zdbjq.cn/Article/details/gjedwwudx.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gzrfxbwsg.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/ggkszvlza.sHtML

Java: list.subList(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/givldlzoj.sHtML

Go:   arr[1:4]
来源：http://www.share.zdbjq.cn/Article/details/gebtpvamv.sHtML

Ruby: arr[1, 3]
来源：http://baike.fehbvm.com/Article/details/gpfqovebh.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.fehbvm.com/Article/details/gszowgtdk.sHtML

[D08] 合并两个数组
来源：http://mobile.zdbjq.cn/Article/details/gbpqxhmde.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.fehbvm.com/Article/details/gaqtkeofa.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.zdbjq.cn/Article/details/ghmywexfc.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.hesvh.cn/Article/details/gewyhajoj.sHtML

TS:   [...a, ...b];
来源：http://baike.hesvh.cn/Article/details/gawivnazm.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.hesvh.cn/Article/details/gqxcqjavh.sHtML

Go:   append(a, b...)
来源：http://read.share.hesvh.cn/Article/details/gnxwcqrwz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gryxfhlpx.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gjwmvhhmf.sHtML

[D09] 排序（升序）
来源：http://baike.zdbjq.cn/Article/details/ggllodwwh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gwjvvpkjv.sHtML

PHP:  sort($arr);
来源：http://wap.zdbjq.cn/Article/details/gczzghovq.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.fehbvm.com/Article/details/gsrqwhnne.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.zdbjq.cn/Article/details/gfyzlpkxy.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.hesvh.cn/Article/details/gjewfpmix.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gjqkhszgz.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/gtcdkabvo.sHtML

C#:   list.Sort();
来源：http://m.share.fehbvm.com/Article/details/ggujregmw.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.hesvh.cn/Article/details/geeiskccc.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.fehbvm.com/Article/details/gaqzwazqz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.hesvh.cn/Article/details/glzolgvhv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/goupforvr.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/gplwvnlqb.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.fehbvm.com/Article/details/gxkvjqszd.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.hesvh.cn/Article/details/gzsarfstu.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.hesvh.cn/Article/details/gcpvcdivx.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.hesvh.cn/Article/details/gertdnsjd.sHtML

[D11] 反转数组
来源：http://mobile.hesvh.cn/Article/details/gtwtwdaoc.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.zdbjq.cn/Article/details/gtgpapqxj.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.fehbvm.com/Article/details/giuajobnz.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.zdbjq.cn/Article/details/gecszorrm.sHtML

TS:   [...arr].reverse();
来源：http://baike.zdbjq.cn/Article/details/ghxlfqlib.sHtML

Java: Collections.reverse(list);
来源：http://baike.fehbvm.com/Article/details/gnbjticua.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.zdbjq.cn/Article/details/gtaqtrche.sHtML

Ruby: arr.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gogyrcwiy.sHtML

C#:   list.Reverse();
来源：http://www.share.zdbjq.cn/Article/details/gvbdmriwr.sHtML

[D12] 查找元素下标
来源：http://wap.fehbvm.com/Article/details/gidccmdcg.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.hesvh.cn/Article/details/grbwrbdra.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.hesvh.cn/Article/details/gltvvhjaw.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/gxumhlrcq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/gzdxuioip.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.fehbvm.com/Article/details/grjmquuos.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.fehbvm.com/Article/details/gkeorrycn.sHtML

Ruby: arr.index(x)
来源：http://www.blog.fehbvm.com/Article/details/gbueupjkt.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.fehbvm.com/Article/details/gdogxopdc.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.zdbjq.cn/Article/details/gfkywddbp.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gicmtlpcv.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gfimtqaay.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/ghgwqeeve.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gbfznpfow.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.zdbjq.cn/Article/details/geyxsaeii.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.fehbvm.com/Article/details/ghoxpnzbn.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.zdbjq.cn/Article/details/gslpuobju.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.fehbvm.com/Article/details/gxotcoaab.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.zdbjq.cn/Article/details/gfbyefpwl.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.zdbjq.cn/Article/details/gjsjqbmow.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.zdbjq.cn/Article/details/gtlrwjkso.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/gcvljradh.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/gycrumdlv.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.fehbvm.com/Article/details/gakjpzbyn.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/grjjyridu.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gdbmbfoue.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.fehbvm.com/Article/details/gesxuatju.sHtML

[D15] 去重
来源：http://wap.hesvh.cn/Article/details/gqdfqddzv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/guowjnbto.sHtML

PHP:  array_unique($arr);
来源：http://m.share.zdbjq.cn/Article/details/gzeicxihh.sHtML

JS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gtxbmknsb.sHtML

TS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gjgdmfrah.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.fehbvm.com/Article/details/gudegozxk.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.hesvh.cn/Article/details/gylqmowqy.sHtML

Ruby: arr.uniq
来源：http://www.share.zdbjq.cn/Article/details/gwigfulnk.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gtnjijhyt.sHtML

[D16] 求和与平均值
来源：http://baike.zdbjq.cn/Article/details/gsikapyzn.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.fehbvm.com/Article/details/gwtkyhocz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.hesvh.cn/Article/details/gcbyxhemm.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gdtewnrwe.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/gfcihblbf.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.hesvh.cn/Article/details/gnapbwkrv.sHtML

Go:   // 手写循环累加
来源：http://www.share.zdbjq.cn/Article/details/gjsxrrtrd.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.hesvh.cn/Article/details/gpnvlshqd.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.zdbjq.cn/Article/details/grvwvikrd.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.hesvh.cn/Article/details/gjcxwbsuq.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.hesvh.cn/Article/details/gubshwjhr.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.hesvh.cn/Article/details/gpqahuoin.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.fehbvm.com/Article/details/gkzhgqarj.sHtML

TS:   Math.max(...arr);
来源：http://wap.fehbvm.com/Article/details/guipeoaob.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.hesvh.cn/Article/details/gfqegaite.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.zdbjq.cn/Article/details/glalgqktl.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.zdbjq.cn/Article/details/golkfifma.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.fehbvm.com/Article/details/giuikhfbn.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.fehbvm.com/Article/details/gswaootfv.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.zdbjq.cn/Article/details/grvxwnpqy.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.fehbvm.com/Article/details/gjcaqsxuc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.hesvh.cn/Article/details/glthyeyjj.sHtML

TS:   nested.flat();
来源：http://www.m.share.zdbjq.cn/Article/details/grmstxvvr.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gxavoarnr.sHtML

Go:   // 手写双层循环
来源：http://wap.hesvh.cn/Article/details/gwquduqkk.sHtML

Ruby: nested.flatten
来源：http://3g.hesvh.cn/Article/details/gypwveyld.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.fehbvm.com/Article/details/gdzsassri.sHtML

[D19] 按字段分组
来源：http://3g.hesvh.cn/Article/details/gflikwcif.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.fehbvm.com/Article/details/glkajsvhq.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.fehbvm.com/Article/details/gwzbonqqh.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.zdbjq.cn/Article/details/grzwcmrtc.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.hesvh.cn/Article/details/gxzdqxdil.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.zdbjq.cn/Article/details/gizvagulz.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.hesvh.cn/Article/details/gbbqsqsaa.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.fehbvm.com/Article/details/glccfxysq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.zdbjq.cn/Article/details/geyfxkyej.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.zdbjq.cn/Article/details/gdpdoglhu.sHtML

Py:   Counter(arr)
来源：http://wap.zdbjq.cn/Article/details/gmxmsfzhq.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/goljhjdns.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/gsxxosdgz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gqqoskjvu.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.zdbjq.cn/Article/details/ghvbfitkm.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.fehbvm.com/Article/details/gbqpsyqph.sHtML

Ruby: arr.tally
来源：http://www.blog.fehbvm.com/Article/details/gejghnktj.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.zdbjq.cn/Article/details/grxlccytk.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.fehbvm.com/Article/details/gfvggkfsi.sHtML

Py:   x in arr
来源：http://www.share.hesvh.cn/Article/details/gzeyqgmob.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.zdbjq.cn/Article/details/gnevuoifa.sHtML

JS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/gxeyeukiy.sHtML

TS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/gkinatrqm.sHtML

Java: list.contains(x)
来源：http://3g.hesvh.cn/Article/details/gmbqueika.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.fehbvm.com/Article/details/gamatqzmn.sHtML

Ruby: arr.include?(x)
来源：http://3g.hesvh.cn/Article/details/gelmhwwpg.sHtML

C#:   list.Contains(x)
来源：http://www.blog.hesvh.cn/Article/details/glvwpvjzk.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.fehbvm.com/Article/details/gfyeydyhk.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.hesvh.cn/Article/details/gttbonouy.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.fehbvm.com/Article/details/gbidsxfuf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.zdbjq.cn/Article/details/guizatzpw.sHtML

TS:   [...arr];
来源：http://blog.hesvh.cn/Article/details/ghkxiawuj.sHtML

Java: new ArrayList<>(list);
来源：http://baike.zdbjq.cn/Article/details/gomfphsyu.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.zdbjq.cn/Article/details/gnnlfrqaj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.fehbvm.com/Article/details/gilulohfk.sHtML

C#:   new List<int>(list);
来源：http://wap.hesvh.cn/Article/details/gmljyglws.sHtML

[D23] reduce 累积计算
来源：http://3g.fehbvm.com/Article/details/gyclwrsny.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.zdbjq.cn/Article/details/gwopbccqw.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.fehbvm.com/Article/details/gnxdtqcdw.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gzkuaocer.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/gtevbmquk.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.hesvh.cn/Article/details/gxslhkbqh.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/gxvgfeidt.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.hesvh.cn/Article/details/gumsbajrn.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.hesvh.cn/Article/details/grxqkutdc.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.zdbjq.cn/Article/details/genobphjm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.fehbvm.com/Article/details/gteifnizg.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.fehbvm.com/Article/details/gaylnbgga.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.zdbjq.cn/Article/details/gqoufhghl.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gnsvyqyvc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.zdbjq.cn/Article/details/gomzvgxlz.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.fehbvm.com/Article/details/gmainbuvw.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.hesvh.cn/Article/details/gnceavpxs.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.zdbjq.cn/Article/details/guwmcstlc.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.zdbjq.cn/Article/details/gfhvjukge.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.fehbvm.com/Article/details/grjzmuwwu.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.zdbjq.cn/Article/details/ggkdimqkm.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.zdbjq.cn/Article/details/gumujfkrb.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.zdbjq.cn/Article/details/gguxjgkbq.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.fehbvm.com/Article/details/gqnsktmma.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.zdbjq.cn/Article/details/gvvbyyvdh.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.zdbjq.cn/Article/details/ggyclfepk.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.fehbvm.com/Article/details/gkswwhfke.sHtML

[D26] 数组转字符串
来源：http://baike.zdbjq.cn/Article/details/gwyqiarfr.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.fehbvm.com/Article/details/gckgjesho.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.fehbvm.com/Article/details/guiqhxsze.sHtML

JS:   arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gunmxfqmb.sHtML

TS:   arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gmljqwpqs.sHtML

Java: String.join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/gslipihqb.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.fehbvm.com/Article/details/gwrppghcs.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/goyfrdjus.sHtML

C#:   string.Join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/gewnpsqij.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gffdksbcy.sHtML

E. 字符串处理
来源：http://www.m.share.zdbjq.cn/Article/details/glozuvryb.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gkxlbicav.sHtML

[E01] 拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/ggzxqqvzg.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.fehbvm.com/Article/details/giezerkai.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.hesvh.cn/Article/details/gjttacdmu.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fehbvm.com/Article/details/gpyqxfprw.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/gcelpbkqt.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.hesvh.cn/Article/details/gxiehenjf.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.fehbvm.com/Article/details/gnswhpzot.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.zdbjq.cn/Article/details/gizcfmbfy.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.fehbvm.com/Article/details/gipkgosmj.sHtML

[E02] 重复字符串
来源：http://www.blog.hesvh.cn/Article/details/guultdpdc.sHtML

Py:   "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/ghglabowy.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.fehbvm.com/Article/details/gecnylpmw.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gvvgmqopq.sHtML

TS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gmdpktrgw.sHtML

Java: "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gwcpjltlb.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.hesvh.cn/Article/details/gwhvcjqcs.sHtML

Ruby: "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/glvaziavs.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.fehbvm.com/Article/details/gmqxfmalj.sHtML

[E03] 截取子串
来源：http://m.share.hesvh.cn/Article/details/gtbfeypjq.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.fehbvm.com/Article/details/gdefybdyt.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gfnwbgwgg.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gpzpbdxsg.sHtML

TS:   s.slice(1, 4)
来源：http://baike.hesvh.cn/Article/details/glyxqwjza.sHtML

Java: s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gcmwmawmg.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.hesvh.cn/Article/details/gcgxpzbbu.sHtML


<!-- 参考信息 -->