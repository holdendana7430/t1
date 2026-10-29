代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.hesvh.cn/Article/details/gsbuagbiu.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.hesvh.cn/Article/details/gjvouvrxp.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.zdbjq.cn/Article/details/gmjumkptc.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.zdbjq.cn/Article/details/gtqlbpdpa.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/gyayljohq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.hesvh.cn/Article/details/gmthzmnnn.sHtML

Java: // 无解构
来源：http://blog.fehbvm.com/Article/details/ghefakxsu.sHtML

Go:   // 无解构
来源：http://wap.hesvh.cn/Article/details/gxuffprdn.sHtML

Ruby: a, b = pair
来源：http://wap.zdbjq.cn/Article/details/gbclgiugo.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.zdbjq.cn/Article/details/gdemqxtmc.sHtML

[C16] 函数 / 方法重载
来源：http://3g.fehbvm.com/Article/details/gyggavwiu.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.zdbjq.cn/Article/details/gwzoebfyu.sHtML

PHP:  // 无重载
来源：http://blog.hesvh.cn/Article/details/gzmoepekd.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.hesvh.cn/Article/details/gqtrypebc.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.fehbvm.com/Article/details/gzbbspgli.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.zdbjq.cn/Article/details/guzpbdkmh.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.hesvh.cn/Article/details/gpasfibvx.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.hesvh.cn/Article/details/ghgjvxtei.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.hesvh.cn/Article/details/gkyasmelg.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gnjppusog.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.fehbvm.com/Article/details/ghurtvbzi.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gjacizjiv.sHtML

[D01] 创建数组 / 列表
来源：http://wap.zdbjq.cn/Article/details/gxudcxafc.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.zdbjq.cn/Article/details/gfeobtmmk.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.hesvh.cn/Article/details/gzjutavip.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.zdbjq.cn/Article/details/ggvttdulo.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.zdbjq.cn/Article/details/gimievnbn.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.fehbvm.com/Article/details/grbuemjxv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.hesvh.cn/Article/details/gajfscvtc.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.fehbvm.com/Article/details/gwfpxujmz.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.hesvh.cn/Article/details/gyxnniqzy.sHtML

[D02] 追加元素到末尾
来源：http://www.share.hesvh.cn/Article/details/gdkbivkhk.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.fehbvm.com/Article/details/gfcjjkpcf.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.fehbvm.com/Article/details/gzazvuvxj.sHtML

JS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/gqcmknjel.sHtML

TS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/ggjkreyji.sHtML

Java: list.add(4);
来源：http://wap.zdbjq.cn/Article/details/gvnembjfk.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.fehbvm.com/Article/details/gkupnllva.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.fehbvm.com/Article/details/gnlajpakv.sHtML

C#:   list.Add(4);
来源：http://m.share.fehbvm.com/Article/details/gaywpwgbm.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.hesvh.cn/Article/details/glougbnpf.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.hesvh.cn/Article/details/gcaoosbtj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.hesvh.cn/Article/details/gkqxoywbt.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.zdbjq.cn/Article/details/gzowesuqb.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.fehbvm.com/Article/details/gkmhkiesl.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/giatraqwu.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.zdbjq.cn/Article/details/geptyvpoa.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.fehbvm.com/Article/details/gsmvpqtfl.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gvghttymn.sHtML

[D04] 删除元素
来源：http://read.share.zdbjq.cn/Article/details/gopuobmni.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.fehbvm.com/Article/details/gbklutvje.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gfurcqehc.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.zdbjq.cn/Article/details/gjswsarrw.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.hesvh.cn/Article/details/gmcsridch.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.fehbvm.com/Article/details/ggpifvhqp.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.zdbjq.cn/Article/details/gwkabnvqi.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.fehbvm.com/Article/details/gzllymzrj.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.hesvh.cn/Article/details/gtknnnolw.sHtML

[D05] 访问与修改元素
来源：http://baike.zdbjq.cn/Article/details/ginkwpxkw.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/goosucbya.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gyqltkfrn.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gurzkjxou.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.fehbvm.com/Article/details/gyidjltkc.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.hesvh.cn/Article/details/gmcgiyxzr.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gyfimbsgd.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gbucfeexy.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gqktkxaox.sHtML

[D06] 数组长度
来源：http://m.share.hesvh.cn/Article/details/gedobixhg.sHtML

Py:   len(arr)
来源：http://blog.fehbvm.com/Article/details/gpkcgxhrh.sHtML

PHP:  count($arr);
来源：http://mobile.fehbvm.com/Article/details/ggzkuhsfb.sHtML

JS:   arr.length
来源：http://www.m.share.hesvh.cn/Article/details/gzjfhhvea.sHtML

TS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/gkfjzszzs.sHtML

Java: list.size();
来源：http://baike.fehbvm.com/Article/details/gzcixorrs.sHtML

Go:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gcuxmllkf.sHtML

Ruby: arr.length; arr.size
来源：http://3g.hesvh.cn/Article/details/gsvwnnkhj.sHtML

C#:   list.Count;
来源：http://blog.hesvh.cn/Article/details/gxffgeirx.sHtML

[D07] 切片 / 取子数组
来源：http://wap.fehbvm.com/Article/details/gzubcuvjw.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.zdbjq.cn/Article/details/gbludvixk.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gakfyxqnb.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gekfvahqt.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gfbzlqgiy.sHtML

Java: list.subList(1, 4);
来源：http://3g.fehbvm.com/Article/details/gxhxiaygt.sHtML

Go:   arr[1:4]
来源：http://blog.fehbvm.com/Article/details/gvkhiymav.sHtML

Ruby: arr[1, 3]
来源：http://3g.hesvh.cn/Article/details/gutmfytfb.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.hesvh.cn/Article/details/gfhpbormr.sHtML

[D08] 合并两个数组
来源：http://m.share.hesvh.cn/Article/details/gbwawoybj.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.fehbvm.com/Article/details/gnsbjjvdn.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.hesvh.cn/Article/details/gwnbcayjq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.fehbvm.com/Article/details/gyljnlqzf.sHtML

TS:   [...a, ...b];
来源：http://read.share.zdbjq.cn/Article/details/ghvsdxgww.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.fehbvm.com/Article/details/ghjhjlfbk.sHtML

Go:   append(a, b...)
来源：http://www.blog.hesvh.cn/Article/details/gmmutmkft.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.fehbvm.com/Article/details/geavkpsua.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.zdbjq.cn/Article/details/gkmtazhfn.sHtML

[D09] 排序（升序）
来源：http://read.share.hesvh.cn/Article/details/gnyzrhwlc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/geekgxwmv.sHtML

PHP:  sort($arr);
来源：http://read.share.fehbvm.com/Article/details/ghmqeykew.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.zdbjq.cn/Article/details/gkleqgixu.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.zdbjq.cn/Article/details/gjqoasifa.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.zdbjq.cn/Article/details/gtkfknchw.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/ghlcczgge.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/grgisfdme.sHtML

C#:   list.Sort();
来源：http://mobile.hesvh.cn/Article/details/gklwhqtvg.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.hesvh.cn/Article/details/gpfxbyail.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.fehbvm.com/Article/details/gmkveghdd.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/gwtzupazu.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/guxxuismu.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gympfisce.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.hesvh.cn/Article/details/gnjmybzer.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.hesvh.cn/Article/details/gqiivstbj.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.fehbvm.com/Article/details/gajvtoyci.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.fehbvm.com/Article/details/gbikckqem.sHtML

[D11] 反转数组
来源：http://baike.zdbjq.cn/Article/details/gestieuxu.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.zdbjq.cn/Article/details/gwyxpbuok.sHtML

PHP:  array_reverse($arr);
来源：http://blog.hesvh.cn/Article/details/gjvulbhlp.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.hesvh.cn/Article/details/grgdolxrx.sHtML

TS:   [...arr].reverse();
来源：http://blog.fehbvm.com/Article/details/gzkrwkosm.sHtML

Java: Collections.reverse(list);
来源：http://blog.zdbjq.cn/Article/details/gsfwobbjp.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.zdbjq.cn/Article/details/gybcwtxar.sHtML

Ruby: arr.reverse
来源：http://read.share.fehbvm.com/Article/details/glhdelxpy.sHtML

C#:   list.Reverse();
来源：http://read.share.hesvh.cn/Article/details/glghsgukc.sHtML

[D12] 查找元素下标
来源：http://blog.hesvh.cn/Article/details/gxuezfxwu.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.fehbvm.com/Article/details/gutojkpwu.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.fehbvm.com/Article/details/gqdslxufc.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/gvurvxefz.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/gfmmgnxhg.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.hesvh.cn/Article/details/gihxkwyza.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gzqfgqonp.sHtML

Ruby: arr.index(x)
来源：http://3g.hesvh.cn/Article/details/ggzdiqqei.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.zdbjq.cn/Article/details/gqwriepvj.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.hesvh.cn/Article/details/grinqtkam.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.hesvh.cn/Article/details/gxfabxnaj.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.fehbvm.com/Article/details/gjquscrwi.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/glwkjvvgp.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/ghvlfzctn.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.zdbjq.cn/Article/details/gjzxvsnav.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.hesvh.cn/Article/details/gpysxywji.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.zdbjq.cn/Article/details/gibpfjkbx.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.fehbvm.com/Article/details/gycqrbypj.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.fehbvm.com/Article/details/gxqcznodo.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.hesvh.cn/Article/details/gnfuclozt.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.fehbvm.com/Article/details/gtfeopxoc.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/gphkyanyp.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.hesvh.cn/Article/details/gudzufsco.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.hesvh.cn/Article/details/gslnusept.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/gisrxfibi.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.hesvh.cn/Article/details/gyrlrnbuk.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.hesvh.cn/Article/details/gmyrbueie.sHtML

[D15] 去重
来源：http://blog.zdbjq.cn/Article/details/gggosuoea.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.fehbvm.com/Article/details/gykjgqifh.sHtML

PHP:  array_unique($arr);
来源：http://www.share.hesvh.cn/Article/details/gplcavrlh.sHtML

JS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gilpguoba.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gxmuovkjj.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.zdbjq.cn/Article/details/ghztrjnlt.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.zdbjq.cn/Article/details/gwkfvhnou.sHtML

Ruby: arr.uniq
来源：http://www.blog.fehbvm.com/Article/details/gkoowkpbo.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.fehbvm.com/Article/details/gzdqiprwh.sHtML

[D16] 求和与平均值
来源：http://www.m.share.fehbvm.com/Article/details/gobjxkgns.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.fehbvm.com/Article/details/gaddunkre.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gbboysfof.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/gkweaubxz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gvecxykkv.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.fehbvm.com/Article/details/gxpclaiiq.sHtML

Go:   // 手写循环累加
来源：http://read.share.fehbvm.com/Article/details/guuvxsydw.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.hesvh.cn/Article/details/gwykkafmd.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.zdbjq.cn/Article/details/gbpvnwzdw.sHtML

[D17] 最大值与最小值
来源：http://3g.hesvh.cn/Article/details/gyvyuzxew.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.zdbjq.cn/Article/details/giwdopnuj.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.zdbjq.cn/Article/details/gdmxcqlbs.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.zdbjq.cn/Article/details/gapsjqyvk.sHtML

TS:   Math.max(...arr);
来源：http://read.share.zdbjq.cn/Article/details/grvcfduiy.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.fehbvm.com/Article/details/gdyqievhj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.hesvh.cn/Article/details/gavwmbksw.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.hesvh.cn/Article/details/gbzxrnnlu.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.hesvh.cn/Article/details/gxodllcjq.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.fehbvm.com/Article/details/gkoowoiwd.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.fehbvm.com/Article/details/gpldvxotx.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.hesvh.cn/Article/details/gqrawyrga.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.zdbjq.cn/Article/details/gjrufwctn.sHtML

TS:   nested.flat();
来源：http://m.share.hesvh.cn/Article/details/gqbnunqmy.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.hesvh.cn/Article/details/gfkzozjrd.sHtML

Go:   // 手写双层循环
来源：http://www.blog.hesvh.cn/Article/details/gigmnqajr.sHtML

Ruby: nested.flatten
来源：http://m.share.hesvh.cn/Article/details/guwegmimv.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.zdbjq.cn/Article/details/ghagohvay.sHtML

[D19] 按字段分组
来源：http://read.share.hesvh.cn/Article/details/gisyyscyi.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.zdbjq.cn/Article/details/guqdnymae.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.zdbjq.cn/Article/details/gnlxyszhj.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.zdbjq.cn/Article/details/glljbwyfx.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.fehbvm.com/Article/details/gojxpjphh.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.fehbvm.com/Article/details/gddzadxlz.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.hesvh.cn/Article/details/gtdqypvdq.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.hesvh.cn/Article/details/gemepaxgr.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.zdbjq.cn/Article/details/glooabsvn.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.zdbjq.cn/Article/details/gbswnzopx.sHtML

Py:   Counter(arr)
来源：http://3g.zdbjq.cn/Article/details/gqmjpkcgo.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.zdbjq.cn/Article/details/gkjggabbr.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/gnxnwjhwf.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/gthfkqbiq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.hesvh.cn/Article/details/ggdocxaoo.sHtML

Go:   // 手写 map[T]int
来源：http://wap.hesvh.cn/Article/details/gdbomxxic.sHtML

Ruby: arr.tally
来源：http://mobile.hesvh.cn/Article/details/gibcahcrm.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.zdbjq.cn/Article/details/gaoroobhm.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.zdbjq.cn/Article/details/gryvbaosb.sHtML

Py:   x in arr
来源：http://wap.hesvh.cn/Article/details/gjlgldzqn.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.hesvh.cn/Article/details/gnrewtqkc.sHtML

JS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/gydnvpnny.sHtML

TS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gkjzeuywt.sHtML

Java: list.contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gwxmclazz.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gpsqfmini.sHtML

Ruby: arr.include?(x)
来源：http://m.share.fehbvm.com/Article/details/gsftahquu.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/grdiyhqvj.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.fehbvm.com/Article/details/gmrhapwrf.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gzlpttiww.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.hesvh.cn/Article/details/gymtrhnav.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.hesvh.cn/Article/details/gghkwhass.sHtML

TS:   [...arr];
来源：http://www.share.zdbjq.cn/Article/details/gphtofmzl.sHtML

Java: new ArrayList<>(list);
来源：http://wap.hesvh.cn/Article/details/gwkhdlwec.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.fehbvm.com/Article/details/gimleypnx.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.zdbjq.cn/Article/details/grsmoahlp.sHtML

C#:   new List<int>(list);
来源：http://www.blog.fehbvm.com/Article/details/gkfeaieyi.sHtML

[D23] reduce 累积计算
来源：http://www.blog.zdbjq.cn/Article/details/gqypzoucz.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.hesvh.cn/Article/details/gqvvabdsl.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.zdbjq.cn/Article/details/gyxboqjco.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/ggruyefcz.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gugasrdpr.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.zdbjq.cn/Article/details/giotijdni.sHtML

Go:   // 手写循环
来源：http://blog.hesvh.cn/Article/details/gqchasowq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.hesvh.cn/Article/details/gditvxjjr.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.fehbvm.com/Article/details/gssdzgqss.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.zdbjq.cn/Article/details/gjpepgqyu.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.fehbvm.com/Article/details/gzxyklkeo.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.fehbvm.com/Article/details/gpswlvreh.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.hesvh.cn/Article/details/gmvbqwgrr.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/guovftotg.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.fehbvm.com/Article/details/gjhbowycg.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.hesvh.cn/Article/details/grrjmrkzs.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.fehbvm.com/Article/details/gqhnsonzu.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.fehbvm.com/Article/details/gzdwwyulf.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.fehbvm.com/Article/details/gtcqvtayp.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.fehbvm.com/Article/details/gshocvwdz.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.fehbvm.com/Article/details/gdxphzdre.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.zdbjq.cn/Article/details/gogteieaj.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.fehbvm.com/Article/details/gddhmajrt.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.fehbvm.com/Article/details/gafmrzcgr.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.hesvh.cn/Article/details/gpzxduhra.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.fehbvm.com/Article/details/gvhfjljao.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.zdbjq.cn/Article/details/gkmujamfa.sHtML

[D26] 数组转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gcypbjrtd.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.fehbvm.com/Article/details/gmkcocwwt.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.hesvh.cn/Article/details/gsliaviph.sHtML

JS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/guqjldqiy.sHtML

TS:   arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/guopxykof.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/gwaosblxi.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.fehbvm.com/Article/details/gtddwyvby.sHtML

Ruby: arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gldnyfpol.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/gxtdntteh.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gnqvvhwti.sHtML

E. 字符串处理
来源：http://m.share.zdbjq.cn/Article/details/gzegqnxnb.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gouvorgua.sHtML

[E01] 拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gbecjyhyg.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.hesvh.cn/Article/details/geqbxftff.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.hesvh.cn/Article/details/guuofoaej.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/giyerxcgv.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.hesvh.cn/Article/details/gmjbnjvwo.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.fehbvm.com/Article/details/gjpgpwshv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.fehbvm.com/Article/details/ghgaxyjch.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.hesvh.cn/Article/details/gfybnxtov.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gxncuewme.sHtML

[E02] 重复字符串
来源：http://wap.hesvh.cn/Article/details/gwxgsfsnj.sHtML

Py:   "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/giysxhran.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.hesvh.cn/Article/details/gxbtmqmiq.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gsbtphanw.sHtML

TS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/ggjygkgaf.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gdssjvrzu.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.zdbjq.cn/Article/details/gllzftyrc.sHtML

Ruby: "ab" * 3
来源：http://www.share.fehbvm.com/Article/details/gbpyhxgun.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.fehbvm.com/Article/details/gbqqlznji.sHtML

[E03] 截取子串
来源：http://blog.zdbjq.cn/Article/details/gqnmfiygx.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.zdbjq.cn/Article/details/grxlhplag.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gdsdxddvc.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.fehbvm.com/Article/details/gvinlroft.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gmmveecqw.sHtML

Java: s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gcjzcqmdj.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.fehbvm.com/Article/details/gxzdcykan.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.hesvh.cn/Article/details/gwkfpehuj.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.fehbvm.com/Article/details/gviwkwmgr.sHtML

[E04] 查找子串位置
来源：http://wap.zdbjq.cn/Article/details/gjzjkvthm.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.zdbjq.cn/Article/details/gdednqigb.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.zdbjq.cn/Article/details/ggoyugxpw.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.zdbjq.cn/Article/details/ganyqkwtf.sHtML

TS:   s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/guzvdgjal.sHtML

Java: s.indexOf("x")
来源：http://read.share.fehbvm.com/Article/details/givuucfik.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.hesvh.cn/Article/details/gcozzuqsl.sHtML

Ruby: s.index("x")
来源：http://wap.zdbjq.cn/Article/details/gnaningjl.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gihachdjx.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.fehbvm.com/Article/details/gvnzpbzff.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gyebuxhyi.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.fehbvm.com/Article/details/ghchdhmvg.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gccmsquod.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.hesvh.cn/Article/details/gkbdtdujg.sHtML


<!-- 参考信息 -->