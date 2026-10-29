代发 wailian999

Ruby: a, b = pair
来源：http://3g.fehbvm.com/Article/details/gecusfenw.sHtML

C#:   var (a, b) = pair;
来源：http://3g.fehbvm.com/Article/details/gmeeihoyb.sHtML

[C16] 函数 / 方法重载
来源：http://blog.zdbjq.cn/Article/details/gyluolqii.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.fehbvm.com/Article/details/gxtllteku.sHtML

PHP:  // 无重载
来源：http://m.share.zdbjq.cn/Article/details/grhtxgbix.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.hesvh.cn/Article/details/gjuqbtpsv.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.hesvh.cn/Article/details/gggvniqbd.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.hesvh.cn/Article/details/gygjmcckz.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.zdbjq.cn/Article/details/gpbbmxwwq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.zdbjq.cn/Article/details/gqvabtkbc.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.hesvh.cn/Article/details/gpmrtpqpl.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gjzxbkcvw.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.zdbjq.cn/Article/details/giyroswig.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gzdbckwvi.sHtML

[D01] 创建数组 / 列表
来源：http://baike.hesvh.cn/Article/details/gkjwobmmj.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.fehbvm.com/Article/details/gradsigah.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/gpovmcjma.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.hesvh.cn/Article/details/gqqqnrjsa.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.fehbvm.com/Article/details/guzgdxgad.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.fehbvm.com/Article/details/glaigxnjr.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.fehbvm.com/Article/details/gilnqypuw.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.hesvh.cn/Article/details/ghvnvjqsw.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.fehbvm.com/Article/details/gwuggwnuw.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.zdbjq.cn/Article/details/gaiqiykzd.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.zdbjq.cn/Article/details/gzopqrfgp.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.fehbvm.com/Article/details/gfwykoris.sHtML

JS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/gllnrfroq.sHtML

TS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gffustrqw.sHtML

Java: list.add(4);
来源：http://wap.fehbvm.com/Article/details/gesmaagje.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.zdbjq.cn/Article/details/gllrzvjja.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.fehbvm.com/Article/details/glkuixfnd.sHtML

C#:   list.Add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/grhrkanbc.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.hesvh.cn/Article/details/gpfasqpel.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.zdbjq.cn/Article/details/gwahuqgrz.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.fehbvm.com/Article/details/gnanuggcw.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.fehbvm.com/Article/details/gpqmuhhbm.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gjazzndtq.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gzdtlrhwh.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gjjcbynjx.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.fehbvm.com/Article/details/gfvuikqtg.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gcnlgtbeb.sHtML

[D04] 删除元素
来源：http://m.share.hesvh.cn/Article/details/gkdjembkc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.hesvh.cn/Article/details/gizwymeeg.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.zdbjq.cn/Article/details/gyhegaabd.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.fehbvm.com/Article/details/ghrconuoz.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.fehbvm.com/Article/details/gyweoanbt.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.fehbvm.com/Article/details/guscsczsw.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.fehbvm.com/Article/details/grvkcpaau.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.fehbvm.com/Article/details/gnmspliqt.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.zdbjq.cn/Article/details/gzxbjfoln.sHtML

[D05] 访问与修改元素
来源：http://www.share.fehbvm.com/Article/details/gbqzieazl.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/groiwllzi.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gjzvankjo.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gskvhdffs.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.zdbjq.cn/Article/details/ggdkqukao.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.fehbvm.com/Article/details/gwvthonvf.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gnmdwndsf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gbtenpdtv.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/grtgjrhsn.sHtML

[D06] 数组长度
来源：http://blog.hesvh.cn/Article/details/gymfhgtpj.sHtML

Py:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gozwhmjjj.sHtML

PHP:  count($arr);
来源：http://www.blog.hesvh.cn/Article/details/gkrfqnfjh.sHtML

JS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/gkkvibvon.sHtML

TS:   arr.length
来源：http://www.m.share.hesvh.cn/Article/details/gcggwrecm.sHtML

Java: list.size();
来源：http://wap.hesvh.cn/Article/details/gambasclf.sHtML

Go:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/gzypwgxnw.sHtML

Ruby: arr.length; arr.size
来源：http://wap.hesvh.cn/Article/details/genagbbxv.sHtML

C#:   list.Count;
来源：http://www.blog.hesvh.cn/Article/details/gneumirhq.sHtML

[D07] 切片 / 取子数组
来源：http://baike.hesvh.cn/Article/details/gdcmjnnot.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.fehbvm.com/Article/details/guewdbuly.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.zdbjq.cn/Article/details/gpwpykofg.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gkdnfdxuo.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gbjfichol.sHtML

Java: list.subList(1, 4);
来源：http://wap.hesvh.cn/Article/details/ggvwlneii.sHtML

Go:   arr[1:4]
来源：http://wap.zdbjq.cn/Article/details/glipqadsx.sHtML

Ruby: arr[1, 3]
来源：http://3g.hesvh.cn/Article/details/gcniynbae.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.zdbjq.cn/Article/details/grpghzgud.sHtML

[D08] 合并两个数组
来源：http://3g.hesvh.cn/Article/details/gswyokkyf.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.fehbvm.com/Article/details/glyuxrtrc.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.fehbvm.com/Article/details/geqkcnbvr.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.fehbvm.com/Article/details/gcpujmqoo.sHtML

TS:   [...a, ...b];
来源：http://baike.zdbjq.cn/Article/details/gcckiiqpj.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.fehbvm.com/Article/details/ghrxtdifc.sHtML

Go:   append(a, b...)
来源：http://3g.hesvh.cn/Article/details/gzslruviv.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.zdbjq.cn/Article/details/ghujaknei.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.hesvh.cn/Article/details/gzsvllxov.sHtML

[D09] 排序（升序）
来源：http://blog.fehbvm.com/Article/details/grhkngpnx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/ggxzknxmj.sHtML

PHP:  sort($arr);
来源：http://wap.fehbvm.com/Article/details/glgzgmjoc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.hesvh.cn/Article/details/gbwzqtpil.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.fehbvm.com/Article/details/ginrcomkv.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.zdbjq.cn/Article/details/gbftvyqkg.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gewtpbneh.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gxqmkbigr.sHtML

C#:   list.Sort();
来源：http://m.share.zdbjq.cn/Article/details/gvlhutuew.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.zdbjq.cn/Article/details/gymomnxlo.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.fehbvm.com/Article/details/gbqwfhwhx.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.zdbjq.cn/Article/details/gndiwnmpu.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/gbdsjvlet.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/grrontpef.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.hesvh.cn/Article/details/gcwhnnuvh.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.hesvh.cn/Article/details/gpdmtptap.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.fehbvm.com/Article/details/geuanapqq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.fehbvm.com/Article/details/gpxkphqrm.sHtML

[D11] 反转数组
来源：http://www.m.share.fehbvm.com/Article/details/gokfjzpww.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.hesvh.cn/Article/details/gjhtkytas.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.fehbvm.com/Article/details/gogjfcooy.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.fehbvm.com/Article/details/gkflhojzs.sHtML

TS:   [...arr].reverse();
来源：http://www.share.hesvh.cn/Article/details/gahyglmpy.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.fehbvm.com/Article/details/gfgggknip.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gzemmqomh.sHtML

Ruby: arr.reverse
来源：http://baike.zdbjq.cn/Article/details/gvxrfoohf.sHtML

C#:   list.Reverse();
来源：http://m.share.hesvh.cn/Article/details/gkwyhvtyn.sHtML

[D12] 查找元素下标
来源：http://www.blog.zdbjq.cn/Article/details/gcaknehge.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.zdbjq.cn/Article/details/gptsydxey.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/guaxneerg.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/gladfeppo.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/gxqhqqsem.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.hesvh.cn/Article/details/gbocitlfg.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gqvnxskbs.sHtML

Ruby: arr.index(x)
来源：http://www.share.hesvh.cn/Article/details/gvjjvgydj.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.zdbjq.cn/Article/details/ghtiluxep.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.zdbjq.cn/Article/details/gqglprewk.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.fehbvm.com/Article/details/gfchkjydp.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.fehbvm.com/Article/details/gjdxvcmzd.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/ggbidytlk.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gjwgiavlv.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.zdbjq.cn/Article/details/gmbavvelm.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.fehbvm.com/Article/details/gmebuogvo.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.hesvh.cn/Article/details/gaziuoxyo.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.fehbvm.com/Article/details/grxwacvds.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.hesvh.cn/Article/details/gqahixxmm.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.fehbvm.com/Article/details/gcizfpqyf.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.fehbvm.com/Article/details/ggnpafbwh.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/giwoltebf.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/grqeushho.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.hesvh.cn/Article/details/gsnjagdjt.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/gffiasmzg.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/glkfiikxn.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.fehbvm.com/Article/details/grbegoehc.sHtML

[D15] 去重
来源：http://3g.hesvh.cn/Article/details/gvghcfpkb.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gwhhsoivi.sHtML

PHP:  array_unique($arr);
来源：http://www.share.fehbvm.com/Article/details/gmdxhthif.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gwzlzjnje.sHtML

TS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gajcbnoon.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.zdbjq.cn/Article/details/godzpydmo.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.zdbjq.cn/Article/details/gucncyiln.sHtML

Ruby: arr.uniq
来源：http://mobile.hesvh.cn/Article/details/gnccexovf.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.zdbjq.cn/Article/details/gkhfhcubw.sHtML

[D16] 求和与平均值
来源：http://m.share.fehbvm.com/Article/details/gedrllsfu.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.fehbvm.com/Article/details/gihhgjsks.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.fehbvm.com/Article/details/gxoalzypi.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gjtmsxmlo.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/grfyzsnms.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.hesvh.cn/Article/details/gjicdvcie.sHtML

Go:   // 手写循环累加
来源：http://www.share.hesvh.cn/Article/details/gqajuaxkn.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.fehbvm.com/Article/details/gcsyevxja.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.hesvh.cn/Article/details/goigadmbl.sHtML

[D17] 最大值与最小值
来源：http://www.share.hesvh.cn/Article/details/gmnvmagdw.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.hesvh.cn/Article/details/gezszdoxo.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.fehbvm.com/Article/details/grkpcqhlf.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.fehbvm.com/Article/details/gpvyzfqyx.sHtML

TS:   Math.max(...arr);
来源：http://3g.zdbjq.cn/Article/details/gepvowfln.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.hesvh.cn/Article/details/gcblwjevu.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.zdbjq.cn/Article/details/gchbfqpoy.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.zdbjq.cn/Article/details/gwwrtqwzu.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.hesvh.cn/Article/details/gcqtjvecf.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.hesvh.cn/Article/details/gkoiifbbl.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.zdbjq.cn/Article/details/gkyamoftf.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.hesvh.cn/Article/details/ghgkdzowy.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.zdbjq.cn/Article/details/gcjxkmvne.sHtML

TS:   nested.flat();
来源：http://www.blog.fehbvm.com/Article/details/ghrdijfxa.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.zdbjq.cn/Article/details/geqevwswc.sHtML

Go:   // 手写双层循环
来源：http://mobile.zdbjq.cn/Article/details/gseyflevc.sHtML

Ruby: nested.flatten
来源：http://www.share.fehbvm.com/Article/details/gsoptdptd.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.hesvh.cn/Article/details/gvnsdlfjt.sHtML

[D19] 按字段分组
来源：http://www.m.share.fehbvm.com/Article/details/gyhdfxrpq.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.hesvh.cn/Article/details/gciymcijl.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.hesvh.cn/Article/details/ggplmcery.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.zdbjq.cn/Article/details/gbtrmmide.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/gfxxeyvoa.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.hesvh.cn/Article/details/giaospfug.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.hesvh.cn/Article/details/gbsivzqae.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.fehbvm.com/Article/details/gnrbeyaly.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.hesvh.cn/Article/details/gotssgnxk.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.fehbvm.com/Article/details/gosaktulx.sHtML

Py:   Counter(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gvmekyrij.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.zdbjq.cn/Article/details/gwfkacpbo.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/gozrbveeq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gwoezuelf.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.fehbvm.com/Article/details/gunfilaqf.sHtML

Go:   // 手写 map[T]int
来源：http://blog.zdbjq.cn/Article/details/gvlftdjoa.sHtML

Ruby: arr.tally
来源：http://baike.zdbjq.cn/Article/details/gsmcgmiuo.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.fehbvm.com/Article/details/gdoxewtky.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.hesvh.cn/Article/details/guxrgenmb.sHtML

Py:   x in arr
来源：http://read.share.hesvh.cn/Article/details/gmkfvyvtr.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.fehbvm.com/Article/details/grgfmcgvl.sHtML

JS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/gnedcgzwo.sHtML

TS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gxyoximlg.sHtML

Java: list.contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gwnwwxkdf.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gvbwiwhcu.sHtML

Ruby: arr.include?(x)
来源：http://3g.hesvh.cn/Article/details/gwoztxvwr.sHtML

C#:   list.Contains(x)
来源：http://3g.hesvh.cn/Article/details/gcbxcyeua.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.fehbvm.com/Article/details/gajiueqzb.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.fehbvm.com/Article/details/ghviwvszk.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.zdbjq.cn/Article/details/gkjfluekq.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.zdbjq.cn/Article/details/gtqqqapgr.sHtML

TS:   [...arr];
来源：http://wap.hesvh.cn/Article/details/gicgforzm.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.hesvh.cn/Article/details/gvurwfylv.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.hesvh.cn/Article/details/gpkikhnvg.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.zdbjq.cn/Article/details/gqyxtrvls.sHtML

C#:   new List<int>(list);
来源：http://baike.fehbvm.com/Article/details/gqbjmcbah.sHtML

[D23] reduce 累积计算
来源：http://3g.hesvh.cn/Article/details/gtytnywfh.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.zdbjq.cn/Article/details/gfhsethym.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.zdbjq.cn/Article/details/goobqeydy.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/gvvykvkmd.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gzugjnsmf.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.fehbvm.com/Article/details/gljzxumwk.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/geyybsdho.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.hesvh.cn/Article/details/gdxzjpcld.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.fehbvm.com/Article/details/gnavnlksx.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.hesvh.cn/Article/details/gbdshanfj.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.zdbjq.cn/Article/details/gqdxtyugn.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.zdbjq.cn/Article/details/gqzobicfl.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.zdbjq.cn/Article/details/gmypbusht.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gzazrnokw.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.fehbvm.com/Article/details/gienrjews.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.fehbvm.com/Article/details/ghhwhwcor.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.zdbjq.cn/Article/details/gzqmhcymr.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.fehbvm.com/Article/details/gsjqtbqdl.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.hesvh.cn/Article/details/getfxpubb.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.hesvh.cn/Article/details/govoelwwb.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.zdbjq.cn/Article/details/gdwvwettd.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.fehbvm.com/Article/details/glvaqgwqp.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.hesvh.cn/Article/details/gimacrjxj.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.fehbvm.com/Article/details/gjbfrahxt.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.zdbjq.cn/Article/details/gcrfnsnpd.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.hesvh.cn/Article/details/gxtagkutr.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gjfxzbako.sHtML

[D26] 数组转字符串
来源：http://m.share.fehbvm.com/Article/details/gvjcyjyxg.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.fehbvm.com/Article/details/gezcsqezh.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.zdbjq.cn/Article/details/gkijshcqx.sHtML

JS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gfmqdocqi.sHtML

TS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gfomcmbyi.sHtML

Java: String.join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/gccuqgfww.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.hesvh.cn/Article/details/gmkawnitb.sHtML

Ruby: arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gcojbuzzy.sHtML

C#:   string.Join(", ", list)
来源：http://blog.fehbvm.com/Article/details/gkhaiuida.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gkpfytezn.sHtML

E. 字符串处理
来源：http://read.share.zdbjq.cn/Article/details/gpugamiat.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gncvldkda.sHtML

[E01] 拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gzaepmbme.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.zdbjq.cn/Article/details/guquseijp.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.zdbjq.cn/Article/details/gmhbyhqyi.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gezgdwfhp.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/gsfjxvykc.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.hesvh.cn/Article/details/gfxcvfoco.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.hesvh.cn/Article/details/gfdrkgbhm.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.hesvh.cn/Article/details/gfeknmyyf.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gqpnjvkto.sHtML

[E02] 重复字符串
来源：http://www.share.fehbvm.com/Article/details/gndducjfx.sHtML

Py:   "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/gmvikuxlp.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.zdbjq.cn/Article/details/gglajclmo.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gndppngcq.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gjsuhvscx.sHtML

Java: "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/grkwsyuml.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.fehbvm.com/Article/details/gvnjwujos.sHtML

Ruby: "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/gkayhbvxj.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.fehbvm.com/Article/details/gnrqjzois.sHtML

[E03] 截取子串
来源：http://3g.zdbjq.cn/Article/details/grswxbbic.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.fehbvm.com/Article/details/glsljighb.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gzslarlzm.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gdrjhwvsy.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gehxkdhwa.sHtML

Java: s.substring(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gaavpwvnk.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.zdbjq.cn/Article/details/gticbzbxz.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.fehbvm.com/Article/details/gbozyooon.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.zdbjq.cn/Article/details/gjttyvlty.sHtML

[E04] 查找子串位置
来源：http://blog.hesvh.cn/Article/details/gowxpzwvf.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.zdbjq.cn/Article/details/gtxxfvrbu.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.fehbvm.com/Article/details/grviamrcj.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.hesvh.cn/Article/details/gbleufpom.sHtML

TS:   s.indexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gdbsgupjm.sHtML

Java: s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/gukkhaesf.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.hesvh.cn/Article/details/gbdmtkvzn.sHtML

Ruby: s.index("x")
来源：http://read.share.fehbvm.com/Article/details/geudqjegy.sHtML

C#:   s.IndexOf("x")
来源：http://wap.fehbvm.com/Article/details/gvitgcpyv.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.hesvh.cn/Article/details/gxgiieckq.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.fehbvm.com/Article/details/gzhbithop.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.fehbvm.com/Article/details/geibtzgyy.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/ghpbosxjy.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.fehbvm.com/Article/details/gesbgeqtf.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gojvqayod.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.zdbjq.cn/Article/details/gyrurmoza.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.hesvh.cn/Article/details/gzniefjic.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.fehbvm.com/Article/details/gvaenvckn.sHtML

[E06] 替换子串
来源：http://mobile.hesvh.cn/Article/details/gmqjarvbk.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/gtbeoztxy.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.fehbvm.com/Article/details/ghvjzgnky.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gpsxooqfj.sHtML


<!-- 参考信息 -->