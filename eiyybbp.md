代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gwgfxvnbj.sHtML

Go:   func add(a, b int) int
来源：http://www.share.hesvh.cn/Article/details/goysuoeck.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.zdbjq.cn/Article/details/gpylvqgdw.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.zdbjq.cn/Article/details/gbtmmgeph.sHtML

[C14] 泛型函数
来源：http://mobile.fehbvm.com/Article/details/gfszuwkmn.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.hesvh.cn/Article/details/gffzbemtv.sHtML

PHP:  // 无泛型
来源：http://read.share.hesvh.cn/Article/details/gvllmnezd.sHtML

JS:   // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gpcdkoizy.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.fehbvm.com/Article/details/gejjclaxt.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.zdbjq.cn/Article/details/gzmqtuwhr.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.zdbjq.cn/Article/details/gsptoxkdg.sHtML

Ruby: # 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gffchotff.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.hesvh.cn/Article/details/gwedpqlgr.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.hesvh.cn/Article/details/gvbyczadx.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.zdbjq.cn/Article/details/gpekovqzy.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.hesvh.cn/Article/details/glriauivh.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.zdbjq.cn/Article/details/grcarborl.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.fehbvm.com/Article/details/gkivducfg.sHtML

Java: // 无解构
来源：http://www.blog.fehbvm.com/Article/details/gukscpgmv.sHtML

Go:   // 无解构
来源：http://mobile.hesvh.cn/Article/details/gnegcarus.sHtML

Ruby: a, b = pair
来源：http://wap.zdbjq.cn/Article/details/gchupnlkg.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.fehbvm.com/Article/details/gmfelbqou.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.zdbjq.cn/Article/details/gcusffryl.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.hesvh.cn/Article/details/gxuxavcar.sHtML

PHP:  // 无重载
来源：http://3g.hesvh.cn/Article/details/gxqzedldi.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.fehbvm.com/Article/details/gfihbqhmx.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.fehbvm.com/Article/details/gcbvdnnat.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.hesvh.cn/Article/details/gtffqevtd.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.zdbjq.cn/Article/details/gnqremdoq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.hesvh.cn/Article/details/gzfiknurg.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.fehbvm.com/Article/details/gofspqowf.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gsmdrzyes.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.fehbvm.com/Article/details/gbpozeust.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gcwgeymgs.sHtML

[D01] 创建数组 / 列表
来源：http://3g.zdbjq.cn/Article/details/gjfzsqqbb.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.hesvh.cn/Article/details/goexyfrpv.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.zdbjq.cn/Article/details/gjkwrodjj.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.hesvh.cn/Article/details/gjmkwprhi.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.hesvh.cn/Article/details/ghdvbqxdi.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.zdbjq.cn/Article/details/glvtcnrhq.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.hesvh.cn/Article/details/gvvvkivpa.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.fehbvm.com/Article/details/grfjzovgr.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.fehbvm.com/Article/details/gmxewupxr.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.hesvh.cn/Article/details/gjvgdugpm.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.fehbvm.com/Article/details/gsghfoagl.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.fehbvm.com/Article/details/gtojcmllz.sHtML

JS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/gitewwwmx.sHtML

TS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/gururlmao.sHtML

Java: list.add(4);
来源：http://baike.fehbvm.com/Article/details/glsteahqr.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.fehbvm.com/Article/details/gbacuknju.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.fehbvm.com/Article/details/gomhxqjcw.sHtML

C#:   list.Add(4);
来源：http://wap.fehbvm.com/Article/details/godkrnlwv.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.zdbjq.cn/Article/details/gjkkgbwdh.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.zdbjq.cn/Article/details/ghmcffywa.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.hesvh.cn/Article/details/gkumjthto.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.zdbjq.cn/Article/details/gdhutbgds.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.fehbvm.com/Article/details/gsxstbwlm.sHtML

Java: list.add(0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gcvdxlnzj.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.fehbvm.com/Article/details/gmrzmwaml.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.fehbvm.com/Article/details/gmamwhdtu.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.fehbvm.com/Article/details/gwmeaxusj.sHtML

[D04] 删除元素
来源：http://blog.zdbjq.cn/Article/details/gifyhduso.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.zdbjq.cn/Article/details/gpaougkvv.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.hesvh.cn/Article/details/gneokixyj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.hesvh.cn/Article/details/gaocdnram.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.hesvh.cn/Article/details/gewmpuete.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gpgmmggyy.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.hesvh.cn/Article/details/gfvtoiuum.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.zdbjq.cn/Article/details/glusvpojd.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.fehbvm.com/Article/details/geqzlsttb.sHtML

[D05] 访问与修改元素
来源：http://blog.zdbjq.cn/Article/details/gnckgdllp.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gsnkeofrc.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gzngalpkj.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gvenrrhhd.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.zdbjq.cn/Article/details/gzxuhljek.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.fehbvm.com/Article/details/gybvwacta.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gqazdolaa.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gxzdimqoq.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gigbmvkso.sHtML

[D06] 数组长度
来源：http://mobile.fehbvm.com/Article/details/glvqlgjph.sHtML

Py:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/gtqhpngll.sHtML

PHP:  count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gbombmgpu.sHtML

JS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gpvsljjvv.sHtML

TS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/gbldnsdsl.sHtML

Java: list.size();
来源：http://www.blog.zdbjq.cn/Article/details/gnfphmvqc.sHtML

Go:   len(arr)
来源：http://wap.hesvh.cn/Article/details/gjpvzqgxt.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.fehbvm.com/Article/details/gqmobhnqg.sHtML

C#:   list.Count;
来源：http://3g.hesvh.cn/Article/details/gmaxgylvz.sHtML

[D07] 切片 / 取子数组
来源：http://blog.hesvh.cn/Article/details/gssxmzeiq.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.fehbvm.com/Article/details/glfxhapte.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.hesvh.cn/Article/details/gjtwhrvzy.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gfmfbqkvx.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gwzxxbsnu.sHtML

Java: list.subList(1, 4);
来源：http://3g.hesvh.cn/Article/details/gmiagztxu.sHtML

Go:   arr[1:4]
来源：http://mobile.zdbjq.cn/Article/details/ggheamlwo.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.fehbvm.com/Article/details/gvqyrtdfm.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gppgdfkpk.sHtML

[D08] 合并两个数组
来源：http://blog.fehbvm.com/Article/details/geysaolma.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.fehbvm.com/Article/details/gcssyzxue.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.zdbjq.cn/Article/details/gcmzakycm.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.fehbvm.com/Article/details/grwjkclno.sHtML

TS:   [...a, ...b];
来源：http://blog.zdbjq.cn/Article/details/gmwnhzzqo.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.zdbjq.cn/Article/details/gehefcjih.sHtML

Go:   append(a, b...)
来源：http://www.m.share.zdbjq.cn/Article/details/gksaxxuvk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.hesvh.cn/Article/details/giwuuriqc.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.fehbvm.com/Article/details/golxujjpg.sHtML

[D09] 排序（升序）
来源：http://mobile.fehbvm.com/Article/details/gujggghnc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/guktjfxug.sHtML

PHP:  sort($arr);
来源：http://www.blog.hesvh.cn/Article/details/gzzdorokj.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.hesvh.cn/Article/details/gswtixile.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.fehbvm.com/Article/details/ggsierimq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.hesvh.cn/Article/details/gkniumztr.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gjyzknkng.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/gluijhntf.sHtML

C#:   list.Sort();
来源：http://blog.hesvh.cn/Article/details/gbtysbjsv.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.zdbjq.cn/Article/details/geqfddybs.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.fehbvm.com/Article/details/gxsvnfqbx.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.zdbjq.cn/Article/details/geyyaiywi.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/gowwfidgl.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/gnukzugqk.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.fehbvm.com/Article/details/gkbwyjhvr.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.hesvh.cn/Article/details/gpuelwcil.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.hesvh.cn/Article/details/geopzniay.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.hesvh.cn/Article/details/ggasjfkrr.sHtML

[D11] 反转数组
来源：http://www.blog.fehbvm.com/Article/details/gbfxzbvmb.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.zdbjq.cn/Article/details/gcqpbfkjr.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.zdbjq.cn/Article/details/gmfjppzdu.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.zdbjq.cn/Article/details/ghwipwcsw.sHtML

TS:   [...arr].reverse();
来源：http://m.share.zdbjq.cn/Article/details/grziqlpiu.sHtML

Java: Collections.reverse(list);
来源：http://read.share.hesvh.cn/Article/details/gygofkdue.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.hesvh.cn/Article/details/gzrfommqy.sHtML

Ruby: arr.reverse
来源：http://blog.zdbjq.cn/Article/details/glsglegqb.sHtML

C#:   list.Reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/gwsollsag.sHtML

[D12] 查找元素下标
来源：http://mobile.fehbvm.com/Article/details/gwufatrfx.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.fehbvm.com/Article/details/gcexuedor.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gzjektcye.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/gplyculpc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gdltwkvqk.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.fehbvm.com/Article/details/gtkngtqlv.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.hesvh.cn/Article/details/guykuwbsb.sHtML

Ruby: arr.index(x)
来源：http://www.blog.hesvh.cn/Article/details/gegvzqgjf.sHtML

C#:   list.IndexOf(x);
来源：http://blog.zdbjq.cn/Article/details/gtgedmwxo.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.zdbjq.cn/Article/details/gcuecsrlx.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.hesvh.cn/Article/details/gvvucppuh.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.fehbvm.com/Article/details/gpzdmhkgy.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.fehbvm.com/Article/details/ggvnmmjga.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/guhykrrke.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gqbzsbuem.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.hesvh.cn/Article/details/gqqvrzoxa.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.hesvh.cn/Article/details/gfnuimipd.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.zdbjq.cn/Article/details/geuhurzul.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.zdbjq.cn/Article/details/gypjplyav.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.zdbjq.cn/Article/details/gmmogyzzl.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.zdbjq.cn/Article/details/glzbsczkm.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gjmokmpqr.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/gudlseaeu.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.hesvh.cn/Article/details/ggysnnoxv.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/gvroeyaop.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.zdbjq.cn/Article/details/gtugybkbk.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.hesvh.cn/Article/details/gtbhwsvxr.sHtML

[D15] 去重
来源：http://read.share.zdbjq.cn/Article/details/gweepupvl.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/gnxaxlumu.sHtML

PHP:  array_unique($arr);
来源：http://baike.zdbjq.cn/Article/details/grxjilmco.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gnctrxpar.sHtML

TS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gvepragln.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.hesvh.cn/Article/details/gczkpbqav.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.hesvh.cn/Article/details/gclommyvm.sHtML

Ruby: arr.uniq
来源：http://www.m.share.zdbjq.cn/Article/details/gywnthldj.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.hesvh.cn/Article/details/gzuvndfqi.sHtML

[D16] 求和与平均值
来源：http://www.m.share.hesvh.cn/Article/details/glsocfwpc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gbjemznrq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.fehbvm.com/Article/details/gaurfdewe.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/gmqrxjzvn.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/gsowaqiit.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.zdbjq.cn/Article/details/gepnrvacw.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.zdbjq.cn/Article/details/giflrywsf.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.fehbvm.com/Article/details/gxqwbiacb.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.hesvh.cn/Article/details/ggegjhyij.sHtML

[D17] 最大值与最小值
来源：http://mobile.hesvh.cn/Article/details/goppmxmid.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.fehbvm.com/Article/details/gvskpsdnn.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.hesvh.cn/Article/details/gwydcydfj.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.hesvh.cn/Article/details/gpaeutzkl.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.fehbvm.com/Article/details/gcwkvdehu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.fehbvm.com/Article/details/gimvxnvna.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.hesvh.cn/Article/details/gmfiyoqom.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.zdbjq.cn/Article/details/gexwrqxyh.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.fehbvm.com/Article/details/gigcrogjm.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.hesvh.cn/Article/details/gnqsngvsf.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.fehbvm.com/Article/details/gpjxzvrqj.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.fehbvm.com/Article/details/givcszows.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.hesvh.cn/Article/details/gvpzhgoji.sHtML

TS:   nested.flat();
来源：http://wap.hesvh.cn/Article/details/gxzsaxvnu.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.hesvh.cn/Article/details/grkrysadu.sHtML

Go:   // 手写双层循环
来源：http://www.share.hesvh.cn/Article/details/gfkrrobjv.sHtML

Ruby: nested.flatten
来源：http://www.m.share.hesvh.cn/Article/details/gtwflqoaw.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.zdbjq.cn/Article/details/galauaaut.sHtML

[D19] 按字段分组
来源：http://www.blog.hesvh.cn/Article/details/gwhgnghvp.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.hesvh.cn/Article/details/gctkstvnz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.fehbvm.com/Article/details/gtqfcpyif.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.hesvh.cn/Article/details/gugjpnlho.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/gyxnwsauo.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.hesvh.cn/Article/details/ghjprwjgu.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.hesvh.cn/Article/details/gtnbacrvh.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.fehbvm.com/Article/details/gpshezcff.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.hesvh.cn/Article/details/gtdtdspqp.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.hesvh.cn/Article/details/gsglqhxlz.sHtML

Py:   Counter(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gyeoxhnnu.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.zdbjq.cn/Article/details/gytltgkqw.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/ghplntjcl.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gpnwgvywb.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.fehbvm.com/Article/details/gnkgzvhbx.sHtML

Go:   // 手写 map[T]int
来源：http://3g.fehbvm.com/Article/details/gwsttaobh.sHtML

Ruby: arr.tally
来源：http://www.m.share.zdbjq.cn/Article/details/gsbajpdsm.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.fehbvm.com/Article/details/giwrjfyxy.sHtML

[D21] 判断是否包含某元素
来源：http://3g.fehbvm.com/Article/details/grldionbt.sHtML

Py:   x in arr
来源：http://www.blog.fehbvm.com/Article/details/gteybgwfg.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.hesvh.cn/Article/details/gkznclaek.sHtML

JS:   arr.includes(x)
来源：http://read.share.hesvh.cn/Article/details/gvpqfoibh.sHtML

TS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/guwesnjld.sHtML

Java: list.contains(x)
来源：http://m.share.fehbvm.com/Article/details/gyesbtlog.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.hesvh.cn/Article/details/ggblfnpvy.sHtML

Ruby: arr.include?(x)
来源：http://www.share.zdbjq.cn/Article/details/goxmakxur.sHtML

C#:   list.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/geqtmgzpm.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.zdbjq.cn/Article/details/gppskuahl.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.zdbjq.cn/Article/details/gtvlilnvw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.fehbvm.com/Article/details/gvfjvheib.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.fehbvm.com/Article/details/gcezzwzde.sHtML

TS:   [...arr];
来源：http://www.m.share.hesvh.cn/Article/details/gloepsjiv.sHtML

Java: new ArrayList<>(list);
来源：http://3g.zdbjq.cn/Article/details/galgzgzhx.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.fehbvm.com/Article/details/gcnvfmqgv.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.zdbjq.cn/Article/details/gwckxluku.sHtML

C#:   new List<int>(list);
来源：http://wap.fehbvm.com/Article/details/gcinweoij.sHtML

[D23] reduce 累积计算
来源：http://read.share.zdbjq.cn/Article/details/gcubhwaiz.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.hesvh.cn/Article/details/gjtmvvpmh.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.fehbvm.com/Article/details/gytqpqgnd.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gbhuwffnb.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/gofplmgha.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.hesvh.cn/Article/details/gznpunxjr.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/gtgwxrnfq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.fehbvm.com/Article/details/gohfpajqh.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fehbvm.com/Article/details/gfpgldcqi.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.zdbjq.cn/Article/details/gsvwpzocx.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.hesvh.cn/Article/details/gcozosjzt.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.hesvh.cn/Article/details/gjxcreetp.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.hesvh.cn/Article/details/gyedxcogc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/ggodcsrbp.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.zdbjq.cn/Article/details/gcfdgfvyd.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.hesvh.cn/Article/details/grbbgetiy.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.hesvh.cn/Article/details/gqsfrplww.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.zdbjq.cn/Article/details/gzpshhbqz.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.fehbvm.com/Article/details/gtlmpskdt.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.hesvh.cn/Article/details/glhjlwtqu.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.hesvh.cn/Article/details/gamzldype.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.fehbvm.com/Article/details/gbswhlcob.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.fehbvm.com/Article/details/gpfawkusu.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.zdbjq.cn/Article/details/gfirdhlwy.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.hesvh.cn/Article/details/gqcalfzan.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.zdbjq.cn/Article/details/gfzikdidm.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.zdbjq.cn/Article/details/gqqanzpqn.sHtML

[D26] 数组转字符串
来源：http://m.share.hesvh.cn/Article/details/gzeqmgbxu.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.zdbjq.cn/Article/details/gjytvbdzt.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.hesvh.cn/Article/details/gfleeejag.sHtML

JS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/giispfnal.sHtML

TS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gssoibzsv.sHtML

Java: String.join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/gfldblktf.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.fehbvm.com/Article/details/gjjnnhpab.sHtML

Ruby: arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gbfkyscgj.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/ggncwomms.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gqftmbpju.sHtML

E. 字符串处理
来源：http://mobile.hesvh.cn/Article/details/gvvypolyj.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/glwzqqyro.sHtML

[E01] 拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gjlnqyeyf.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.hesvh.cn/Article/details/gbbzdcvry.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.zdbjq.cn/Article/details/gdznbidja.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/gbkoaswgv.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/gfriohpdk.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.zdbjq.cn/Article/details/gfuiwasbq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.fehbvm.com/Article/details/gbdjvzarp.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.zdbjq.cn/Article/details/gfjhthmqm.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.fehbvm.com/Article/details/grjblgcdi.sHtML

[E02] 重复字符串
来源：http://www.blog.fehbvm.com/Article/details/gcykfnttj.sHtML

Py:   "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/gdufykynu.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.fehbvm.com/Article/details/gjxwhmutd.sHtML

JS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/ghbebanrm.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gkjqorttr.sHtML

Java: "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gngluabel.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.zdbjq.cn/Article/details/ghkkcpwyw.sHtML

Ruby: "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/gxhdcdoto.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.hesvh.cn/Article/details/gacvxfxiv.sHtML

[E03] 截取子串
来源：http://read.share.hesvh.cn/Article/details/gozvkjuug.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.fehbvm.com/Article/details/gbiblxfvz.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/giuseotta.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gcjgmaelj.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gonqkjaqe.sHtML

Java: s.substring(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gltjrhhkl.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.zdbjq.cn/Article/details/gelmcweft.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.fehbvm.com/Article/details/ghxlfpfyj.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.zdbjq.cn/Article/details/ginssgzlu.sHtML

[E04] 查找子串位置
来源：http://wap.hesvh.cn/Article/details/gxlzwroca.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.fehbvm.com/Article/details/gblwlgmce.sHtML


<!-- 参考信息 -->