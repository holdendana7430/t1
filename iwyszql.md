代发 wailian999

[C14] 泛型函数
来源：http://www.share.zdbjq.cn/Article/details/gohtwwvbe.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.zdbjq.cn/Article/details/gyvdmrguv.sHtML

PHP:  // 无泛型
来源：http://www.share.fehbvm.com/Article/details/geagpwykf.sHtML

JS:   // 无泛型
来源：http://blog.fehbvm.com/Article/details/gjlfemeal.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.zdbjq.cn/Article/details/gsdfjhnbq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.hesvh.cn/Article/details/gzvmdfslu.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.hesvh.cn/Article/details/gobqiwqmz.sHtML

Ruby: # 无泛型
来源：http://blog.zdbjq.cn/Article/details/gzsncihct.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.zdbjq.cn/Article/details/gheofdgpg.sHtML

[C15] 解构 / 展开参数
来源：http://blog.hesvh.cn/Article/details/gehyhmgcz.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.hesvh.cn/Article/details/gqawxlbqj.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.hesvh.cn/Article/details/gmxqmfkfi.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/gkkgiojfn.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.fehbvm.com/Article/details/gujjhelqz.sHtML

Java: // 无解构
来源：http://www.blog.zdbjq.cn/Article/details/gvztojfxj.sHtML

Go:   // 无解构
来源：http://www.share.hesvh.cn/Article/details/glbbyuoot.sHtML

Ruby: a, b = pair
来源：http://blog.zdbjq.cn/Article/details/ghqqqgjev.sHtML

C#:   var (a, b) = pair;
来源：http://baike.fehbvm.com/Article/details/gbcnrlzpj.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.hesvh.cn/Article/details/gfvwegkgr.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.zdbjq.cn/Article/details/gcbcpqfzj.sHtML

PHP:  // 无重载
来源：http://www.m.share.hesvh.cn/Article/details/gjadcaodq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.zdbjq.cn/Article/details/gtxnmurwj.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.fehbvm.com/Article/details/gcnvlxyrh.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.zdbjq.cn/Article/details/gvkcrmymf.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.hesvh.cn/Article/details/gwmcuymiq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.hesvh.cn/Article/details/gctftapqq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.hesvh.cn/Article/details/gteoufaer.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gdbwagwvd.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.zdbjq.cn/Article/details/glbttpuqx.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gnirowxth.sHtML

[D01] 创建数组 / 列表
来源：http://baike.fehbvm.com/Article/details/gezuntyox.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.zdbjq.cn/Article/details/gpmmamrws.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.zdbjq.cn/Article/details/gnzhknfci.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.hesvh.cn/Article/details/grjdcwbfy.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.zdbjq.cn/Article/details/gnsuupdwd.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.fehbvm.com/Article/details/gskrpaqrx.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.hesvh.cn/Article/details/gbnhkksfq.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.zdbjq.cn/Article/details/gljswgvfn.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.fehbvm.com/Article/details/gkmvsavwc.sHtML

[D02] 追加元素到末尾
来源：http://mobile.fehbvm.com/Article/details/goegbvfna.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.fehbvm.com/Article/details/gfroehqjn.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.zdbjq.cn/Article/details/ggjqrixvb.sHtML

JS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/gssdavxtc.sHtML

TS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/gklcctduk.sHtML

Java: list.add(4);
来源：http://3g.hesvh.cn/Article/details/giegonksj.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.fehbvm.com/Article/details/gztbqkbgk.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.fehbvm.com/Article/details/gkvgqpdkt.sHtML

C#:   list.Add(4);
来源：http://mobile.zdbjq.cn/Article/details/gujtigogk.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.fehbvm.com/Article/details/ggongkvyq.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.zdbjq.cn/Article/details/gcbjfkscm.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.zdbjq.cn/Article/details/gxggcgnnl.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.zdbjq.cn/Article/details/gwnnxrkmc.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.fehbvm.com/Article/details/gytneyidl.sHtML

Java: list.add(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gqwuvicdk.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.fehbvm.com/Article/details/gqqamamst.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.zdbjq.cn/Article/details/gqgnqactv.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.fehbvm.com/Article/details/gtlhvjgzs.sHtML

[D04] 删除元素
来源：http://3g.hesvh.cn/Article/details/gtembmgrx.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.hesvh.cn/Article/details/gcugxilvt.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.fehbvm.com/Article/details/gqwhsknwp.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.hesvh.cn/Article/details/gjzwgtgmg.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.zdbjq.cn/Article/details/gaiiczuqs.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.fehbvm.com/Article/details/gmuvtttar.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.fehbvm.com/Article/details/gosxfrwnc.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.fehbvm.com/Article/details/grqiiexky.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.fehbvm.com/Article/details/gyukmydno.sHtML

[D05] 访问与修改元素
来源：http://wap.zdbjq.cn/Article/details/gddnojagc.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/grghlcwml.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gdrgtqqpj.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gwgqrsnxz.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.fehbvm.com/Article/details/gtqgiruih.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.zdbjq.cn/Article/details/gohplzxmi.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gmduxgfhz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gbatyohya.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gvrfwizdu.sHtML

[D06] 数组长度
来源：http://read.share.fehbvm.com/Article/details/gnjcjgeua.sHtML

Py:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gfeammkqm.sHtML

PHP:  count($arr);
来源：http://blog.fehbvm.com/Article/details/gltroquhv.sHtML

JS:   arr.length
来源：http://wap.fehbvm.com/Article/details/goedconjh.sHtML

TS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gbkulzsvt.sHtML

Java: list.size();
来源：http://www.share.hesvh.cn/Article/details/gdgnxvkac.sHtML

Go:   len(arr)
来源：http://wap.hesvh.cn/Article/details/gftnefjjf.sHtML

Ruby: arr.length; arr.size
来源：http://3g.hesvh.cn/Article/details/gtmvrirlr.sHtML

C#:   list.Count;
来源：http://read.share.hesvh.cn/Article/details/guyxxnajz.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.zdbjq.cn/Article/details/gcmribczb.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.hesvh.cn/Article/details/gebfeiprg.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.fehbvm.com/Article/details/gmwkaqcsr.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gozromolj.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gusoyfnmx.sHtML

Java: list.subList(1, 4);
来源：http://wap.hesvh.cn/Article/details/gbhlsudbf.sHtML

Go:   arr[1:4]
来源：http://m.share.hesvh.cn/Article/details/gbjsjyged.sHtML

Ruby: arr[1, 3]
来源：http://www.share.zdbjq.cn/Article/details/gjzoylidc.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.hesvh.cn/Article/details/ghbxrxzlt.sHtML

[D08] 合并两个数组
来源：http://m.share.hesvh.cn/Article/details/gsfhbdteh.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.hesvh.cn/Article/details/gugnmdyin.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.fehbvm.com/Article/details/gmemlkwab.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.hesvh.cn/Article/details/gatqlzlny.sHtML

TS:   [...a, ...b];
来源：http://wap.fehbvm.com/Article/details/gzhzxgzha.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.zdbjq.cn/Article/details/glyhvvrfx.sHtML

Go:   append(a, b...)
来源：http://baike.fehbvm.com/Article/details/gjyqnkeqx.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.zdbjq.cn/Article/details/gsqjbuobv.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.zdbjq.cn/Article/details/gavzdnlsy.sHtML

[D09] 排序（升序）
来源：http://read.share.fehbvm.com/Article/details/gfsvwbqwy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gvzzgdrde.sHtML

PHP:  sort($arr);
来源：http://blog.hesvh.cn/Article/details/gkbndqbnb.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.zdbjq.cn/Article/details/gcqlzhnfj.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.hesvh.cn/Article/details/gxwcufncd.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.fehbvm.com/Article/details/gxeycclgd.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/gsrzvokwk.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/giiscdlpp.sHtML

C#:   list.Sort();
来源：http://www.share.zdbjq.cn/Article/details/gwapguehk.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.hesvh.cn/Article/details/gzoxttipg.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.hesvh.cn/Article/details/gbiiqeagy.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.zdbjq.cn/Article/details/gypgwtjmd.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/gjqmpyocj.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/gcsmvgxnf.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.zdbjq.cn/Article/details/gwkkpbpws.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.zdbjq.cn/Article/details/giomflwxr.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.zdbjq.cn/Article/details/gjejfymsz.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.hesvh.cn/Article/details/ggtjrqvmg.sHtML

[D11] 反转数组
来源：http://3g.fehbvm.com/Article/details/gnoccdpli.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.hesvh.cn/Article/details/gxdhcvohg.sHtML

PHP:  array_reverse($arr);
来源：http://baike.fehbvm.com/Article/details/gjetjcfpu.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.hesvh.cn/Article/details/ghiyisvgq.sHtML

TS:   [...arr].reverse();
来源：http://www.share.hesvh.cn/Article/details/gyrcmyqdv.sHtML

Java: Collections.reverse(list);
来源：http://wap.fehbvm.com/Article/details/gzedjseqg.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.zdbjq.cn/Article/details/gjidzqlop.sHtML

Ruby: arr.reverse
来源：http://3g.hesvh.cn/Article/details/gnjfnifll.sHtML

C#:   list.Reverse();
来源：http://m.share.zdbjq.cn/Article/details/gcwtxvkme.sHtML

[D12] 查找元素下标
来源：http://mobile.fehbvm.com/Article/details/gsruwamlg.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.zdbjq.cn/Article/details/gsgrmvhjg.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gmtleoupu.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gffxamivr.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/gzgwlttnm.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.hesvh.cn/Article/details/girrlbnkq.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gwimbaeuw.sHtML

Ruby: arr.index(x)
来源：http://m.share.zdbjq.cn/Article/details/gedttokxa.sHtML

C#:   list.IndexOf(x);
来源：http://3g.hesvh.cn/Article/details/givwgsizw.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.hesvh.cn/Article/details/gepyeofnv.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.hesvh.cn/Article/details/gvxljyrxs.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.zdbjq.cn/Article/details/gvaidkytj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/gktpbcnwr.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/gqcnsowmp.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.zdbjq.cn/Article/details/gedoabcul.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.zdbjq.cn/Article/details/gtmfevhmj.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.fehbvm.com/Article/details/gmyczwhmq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.hesvh.cn/Article/details/gjgfamtjz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.hesvh.cn/Article/details/gbbeqmjxt.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.zdbjq.cn/Article/details/gzsjnnrjp.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.hesvh.cn/Article/details/gukushrxb.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/gcajrnost.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/gnypgvuqq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.hesvh.cn/Article/details/geovtnkyq.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/goebuferr.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gvhmcdbkr.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.zdbjq.cn/Article/details/gvpnizbkt.sHtML

[D15] 去重
来源：http://www.blog.fehbvm.com/Article/details/glluvpvbk.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.hesvh.cn/Article/details/gbuxahahq.sHtML

PHP:  array_unique($arr);
来源：http://3g.zdbjq.cn/Article/details/gjzylbplh.sHtML

JS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gtcfcwvpj.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gcngeujqp.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.hesvh.cn/Article/details/gljzeimxz.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.zdbjq.cn/Article/details/gsiiajumk.sHtML

Ruby: arr.uniq
来源：http://mobile.hesvh.cn/Article/details/gorbrxvld.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.hesvh.cn/Article/details/guwslobni.sHtML

[D16] 求和与平均值
来源：http://www.m.share.fehbvm.com/Article/details/gxuiyzdfg.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.zdbjq.cn/Article/details/gwxatwlqy.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.hesvh.cn/Article/details/gozzgnxec.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/grhleqbbz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gmssxjcem.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.zdbjq.cn/Article/details/govmuatop.sHtML

Go:   // 手写循环累加
来源：http://www.blog.zdbjq.cn/Article/details/gltkjipqm.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.hesvh.cn/Article/details/gbrddcxco.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.hesvh.cn/Article/details/grbcompfi.sHtML

[D17] 最大值与最小值
来源：http://blog.zdbjq.cn/Article/details/gqntapffj.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.zdbjq.cn/Article/details/glvhfssmg.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.hesvh.cn/Article/details/gvbberunt.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.hesvh.cn/Article/details/ghxteuwgl.sHtML

TS:   Math.max(...arr);
来源：http://baike.zdbjq.cn/Article/details/gyxjwskov.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.zdbjq.cn/Article/details/gdzuqmacy.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.fehbvm.com/Article/details/gwdudmsyh.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.fehbvm.com/Article/details/gqpqzwdbn.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.fehbvm.com/Article/details/gscefvbva.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.fehbvm.com/Article/details/guabeoxwu.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.fehbvm.com/Article/details/gwkbwrvnk.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.hesvh.cn/Article/details/goxmdlvof.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.fehbvm.com/Article/details/gbfzpmavp.sHtML

TS:   nested.flat();
来源：http://www.share.hesvh.cn/Article/details/gfjviwqkk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.fehbvm.com/Article/details/gnnavaafn.sHtML

Go:   // 手写双层循环
来源：http://blog.hesvh.cn/Article/details/gxxpuhxes.sHtML

Ruby: nested.flatten
来源：http://wap.hesvh.cn/Article/details/gpapyfatu.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.hesvh.cn/Article/details/gngdurazd.sHtML

[D19] 按字段分组
来源：http://blog.hesvh.cn/Article/details/glsgqdxbv.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.zdbjq.cn/Article/details/gfxmjavux.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.fehbvm.com/Article/details/gckuvziof.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.zdbjq.cn/Article/details/gebbiqglq.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/guncwrmbk.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.zdbjq.cn/Article/details/gkhindhaj.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.fehbvm.com/Article/details/gtpudlpbf.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.hesvh.cn/Article/details/ggzbfuaux.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.zdbjq.cn/Article/details/gqknnptko.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.hesvh.cn/Article/details/gpecjauww.sHtML

Py:   Counter(arr)
来源：http://read.share.hesvh.cn/Article/details/gvxxlhryi.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.zdbjq.cn/Article/details/ghwqfthxy.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/ghsbkjzop.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/gbsqfiiqm.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.zdbjq.cn/Article/details/gerbiteom.sHtML

Go:   // 手写 map[T]int
来源：http://wap.zdbjq.cn/Article/details/grxjlhfiw.sHtML

Ruby: arr.tally
来源：http://mobile.zdbjq.cn/Article/details/gsxfjhiec.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.fehbvm.com/Article/details/gapngycmy.sHtML

[D21] 判断是否包含某元素
来源：http://wap.hesvh.cn/Article/details/gnhwxniuy.sHtML

Py:   x in arr
来源：http://www.m.share.hesvh.cn/Article/details/gvxemsrfq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.hesvh.cn/Article/details/gfhkucxxh.sHtML

JS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/giiagrvfp.sHtML

TS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gsaidafsu.sHtML

Java: list.contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/ggiouycnl.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gaywxlhaa.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.hesvh.cn/Article/details/gfyhwwxfn.sHtML

C#:   list.Contains(x)
来源：http://blog.fehbvm.com/Article/details/gluezrevq.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.zdbjq.cn/Article/details/guvqkbxqp.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.fehbvm.com/Article/details/gaqvlituw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.hesvh.cn/Article/details/gnrjyfgcq.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.fehbvm.com/Article/details/gmhhlpwmt.sHtML

TS:   [...arr];
来源：http://m.share.zdbjq.cn/Article/details/gbwypqhml.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.zdbjq.cn/Article/details/gbesfygfg.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.fehbvm.com/Article/details/goijzfhyh.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.hesvh.cn/Article/details/gkakdriwa.sHtML

C#:   new List<int>(list);
来源：http://read.share.zdbjq.cn/Article/details/gtlkzemyl.sHtML

[D23] reduce 累积计算
来源：http://mobile.zdbjq.cn/Article/details/ghxfzrunu.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/ggkjuibil.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.zdbjq.cn/Article/details/gidzrqljd.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/gvvazyjft.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/gpxdqplxb.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.fehbvm.com/Article/details/gehkrcktn.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/gfhnwccqc.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.hesvh.cn/Article/details/gphmxuhwg.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.hesvh.cn/Article/details/gpedcuezy.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.zdbjq.cn/Article/details/gbaznoetk.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.fehbvm.com/Article/details/gspmgjgvf.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.fehbvm.com/Article/details/gwqrbyngc.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.zdbjq.cn/Article/details/grhzldrax.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/ggzodfhuy.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.hesvh.cn/Article/details/giftuwfmz.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.zdbjq.cn/Article/details/gbjvkyrik.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.fehbvm.com/Article/details/gvjhuelem.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.hesvh.cn/Article/details/gctpxcxhy.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.zdbjq.cn/Article/details/gafdyldzx.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.zdbjq.cn/Article/details/gtnjrxvkg.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.fehbvm.com/Article/details/gdistcpsa.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.hesvh.cn/Article/details/glctqqzmq.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.fehbvm.com/Article/details/gllfjuwbb.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.fehbvm.com/Article/details/geubuyrqr.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.zdbjq.cn/Article/details/gpkvmzwwv.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.hesvh.cn/Article/details/gyrubwksy.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.hesvh.cn/Article/details/gejwridol.sHtML

[D26] 数组转字符串
来源：http://baike.zdbjq.cn/Article/details/gzeoegfws.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.fehbvm.com/Article/details/gbezctibt.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.fehbvm.com/Article/details/gfjycyojz.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/geopourqj.sHtML

TS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gopjqfnxu.sHtML

Java: String.join(", ", list)
来源：http://3g.fehbvm.com/Article/details/gwasnfezv.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.fehbvm.com/Article/details/gxkewvjgj.sHtML

Ruby: arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gumwfrciu.sHtML

C#:   string.Join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gudhbxeok.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/geilvifnz.sHtML

E. 字符串处理
来源：http://wap.fehbvm.com/Article/details/gcvwvjxfz.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gwitwikho.sHtML

[E01] 拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gqywmqonp.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.fehbvm.com/Article/details/gmaogahzn.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.fehbvm.com/Article/details/gforxqaqw.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/gmufopdzq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/gsgtbtrgv.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.hesvh.cn/Article/details/gnagjxrxx.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.fehbvm.com/Article/details/gmtzkqgcu.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.hesvh.cn/Article/details/ghzxdirsc.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.hesvh.cn/Article/details/glmnwkdqm.sHtML

[E02] 重复字符串
来源：http://www.blog.zdbjq.cn/Article/details/gsnmvtddu.sHtML

Py:   "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/ghbmkmjxn.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.fehbvm.com/Article/details/gydkdlmpu.sHtML

JS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/grebdknld.sHtML

TS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gkrdamtan.sHtML

Java: "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gufoqxjtd.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.zdbjq.cn/Article/details/gazzzvspr.sHtML

Ruby: "ab" * 3
来源：http://m.share.hesvh.cn/Article/details/gortyipej.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.hesvh.cn/Article/details/glqnsvkwn.sHtML

[E03] 截取子串
来源：http://m.share.hesvh.cn/Article/details/gnmdgxexi.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.hesvh.cn/Article/details/gzvifgdec.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/glsxxgrte.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/grpqawowd.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gipdgqhah.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gyftiyncl.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.fehbvm.com/Article/details/gqjndvoas.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.zdbjq.cn/Article/details/grogkcvws.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.hesvh.cn/Article/details/gtzusybiq.sHtML

[E04] 查找子串位置
来源：http://www.blog.hesvh.cn/Article/details/grwzbpwzq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.fehbvm.com/Article/details/gyhybgrku.sHtML

PHP:  strpos($s, "x");
来源：http://blog.fehbvm.com/Article/details/gcbmzezkc.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.fehbvm.com/Article/details/gdouxvfom.sHtML

TS:   s.indexOf("x")
来源：http://3g.fehbvm.com/Article/details/girofveds.sHtML

Java: s.indexOf("x")
来源：http://www.share.fehbvm.com/Article/details/giptatlup.sHtML


<!-- 参考信息 -->