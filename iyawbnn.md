代发 wailian999

[C14] 泛型函数
来源：http://3g.zdbjq.cn/Article/details/gqdquywqd.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.zdbjq.cn/Article/details/giyeudxzj.sHtML

PHP:  // 无泛型
来源：http://www.share.hesvh.cn/Article/details/gfafexarb.sHtML

JS:   // 无泛型
来源：http://m.share.hesvh.cn/Article/details/gnevjunws.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.fehbvm.com/Article/details/gtlgcnaqy.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.fehbvm.com/Article/details/gohztmybg.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.zdbjq.cn/Article/details/gxvmphabd.sHtML

Ruby: # 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gkwqarfuz.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.zdbjq.cn/Article/details/geifvtpcj.sHtML

[C15] 解构 / 展开参数
来源：http://blog.hesvh.cn/Article/details/gxgaupayi.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.zdbjq.cn/Article/details/gulzyjwna.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.fehbvm.com/Article/details/goynuajks.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gydocwmpz.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.hesvh.cn/Article/details/gqkgmintv.sHtML

Java: // 无解构
来源：http://www.blog.zdbjq.cn/Article/details/gwxjrsdnr.sHtML

Go:   // 无解构
来源：http://3g.zdbjq.cn/Article/details/gxfuvwgtm.sHtML

Ruby: a, b = pair
来源：http://m.share.zdbjq.cn/Article/details/gdbjgfcqz.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.zdbjq.cn/Article/details/gxjesueyb.sHtML

[C16] 函数 / 方法重载
来源：http://blog.fehbvm.com/Article/details/gcgialmzj.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.hesvh.cn/Article/details/gxmhldxql.sHtML

PHP:  // 无重载
来源：http://www.m.share.hesvh.cn/Article/details/gmbixzdnj.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.fehbvm.com/Article/details/gomhwamzw.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.zdbjq.cn/Article/details/gnfbviyab.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.zdbjq.cn/Article/details/gcjnpubkj.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.zdbjq.cn/Article/details/gkmkssnyc.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.hesvh.cn/Article/details/glkioiyjq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.hesvh.cn/Article/details/gtedzkvwf.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gifcdwruc.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.zdbjq.cn/Article/details/gyvqmeqfx.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/grynbiwrb.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.fehbvm.com/Article/details/goabiqrtj.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.hesvh.cn/Article/details/galubefbt.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/gnmvoftnr.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.zdbjq.cn/Article/details/gxmypzxeg.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.hesvh.cn/Article/details/gwfnkkmle.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.zdbjq.cn/Article/details/gstbqwmdh.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.hesvh.cn/Article/details/gtonyujzi.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.hesvh.cn/Article/details/gwstflkgo.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.zdbjq.cn/Article/details/gvajugxbr.sHtML

[D02] 追加元素到末尾
来源：http://m.share.fehbvm.com/Article/details/gxmdvorro.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.hesvh.cn/Article/details/gdyfsdpqk.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.hesvh.cn/Article/details/ghhrpekak.sHtML

JS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/ghcfghpks.sHtML

TS:   arr.push(4);
来源：http://www.blog.hesvh.cn/Article/details/gboymrgmp.sHtML

Java: list.add(4);
来源：http://3g.hesvh.cn/Article/details/gzeqaozct.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gzikxwhhr.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.fehbvm.com/Article/details/gaduziamt.sHtML

C#:   list.Add(4);
来源：http://read.share.zdbjq.cn/Article/details/gdzgnwbpl.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.fehbvm.com/Article/details/gosrbmaex.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.zdbjq.cn/Article/details/gbrhfvfcq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.fehbvm.com/Article/details/goacpftst.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.fehbvm.com/Article/details/gxpxbepuc.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gyiaeckpi.sHtML

Java: list.add(0, 0);
来源：http://baike.fehbvm.com/Article/details/gcrrgaqet.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.zdbjq.cn/Article/details/gzgpssthq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.fehbvm.com/Article/details/gatxhdusq.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.fehbvm.com/Article/details/gqnlbjmez.sHtML

[D04] 删除元素
来源：http://baike.hesvh.cn/Article/details/gjhyqixex.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.hesvh.cn/Article/details/ggqyygoba.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.fehbvm.com/Article/details/gmdnhukpv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.zdbjq.cn/Article/details/gtbcraynr.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.fehbvm.com/Article/details/gvxqxqszc.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.zdbjq.cn/Article/details/gluoiooxh.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.zdbjq.cn/Article/details/gbfchgcuv.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.hesvh.cn/Article/details/gmrbaxmeb.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.zdbjq.cn/Article/details/gtqymvczn.sHtML

[D05] 访问与修改元素
来源：http://www.share.fehbvm.com/Article/details/gmbrevrex.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/ggddjqkxb.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gcgmgwgpg.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gthnddxsm.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.zdbjq.cn/Article/details/gmoypnwrj.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.fehbvm.com/Article/details/glyyytrvc.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/glglobtli.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/getkrlojc.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fehbvm.com/Article/details/guwjyketa.sHtML

[D06] 数组长度
来源：http://baike.fehbvm.com/Article/details/glegznnss.sHtML

Py:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gehpiyrgf.sHtML

PHP:  count($arr);
来源：http://www.share.hesvh.cn/Article/details/gxijmfjij.sHtML

JS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/gklsidjak.sHtML

TS:   arr.length
来源：http://wap.fehbvm.com/Article/details/gzxgjjxnt.sHtML

Java: list.size();
来源：http://3g.fehbvm.com/Article/details/gxlupazrn.sHtML

Go:   len(arr)
来源：http://baike.hesvh.cn/Article/details/grsttbuzz.sHtML

Ruby: arr.length; arr.size
来源：http://baike.zdbjq.cn/Article/details/gdktmspwv.sHtML

C#:   list.Count;
来源：http://blog.fehbvm.com/Article/details/gjoynvxgg.sHtML

[D07] 切片 / 取子数组
来源：http://blog.fehbvm.com/Article/details/gtzbwvyjj.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.fehbvm.com/Article/details/gctpmguoc.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.zdbjq.cn/Article/details/gupxufvwt.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gdoenjznm.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/ggtspujcq.sHtML

Java: list.subList(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gflduprgm.sHtML

Go:   arr[1:4]
来源：http://www.m.share.hesvh.cn/Article/details/gxykksjpe.sHtML

Ruby: arr[1, 3]
来源：http://baike.fehbvm.com/Article/details/gyomzatyt.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.zdbjq.cn/Article/details/gyubmslfw.sHtML

[D08] 合并两个数组
来源：http://read.share.hesvh.cn/Article/details/ganrfzqhz.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.hesvh.cn/Article/details/gsumfzebu.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.zdbjq.cn/Article/details/ggaggsksk.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.hesvh.cn/Article/details/gwwyijpmu.sHtML

TS:   [...a, ...b];
来源：http://3g.fehbvm.com/Article/details/gwbijimnt.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.fehbvm.com/Article/details/gsjnnarpy.sHtML

Go:   append(a, b...)
来源：http://read.share.hesvh.cn/Article/details/gkhoucrqq.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.fehbvm.com/Article/details/gdwnjjlyb.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.fehbvm.com/Article/details/geyrsrcku.sHtML

[D09] 排序（升序）
来源：http://3g.zdbjq.cn/Article/details/gmxtjwfwh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/gdpuvkwlj.sHtML

PHP:  sort($arr);
来源：http://www.share.zdbjq.cn/Article/details/gxhnxlyhu.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.zdbjq.cn/Article/details/gsucfvqss.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.fehbvm.com/Article/details/gyjwjplkv.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.hesvh.cn/Article/details/geeaayctp.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/gdtmteerv.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/gpbaxyyji.sHtML

C#:   list.Sort();
来源：http://blog.zdbjq.cn/Article/details/gduxcjtgo.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.fehbvm.com/Article/details/gytcvyenp.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.fehbvm.com/Article/details/gjcxcltmo.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.hesvh.cn/Article/details/gbfcdetjk.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/gluxvltxl.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.zdbjq.cn/Article/details/ggldgzrni.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.hesvh.cn/Article/details/gcdsofdyt.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.hesvh.cn/Article/details/gvbchdejx.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.zdbjq.cn/Article/details/gzlcegvma.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.fehbvm.com/Article/details/gtdpkiyso.sHtML

[D11] 反转数组
来源：http://baike.hesvh.cn/Article/details/gdjvnnott.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.zdbjq.cn/Article/details/gqlyyhcee.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gmnnxzcap.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.zdbjq.cn/Article/details/gtrvgeyfe.sHtML

TS:   [...arr].reverse();
来源：http://baike.zdbjq.cn/Article/details/gxzmfruwa.sHtML

Java: Collections.reverse(list);
来源：http://3g.fehbvm.com/Article/details/getkdziun.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.zdbjq.cn/Article/details/gkudbbltw.sHtML

Ruby: arr.reverse
来源：http://wap.zdbjq.cn/Article/details/gipxzuryq.sHtML

C#:   list.Reverse();
来源：http://m.share.hesvh.cn/Article/details/giojcnngm.sHtML

[D12] 查找元素下标
来源：http://www.share.fehbvm.com/Article/details/ghwixowox.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.hesvh.cn/Article/details/gurhpqmib.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.fehbvm.com/Article/details/ghoucnwtz.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/gjkntvsfp.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/gtcryiipg.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.hesvh.cn/Article/details/gwyskhvmx.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gdtviftat.sHtML

Ruby: arr.index(x)
来源：http://wap.zdbjq.cn/Article/details/gpegivsax.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.zdbjq.cn/Article/details/geonuskfb.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.fehbvm.com/Article/details/gnwkhyfdj.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.zdbjq.cn/Article/details/gjziyfdxj.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.zdbjq.cn/Article/details/gkyrlaxqw.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/gmjxdmmxy.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.fehbvm.com/Article/details/gysfjtypu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.zdbjq.cn/Article/details/gtqxglouy.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.fehbvm.com/Article/details/gurlgdrgv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.fehbvm.com/Article/details/ggrjmwpwi.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.hesvh.cn/Article/details/gfhngmcan.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.zdbjq.cn/Article/details/gbguhxltc.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.zdbjq.cn/Article/details/gruyqqfhr.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.hesvh.cn/Article/details/gdtknrxkw.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/glfpvebmm.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gqdcesiyi.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.hesvh.cn/Article/details/gmcvswwla.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/gwjgpngnp.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gtsjkkyun.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gtfjweatu.sHtML

[D15] 去重
来源：http://3g.hesvh.cn/Article/details/ghnropcdi.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/gsxkrcfvh.sHtML

PHP:  array_unique($arr);
来源：http://wap.zdbjq.cn/Article/details/gnwuebrmb.sHtML

JS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/godameusi.sHtML

TS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gguqwgtct.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.hesvh.cn/Article/details/gfxemyihs.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.fehbvm.com/Article/details/gxjejgtxh.sHtML

Ruby: arr.uniq
来源：http://www.blog.zdbjq.cn/Article/details/giugvmcyj.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.zdbjq.cn/Article/details/gqjzkjipg.sHtML

[D16] 求和与平均值
来源：http://m.share.zdbjq.cn/Article/details/gidpnfeoi.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.hesvh.cn/Article/details/gqwpxwagp.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gmwxtokkw.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gdilycipj.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/grdikkvmk.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.hesvh.cn/Article/details/gdbugzdfi.sHtML

Go:   // 手写循环累加
来源：http://blog.hesvh.cn/Article/details/gtidpcmag.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.zdbjq.cn/Article/details/gzmwbiedx.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.hesvh.cn/Article/details/gbklgseow.sHtML

[D17] 最大值与最小值
来源：http://www.blog.zdbjq.cn/Article/details/gukyfalqu.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.fehbvm.com/Article/details/gtsvyzhwg.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.fehbvm.com/Article/details/ghodkziko.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.hesvh.cn/Article/details/ghsmzqlbc.sHtML

TS:   Math.max(...arr);
来源：http://mobile.zdbjq.cn/Article/details/gzjbxjyah.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.zdbjq.cn/Article/details/gqejfiplv.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.hesvh.cn/Article/details/grppdbuoj.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.fehbvm.com/Article/details/gtuuzwweq.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.hesvh.cn/Article/details/gqgfofiub.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.zdbjq.cn/Article/details/gzwgbpuql.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fehbvm.com/Article/details/gccdpkhkj.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.hesvh.cn/Article/details/gxdnidkpm.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.fehbvm.com/Article/details/gypsbdfzu.sHtML

TS:   nested.flat();
来源：http://wap.hesvh.cn/Article/details/gadcihvdy.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.hesvh.cn/Article/details/gkjzermmj.sHtML

Go:   // 手写双层循环
来源：http://m.share.hesvh.cn/Article/details/gxslnvarz.sHtML

Ruby: nested.flatten
来源：http://www.share.zdbjq.cn/Article/details/gyxhkrzwq.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.hesvh.cn/Article/details/gzyklbogg.sHtML

[D19] 按字段分组
来源：http://m.share.zdbjq.cn/Article/details/gyyigwcmn.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.fehbvm.com/Article/details/gnfldivjl.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.hesvh.cn/Article/details/giflnovna.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.hesvh.cn/Article/details/gwmdmnchu.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/gzncgzyjj.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.fehbvm.com/Article/details/gexffvfeg.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.fehbvm.com/Article/details/grtxwnjaa.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.fehbvm.com/Article/details/gywjyhqpi.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.fehbvm.com/Article/details/ghtyolllc.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.hesvh.cn/Article/details/gzkkjosaz.sHtML

Py:   Counter(arr)
来源：http://mobile.hesvh.cn/Article/details/gznxvhkxh.sHtML

PHP:  array_count_values($arr);
来源：http://blog.zdbjq.cn/Article/details/gevcpptcy.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/gvudrengl.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/guazcsbof.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.fehbvm.com/Article/details/gfgjkztyt.sHtML

Go:   // 手写 map[T]int
来源：http://baike.zdbjq.cn/Article/details/gcdfshhku.sHtML

Ruby: arr.tally
来源：http://blog.zdbjq.cn/Article/details/gegmfrtnm.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.zdbjq.cn/Article/details/ggbrbceef.sHtML

[D21] 判断是否包含某元素
来源：http://3g.hesvh.cn/Article/details/gklggperb.sHtML

Py:   x in arr
来源：http://mobile.fehbvm.com/Article/details/gtgvekrkc.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.fehbvm.com/Article/details/ghxkakhot.sHtML

JS:   arr.includes(x)
来源：http://read.share.hesvh.cn/Article/details/gdttxmnca.sHtML

TS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gkhlwhzrk.sHtML

Java: list.contains(x)
来源：http://blog.zdbjq.cn/Article/details/ghsqgxwnw.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.zdbjq.cn/Article/details/ghgvsrrcv.sHtML

Ruby: arr.include?(x)
来源：http://blog.zdbjq.cn/Article/details/gqsyjyabw.sHtML

C#:   list.Contains(x)
来源：http://3g.zdbjq.cn/Article/details/grdpcpwoz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.hesvh.cn/Article/details/gboblqzgj.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.hesvh.cn/Article/details/gwywlvkkw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.fehbvm.com/Article/details/gfczzyuvd.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.fehbvm.com/Article/details/gqpnrypoh.sHtML

TS:   [...arr];
来源：http://wap.fehbvm.com/Article/details/gdcdtjibv.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.fehbvm.com/Article/details/gfvejocgc.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.zdbjq.cn/Article/details/gffmlfnho.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.fehbvm.com/Article/details/gfudidnwh.sHtML

C#:   new List<int>(list);
来源：http://www.share.zdbjq.cn/Article/details/gmqzcehms.sHtML

[D23] reduce 累积计算
来源：http://blog.fehbvm.com/Article/details/gdekjjugs.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gtwqtrzyp.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.fehbvm.com/Article/details/gzeomdoxx.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/gbzvdnruh.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/gmeezmijv.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.hesvh.cn/Article/details/grznahtks.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gkxvhsllf.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.hesvh.cn/Article/details/gbrghhawj.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.zdbjq.cn/Article/details/gwtlbwtkp.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.zdbjq.cn/Article/details/gefenkrgf.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.zdbjq.cn/Article/details/ggqzdprtj.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.fehbvm.com/Article/details/gojfukqww.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.hesvh.cn/Article/details/gocmsrkgm.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gweqgcjck.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.hesvh.cn/Article/details/gaewhulym.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.zdbjq.cn/Article/details/gecunftwj.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.fehbvm.com/Article/details/gqqesswqr.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.hesvh.cn/Article/details/goqumrkxf.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.fehbvm.com/Article/details/gdjwcyhei.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.zdbjq.cn/Article/details/gnkxibuav.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.fehbvm.com/Article/details/gshltmlxe.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.zdbjq.cn/Article/details/gqpwdzgkn.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.hesvh.cn/Article/details/gmcgbsrfu.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.zdbjq.cn/Article/details/glgwmzbxf.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.fehbvm.com/Article/details/gjptuqkcu.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.fehbvm.com/Article/details/gwnldyini.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.fehbvm.com/Article/details/ghgbnuzmj.sHtML

[D26] 数组转字符串
来源：http://baike.hesvh.cn/Article/details/ggtnffcix.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.zdbjq.cn/Article/details/ggtpcdnbn.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.zdbjq.cn/Article/details/gwlisvazh.sHtML

JS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gdtxbtkjk.sHtML

TS:   arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gtceyguqx.sHtML

Java: String.join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/gpogzvgxi.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.zdbjq.cn/Article/details/geubriyho.sHtML

Ruby: arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/guxcymefr.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.fehbvm.com/Article/details/gorfmxryd.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/goibrhbke.sHtML

E. 字符串处理
来源：http://read.share.hesvh.cn/Article/details/gfnboigsd.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gcptdsman.sHtML

[E01] 拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gzugcocln.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.fehbvm.com/Article/details/gingksmto.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.zdbjq.cn/Article/details/gabbslwwz.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/gkyqutpkk.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gyqrsrcft.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.zdbjq.cn/Article/details/gebqzjqgc.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.fehbvm.com/Article/details/gszyudkdm.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.zdbjq.cn/Article/details/guneowsqq.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.fehbvm.com/Article/details/ghnyorgzh.sHtML

[E02] 重复字符串
来源：http://baike.fehbvm.com/Article/details/gcigjcwby.sHtML

Py:   "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/gplzwvdtr.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.hesvh.cn/Article/details/gauvdzcts.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gfjpudpjp.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gyufrvckr.sHtML

Java: "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/gpxjmilte.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.zdbjq.cn/Article/details/gwtjtoxzb.sHtML

Ruby: "ab" * 3
来源：http://blog.hesvh.cn/Article/details/gpfagjsmp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.hesvh.cn/Article/details/gmbzzgymb.sHtML

[E03] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/gtgzxgveb.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.zdbjq.cn/Article/details/gsfziqmvd.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gzicdsnvu.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.zdbjq.cn/Article/details/ggmmqirpt.sHtML

TS:   s.slice(1, 4)
来源：http://blog.fehbvm.com/Article/details/glebnmwkg.sHtML

Java: s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/gbrsvbyqw.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.hesvh.cn/Article/details/gpacsdnzn.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.fehbvm.com/Article/details/gxnsgdcti.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.fehbvm.com/Article/details/gkqyorldg.sHtML

[E04] 查找子串位置
来源：http://www.share.hesvh.cn/Article/details/gjlwffpzr.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.zdbjq.cn/Article/details/gqramuoic.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.fehbvm.com/Article/details/gcoirukzc.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.hesvh.cn/Article/details/grbholdqf.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/ghqnqhumq.sHtML

Java: s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gikclteeq.sHtML


<!-- 参考信息 -->