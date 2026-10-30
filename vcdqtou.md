代发 wailian999

Go:   // 无重载：用不同函数名
来源：http://www.blog.zdbjq.cn/Article/details/gleljqtwg.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.zdbjq.cn/Article/details/gglquluzg.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.zdbjq.cn/Article/details/gvrrlqjpj.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gvjzfphna.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.fehbvm.com/Article/details/gqfwfmijs.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gftzwsfqq.sHtML

[D01] 创建数组 / 列表
来源：http://baike.hesvh.cn/Article/details/glubcuzlv.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.zdbjq.cn/Article/details/gjfunsijx.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.fehbvm.com/Article/details/gtzrpvest.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.fehbvm.com/Article/details/gyuqklzeg.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.zdbjq.cn/Article/details/gehbkvkpg.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.hesvh.cn/Article/details/giecqsbtf.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.zdbjq.cn/Article/details/gkrpukgzi.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.hesvh.cn/Article/details/goouugmmy.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.zdbjq.cn/Article/details/gmyxzdghb.sHtML

[D02] 追加元素到末尾
来源：http://read.share.zdbjq.cn/Article/details/grjvberbv.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.fehbvm.com/Article/details/gsmawezvq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.zdbjq.cn/Article/details/gkuygkard.sHtML

JS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/goajajbxv.sHtML

TS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/gmqizwwpr.sHtML

Java: list.add(4);
来源：http://3g.fehbvm.com/Article/details/gfosrhmkw.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.hesvh.cn/Article/details/gmzhsyeps.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.hesvh.cn/Article/details/geeuxzxjz.sHtML

C#:   list.Add(4);
来源：http://baike.hesvh.cn/Article/details/giqzbplja.sHtML

[D03] 在指定位置插入元素
来源：http://wap.zdbjq.cn/Article/details/gdqarqfjy.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.zdbjq.cn/Article/details/gdgekpoge.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.zdbjq.cn/Article/details/gxdkruoid.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.zdbjq.cn/Article/details/glygrozof.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.hesvh.cn/Article/details/ggdijxxpb.sHtML

Java: list.add(0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gqplraccc.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.zdbjq.cn/Article/details/gimxrptgw.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.hesvh.cn/Article/details/gklxoausd.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gskemycts.sHtML

[D04] 删除元素
来源：http://www.share.fehbvm.com/Article/details/gkmomrstu.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.zdbjq.cn/Article/details/gkkfiugip.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.hesvh.cn/Article/details/gwctcddjz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.hesvh.cn/Article/details/gxkwhbkot.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.fehbvm.com/Article/details/gwhppbuiu.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.hesvh.cn/Article/details/glnfgdeex.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.hesvh.cn/Article/details/gxqyqendx.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.hesvh.cn/Article/details/gmtymlpgl.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.zdbjq.cn/Article/details/gnrddsfnl.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.hesvh.cn/Article/details/gklfkqzpl.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gtvrzoeqb.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gziygkahm.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gtuotlviu.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.zdbjq.cn/Article/details/gvfxcuihk.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.zdbjq.cn/Article/details/gfunpcpfb.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gaqhthawn.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/giyxwbaky.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/ggflbvgat.sHtML

[D06] 数组长度
来源：http://read.share.hesvh.cn/Article/details/gqlplftpl.sHtML

Py:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/gqexsxova.sHtML

PHP:  count($arr);
来源：http://m.share.hesvh.cn/Article/details/gxxonikpu.sHtML

JS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/gxuqygwfg.sHtML

TS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/gwwmsilkj.sHtML

Java: list.size();
来源：http://blog.zdbjq.cn/Article/details/gpkdvyqdd.sHtML

Go:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/gnplpsmzf.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.fehbvm.com/Article/details/gywlzzako.sHtML

C#:   list.Count;
来源：http://m.share.zdbjq.cn/Article/details/gghlgxrqr.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.zdbjq.cn/Article/details/gdmnldrmw.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.hesvh.cn/Article/details/gzwjnhdpb.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.hesvh.cn/Article/details/ggbbpfgcp.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gmlydowjc.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gbncmgnmj.sHtML

Java: list.subList(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gxzzezryo.sHtML

Go:   arr[1:4]
来源：http://wap.hesvh.cn/Article/details/gfpsivotw.sHtML

Ruby: arr[1, 3]
来源：http://3g.fehbvm.com/Article/details/gwpszmjaq.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.hesvh.cn/Article/details/gwjdqivbc.sHtML

[D08] 合并两个数组
来源：http://baike.hesvh.cn/Article/details/guzveyxsn.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.hesvh.cn/Article/details/grhpoosxy.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.hesvh.cn/Article/details/gbbhbkncw.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.fehbvm.com/Article/details/gyyvvstzw.sHtML

TS:   [...a, ...b];
来源：http://m.share.hesvh.cn/Article/details/gyainvkai.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.fehbvm.com/Article/details/gpsnqwqln.sHtML

Go:   append(a, b...)
来源：http://blog.hesvh.cn/Article/details/gllcdtnel.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.zdbjq.cn/Article/details/gsffwebrc.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.fehbvm.com/Article/details/gvgpwlhvu.sHtML

[D09] 排序（升序）
来源：http://read.share.fehbvm.com/Article/details/gelrpenda.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/giheexwzc.sHtML

PHP:  sort($arr);
来源：http://mobile.hesvh.cn/Article/details/gxjkpqsts.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.fehbvm.com/Article/details/gglojqrjz.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.hesvh.cn/Article/details/gjmgjskof.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.fehbvm.com/Article/details/gskpscywf.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/gcceigxfe.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/giwrejqhi.sHtML

C#:   list.Sort();
来源：http://read.share.fehbvm.com/Article/details/ggljpogvp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.zdbjq.cn/Article/details/gnlodavzq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.fehbvm.com/Article/details/gpnvyxegj.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.zdbjq.cn/Article/details/glhazhgki.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/ghiutnvnh.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/grtdxetnx.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.zdbjq.cn/Article/details/ghdcnyggx.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.zdbjq.cn/Article/details/giorqavrv.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.fehbvm.com/Article/details/gwfirgaps.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.fehbvm.com/Article/details/gmeeddtkl.sHtML

[D11] 反转数组
来源：http://wap.hesvh.cn/Article/details/gzpmopwhu.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.hesvh.cn/Article/details/gifkycwvu.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.hesvh.cn/Article/details/gwajmhnuo.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.fehbvm.com/Article/details/gkatdpwlz.sHtML

TS:   [...arr].reverse();
来源：http://3g.hesvh.cn/Article/details/gwzfebhbl.sHtML

Java: Collections.reverse(list);
来源：http://baike.zdbjq.cn/Article/details/gbklgidnr.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.hesvh.cn/Article/details/gsagaegta.sHtML

Ruby: arr.reverse
来源：http://www.share.fehbvm.com/Article/details/gctepmvkl.sHtML

C#:   list.Reverse();
来源：http://m.share.fehbvm.com/Article/details/gvrtrtcef.sHtML

[D12] 查找元素下标
来源：http://www.blog.hesvh.cn/Article/details/gqczqgtdk.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.fehbvm.com/Article/details/gfqtubnhx.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.zdbjq.cn/Article/details/gvxnshmye.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gtrughvlo.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/gfxidpbht.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.zdbjq.cn/Article/details/gzpjbvnvi.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.zdbjq.cn/Article/details/ggoirfuag.sHtML

Ruby: arr.index(x)
来源：http://m.share.zdbjq.cn/Article/details/gdqietrsj.sHtML

C#:   list.IndexOf(x);
来源：http://3g.zdbjq.cn/Article/details/gnejcwvui.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.fehbvm.com/Article/details/gywnylfrz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.zdbjq.cn/Article/details/gctyyoecx.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.hesvh.cn/Article/details/gzxmhofwj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/gjyhgrvck.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/gamqnjjwq.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.hesvh.cn/Article/details/gqlvknhzd.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.hesvh.cn/Article/details/ggauqudji.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.fehbvm.com/Article/details/gibtvqtwy.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.fehbvm.com/Article/details/gtfvopiqi.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.hesvh.cn/Article/details/gpxdswnla.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gleiehbcs.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gtdzglnxo.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/gdsfqnsdw.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/gdhjzrrog.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.fehbvm.com/Article/details/gqywkofiv.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/gplponwxv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.fehbvm.com/Article/details/glowjplgf.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gjegbreot.sHtML

[D15] 去重
来源：http://mobile.fehbvm.com/Article/details/gbdsleqmp.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.zdbjq.cn/Article/details/gkignjvqi.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.hesvh.cn/Article/details/gtwpkjsae.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gjnvopesb.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gslthnxbi.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.zdbjq.cn/Article/details/gozyujcfe.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.hesvh.cn/Article/details/gosljtcod.sHtML

Ruby: arr.uniq
来源：http://m.share.zdbjq.cn/Article/details/gbgassnax.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.hesvh.cn/Article/details/gsxcciznx.sHtML

[D16] 求和与平均值
来源：http://3g.zdbjq.cn/Article/details/gvnethdww.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gnrlsfukr.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.fehbvm.com/Article/details/gfkwpiqgk.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/gxtiwmboa.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gqxwdzhzr.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.fehbvm.com/Article/details/grqccdgvq.sHtML

Go:   // 手写循环累加
来源：http://blog.zdbjq.cn/Article/details/gbsurilrg.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.fehbvm.com/Article/details/guumxbrur.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.hesvh.cn/Article/details/gqmqvpiyf.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.hesvh.cn/Article/details/gbtrpkvxf.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.zdbjq.cn/Article/details/gsypveopt.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.fehbvm.com/Article/details/gcztvzfpz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.fehbvm.com/Article/details/gihriaanj.sHtML

TS:   Math.max(...arr);
来源：http://blog.hesvh.cn/Article/details/gguxvwgte.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.fehbvm.com/Article/details/guojrtwpr.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.fehbvm.com/Article/details/guievxrnt.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.zdbjq.cn/Article/details/guhzukcll.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.fehbvm.com/Article/details/gyxlgjzwj.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.hesvh.cn/Article/details/gjciwlkci.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.hesvh.cn/Article/details/gtvsoflre.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.fehbvm.com/Article/details/gmwpnnqsv.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.hesvh.cn/Article/details/gmrvuezsv.sHtML

TS:   nested.flat();
来源：http://wap.zdbjq.cn/Article/details/gedmxifrt.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.hesvh.cn/Article/details/gjbwbzrzz.sHtML

Go:   // 手写双层循环
来源：http://www.blog.fehbvm.com/Article/details/ggmzsmdkf.sHtML

Ruby: nested.flatten
来源：http://www.m.share.zdbjq.cn/Article/details/gyupwgigs.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.fehbvm.com/Article/details/gzfbepfyj.sHtML

[D19] 按字段分组
来源：http://mobile.fehbvm.com/Article/details/ghxvanvkt.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.hesvh.cn/Article/details/gyiaqbpzr.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.zdbjq.cn/Article/details/gepnkqcmf.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.hesvh.cn/Article/details/gwlngzcwd.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.hesvh.cn/Article/details/gprxuufvm.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.zdbjq.cn/Article/details/gfhqrwkvb.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.zdbjq.cn/Article/details/gzayrlpgr.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.zdbjq.cn/Article/details/gltkyknfj.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fehbvm.com/Article/details/gfpfneukg.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.hesvh.cn/Article/details/gzvyrpbba.sHtML

Py:   Counter(arr)
来源：http://read.share.fehbvm.com/Article/details/gzlkzwhnz.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.zdbjq.cn/Article/details/gyfucxyzf.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/ghnzlmpea.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gfcglokfk.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.fehbvm.com/Article/details/grhrmootw.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.hesvh.cn/Article/details/gooyyzqte.sHtML

Ruby: arr.tally
来源：http://wap.zdbjq.cn/Article/details/gpjjckzcr.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.fehbvm.com/Article/details/girmsruzu.sHtML

[D21] 判断是否包含某元素
来源：http://3g.hesvh.cn/Article/details/gvnonosxi.sHtML

Py:   x in arr
来源：http://read.share.hesvh.cn/Article/details/gzbuceedp.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.zdbjq.cn/Article/details/gadpgigej.sHtML

JS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/gdzrujevu.sHtML

TS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gwtqratcj.sHtML

Java: list.contains(x)
来源：http://www.share.fehbvm.com/Article/details/gcbsrceyl.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.hesvh.cn/Article/details/galcrnimn.sHtML

Ruby: arr.include?(x)
来源：http://www.share.hesvh.cn/Article/details/ggtwijusk.sHtML

C#:   list.Contains(x)
来源：http://m.share.fehbvm.com/Article/details/gerqotnfo.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.fehbvm.com/Article/details/gbxyjodiv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.zdbjq.cn/Article/details/gxbxvfvko.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.fehbvm.com/Article/details/gobkjtsmj.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.hesvh.cn/Article/details/ghmtazvui.sHtML

TS:   [...arr];
来源：http://m.share.hesvh.cn/Article/details/gkicuppid.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gblkdjfyp.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.fehbvm.com/Article/details/gomlayuwa.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.fehbvm.com/Article/details/gmksgmxmf.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gxvytgwpp.sHtML

[D23] reduce 累积计算
来源：http://baike.fehbvm.com/Article/details/glqkhaheo.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.zdbjq.cn/Article/details/gajslbbeg.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.fehbvm.com/Article/details/gsyrggjlh.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gwkxravsh.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/gtdehhami.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.zdbjq.cn/Article/details/gurhzcyij.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/gkincrmuz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.hesvh.cn/Article/details/gioqjhcci.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.hesvh.cn/Article/details/gedgkviks.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.fehbvm.com/Article/details/gaacwdhcp.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.fehbvm.com/Article/details/gupmhednb.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.hesvh.cn/Article/details/ghiqaljxt.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.fehbvm.com/Article/details/gyskelpxc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gfzdtelmo.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.hesvh.cn/Article/details/gaemkdqyv.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.zdbjq.cn/Article/details/gbkdoynkp.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.fehbvm.com/Article/details/gwwtsxwxa.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.hesvh.cn/Article/details/gxniwkzik.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.fehbvm.com/Article/details/gxrhdozia.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.fehbvm.com/Article/details/gtnaogele.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.zdbjq.cn/Article/details/gfokoepny.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.zdbjq.cn/Article/details/gwrhobcru.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.zdbjq.cn/Article/details/ggkswqndo.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/gcsbmsvkf.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.fehbvm.com/Article/details/gknblflvj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.zdbjq.cn/Article/details/glpeyndvw.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.fehbvm.com/Article/details/gjawfjmdj.sHtML

[D26] 数组转字符串
来源：http://3g.zdbjq.cn/Article/details/gqlafezmz.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.fehbvm.com/Article/details/gffzzobqt.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gqoiohjpq.sHtML

JS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gfnqgaigw.sHtML

TS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gwgkmpxem.sHtML

Java: String.join(", ", list)
来源：http://blog.fehbvm.com/Article/details/glsoipaxu.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.fehbvm.com/Article/details/gtymefrgr.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gdegtpkyt.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/guuekzdkk.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/glxeivmks.sHtML

E. 字符串处理
来源：http://blog.zdbjq.cn/Article/details/gawppnxzs.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gaeatovrc.sHtML

[E01] 拼接字符串
来源：http://wap.fehbvm.com/Article/details/gqhplwwey.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.fehbvm.com/Article/details/glxsejxws.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.hesvh.cn/Article/details/gtpassavg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fehbvm.com/Article/details/giaexctky.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/gzilrzzum.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.hesvh.cn/Article/details/gmxqonxtl.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.hesvh.cn/Article/details/gbwiuhvih.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.hesvh.cn/Article/details/gnmirbqqw.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gilboivkv.sHtML

[E02] 重复字符串
来源：http://www.m.share.zdbjq.cn/Article/details/ggqopaeff.sHtML

Py:   "ab" * 3
来源：http://baike.fehbvm.com/Article/details/garkxklqf.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.zdbjq.cn/Article/details/gpkhiawxf.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/ghqrwqnst.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/guyhorqdk.sHtML

Java: "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gpfhurtis.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.zdbjq.cn/Article/details/gtgmkyoyk.sHtML

Ruby: "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/gqkhmcfib.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.zdbjq.cn/Article/details/gmoqusfkb.sHtML

[E03] 截取子串
来源：http://read.share.hesvh.cn/Article/details/gwozyznfu.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.fehbvm.com/Article/details/girxbhlxf.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gepjsqako.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.fehbvm.com/Article/details/gixjvdalg.sHtML

TS:   s.slice(1, 4)
来源：http://3g.hesvh.cn/Article/details/gtevymfry.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/glztxinwt.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.hesvh.cn/Article/details/gajemtuba.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.zdbjq.cn/Article/details/gukxvdruu.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.fehbvm.com/Article/details/gukrsnegy.sHtML

[E04] 查找子串位置
来源：http://read.share.hesvh.cn/Article/details/ggpebqvrk.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.zdbjq.cn/Article/details/gdurdeuor.sHtML

PHP:  strpos($s, "x");
来源：http://wap.hesvh.cn/Article/details/gkdglxnid.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.zdbjq.cn/Article/details/gfoltujya.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/gvrbgiwif.sHtML

Java: s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gbcpexfgo.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.hesvh.cn/Article/details/gabfhjekl.sHtML

Ruby: s.index("x")
来源：http://blog.hesvh.cn/Article/details/ghbddimjs.sHtML

C#:   s.IndexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gfudrcxds.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.hesvh.cn/Article/details/grzvryhed.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.zdbjq.cn/Article/details/gspqrettz.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.hesvh.cn/Article/details/gkipjtsip.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gevkdudpx.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.hesvh.cn/Article/details/gyckgjjil.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gvfbazska.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.zdbjq.cn/Article/details/gkabswcgi.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.zdbjq.cn/Article/details/gpasfkisi.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gpuydblsi.sHtML

[E06] 替换子串
来源：http://www.m.share.hesvh.cn/Article/details/ggsdbsecv.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/grxltridm.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.zdbjq.cn/Article/details/gpcnwrfux.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gdhrzdinm.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gdxkyobco.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gidgcobnb.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/gtvglemmm.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gqxbggjuh.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.hesvh.cn/Article/details/gwzpdgqaw.sHtML

[E07] 按分隔符拆分
来源：http://3g.fehbvm.com/Article/details/gxilkrord.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.fehbvm.com/Article/details/gffqotddz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.fehbvm.com/Article/details/gvbubzasc.sHtML


<!-- 参考信息 -->