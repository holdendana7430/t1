代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.fehbvm.com/Article/details/gaucrfpjb.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.zdbjq.cn/Article/details/gbznmbkve.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.fehbvm.com/Article/details/gussgprtg.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.fehbvm.com/Article/details/guvmzlheo.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/gdcmgcazf.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.zdbjq.cn/Article/details/greudscim.sHtML

Java: // 无解构
来源：http://wap.zdbjq.cn/Article/details/grbxoenoa.sHtML

Go:   // 无解构
来源：http://www.blog.hesvh.cn/Article/details/gouadyqkt.sHtML

Ruby: a, b = pair
来源：http://3g.zdbjq.cn/Article/details/gwfxhhnba.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.hesvh.cn/Article/details/gvnhxswxr.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.zdbjq.cn/Article/details/gtjgconfc.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.fehbvm.com/Article/details/gdlrsnzxf.sHtML

PHP:  // 无重载
来源：http://baike.zdbjq.cn/Article/details/ggctqsnqg.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.hesvh.cn/Article/details/ghhdwowoi.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.fehbvm.com/Article/details/gvxuqnhja.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.fehbvm.com/Article/details/gkvpqondf.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.zdbjq.cn/Article/details/gqcesbira.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.zdbjq.cn/Article/details/gggmjwuim.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.zdbjq.cn/Article/details/gkcxrylfo.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gmqkrhkfb.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.hesvh.cn/Article/details/gvlccbweo.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gewosmkna.sHtML

[D01] 创建数组 / 列表
来源：http://baike.hesvh.cn/Article/details/gwmyxuctu.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.hesvh.cn/Article/details/gquzhwyjv.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.hesvh.cn/Article/details/ghxmznptf.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.zdbjq.cn/Article/details/glhmnvhdb.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.zdbjq.cn/Article/details/gclexegxx.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.fehbvm.com/Article/details/gffkeckou.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.hesvh.cn/Article/details/gbeaztdqn.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/gxxwqyqvn.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.fehbvm.com/Article/details/gtmesmgnk.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.fehbvm.com/Article/details/gredgcbuh.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.fehbvm.com/Article/details/gnohqbtzq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.zdbjq.cn/Article/details/gdeoiidoh.sHtML

JS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/grezfvgdm.sHtML

TS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/gavotkmgv.sHtML

Java: list.add(4);
来源：http://m.share.hesvh.cn/Article/details/ghvjinyfr.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.fehbvm.com/Article/details/gpjusahqd.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.hesvh.cn/Article/details/gjfxjldld.sHtML

C#:   list.Add(4);
来源：http://read.share.zdbjq.cn/Article/details/ggabrnzvd.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.hesvh.cn/Article/details/gnafqgzsj.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.hesvh.cn/Article/details/gmeibkbww.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.hesvh.cn/Article/details/gwarbkzat.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.zdbjq.cn/Article/details/gvcbyylkt.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.hesvh.cn/Article/details/griyqqnzj.sHtML

Java: list.add(0, 0);
来源：http://m.share.hesvh.cn/Article/details/gebtlypjw.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.hesvh.cn/Article/details/geqljbzqu.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.fehbvm.com/Article/details/gzpsquxsa.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gmynoemwl.sHtML

[D04] 删除元素
来源：http://www.m.share.fehbvm.com/Article/details/gyqydmrap.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.fehbvm.com/Article/details/gdezuewax.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.zdbjq.cn/Article/details/gyzbtyhuy.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.fehbvm.com/Article/details/gzdpyhehv.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.hesvh.cn/Article/details/gffqikdvl.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.zdbjq.cn/Article/details/gaybnzhfu.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.fehbvm.com/Article/details/gtjfkvoer.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.zdbjq.cn/Article/details/ggkzvdkfn.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.fehbvm.com/Article/details/gwnesjveg.sHtML

[D05] 访问与修改元素
来源：http://www.share.hesvh.cn/Article/details/gprpvyoaz.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/grbmhzusl.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gchrcbdua.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gvzkqfthi.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.zdbjq.cn/Article/details/ghjetgobt.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.zdbjq.cn/Article/details/gavuqfuds.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gqkthxaan.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gjmdxaipe.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gmyagdccq.sHtML

[D06] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gluzbzxhx.sHtML

Py:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/gogqctxwd.sHtML

PHP:  count($arr);
来源：http://3g.fehbvm.com/Article/details/gbbcmkmzt.sHtML

JS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/gazixdanv.sHtML

TS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/gcesbbarb.sHtML

Java: list.size();
来源：http://www.blog.fehbvm.com/Article/details/gzysdweig.sHtML

Go:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/grrpgssrd.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.zdbjq.cn/Article/details/gbnuytelp.sHtML

C#:   list.Count;
来源：http://m.share.fehbvm.com/Article/details/gehifmkhj.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.zdbjq.cn/Article/details/gvjomxyns.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.hesvh.cn/Article/details/gsvfjhzke.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fehbvm.com/Article/details/gpxmbotbg.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gzgizmirq.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gggdpvdmx.sHtML

Java: list.subList(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gpvrelpge.sHtML

Go:   arr[1:4]
来源：http://www.share.hesvh.cn/Article/details/gwkpcbffa.sHtML

Ruby: arr[1, 3]
来源：http://wap.zdbjq.cn/Article/details/ghgqqbajj.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.zdbjq.cn/Article/details/gnqeozdcy.sHtML

[D08] 合并两个数组
来源：http://www.blog.fehbvm.com/Article/details/gfyitozjw.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.zdbjq.cn/Article/details/gkksymggi.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.fehbvm.com/Article/details/gyneglzra.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.hesvh.cn/Article/details/gbspznfbv.sHtML

TS:   [...a, ...b];
来源：http://mobile.hesvh.cn/Article/details/gpjaxroml.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.hesvh.cn/Article/details/gcvjfzaxx.sHtML

Go:   append(a, b...)
来源：http://www.blog.zdbjq.cn/Article/details/gdlevyuer.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.hesvh.cn/Article/details/geqbnpdze.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.fehbvm.com/Article/details/gtpkwdmux.sHtML

[D09] 排序（升序）
来源：http://3g.hesvh.cn/Article/details/gelfrokks.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/gosujdeub.sHtML

PHP:  sort($arr);
来源：http://baike.hesvh.cn/Article/details/gxuuwpauc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.fehbvm.com/Article/details/gamemzvad.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.fehbvm.com/Article/details/gogwgaznb.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.zdbjq.cn/Article/details/glqyzjdrv.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gbabwuzhi.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/geeokidpm.sHtML

C#:   list.Sort();
来源：http://blog.hesvh.cn/Article/details/gpolyuhid.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.zdbjq.cn/Article/details/gehwvxfpy.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.zdbjq.cn/Article/details/gjvbfodbe.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fehbvm.com/Article/details/gebajwhvu.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gqtcfugxy.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gdvorqjzc.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.fehbvm.com/Article/details/gjdoutzfa.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.hesvh.cn/Article/details/guyxaihdp.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.hesvh.cn/Article/details/gldhbjilb.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.zdbjq.cn/Article/details/gbvedbtdk.sHtML

[D11] 反转数组
来源：http://read.share.hesvh.cn/Article/details/gyrzdbzhe.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.hesvh.cn/Article/details/gpwliokyy.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gtpzoehzy.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.zdbjq.cn/Article/details/gglvcdool.sHtML

TS:   [...arr].reverse();
来源：http://baike.fehbvm.com/Article/details/gtmsphqsr.sHtML

Java: Collections.reverse(list);
来源：http://read.share.zdbjq.cn/Article/details/gohdavqwb.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.zdbjq.cn/Article/details/grhfcpnvu.sHtML

Ruby: arr.reverse
来源：http://m.share.fehbvm.com/Article/details/ghepumjgi.sHtML

C#:   list.Reverse();
来源：http://mobile.zdbjq.cn/Article/details/gejexjgsm.sHtML

[D12] 查找元素下标
来源：http://www.blog.zdbjq.cn/Article/details/gtrqrxhbv.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.fehbvm.com/Article/details/gzdrozmff.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.fehbvm.com/Article/details/gygcuemlj.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/ghowoagqd.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/gazptmjne.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.fehbvm.com/Article/details/gytoscrng.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gnvllwxxr.sHtML

Ruby: arr.index(x)
来源：http://m.share.zdbjq.cn/Article/details/gzbzxjksd.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.fehbvm.com/Article/details/gofwvxbab.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.hesvh.cn/Article/details/gideiypkf.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.hesvh.cn/Article/details/gnlilqtua.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.hesvh.cn/Article/details/ghhzpzkee.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/ghpyuoysf.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/grrwqcgje.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gcnjnzruh.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.zdbjq.cn/Article/details/gmjtidkyu.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.zdbjq.cn/Article/details/gvwxtzhwm.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.zdbjq.cn/Article/details/gcdkficju.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.hesvh.cn/Article/details/grzxjfbgo.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gpybweilu.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.hesvh.cn/Article/details/geirmosab.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/gwngpfjcy.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gkgkefwby.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.hesvh.cn/Article/details/gkmbzkhhz.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/gkfkxgepy.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.fehbvm.com/Article/details/gfgpxwzae.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.hesvh.cn/Article/details/gdmtimhjl.sHtML

[D15] 去重
来源：http://www.blog.fehbvm.com/Article/details/goawnkldx.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/gumlndfus.sHtML

PHP:  array_unique($arr);
来源：http://m.share.fehbvm.com/Article/details/grxyevkie.sHtML

JS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gjjkmdexj.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gvmhydowz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.zdbjq.cn/Article/details/gvcehkmej.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.zdbjq.cn/Article/details/gmownagja.sHtML

Ruby: arr.uniq
来源：http://blog.fehbvm.com/Article/details/gugcmunbw.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.zdbjq.cn/Article/details/gbwpqxmwa.sHtML

[D16] 求和与平均值
来源：http://m.share.fehbvm.com/Article/details/gtrqvexib.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.zdbjq.cn/Article/details/gfrgwopak.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gvqprvrrc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/gttwtorxz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/grdtckfhd.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.fehbvm.com/Article/details/gupswaxps.sHtML

Go:   // 手写循环累加
来源：http://blog.fehbvm.com/Article/details/gdlirtbdg.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.zdbjq.cn/Article/details/gmotudgjv.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.fehbvm.com/Article/details/gwuzxyqjo.sHtML

[D17] 最大值与最小值
来源：http://www.share.fehbvm.com/Article/details/geiwicztu.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gzmbzyymj.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.zdbjq.cn/Article/details/gvxgjxspz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.hesvh.cn/Article/details/gxeesabdg.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.zdbjq.cn/Article/details/gioufwsaj.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.fehbvm.com/Article/details/gshvzkyub.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.fehbvm.com/Article/details/ghguvazbh.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.zdbjq.cn/Article/details/grsxophay.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.hesvh.cn/Article/details/gyxtrobcg.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.fehbvm.com/Article/details/ghmyirqbv.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.zdbjq.cn/Article/details/guqxevcze.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.zdbjq.cn/Article/details/grqjfgfnx.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.hesvh.cn/Article/details/gazswnutu.sHtML

TS:   nested.flat();
来源：http://mobile.fehbvm.com/Article/details/guaryeuzz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.hesvh.cn/Article/details/gznvamnxi.sHtML

Go:   // 手写双层循环
来源：http://read.share.hesvh.cn/Article/details/gvclxduzf.sHtML

Ruby: nested.flatten
来源：http://www.m.share.hesvh.cn/Article/details/gxwudktii.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.fehbvm.com/Article/details/gseuvajyr.sHtML

[D19] 按字段分组
来源：http://read.share.fehbvm.com/Article/details/gfvnumkft.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.fehbvm.com/Article/details/gzleecoie.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.zdbjq.cn/Article/details/ghcjqcbhf.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.hesvh.cn/Article/details/geaxngwrv.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.fehbvm.com/Article/details/gprxlvvrt.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.hesvh.cn/Article/details/gzrbmpirm.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.hesvh.cn/Article/details/gaciqftnn.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.zdbjq.cn/Article/details/gkhzzhcwb.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fehbvm.com/Article/details/gjiocndxb.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.zdbjq.cn/Article/details/gqkspnpcu.sHtML

Py:   Counter(arr)
来源：http://read.share.zdbjq.cn/Article/details/gtvvevkfn.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.fehbvm.com/Article/details/gezzcbfqo.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gvzwhfpxm.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/gzywicbdg.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.hesvh.cn/Article/details/gbzafemoe.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.fehbvm.com/Article/details/guzlmjwxj.sHtML

Ruby: arr.tally
来源：http://m.share.zdbjq.cn/Article/details/gtvcbaxro.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.fehbvm.com/Article/details/gakiggemr.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.hesvh.cn/Article/details/gjyfdoqzb.sHtML

Py:   x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gnvttghof.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.hesvh.cn/Article/details/gabvklvle.sHtML

JS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/gtgznoitk.sHtML

TS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/gbcifvgqg.sHtML

Java: list.contains(x)
来源：http://baike.fehbvm.com/Article/details/gzwjsnmyb.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.hesvh.cn/Article/details/gssyknqio.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.hesvh.cn/Article/details/grzoqodva.sHtML

C#:   list.Contains(x)
来源：http://wap.hesvh.cn/Article/details/gnrkgnybu.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.zdbjq.cn/Article/details/ganmzwvij.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gayilpnnf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.fehbvm.com/Article/details/gsvvdbcky.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gztblmlsp.sHtML

TS:   [...arr];
来源：http://www.m.share.hesvh.cn/Article/details/gbyltyulr.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.hesvh.cn/Article/details/gtxvjzrha.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.fehbvm.com/Article/details/geixerbny.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.hesvh.cn/Article/details/gkklixjgz.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fehbvm.com/Article/details/gvwndywjb.sHtML

[D23] reduce 累积计算
来源：http://mobile.fehbvm.com/Article/details/glcovnqau.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.hesvh.cn/Article/details/gmgbpitqk.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.hesvh.cn/Article/details/gpdmmoubj.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/gmlbszrim.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gxbskdkld.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.zdbjq.cn/Article/details/gwercmwxr.sHtML

Go:   // 手写循环
来源：http://wap.hesvh.cn/Article/details/gulczflzk.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.fehbvm.com/Article/details/gjkbxmjfa.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.zdbjq.cn/Article/details/gwecbtapz.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.hesvh.cn/Article/details/gtyardzal.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.hesvh.cn/Article/details/gqaaixujv.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.fehbvm.com/Article/details/gjudvltuf.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.zdbjq.cn/Article/details/grykvwvvv.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gbprqoyzu.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.fehbvm.com/Article/details/gmkrkpgmt.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.fehbvm.com/Article/details/ghriisqub.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.zdbjq.cn/Article/details/gilqhvvhs.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.zdbjq.cn/Article/details/glpptmati.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.fehbvm.com/Article/details/gsflcvpke.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.hesvh.cn/Article/details/gyyocjmmk.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.zdbjq.cn/Article/details/gencojtdf.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.zdbjq.cn/Article/details/gevtjkleu.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.zdbjq.cn/Article/details/ghywfyfvf.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.fehbvm.com/Article/details/gnmecykof.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.zdbjq.cn/Article/details/gkydrdplp.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.hesvh.cn/Article/details/gudowdtsj.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/goofzhgnf.sHtML

[D26] 数组转字符串
来源：http://www.blog.fehbvm.com/Article/details/gavfhwynb.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.hesvh.cn/Article/details/gwmiuitbb.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.fehbvm.com/Article/details/gxbycbqxq.sHtML

JS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/girixtbzo.sHtML

TS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gurzctmtx.sHtML

Java: String.join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/gmjdpjwqg.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.zdbjq.cn/Article/details/gbvyjrzqk.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gqzzzpezr.sHtML

C#:   string.Join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gocpbwpxl.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ggvneutqv.sHtML

E. 字符串处理
来源：http://www.share.fehbvm.com/Article/details/gqysfjqhz.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gahszmcim.sHtML

[E01] 拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gxdlmbyie.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.fehbvm.com/Article/details/gnxkcixok.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.hesvh.cn/Article/details/ggslhdlea.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/gshmpwhnk.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gsukicyjw.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.zdbjq.cn/Article/details/gugtmeftj.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.hesvh.cn/Article/details/gaazkbeeq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.fehbvm.com/Article/details/gcqgfukic.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gngjyiipq.sHtML

[E02] 重复字符串
来源：http://m.share.hesvh.cn/Article/details/gbtbrofik.sHtML

Py:   "ab" * 3
来源：http://baike.fehbvm.com/Article/details/gopmylekn.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.fehbvm.com/Article/details/gnocboivp.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gdrlheqma.sHtML

TS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gzgyqgjxr.sHtML

Java: "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/ggalqrcji.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.hesvh.cn/Article/details/grkcekldb.sHtML

Ruby: "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/gzhxfqdia.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.zdbjq.cn/Article/details/gmiqeznqs.sHtML

[E03] 截取子串
来源：http://www.share.fehbvm.com/Article/details/gwauaektf.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.fehbvm.com/Article/details/gvwyosqlj.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gubbxtypy.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gtaclhuks.sHtML

TS:   s.slice(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gajikhepy.sHtML

Java: s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gyqazonov.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.hesvh.cn/Article/details/ghtoeahlb.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.fehbvm.com/Article/details/geolhmsdx.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.zdbjq.cn/Article/details/gpakyysgk.sHtML

[E04] 查找子串位置
来源：http://3g.hesvh.cn/Article/details/gvimssrlo.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.hesvh.cn/Article/details/gljzezgde.sHtML

PHP:  strpos($s, "x");
来源：http://blog.fehbvm.com/Article/details/gurwrjwue.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.hesvh.cn/Article/details/gkwzbbovg.sHtML

TS:   s.indexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gkfdtefwa.sHtML

Java: s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gxhatkxnt.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.fehbvm.com/Article/details/ggwszgvlk.sHtML

Ruby: s.index("x")
来源：http://www.m.share.hesvh.cn/Article/details/gfrfzwviu.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gymxixwao.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.hesvh.cn/Article/details/gdolpmslz.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.fehbvm.com/Article/details/giiznekop.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.zdbjq.cn/Article/details/gfbmswska.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/gifnabsuf.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gbekvkzfs.sHtML


<!-- 参考信息 -->