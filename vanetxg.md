代发 wailian999

[C14] 泛型函数
来源：http://read.share.hesvh.cn/Article/details/gxvvuvjsl.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.fehbvm.com/Article/details/gqewjydtx.sHtML

PHP:  // 无泛型
来源：http://blog.zdbjq.cn/Article/details/giikxnobq.sHtML

JS:   // 无泛型
来源：http://wap.fehbvm.com/Article/details/gnuijtxdr.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.zdbjq.cn/Article/details/gnghftlyi.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.hesvh.cn/Article/details/gbsczjxrw.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.zdbjq.cn/Article/details/gkshxmrig.sHtML

Ruby: # 无泛型
来源：http://www.share.hesvh.cn/Article/details/gclrkscpa.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.hesvh.cn/Article/details/gwwdyjlab.sHtML

[C15] 解构 / 展开参数
来源：http://wap.hesvh.cn/Article/details/giuslnjzx.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.hesvh.cn/Article/details/gybvaorgw.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.fehbvm.com/Article/details/gkrvmzrom.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.fehbvm.com/Article/details/ghntiyady.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.fehbvm.com/Article/details/gkstaxeph.sHtML

Java: // 无解构
来源：http://blog.zdbjq.cn/Article/details/gwxjuabul.sHtML

Go:   // 无解构
来源：http://wap.fehbvm.com/Article/details/gijygrgqc.sHtML

Ruby: a, b = pair
来源：http://baike.hesvh.cn/Article/details/glhkaiypx.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.fehbvm.com/Article/details/gbyrdhbvi.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.zdbjq.cn/Article/details/gdqwgnkyp.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.zdbjq.cn/Article/details/gtcanhwcd.sHtML

PHP:  // 无重载
来源：http://www.blog.fehbvm.com/Article/details/gehrbbkeh.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.zdbjq.cn/Article/details/gvoedckgt.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.fehbvm.com/Article/details/gpikpegli.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.fehbvm.com/Article/details/gjeedgvub.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.hesvh.cn/Article/details/gqurpgabv.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.fehbvm.com/Article/details/gsycyazvk.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.hesvh.cn/Article/details/gxwjdvobc.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ghwibkkhm.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.zdbjq.cn/Article/details/gqiybwhbj.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gaxpvxxvt.sHtML

[D01] 创建数组 / 列表
来源：http://blog.zdbjq.cn/Article/details/gjvqawzkm.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.fehbvm.com/Article/details/gkrjeecji.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.hesvh.cn/Article/details/gtqrvycxz.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/gtoxbsdix.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.zdbjq.cn/Article/details/gsbxkvier.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.fehbvm.com/Article/details/gygrbmgoz.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.fehbvm.com/Article/details/gyrlzkpvl.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.hesvh.cn/Article/details/gwvtrsgtw.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.zdbjq.cn/Article/details/goiwntazg.sHtML

[D02] 追加元素到末尾
来源：http://3g.hesvh.cn/Article/details/geqbwsjow.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.zdbjq.cn/Article/details/gssgzmtpp.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.hesvh.cn/Article/details/gprcgtypt.sHtML

JS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/gptgjgkxd.sHtML

TS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/gyobfxbhc.sHtML

Java: list.add(4);
来源：http://read.share.zdbjq.cn/Article/details/gzkwoypzm.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.hesvh.cn/Article/details/gquofzioq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.hesvh.cn/Article/details/glgimmbpz.sHtML

C#:   list.Add(4);
来源：http://3g.zdbjq.cn/Article/details/gebhckgja.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.hesvh.cn/Article/details/gnhktafnt.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.fehbvm.com/Article/details/gkzkdvzzd.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.fehbvm.com/Article/details/gtijcgful.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.zdbjq.cn/Article/details/goktoclmv.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.hesvh.cn/Article/details/gnvefisog.sHtML

Java: list.add(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gimxmfjab.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.zdbjq.cn/Article/details/gtdkypsdw.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.zdbjq.cn/Article/details/gobsmfznx.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.fehbvm.com/Article/details/gifzjbhal.sHtML

[D04] 删除元素
来源：http://www.blog.fehbvm.com/Article/details/geucyqegw.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.hesvh.cn/Article/details/gpccqjeaa.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gjpxsafsk.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.hesvh.cn/Article/details/gdcvhejbe.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.zdbjq.cn/Article/details/gvkllrotl.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.fehbvm.com/Article/details/glpmzcwbe.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.fehbvm.com/Article/details/gscaibvgj.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.zdbjq.cn/Article/details/gajkqcxyy.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.fehbvm.com/Article/details/gwczysnga.sHtML

[D05] 访问与修改元素
来源：http://3g.fehbvm.com/Article/details/gyytehdfz.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gpihukyfo.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gwtgwvivi.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gzimspkrk.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.hesvh.cn/Article/details/gkjkfschb.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.fehbvm.com/Article/details/gwyoajxjo.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/ggxkengdm.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gttukngiu.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/glanxwodo.sHtML

[D06] 数组长度
来源：http://blog.fehbvm.com/Article/details/ghnidxqsv.sHtML

Py:   len(arr)
来源：http://blog.fehbvm.com/Article/details/gqzkapkux.sHtML

PHP:  count($arr);
来源：http://blog.fehbvm.com/Article/details/grxggzfpf.sHtML

JS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/gsgqpvsnj.sHtML

TS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/goiawmchb.sHtML

Java: list.size();
来源：http://www.m.share.zdbjq.cn/Article/details/gpcfdldtk.sHtML

Go:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gywqmuexi.sHtML

Ruby: arr.length; arr.size
来源：http://3g.hesvh.cn/Article/details/gbtigjxdq.sHtML

C#:   list.Count;
来源：http://baike.fehbvm.com/Article/details/gygmhyndx.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.fehbvm.com/Article/details/gzwzdacub.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.zdbjq.cn/Article/details/gpkubflfz.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gqxzbmgyu.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gvaiwkcju.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gfphuonuh.sHtML

Java: list.subList(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gjqdrkmgu.sHtML

Go:   arr[1:4]
来源：http://3g.hesvh.cn/Article/details/gtybajgif.sHtML

Ruby: arr[1, 3]
来源：http://mobile.fehbvm.com/Article/details/guwwuyipg.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.zdbjq.cn/Article/details/gdfynsfhv.sHtML

[D08] 合并两个数组
来源：http://blog.fehbvm.com/Article/details/gxldpuxwi.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.hesvh.cn/Article/details/gylivywsm.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.zdbjq.cn/Article/details/gczpejogp.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.fehbvm.com/Article/details/gmgxotimr.sHtML

TS:   [...a, ...b];
来源：http://wap.zdbjq.cn/Article/details/gydarrdng.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.hesvh.cn/Article/details/gespzhrac.sHtML

Go:   append(a, b...)
来源：http://www.share.zdbjq.cn/Article/details/gspgxdcdq.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.zdbjq.cn/Article/details/guhcabtnr.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.hesvh.cn/Article/details/gzfjvcbcw.sHtML

[D09] 排序（升序）
来源：http://wap.zdbjq.cn/Article/details/glvuhztti.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/gwyiurcwv.sHtML

PHP:  sort($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gqyfkyvhu.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.zdbjq.cn/Article/details/gmidanqng.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.zdbjq.cn/Article/details/gobxxodlz.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.zdbjq.cn/Article/details/gppkzlbjz.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gafjavfqc.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/gbxixcczp.sHtML

C#:   list.Sort();
来源：http://www.blog.hesvh.cn/Article/details/gxpctgwnk.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.fehbvm.com/Article/details/gidfrqbqx.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.hesvh.cn/Article/details/ghsjtftcv.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/gzdbbcidj.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gyezmpbtl.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/gfsckaqpc.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.hesvh.cn/Article/details/gnlctuwcx.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.fehbvm.com/Article/details/gvoysrdxg.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.fehbvm.com/Article/details/guduzujsf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.hesvh.cn/Article/details/gyjwbytgr.sHtML

[D11] 反转数组
来源：http://wap.hesvh.cn/Article/details/gteqqoxow.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.hesvh.cn/Article/details/gdpcjfsuj.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.hesvh.cn/Article/details/gtbmhkpdj.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.hesvh.cn/Article/details/golrbmfhd.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.fehbvm.com/Article/details/gjlxygpzd.sHtML

Java: Collections.reverse(list);
来源：http://wap.hesvh.cn/Article/details/ggmcborkp.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.hesvh.cn/Article/details/gfdaffnow.sHtML

Ruby: arr.reverse
来源：http://blog.zdbjq.cn/Article/details/ghnwtphwv.sHtML

C#:   list.Reverse();
来源：http://m.share.fehbvm.com/Article/details/gfoaqwtzw.sHtML

[D12] 查找元素下标
来源：http://mobile.fehbvm.com/Article/details/gnsoyvrmp.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.hesvh.cn/Article/details/gbjktchjc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.hesvh.cn/Article/details/gjrgaazuf.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/glmcnsimt.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/gyaitymmj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.zdbjq.cn/Article/details/gnvklmyra.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gcmntrnrc.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.fehbvm.com/Article/details/gmrsnyrqi.sHtML

C#:   list.IndexOf(x);
来源：http://blog.zdbjq.cn/Article/details/ggokpgrtj.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.zdbjq.cn/Article/details/gktamnpts.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.hesvh.cn/Article/details/gcgcyeytb.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.fehbvm.com/Article/details/gfuzlqlof.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gfbxruoit.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/getwqcphe.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.fehbvm.com/Article/details/gkbibriag.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.zdbjq.cn/Article/details/gkkubjubf.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.zdbjq.cn/Article/details/gcgxxfupn.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.hesvh.cn/Article/details/gcgwcwzbh.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.zdbjq.cn/Article/details/gjchobxop.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.zdbjq.cn/Article/details/gtfcvaakn.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.hesvh.cn/Article/details/gguotynnp.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gxdodbxzt.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/guqbkdfcl.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.fehbvm.com/Article/details/gtvddpjau.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/gmryfdolc.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.fehbvm.com/Article/details/gkpycxrbp.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.zdbjq.cn/Article/details/ghtwlweou.sHtML

[D15] 去重
来源：http://mobile.zdbjq.cn/Article/details/gjzyyvhed.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/gcifietpb.sHtML

PHP:  array_unique($arr);
来源：http://wap.hesvh.cn/Article/details/guvsvvrly.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gijyttbgi.sHtML

TS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/geawskrqa.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.zdbjq.cn/Article/details/gyiieijrs.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.zdbjq.cn/Article/details/grbndvitn.sHtML

Ruby: arr.uniq
来源：http://3g.zdbjq.cn/Article/details/gcfmgmzpi.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.hesvh.cn/Article/details/guavpyjih.sHtML

[D16] 求和与平均值
来源：http://blog.hesvh.cn/Article/details/glkuouwir.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.hesvh.cn/Article/details/gbprmjykg.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.fehbvm.com/Article/details/glidttyza.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gcqjnzhml.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gqinsyits.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.fehbvm.com/Article/details/gkkgwgxdw.sHtML

Go:   // 手写循环累加
来源：http://read.share.zdbjq.cn/Article/details/gukymcrlv.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.zdbjq.cn/Article/details/gkpzspwue.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.zdbjq.cn/Article/details/gfrfskynq.sHtML

[D17] 最大值与最小值
来源：http://3g.zdbjq.cn/Article/details/gqcwmcgzi.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.fehbvm.com/Article/details/gzzmzzbwn.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gxyvzndtt.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.hesvh.cn/Article/details/gauofzzxm.sHtML

TS:   Math.max(...arr);
来源：http://wap.hesvh.cn/Article/details/gimrtozde.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.fehbvm.com/Article/details/gbsqccier.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.hesvh.cn/Article/details/grxyrtuzv.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.fehbvm.com/Article/details/gjwkdefut.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.zdbjq.cn/Article/details/gdnruuwzn.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.hesvh.cn/Article/details/genhifszz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.fehbvm.com/Article/details/gavejaydq.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.hesvh.cn/Article/details/glymbzeuw.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.fehbvm.com/Article/details/glkqxxnmg.sHtML

TS:   nested.flat();
来源：http://blog.hesvh.cn/Article/details/gtjtfzibh.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.fehbvm.com/Article/details/geqvszeqx.sHtML

Go:   // 手写双层循环
来源：http://www.share.fehbvm.com/Article/details/gufwxrciy.sHtML

Ruby: nested.flatten
来源：http://blog.hesvh.cn/Article/details/gagucqhgv.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.hesvh.cn/Article/details/gqfxfxaon.sHtML

[D19] 按字段分组
来源：http://baike.hesvh.cn/Article/details/gksuaxrwc.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.zdbjq.cn/Article/details/gkyvbuljf.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.fehbvm.com/Article/details/gtdwqecpl.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.hesvh.cn/Article/details/gipebvosh.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.hesvh.cn/Article/details/gcskbsneh.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.hesvh.cn/Article/details/geumvkexp.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.zdbjq.cn/Article/details/gqxkkxhut.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.fehbvm.com/Article/details/gqdsbxzem.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.zdbjq.cn/Article/details/gxbldxpfs.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.hesvh.cn/Article/details/ggamwnvet.sHtML

Py:   Counter(arr)
来源：http://www.share.zdbjq.cn/Article/details/ggqfkahso.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.fehbvm.com/Article/details/gwjydzfip.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/grmljghrm.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/gzafadybs.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.fehbvm.com/Article/details/gynfwcpok.sHtML

Go:   // 手写 map[T]int
来源：http://wap.zdbjq.cn/Article/details/gffyqlvil.sHtML

Ruby: arr.tally
来源：http://wap.hesvh.cn/Article/details/gxykruerj.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.fehbvm.com/Article/details/gqizrodnf.sHtML

[D21] 判断是否包含某元素
来源：http://baike.fehbvm.com/Article/details/gigzxtmye.sHtML

Py:   x in arr
来源：http://www.blog.hesvh.cn/Article/details/gluotxszb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.fehbvm.com/Article/details/gcvvgjkum.sHtML

JS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gelmxndog.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gcdomajjv.sHtML

Java: list.contains(x)
来源：http://blog.hesvh.cn/Article/details/gczemuouh.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.hesvh.cn/Article/details/gbbutthpe.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.zdbjq.cn/Article/details/gjmmtvjgg.sHtML

C#:   list.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gqfgcwexo.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.hesvh.cn/Article/details/gjhualktw.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.hesvh.cn/Article/details/guynfzmdi.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.zdbjq.cn/Article/details/gveqpzzak.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.fehbvm.com/Article/details/gxojmxkrb.sHtML

TS:   [...arr];
来源：http://www.share.hesvh.cn/Article/details/gekalkjqo.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.fehbvm.com/Article/details/gurqhusys.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.hesvh.cn/Article/details/gqkwoftlk.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.hesvh.cn/Article/details/grirytvfc.sHtML

C#:   new List<int>(list);
来源：http://mobile.hesvh.cn/Article/details/geestasqr.sHtML

[D23] reduce 累积计算
来源：http://read.share.hesvh.cn/Article/details/glkrwpopo.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.hesvh.cn/Article/details/glycudjaf.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.zdbjq.cn/Article/details/gcqygxbnf.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gnxvxoblv.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.hesvh.cn/Article/details/guvxmgiwp.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.hesvh.cn/Article/details/gktxvpjbd.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/gucqbfsrm.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.hesvh.cn/Article/details/ghdxutpse.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.hesvh.cn/Article/details/gfiyqxhhl.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.fehbvm.com/Article/details/glmalbuiz.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.hesvh.cn/Article/details/gdwmneean.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.fehbvm.com/Article/details/gxxnjwgtt.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.fehbvm.com/Article/details/ggzlpeeqx.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.zdbjq.cn/Article/details/ghboznhgl.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.fehbvm.com/Article/details/ghhskxwdv.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.zdbjq.cn/Article/details/grlleezrt.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.fehbvm.com/Article/details/gdoebjfzj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.hesvh.cn/Article/details/gdsbcqvct.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.hesvh.cn/Article/details/gueonefdg.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.hesvh.cn/Article/details/gzfatzvxp.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.fehbvm.com/Article/details/gffshkgvs.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.fehbvm.com/Article/details/gpigvhcon.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.zdbjq.cn/Article/details/gwptqpqfy.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.zdbjq.cn/Article/details/gamgwdxbz.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.hesvh.cn/Article/details/gknabpmpg.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.fehbvm.com/Article/details/gytaeqhec.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.fehbvm.com/Article/details/gszejqbej.sHtML

[D26] 数组转字符串
来源：http://www.blog.fehbvm.com/Article/details/gynequoii.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.zdbjq.cn/Article/details/glfpkxfsk.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.hesvh.cn/Article/details/gfcyracwc.sHtML

JS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gafwkgprq.sHtML

TS:   arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gyonxbjgu.sHtML

Java: String.join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/gqivthhgl.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.fehbvm.com/Article/details/gxvqxfgpq.sHtML

Ruby: arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gjqayyjbh.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/genblpaik.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gporpbzjz.sHtML

E. 字符串处理
来源：http://baike.hesvh.cn/Article/details/gjtrtyvzm.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqrtrgpcm.sHtML

[E01] 拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gdhajirzz.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.fehbvm.com/Article/details/ghqukdjiq.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.fehbvm.com/Article/details/gffaclgnn.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/gkqmbejga.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/ghgtaemut.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.fehbvm.com/Article/details/gcvkokdiy.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gokexdlux.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.zdbjq.cn/Article/details/gxuwqjfnf.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.fehbvm.com/Article/details/gxvmodeys.sHtML

[E02] 重复字符串
来源：http://baike.fehbvm.com/Article/details/gymwoigwi.sHtML

Py:   "ab" * 3
来源：http://baike.hesvh.cn/Article/details/gutudzefx.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.fehbvm.com/Article/details/gtwctznpb.sHtML

JS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gzfzmluly.sHtML

TS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/glnddkmii.sHtML

Java: "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/geyjcceai.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.zdbjq.cn/Article/details/giqzaluoj.sHtML

Ruby: "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/gdhxgfsft.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.zdbjq.cn/Article/details/goxymobny.sHtML

[E03] 截取子串
来源：http://read.share.fehbvm.com/Article/details/gbeuzvsaa.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.fehbvm.com/Article/details/gocdoaaru.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gvdwtsgug.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/gctnjfews.sHtML

TS:   s.slice(1, 4)
来源：http://baike.hesvh.cn/Article/details/gbsnzfkxw.sHtML

Java: s.substring(1, 4)
来源：http://blog.zdbjq.cn/Article/details/ghprgnaal.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gkmmvtsqr.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.zdbjq.cn/Article/details/gqilfokqi.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.fehbvm.com/Article/details/gvwwwsgoo.sHtML

[E04] 查找子串位置
来源：http://blog.fehbvm.com/Article/details/gvhsnmaoz.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.zdbjq.cn/Article/details/gzdmtaiol.sHtML

PHP:  strpos($s, "x");
来源：http://3g.zdbjq.cn/Article/details/gbuxifhwo.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.hesvh.cn/Article/details/ggdbvvdzb.sHtML

TS:   s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/glctoseul.sHtML

Java: s.indexOf("x")
来源：http://baike.hesvh.cn/Article/details/giaotcgjj.sHtML


<!-- 参考信息 -->