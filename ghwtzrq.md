代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://mobile.fanxiaobao.xyz/Article/details/ggazqmpkg.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.fanxiaobao.xyz/Article/details/gbflxaqap.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/ggybauccc.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.fanxiaobao.xyz/Article/details/gopvkhedl.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.fanxiaobao.xyz/Article/details/gxuiuqcly.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobxriivr.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.fanxiaobao.xyz/Article/details/gyibqtsew.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedawliiz.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gztecrqom.sHtML

Go:   func add(a, b int) int
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvizgtym.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.fanxiaobao.xyz/Article/details/gpcezrgbp.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtypfeppy.sHtML

[C14] 泛型函数
来源：http://wap.fanxiaobao.xyz/Article/details/ghurtinxc.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.fanxiaobao.xyz/Article/details/ggrlzgadr.sHtML

PHP:  // 无泛型
来源：http://blog.fanxiaobao.xyz/Article/details/gumpaugqs.sHtML

JS:   // 无泛型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqwsfdalb.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.fanxiaobao.xyz/Article/details/gmqikgpuf.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.fanxiaobao.xyz/Article/details/gzwevbxbf.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqmyotwdv.sHtML

Ruby: # 无泛型
来源：http://read.share.fanxiaobao.xyz/Article/details/glqxbekpo.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.fanxiaobao.xyz/Article/details/gltsbygvg.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gaqswneao.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.fanxiaobao.xyz/Article/details/gitgslbpd.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.fanxiaobao.xyz/Article/details/gygxiagrz.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwylmjdl.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbeahdhf.sHtML

Java: // 无解构
来源：http://m.share.fanxiaobao.xyz/Article/details/gkakjgrwj.sHtML

Go:   // 无解构
来源：http://baike.fanxiaobao.xyz/Article/details/gjyxtnkii.sHtML

Ruby: a, b = pair
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmskkpsdk.sHtML

C#:   var (a, b) = pair;
来源：http://wap.fanxiaobao.xyz/Article/details/gqqfbqbqq.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.fanxiaobao.xyz/Article/details/gomxebtzq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.fanxiaobao.xyz/Article/details/gfhsuhxlq.sHtML

PHP:  // 无重载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpstesnc.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.fanxiaobao.xyz/Article/details/ggkebkruz.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.fanxiaobao.xyz/Article/details/gippmbheg.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gczvswuuk.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.fanxiaobao.xyz/Article/details/glsbjrlkk.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gdxuofdtr.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gosxjclif.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlzoulnq.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.fanxiaobao.xyz/Article/details/gybayjelp.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gcvmgdwfs.sHtML

[D01] 创建数组 / 列表
来源：http://wap.fanxiaobao.xyz/Article/details/grqklgfmr.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.fanxiaobao.xyz/Article/details/gguwbeigw.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.fanxiaobao.xyz/Article/details/gmlmzdtor.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.fanxiaobao.xyz/Article/details/gpgjwqrcj.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.fanxiaobao.xyz/Article/details/gzyupapub.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzjapxnn.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqbftkiw.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.fanxiaobao.xyz/Article/details/gapgvfpbv.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.fanxiaobao.xyz/Article/details/galmermym.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/giaitwjdu.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.fanxiaobao.xyz/Article/details/gbjsxhzkg.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.fanxiaobao.xyz/Article/details/gjlmzwjau.sHtML

JS:   arr.push(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzsxxjip.sHtML

TS:   arr.push(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbrfnxdud.sHtML

Java: list.add(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gvcrhyzrn.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.fanxiaobao.xyz/Article/details/grpnscbax.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghiondnqt.sHtML

C#:   list.Add(4);
来源：http://baike.fanxiaobao.xyz/Article/details/glypuqzld.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjmrprwr.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gugihnqsq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.fanxiaobao.xyz/Article/details/ggndqtcbk.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.fanxiaobao.xyz/Article/details/gdcbvczmy.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.fanxiaobao.xyz/Article/details/grojrhxyg.sHtML

Java: list.add(0, 0);
来源：http://baike.fanxiaobao.xyz/Article/details/gsstwmvtt.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghzqqflqw.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.fanxiaobao.xyz/Article/details/gvqsqvcxl.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/gyibdxsxh.sHtML

[D04] 删除元素
来源：http://baike.fanxiaobao.xyz/Article/details/gkqxzspnw.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giobjmjpi.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gpbfrtmnr.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.fanxiaobao.xyz/Article/details/gtbigqllc.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbpdfzboq.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxmxvguq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyguxwemk.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjozecmqh.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.fanxiaobao.xyz/Article/details/gpjjhroen.sHtML

[D05] 访问与修改元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqvewumga.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fanxiaobao.xyz/Article/details/gsgyfceaa.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.fanxiaobao.xyz/Article/details/gdmrnmynw.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzbunrgq.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxupeoutn.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.fanxiaobao.xyz/Article/details/glxdxdzlg.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.fanxiaobao.xyz/Article/details/grrwozbge.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fanxiaobao.xyz/Article/details/gcimyausa.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.fanxiaobao.xyz/Article/details/gbnlvfenm.sHtML

[D06] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/goapclqqr.sHtML

Py:   len(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gtygepaqb.sHtML

PHP:  count($arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gnritwwbg.sHtML

JS:   arr.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gbvliyqth.sHtML

TS:   arr.length
来源：http://read.share.fanxiaobao.xyz/Article/details/grweduqsk.sHtML

Java: list.size();
来源：http://wap.fanxiaobao.xyz/Article/details/gylwszikn.sHtML

Go:   len(arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gylentpyr.sHtML

Ruby: arr.length; arr.size
来源：http://blog.fanxiaobao.xyz/Article/details/gamtonuyv.sHtML

C#:   list.Count;
来源：http://blog.fanxiaobao.xyz/Article/details/govnrnuas.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gqstbdjji.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.fanxiaobao.xyz/Article/details/grpblopvv.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.fanxiaobao.xyz/Article/details/geuanzmgu.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxthvmmvd.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.fanxiaobao.xyz/Article/details/glrkvnfgf.sHtML

Java: list.subList(1, 4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkcotbggy.sHtML

Go:   arr[1:4]
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwfkmtgs.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggeiwhaeo.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.fanxiaobao.xyz/Article/details/ggkbxshmo.sHtML

[D08] 合并两个数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvbmylwh.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.fanxiaobao.xyz/Article/details/gctdczqzt.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gefwdemxj.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzogchdcp.sHtML

TS:   [...a, ...b];
来源：http://mobile.fanxiaobao.xyz/Article/details/gmildixud.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaokpnaka.sHtML

Go:   append(a, b...)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpgyiwagw.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gswxecmbf.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjrwubsf.sHtML

[D09] 排序（升序）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtrvkaju.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcwsnrvsc.sHtML

PHP:  sort($arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdshzicby.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgvezhlc.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztrmvphq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbkfhnblq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gdhwdhnod.sHtML

Ruby: arr.sort
来源：http://baike.fanxiaobao.xyz/Article/details/gbqfslhwm.sHtML

C#:   list.Sort();
来源：http://mobile.fanxiaobao.xyz/Article/details/gywvqdnod.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.fanxiaobao.xyz/Article/details/gwjyfajca.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxnmyhwj.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfksiqan.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fanxiaobao.xyz/Article/details/gncrlyuab.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvaypdmak.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.fanxiaobao.xyz/Article/details/gidxbhvmy.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.fanxiaobao.xyz/Article/details/girjbbrfz.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwsalyxs.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gleaddauk.sHtML

[D11] 反转数组
来源：http://wap.fanxiaobao.xyz/Article/details/gzrlzoqbb.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.fanxiaobao.xyz/Article/details/gdccsxhek.sHtML

PHP:  array_reverse($arr);
来源：http://wap.fanxiaobao.xyz/Article/details/guvwfkuap.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.fanxiaobao.xyz/Article/details/gittafrih.sHtML

TS:   [...arr].reverse();
来源：http://read.share.fanxiaobao.xyz/Article/details/gajbhjdop.sHtML

Java: Collections.reverse(list);
来源：http://wap.fanxiaobao.xyz/Article/details/gdbovkzwf.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdwhifwm.sHtML

Ruby: arr.reverse
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvwyxrraz.sHtML

C#:   list.Reverse();
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxhcrwea.sHtML

[D12] 查找元素下标
来源：http://3g.fanxiaobao.xyz/Article/details/gxqbtlxdi.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.fanxiaobao.xyz/Article/details/gafqkbicd.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhfbcjdz.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fanxiaobao.xyz/Article/details/gkqprvbyi.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fanxiaobao.xyz/Article/details/gpaiimzpq.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhracacz.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gssfmknld.sHtML

Ruby: arr.index(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmnfhkmm.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmnfuqyj.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.fanxiaobao.xyz/Article/details/gamdpdrpi.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.fanxiaobao.xyz/Article/details/gcerwmreo.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxdhuhld.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.fanxiaobao.xyz/Article/details/gfauxrpui.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gafbmjgnj.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.fanxiaobao.xyz/Article/details/gugqdevrm.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.fanxiaobao.xyz/Article/details/girvmkxcd.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjceoibpp.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.fanxiaobao.xyz/Article/details/gzphgedza.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.fanxiaobao.xyz/Article/details/gveuywwsh.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.fanxiaobao.xyz/Article/details/gyonwefbi.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gwiblwlvx.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkeftyfjt.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gbhrmhsvx.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.fanxiaobao.xyz/Article/details/gdpqakeud.sHtML

Go:   // 手写循环
来源：http://wap.fanxiaobao.xyz/Article/details/guijsizew.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqaedyeny.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdnpkskkl.sHtML

[D15] 去重
来源：http://blog.fanxiaobao.xyz/Article/details/gtfknrtje.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmmnxwwv.sHtML

PHP:  array_unique($arr);
来源：http://3g.fanxiaobao.xyz/Article/details/gwvfliyfq.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.fanxiaobao.xyz/Article/details/gjpilboxq.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.fanxiaobao.xyz/Article/details/greabrmwn.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.fanxiaobao.xyz/Article/details/grmantaes.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawcaeafw.sHtML

Ruby: arr.uniq
来源：http://baike.fanxiaobao.xyz/Article/details/geyahcuvv.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gvnppkicp.sHtML

[D16] 求和与平均值
来源：http://3g.fanxiaobao.xyz/Article/details/gikfnmvmi.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gicnocqss.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxiaumbud.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmtwgghx.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjehhqmsh.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.fanxiaobao.xyz/Article/details/gxhbsbuvy.sHtML

Go:   // 手写循环累加
来源：http://wap.fanxiaobao.xyz/Article/details/gbvklmbcy.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbgccony.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonsdxdyf.sHtML

[D17] 最大值与最小值
来源：http://wap.fanxiaobao.xyz/Article/details/goqnvfyat.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/glghzetdm.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.fanxiaobao.xyz/Article/details/gyengjtkt.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gwhoqmxix.sHtML

TS:   Math.max(...arr);
来源：http://baike.fanxiaobao.xyz/Article/details/gpggsrxco.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.fanxiaobao.xyz/Article/details/glrzynmql.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gohahgidw.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.fanxiaobao.xyz/Article/details/goxvxsppd.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.fanxiaobao.xyz/Article/details/gyazjjjlp.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.fanxiaobao.xyz/Article/details/gdbwogcta.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.fanxiaobao.xyz/Article/details/goguzaezj.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.fanxiaobao.xyz/Article/details/gtfaadnui.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fanxiaobao.xyz/Article/details/gentjaubd.sHtML

TS:   nested.flat();
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwmagsef.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gsfuvbpsw.sHtML

Go:   // 手写双层循环
来源：http://wap.fanxiaobao.xyz/Article/details/gtmnpahfc.sHtML

Ruby: nested.flatten
来源：http://mobile.fanxiaobao.xyz/Article/details/grkbbzmpb.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/grhoqntmi.sHtML

[D19] 按字段分组
来源：http://blog.fanxiaobao.xyz/Article/details/gbekzuovs.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gkhtucdbk.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.fanxiaobao.xyz/Article/details/gldozalxb.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.fanxiaobao.xyz/Article/details/gvniytaof.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.fanxiaobao.xyz/Article/details/gtumwawmw.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.fanxiaobao.xyz/Article/details/ghikqmynp.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.fanxiaobao.xyz/Article/details/gthidqxmj.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.fanxiaobao.xyz/Article/details/grxenasoa.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.fanxiaobao.xyz/Article/details/gogiwddgc.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzrofddl.sHtML

Py:   Counter(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/giwxsgmtt.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gurrylfps.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbsgrxzzd.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fanxiaobao.xyz/Article/details/glkjpdivs.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.fanxiaobao.xyz/Article/details/gfdcrlgss.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqdsrwsow.sHtML

Ruby: arr.tally
来源：http://mobile.fanxiaobao.xyz/Article/details/grivahxkz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjjzdxtg.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gaalswhnk.sHtML

Py:   x in arr
来源：http://baike.fanxiaobao.xyz/Article/details/gngjjompg.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.fanxiaobao.xyz/Article/details/glmbbnyjh.sHtML

JS:   arr.includes(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhfysitt.sHtML

TS:   arr.includes(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/guuztwtlz.sHtML

Java: list.contains(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gbylngteu.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.fanxiaobao.xyz/Article/details/goheegwmw.sHtML

Ruby: arr.include?(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gjrgvrxae.sHtML

C#:   list.Contains(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghxhwppmb.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzdtlqav.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/giqedctbp.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.fanxiaobao.xyz/Article/details/gzkbzqipj.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gxnzgvdho.sHtML

TS:   [...arr];
来源：http://wap.fanxiaobao.xyz/Article/details/gbnuhidfs.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmnqktxel.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdgedvogh.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.fanxiaobao.xyz/Article/details/gjoczsghz.sHtML

C#:   new List<int>(list);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzuqfjox.sHtML

[D23] reduce 累积计算
来源：http://m.share.fanxiaobao.xyz/Article/details/gbyazibqc.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.fanxiaobao.xyz/Article/details/galzxplgb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/glmfzpagx.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fanxiaobao.xyz/Article/details/gdbrjauin.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golvkcewx.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gugjyywdn.sHtML

Go:   // 手写循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqlgtyvi.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.fanxiaobao.xyz/Article/details/gzwvylewq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gykqchucb.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxppdkki.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.fanxiaobao.xyz/Article/details/gcmrgtifr.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geokyjkvu.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtshycure.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gccytdxkg.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.fanxiaobao.xyz/Article/details/gowxyzxfb.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.fanxiaobao.xyz/Article/details/gtljzglkv.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjvaxsdg.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwhyfoja.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.fanxiaobao.xyz/Article/details/gndskcxfd.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.fanxiaobao.xyz/Article/details/gxnxqbuat.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.fanxiaobao.xyz/Article/details/gfbyidizu.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqywksgb.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.fanxiaobao.xyz/Article/details/gczkfvtaf.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzllxrov.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.fanxiaobao.xyz/Article/details/glbtindkw.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/geosezcbz.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gtomxlfnk.sHtML

[D26] 数组转字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gxqxhqahs.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.fanxiaobao.xyz/Article/details/gvlbajdua.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/gempqwnwl.sHtML

JS:   arr.join(", ")
来源：http://wap.fanxiaobao.xyz/Article/details/gglavvyev.sHtML

TS:   arr.join(", ")
来源：http://3g.fanxiaobao.xyz/Article/details/gkwubgxwe.sHtML

Java: String.join(", ", list)
来源：http://baike.fanxiaobao.xyz/Article/details/gyefpvjhg.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.fanxiaobao.xyz/Article/details/gabzksqli.sHtML

Ruby: arr.join(", ")
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwtxktdk.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdqczmlyd.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gcclzrxeu.sHtML

E. 字符串处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gztahmwfv.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gvifmestj.sHtML

[E01] 拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gbdpvstch.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.fanxiaobao.xyz/Article/details/gzykzwpqo.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.fanxiaobao.xyz/Article/details/guuhxcoqi.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fanxiaobao.xyz/Article/details/gzfrouphy.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fanxiaobao.xyz/Article/details/gaanzbukh.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbmhjoqj.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.fanxiaobao.xyz/Article/details/gcvrqqdnd.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.fanxiaobao.xyz/Article/details/giptgbdgg.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvnzwcow.sHtML

[E02] 重复字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchdlhhua.sHtML

Py:   "ab" * 3
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwgbgpsum.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjrwogpby.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwvjzcoo.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmoxnfnlo.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpjqgcrt.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/giuqcfqyv.sHtML

Ruby: "ab" * 3
来源：http://mobile.fanxiaobao.xyz/Article/details/gmyrxifac.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.fanxiaobao.xyz/Article/details/gbzwjlcmf.sHtML

[E03] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/gxprjhuuk.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.fanxiaobao.xyz/Article/details/gsmmpesac.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.fanxiaobao.xyz/Article/details/gappojexm.sHtML


<!-- 参考信息 -->