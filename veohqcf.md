代发 wailian999

PHP:  // 无重载
来源：http://m.share.zdbjq.cn/Article/details/gdpjdojoo.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.hesvh.cn/Article/details/gpbcorodf.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.zdbjq.cn/Article/details/gzhdcjqxk.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.zdbjq.cn/Article/details/gzdyvklqn.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.fehbvm.com/Article/details/gyorewylr.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.hesvh.cn/Article/details/gbguqkxdg.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.zdbjq.cn/Article/details/gpstwfwqf.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gqxgewxta.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.fehbvm.com/Article/details/gygapsesr.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gmkrpojvd.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.fehbvm.com/Article/details/gxlarclvn.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.fehbvm.com/Article/details/gflojspcl.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/gtayuvrgn.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.fehbvm.com/Article/details/ggszleqvy.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.zdbjq.cn/Article/details/gyfqtymgv.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.fehbvm.com/Article/details/ghbhnmimj.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.hesvh.cn/Article/details/grlccodvq.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.fehbvm.com/Article/details/gouigfoec.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.zdbjq.cn/Article/details/gghfrgtyp.sHtML

[D02] 追加元素到末尾
来源：http://baike.hesvh.cn/Article/details/gnmqxedng.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.fehbvm.com/Article/details/gpybnekgx.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.hesvh.cn/Article/details/gqwnizhkk.sHtML

JS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/gbnvafuhs.sHtML

TS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/gtjizixho.sHtML

Java: list.add(4);
来源：http://m.share.fehbvm.com/Article/details/gdjhznkca.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.zdbjq.cn/Article/details/gflqztnuu.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.hesvh.cn/Article/details/glwvyobda.sHtML

C#:   list.Add(4);
来源：http://www.share.zdbjq.cn/Article/details/gbasbigez.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.hesvh.cn/Article/details/gwklrzxuc.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fehbvm.com/Article/details/gitefjgve.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.zdbjq.cn/Article/details/gmjzaepxg.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.zdbjq.cn/Article/details/gpprqcceq.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.fehbvm.com/Article/details/glivcvywp.sHtML

Java: list.add(0, 0);
来源：http://wap.zdbjq.cn/Article/details/gqvpmgtsg.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.hesvh.cn/Article/details/glvbgzhqs.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.hesvh.cn/Article/details/gbbjgrlok.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/ghcvbibnl.sHtML

[D04] 删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gjbcggjec.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.fehbvm.com/Article/details/ghuxtxmcz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.fehbvm.com/Article/details/gtivsqrze.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.hesvh.cn/Article/details/gwuvjsexp.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.fehbvm.com/Article/details/gmzbednsv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.fehbvm.com/Article/details/gozuhcsqj.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.zdbjq.cn/Article/details/gcockodvc.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.zdbjq.cn/Article/details/gjprwnsex.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.hesvh.cn/Article/details/gfovwtryt.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.fehbvm.com/Article/details/gmyyoiqdv.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gsabxboyq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gxxennqig.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gaysvoicl.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.zdbjq.cn/Article/details/gyshwyxdv.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.fehbvm.com/Article/details/gbqveeiwy.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gzzvfsgmr.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gwmhkqvql.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/ganbzmujj.sHtML

[D06] 数组长度
来源：http://www.share.hesvh.cn/Article/details/gqunjjilm.sHtML

Py:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gdnnndzch.sHtML

PHP:  count($arr);
来源：http://m.share.zdbjq.cn/Article/details/ggsjypmub.sHtML

JS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/grlaerrvc.sHtML

TS:   arr.length
来源：http://blog.hesvh.cn/Article/details/gtfbagzni.sHtML

Java: list.size();
来源：http://www.m.share.fehbvm.com/Article/details/gyyilknry.sHtML

Go:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gtiflqsaf.sHtML

Ruby: arr.length; arr.size
来源：http://3g.hesvh.cn/Article/details/gdzcnsawj.sHtML

C#:   list.Count;
来源：http://wap.fehbvm.com/Article/details/gmyfetljr.sHtML

[D07] 切片 / 取子数组
来源：http://blog.hesvh.cn/Article/details/gokwddyhs.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.zdbjq.cn/Article/details/gffkkpdpk.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.hesvh.cn/Article/details/geesqojne.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gyvxwmwah.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gssqbqidu.sHtML

Java: list.subList(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gqxzviohz.sHtML

Go:   arr[1:4]
来源：http://blog.fehbvm.com/Article/details/gnyzmkgco.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gufhmjrlr.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.zdbjq.cn/Article/details/gcwqgosno.sHtML

[D08] 合并两个数组
来源：http://3g.fehbvm.com/Article/details/gyfjjajda.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.hesvh.cn/Article/details/gsahvdaaz.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.hesvh.cn/Article/details/gsmspgmzy.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.hesvh.cn/Article/details/gslsqdaws.sHtML

TS:   [...a, ...b];
来源：http://wap.zdbjq.cn/Article/details/ggfehtoqt.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.fehbvm.com/Article/details/guxtfyamw.sHtML

Go:   append(a, b...)
来源：http://mobile.zdbjq.cn/Article/details/grktkfqjo.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.zdbjq.cn/Article/details/gdrvjsoqq.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/ghympppqi.sHtML

[D09] 排序（升序）
来源：http://3g.zdbjq.cn/Article/details/gmzhogbye.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gwjuthfcu.sHtML

PHP:  sort($arr);
来源：http://www.share.fehbvm.com/Article/details/ghimqgdws.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.zdbjq.cn/Article/details/gapijsfcg.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.hesvh.cn/Article/details/gyshnfawm.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.hesvh.cn/Article/details/grmlpctee.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gszawlppz.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gjofzkdki.sHtML

C#:   list.Sort();
来源：http://m.share.hesvh.cn/Article/details/gcjferepj.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.hesvh.cn/Article/details/gynspbiyt.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gdycjxmug.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.hesvh.cn/Article/details/ggvytalea.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gttopnzsv.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/gfnphnjyq.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.hesvh.cn/Article/details/gxnfmpuwl.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.fehbvm.com/Article/details/gensqiure.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.hesvh.cn/Article/details/gulispyey.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.zdbjq.cn/Article/details/gnwgnvpxe.sHtML

[D11] 反转数组
来源：http://www.blog.zdbjq.cn/Article/details/gszzahlxp.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.fehbvm.com/Article/details/gcnhelumc.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gqskqsanb.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.zdbjq.cn/Article/details/gmhvsznvb.sHtML

TS:   [...arr].reverse();
来源：http://3g.hesvh.cn/Article/details/ghtpxupck.sHtML

Java: Collections.reverse(list);
来源：http://baike.fehbvm.com/Article/details/gggqkidtk.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.zdbjq.cn/Article/details/gtixvymef.sHtML

Ruby: arr.reverse
来源：http://blog.fehbvm.com/Article/details/gqpqbzkfq.sHtML

C#:   list.Reverse();
来源：http://m.share.zdbjq.cn/Article/details/gegdrkwhr.sHtML

[D12] 查找元素下标
来源：http://m.share.hesvh.cn/Article/details/gmquxficz.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.fehbvm.com/Article/details/gljpbuzol.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.zdbjq.cn/Article/details/ghzlaxzae.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/gymmnnrwf.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fehbvm.com/Article/details/gaugiyvel.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.hesvh.cn/Article/details/grrtgjbtr.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gvrrjfulv.sHtML

Ruby: arr.index(x)
来源：http://read.share.hesvh.cn/Article/details/gclgmushh.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.hesvh.cn/Article/details/gdurtonvz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.hesvh.cn/Article/details/gbnmcvptw.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.hesvh.cn/Article/details/ghzcwkiyo.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.hesvh.cn/Article/details/gsvyohvzn.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/ggdyxzdmg.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/greazfwqb.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.fehbvm.com/Article/details/gdebgjnzv.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.zdbjq.cn/Article/details/guawzxxjv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.hesvh.cn/Article/details/gethdevhc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.hesvh.cn/Article/details/gurxhlont.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.hesvh.cn/Article/details/gtfemwkzg.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.zdbjq.cn/Article/details/ggsajqkos.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gctmtpimz.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gwbkzqhun.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/ggxudloum.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.zdbjq.cn/Article/details/gceihuowd.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/guwvbrenu.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.hesvh.cn/Article/details/gouktyrbu.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.hesvh.cn/Article/details/gpxnrflrf.sHtML

[D15] 去重
来源：http://www.share.fehbvm.com/Article/details/gszncohlm.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.fehbvm.com/Article/details/gjxfwwhzq.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.hesvh.cn/Article/details/glwsebjbf.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gfdljxfdl.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/ghjbhvnbw.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.fehbvm.com/Article/details/gxmytbabu.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.fehbvm.com/Article/details/gfzwwvpff.sHtML

Ruby: arr.uniq
来源：http://wap.zdbjq.cn/Article/details/gjhifhorj.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.hesvh.cn/Article/details/gnewaburc.sHtML

[D16] 求和与平均值
来源：http://baike.fehbvm.com/Article/details/gnuewzbvb.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.fehbvm.com/Article/details/gxmydswen.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.hesvh.cn/Article/details/gbygzxnil.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/gplgmmnzy.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gvvxcwthl.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.fehbvm.com/Article/details/guhllyumz.sHtML

Go:   // 手写循环累加
来源：http://mobile.fehbvm.com/Article/details/gzmbibsml.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.zdbjq.cn/Article/details/givllctfv.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.zdbjq.cn/Article/details/gvjpjxlqo.sHtML

[D17] 最大值与最小值
来源：http://3g.hesvh.cn/Article/details/gduswepir.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.zdbjq.cn/Article/details/gsmxrzcnr.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.hesvh.cn/Article/details/gvsznhheu.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.zdbjq.cn/Article/details/gpmmltbml.sHtML

TS:   Math.max(...arr);
来源：http://blog.zdbjq.cn/Article/details/gbrfpwaar.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.hesvh.cn/Article/details/gqdkketqk.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.fehbvm.com/Article/details/gmvfxakhb.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.hesvh.cn/Article/details/gtawttngw.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.fehbvm.com/Article/details/ghygnevik.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.zdbjq.cn/Article/details/gntsoichl.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.zdbjq.cn/Article/details/gwhxopfdi.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.fehbvm.com/Article/details/gvabtdafb.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.fehbvm.com/Article/details/gvptlmbdy.sHtML

TS:   nested.flat();
来源：http://www.m.share.fehbvm.com/Article/details/gjblmriec.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.fehbvm.com/Article/details/ghuskpyxl.sHtML

Go:   // 手写双层循环
来源：http://3g.zdbjq.cn/Article/details/gjwupowpf.sHtML

Ruby: nested.flatten
来源：http://mobile.zdbjq.cn/Article/details/gbvyqrfxw.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.fehbvm.com/Article/details/guaufnvog.sHtML

[D19] 按字段分组
来源：http://www.m.share.fehbvm.com/Article/details/gopmzhlop.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.hesvh.cn/Article/details/gsrkbrkpk.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.zdbjq.cn/Article/details/gdxrepluh.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.fehbvm.com/Article/details/gwogwygby.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/ghvikytxz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.fehbvm.com/Article/details/gxlycrfgz.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.zdbjq.cn/Article/details/grsjhcfex.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.fehbvm.com/Article/details/guichudfg.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.zdbjq.cn/Article/details/gqoiukfhw.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.fehbvm.com/Article/details/genufadug.sHtML

Py:   Counter(arr)
来源：http://read.share.zdbjq.cn/Article/details/gilfsizvg.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.hesvh.cn/Article/details/gozesqcev.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/glzivjwxj.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fehbvm.com/Article/details/gadgdrtjq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.zdbjq.cn/Article/details/gqjycbjee.sHtML

Go:   // 手写 map[T]int
来源：http://baike.zdbjq.cn/Article/details/grcwmxhsd.sHtML

Ruby: arr.tally
来源：http://wap.hesvh.cn/Article/details/gyoobpwar.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.hesvh.cn/Article/details/godngjktz.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.hesvh.cn/Article/details/gnwatytet.sHtML

Py:   x in arr
来源：http://www.blog.hesvh.cn/Article/details/gwrcjvwwa.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.fehbvm.com/Article/details/gexhzzvjy.sHtML

JS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/ghdauouie.sHtML

TS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/gwctxllyx.sHtML

Java: list.contains(x)
来源：http://www.share.hesvh.cn/Article/details/gnqnpgxgz.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gmqgzbrvm.sHtML

Ruby: arr.include?(x)
来源：http://read.share.hesvh.cn/Article/details/gmzgsutde.sHtML

C#:   list.Contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gltsqfznu.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.zdbjq.cn/Article/details/gdphhenrd.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.hesvh.cn/Article/details/gvjdpgxdl.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.hesvh.cn/Article/details/gzhikagfc.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.hesvh.cn/Article/details/gphkjsmrp.sHtML

TS:   [...arr];
来源：http://read.share.fehbvm.com/Article/details/gtwwrxghl.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.hesvh.cn/Article/details/gfdqozdsb.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.fehbvm.com/Article/details/gactafpxg.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.zdbjq.cn/Article/details/giczcwfje.sHtML

C#:   new List<int>(list);
来源：http://baike.fehbvm.com/Article/details/gomnyzxtn.sHtML

[D23] reduce 累积计算
来源：http://3g.fehbvm.com/Article/details/glcsvawxv.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.fehbvm.com/Article/details/gmpwxenhf.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.zdbjq.cn/Article/details/geluozjsw.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/gtwiwkbqm.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/ghexryxjz.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.fehbvm.com/Article/details/ghmyfzaew.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/guxlnuixw.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.zdbjq.cn/Article/details/gajmxfezu.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.fehbvm.com/Article/details/gzybvhach.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.hesvh.cn/Article/details/gazlrgwct.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.fehbvm.com/Article/details/gjegiijjp.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.fehbvm.com/Article/details/goqbbclnb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.hesvh.cn/Article/details/golgvhtdy.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.zdbjq.cn/Article/details/ggjaqgonc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.hesvh.cn/Article/details/gtujakupx.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.zdbjq.cn/Article/details/gabyivpnf.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.hesvh.cn/Article/details/grkcmhttq.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.zdbjq.cn/Article/details/gupdezmoj.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.zdbjq.cn/Article/details/gvvqnwnhe.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.zdbjq.cn/Article/details/gripuevza.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.zdbjq.cn/Article/details/ghhvcndab.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.hesvh.cn/Article/details/gzxiipftd.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.zdbjq.cn/Article/details/guyjehngx.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.zdbjq.cn/Article/details/gruncrmcq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.zdbjq.cn/Article/details/gwubmcwtv.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.zdbjq.cn/Article/details/gyezczwve.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.hesvh.cn/Article/details/gyktykton.sHtML

[D26] 数组转字符串
来源：http://m.share.fehbvm.com/Article/details/ggsvveema.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.hesvh.cn/Article/details/gbgxzdbqs.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.fehbvm.com/Article/details/gomnwfecu.sHtML

JS:   arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gbosixhrw.sHtML

TS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gcxclsrpr.sHtML

Java: String.join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/ggqlwecrg.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.hesvh.cn/Article/details/gqbljmabh.sHtML

Ruby: arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gwatcfcvg.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.fehbvm.com/Article/details/gogmwhlcx.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/grqdaaoap.sHtML

E. 字符串处理
来源：http://wap.hesvh.cn/Article/details/grptbmyqm.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzrkmtbvs.sHtML

[E01] 拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gbmksolxw.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.fehbvm.com/Article/details/gvhqyrzyo.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.hesvh.cn/Article/details/gqbgeglgo.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gubmaylfp.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/gnktchrro.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.fehbvm.com/Article/details/gxdqugoqv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.hesvh.cn/Article/details/gahnnkwdd.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.hesvh.cn/Article/details/gyxkatdvx.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gmrymgzmn.sHtML

[E02] 重复字符串
来源：http://www.blog.hesvh.cn/Article/details/gbsbbbmin.sHtML

Py:   "ab" * 3
来源：http://www.m.share.hesvh.cn/Article/details/gvvxccxhu.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.zdbjq.cn/Article/details/gwszcyptq.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gyizyqkgm.sHtML

TS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/guudpvapc.sHtML

Java: "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gqxizswvg.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.hesvh.cn/Article/details/gkexsvbtc.sHtML

Ruby: "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/glxjefrmg.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.hesvh.cn/Article/details/gpcssrgjz.sHtML

[E03] 截取子串
来源：http://wap.zdbjq.cn/Article/details/gnehagjry.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.fehbvm.com/Article/details/gzyioskur.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gnhqdracy.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/gdqjmubhz.sHtML

TS:   s.slice(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gpstbtqmz.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gauwhymbm.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.hesvh.cn/Article/details/ggcogkzyw.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.fehbvm.com/Article/details/gxiiyucgf.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.hesvh.cn/Article/details/gqgcmxlmc.sHtML

[E04] 查找子串位置
来源：http://www.share.zdbjq.cn/Article/details/gnmrcvyqs.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.zdbjq.cn/Article/details/gdxxatzxh.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.zdbjq.cn/Article/details/gruhecugv.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.hesvh.cn/Article/details/gxcvmpqyt.sHtML

TS:   s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/gwaygrwqd.sHtML

Java: s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gmhxjqsap.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.fehbvm.com/Article/details/gzavojaom.sHtML

Ruby: s.index("x")
来源：http://wap.zdbjq.cn/Article/details/gpexucwzl.sHtML

C#:   s.IndexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gkwzpxokn.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.fehbvm.com/Article/details/gixnvngrz.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.hesvh.cn/Article/details/goumypypn.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.fehbvm.com/Article/details/gdkturnfl.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gnhechfrz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.zdbjq.cn/Article/details/gmvaobnlb.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/gzqhvjsvb.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.fehbvm.com/Article/details/ggsxvobvh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.hesvh.cn/Article/details/gsgilhxje.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gkplbhnkb.sHtML

[E06] 替换子串
来源：http://wap.hesvh.cn/Article/details/ggwwokhgj.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/gdjpwwteo.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.fehbvm.com/Article/details/gbkihdkbk.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gtcchvvja.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gufuwzwqd.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gudwdcpdm.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/gbxhqicds.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.fehbvm.com/Article/details/gfbeivvts.sHtML


<!-- 参考信息 -->