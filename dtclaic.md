代发 wailian999

Go:   // 无重载：用不同函数名
来源：http://www.share.hesvh.cn/Article/details/gkxacqaxc.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.hesvh.cn/Article/details/gxiqokyge.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.zdbjq.cn/Article/details/gpnxufmrg.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gzuzebxcl.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.fehbvm.com/Article/details/ggyrqkweg.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gjiasoriy.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.zdbjq.cn/Article/details/gizcuxrgy.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.zdbjq.cn/Article/details/gyshvawek.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.hesvh.cn/Article/details/gskguoclf.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.zdbjq.cn/Article/details/gaxaqihct.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.fehbvm.com/Article/details/gvoactwaa.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.zdbjq.cn/Article/details/gqkqvguzk.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.fehbvm.com/Article/details/gzsxcrlcj.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.fehbvm.com/Article/details/gafxhaeld.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.zdbjq.cn/Article/details/gdedqxxkr.sHtML

[D02] 追加元素到末尾
来源：http://blog.fehbvm.com/Article/details/ghvfpzdrc.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.hesvh.cn/Article/details/gmjapbckh.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.hesvh.cn/Article/details/ggfnanysu.sHtML

JS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/glbuoqbqx.sHtML

TS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/gdejwjvbk.sHtML

Java: list.add(4);
来源：http://wap.fehbvm.com/Article/details/gunubtfqf.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.zdbjq.cn/Article/details/gbaynjvjo.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.fehbvm.com/Article/details/gebxjfutx.sHtML

C#:   list.Add(4);
来源：http://read.share.zdbjq.cn/Article/details/ghzburwvg.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.fehbvm.com/Article/details/gdvznardq.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.zdbjq.cn/Article/details/gypubbvek.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.fehbvm.com/Article/details/guxmzzucf.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.hesvh.cn/Article/details/gvhkhtcxz.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.hesvh.cn/Article/details/gfjnmidew.sHtML

Java: list.add(0, 0);
来源：http://blog.hesvh.cn/Article/details/grwusxtrz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.zdbjq.cn/Article/details/glxmyaqzz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.hesvh.cn/Article/details/gpfghyouc.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.hesvh.cn/Article/details/gkysawcml.sHtML

[D04] 删除元素
来源：http://www.blog.fehbvm.com/Article/details/gzyqcjnsa.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.zdbjq.cn/Article/details/ggssidgjs.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.hesvh.cn/Article/details/gzidmvvqp.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.hesvh.cn/Article/details/gggxiblqs.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.hesvh.cn/Article/details/gncsrcwlu.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.fehbvm.com/Article/details/gwvczgpsl.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.fehbvm.com/Article/details/gtjqqukxl.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.zdbjq.cn/Article/details/gzbibtbqz.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.fehbvm.com/Article/details/geeqcorqz.sHtML

[D05] 访问与修改元素
来源：http://baike.fehbvm.com/Article/details/gwdrktayq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gedcuaicz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gjrucvwkq.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gcprlojtt.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.zdbjq.cn/Article/details/gsqlzqfeq.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.zdbjq.cn/Article/details/gfkgsqlqk.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gnqvjmqrp.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/glwhjalwt.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.hesvh.cn/Article/details/grazjbfot.sHtML

[D06] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/gpnzzjict.sHtML

Py:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/gmhbucyqr.sHtML

PHP:  count($arr);
来源：http://mobile.fehbvm.com/Article/details/gffethjvu.sHtML

JS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/gwrvciwjt.sHtML

TS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/gxqfznhzl.sHtML

Java: list.size();
来源：http://3g.hesvh.cn/Article/details/gzqaadlbb.sHtML

Go:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gxjokpuoi.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.fehbvm.com/Article/details/gkfvyqdim.sHtML

C#:   list.Count;
来源：http://3g.hesvh.cn/Article/details/ghpzcfqfc.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.zdbjq.cn/Article/details/gryoqsykx.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.zdbjq.cn/Article/details/gqkcnmfdy.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.hesvh.cn/Article/details/gtuugrjld.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gkzviuczy.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gocevdwja.sHtML

Java: list.subList(1, 4);
来源：http://baike.hesvh.cn/Article/details/gyfwxzwhv.sHtML

Go:   arr[1:4]
来源：http://www.blog.hesvh.cn/Article/details/gtmxpmdyr.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gjnwxyzft.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.fehbvm.com/Article/details/goaueqmkf.sHtML

[D08] 合并两个数组
来源：http://read.share.hesvh.cn/Article/details/godoxbmru.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.zdbjq.cn/Article/details/gdfvedfxr.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.fehbvm.com/Article/details/gdpucmxdx.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.hesvh.cn/Article/details/gwwvtaqht.sHtML

TS:   [...a, ...b];
来源：http://mobile.fehbvm.com/Article/details/gqksntxzu.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.zdbjq.cn/Article/details/gypunwqmd.sHtML

Go:   append(a, b...)
来源：http://mobile.hesvh.cn/Article/details/gchwmtvqa.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.hesvh.cn/Article/details/gygfvhflv.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gefjnxbol.sHtML

[D09] 排序（升序）
来源：http://m.share.fehbvm.com/Article/details/gdydymkzh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/gipsdnrno.sHtML

PHP:  sort($arr);
来源：http://www.blog.hesvh.cn/Article/details/gegcedndq.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.zdbjq.cn/Article/details/gbqurxowh.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.zdbjq.cn/Article/details/gommgxgve.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.fehbvm.com/Article/details/gpeienefa.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gfubinrfr.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gjzlhgmdy.sHtML

C#:   list.Sort();
来源：http://3g.hesvh.cn/Article/details/gmqmrkkva.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.hesvh.cn/Article/details/gixfbttvu.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.hesvh.cn/Article/details/gnilejaxr.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/gaegymxwu.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/gpzdbhspd.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/gtujuqdhj.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.fehbvm.com/Article/details/gbvwjautk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.zdbjq.cn/Article/details/gomlsuyfs.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.fehbvm.com/Article/details/ghyyiksie.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.fehbvm.com/Article/details/gwqczjwgl.sHtML

[D11] 反转数组
来源：http://blog.hesvh.cn/Article/details/grlakzwha.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.zdbjq.cn/Article/details/gevowkwip.sHtML

PHP:  array_reverse($arr);
来源：http://baike.hesvh.cn/Article/details/gazppiyuv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.fehbvm.com/Article/details/gbzivoobk.sHtML

TS:   [...arr].reverse();
来源：http://m.share.zdbjq.cn/Article/details/gccisyonv.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.hesvh.cn/Article/details/gtfbfifzb.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.hesvh.cn/Article/details/gjqcldtmr.sHtML

Ruby: arr.reverse
来源：http://3g.fehbvm.com/Article/details/gerleavhu.sHtML

C#:   list.Reverse();
来源：http://mobile.zdbjq.cn/Article/details/ggzubokpg.sHtML

[D12] 查找元素下标
来源：http://www.m.share.hesvh.cn/Article/details/gyvnwrdfm.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.fehbvm.com/Article/details/gwhlhclxc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.fehbvm.com/Article/details/gacsqulre.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.hesvh.cn/Article/details/gqawrdxqk.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/gsgqkapir.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.fehbvm.com/Article/details/gpbtolkbd.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gedqvvgdp.sHtML

Ruby: arr.index(x)
来源：http://3g.hesvh.cn/Article/details/gldymxmxx.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.hesvh.cn/Article/details/gejczijjl.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.hesvh.cn/Article/details/gvqcuyopn.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.fehbvm.com/Article/details/gukvyifyb.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gwcqfgdci.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/gvayqdmog.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/gdaxrfmmn.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.zdbjq.cn/Article/details/gfhbzzbbf.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.fehbvm.com/Article/details/gpyqgfeys.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.zdbjq.cn/Article/details/gnfilxekw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.fehbvm.com/Article/details/gmgjugbte.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.hesvh.cn/Article/details/gikxeuwvx.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gbhqdsptl.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.zdbjq.cn/Article/details/grpymbsyb.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.hesvh.cn/Article/details/gjuxvpfnt.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/ghplzrrqk.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.fehbvm.com/Article/details/gmowrydbi.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/gtzywqgmb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gurqzdeql.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.hesvh.cn/Article/details/gdjgavcgz.sHtML

[D15] 去重
来源：http://mobile.hesvh.cn/Article/details/gnmcemyjs.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.hesvh.cn/Article/details/gyhizuqek.sHtML

PHP:  array_unique($arr);
来源：http://read.share.zdbjq.cn/Article/details/gjbgkskdp.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gxaquyysu.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gknomkqvy.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.fehbvm.com/Article/details/ghydcsgxw.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.zdbjq.cn/Article/details/gpuhssdjm.sHtML

Ruby: arr.uniq
来源：http://www.blog.hesvh.cn/Article/details/gkftxzier.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gladtzkho.sHtML

[D16] 求和与平均值
来源：http://blog.hesvh.cn/Article/details/giwlyaigm.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.fehbvm.com/Article/details/ghrvtlsrn.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.zdbjq.cn/Article/details/gvciscymx.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gpmfxswse.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/giwcbhbvu.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.zdbjq.cn/Article/details/gtdbiqmsa.sHtML

Go:   // 手写循环累加
来源：http://www.share.fehbvm.com/Article/details/gcyelbjrq.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.hesvh.cn/Article/details/ggnrcqslv.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.fehbvm.com/Article/details/gghjctxoy.sHtML

[D17] 最大值与最小值
来源：http://m.share.zdbjq.cn/Article/details/grzimrjgt.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.fehbvm.com/Article/details/glqosiihe.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.hesvh.cn/Article/details/givuyjpbo.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gqbfxtmlj.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.fehbvm.com/Article/details/gtviwtqic.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gaoutkyno.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.fehbvm.com/Article/details/ggcphbvgg.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.hesvh.cn/Article/details/gznamxeco.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.zdbjq.cn/Article/details/gwkjnikvm.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.zdbjq.cn/Article/details/gxjcavfhr.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.fehbvm.com/Article/details/gogbnwsor.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fehbvm.com/Article/details/gwrvrjfcy.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.zdbjq.cn/Article/details/gkuabnrje.sHtML

TS:   nested.flat();
来源：http://www.share.fehbvm.com/Article/details/gbbzqjreu.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.zdbjq.cn/Article/details/gamvvstfn.sHtML

Go:   // 手写双层循环
来源：http://3g.zdbjq.cn/Article/details/gjnjocewx.sHtML

Ruby: nested.flatten
来源：http://m.share.zdbjq.cn/Article/details/gqqsemhix.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.fehbvm.com/Article/details/gtytvsliz.sHtML

[D19] 按字段分组
来源：http://www.m.share.fehbvm.com/Article/details/gbvrjbxmz.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.fehbvm.com/Article/details/gtaqbjgzu.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.hesvh.cn/Article/details/giqqzzban.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.zdbjq.cn/Article/details/gllysjeuv.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/gxtguynzh.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.fehbvm.com/Article/details/ggirkemvy.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.hesvh.cn/Article/details/gbhjlbguw.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.hesvh.cn/Article/details/gcxqvutks.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fehbvm.com/Article/details/gecwbrkan.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.zdbjq.cn/Article/details/gkgwprxrc.sHtML

Py:   Counter(arr)
来源：http://baike.zdbjq.cn/Article/details/gjxqucuyg.sHtML

PHP:  array_count_values($arr);
来源：http://blog.fehbvm.com/Article/details/gtnjvqehs.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fehbvm.com/Article/details/geejkcaid.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/ghgpqgfis.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.fehbvm.com/Article/details/ghwohznie.sHtML

Go:   // 手写 map[T]int
来源：http://3g.zdbjq.cn/Article/details/gbsdhlofz.sHtML

Ruby: arr.tally
来源：http://mobile.fehbvm.com/Article/details/gmlbjnbom.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.hesvh.cn/Article/details/goaiacawp.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.fehbvm.com/Article/details/gdprprfpg.sHtML

Py:   x in arr
来源：http://www.share.fehbvm.com/Article/details/gqyhfjmui.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.zdbjq.cn/Article/details/gdcnapktu.sHtML

JS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/gyawgykua.sHtML

TS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gzrtdccbp.sHtML

Java: list.contains(x)
来源：http://m.share.fehbvm.com/Article/details/gkfzlitaa.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.hesvh.cn/Article/details/gzgakhrin.sHtML

Ruby: arr.include?(x)
来源：http://m.share.zdbjq.cn/Article/details/geuriayee.sHtML

C#:   list.Contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gdvmhywbi.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.zdbjq.cn/Article/details/gnwkiqyhx.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.zdbjq.cn/Article/details/gaqgvdekh.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.zdbjq.cn/Article/details/gkjtgktls.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.zdbjq.cn/Article/details/gabgbwyyi.sHtML

TS:   [...arr];
来源：http://www.share.zdbjq.cn/Article/details/gisujcthl.sHtML

Java: new ArrayList<>(list);
来源：http://3g.hesvh.cn/Article/details/gntrucxtc.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.fehbvm.com/Article/details/gibydcnlb.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.hesvh.cn/Article/details/gvjbvdhfu.sHtML

C#:   new List<int>(list);
来源：http://baike.fehbvm.com/Article/details/goxgfaevf.sHtML

[D23] reduce 累积计算
来源：http://3g.hesvh.cn/Article/details/geekieqze.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.fehbvm.com/Article/details/glfimmazr.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.hesvh.cn/Article/details/gkwloafsv.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gksuuogey.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/gfwfpwmwq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.hesvh.cn/Article/details/gadolslan.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/gsngqfsgt.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.fehbvm.com/Article/details/gyzyuwvxt.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.zdbjq.cn/Article/details/gloyrfroo.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.zdbjq.cn/Article/details/gptqywqxg.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.fehbvm.com/Article/details/gkzpydmvo.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.zdbjq.cn/Article/details/gdwjnhgai.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.zdbjq.cn/Article/details/gbsbkhuab.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gjkglgqkf.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.hesvh.cn/Article/details/gbemykpex.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.zdbjq.cn/Article/details/gqgbuxkpe.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.hesvh.cn/Article/details/gxzutvayc.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.hesvh.cn/Article/details/gwpqdnksw.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.hesvh.cn/Article/details/gceselxoz.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.hesvh.cn/Article/details/guijhylri.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.hesvh.cn/Article/details/gwbjdfugm.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.zdbjq.cn/Article/details/gcucvyxdu.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.zdbjq.cn/Article/details/gtphvcgdq.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.zdbjq.cn/Article/details/gnuunhbpo.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.zdbjq.cn/Article/details/glyunautx.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.fehbvm.com/Article/details/guleybdio.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gfxqnvksy.sHtML

[D26] 数组转字符串
来源：http://read.share.hesvh.cn/Article/details/givhamhha.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.fehbvm.com/Article/details/gfggkatda.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.hesvh.cn/Article/details/ghvuowtrr.sHtML

JS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gzociyjxh.sHtML

TS:   arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/grmjzzoby.sHtML

Java: String.join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/gvjvnavnp.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.zdbjq.cn/Article/details/gaugumccg.sHtML

Ruby: arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gvmicazkh.sHtML

C#:   string.Join(", ", list)
来源：http://wap.fehbvm.com/Article/details/gmwotqyxs.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gckhetukt.sHtML

E. 字符串处理
来源：http://baike.fehbvm.com/Article/details/ggbjpcpal.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjbvxiuuj.sHtML

[E01] 拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gztapqvez.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.fehbvm.com/Article/details/gqhuirjgi.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.fehbvm.com/Article/details/gmtlyruvg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/grbeyujoc.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fehbvm.com/Article/details/ghpjzmano.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.hesvh.cn/Article/details/gcpazitnl.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.fehbvm.com/Article/details/ghwzgqmbl.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.hesvh.cn/Article/details/gyqudhlqo.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gzxpwxxbo.sHtML

[E02] 重复字符串
来源：http://wap.zdbjq.cn/Article/details/gyrzstnyr.sHtML

Py:   "ab" * 3
来源：http://wap.fehbvm.com/Article/details/gcdzomlkr.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.hesvh.cn/Article/details/gtkjpnfuj.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gjeygkgsw.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gidfmdscc.sHtML

Java: "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gebjxgnbd.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.hesvh.cn/Article/details/griglwaaf.sHtML

Ruby: "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/gamjmhulv.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.hesvh.cn/Article/details/gpqvgrjlh.sHtML

[E03] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/gsbddbjqs.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.hesvh.cn/Article/details/gqnqqweil.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gxvjeixgi.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/gumqgvirx.sHtML

TS:   s.slice(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gyxqwwfvm.sHtML

Java: s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gtxdvpaki.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.fehbvm.com/Article/details/gafrodfbt.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.hesvh.cn/Article/details/godokyzmw.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.hesvh.cn/Article/details/gwabvieuy.sHtML

[E04] 查找子串位置
来源：http://blog.zdbjq.cn/Article/details/gpxioluto.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.zdbjq.cn/Article/details/gsdibrufm.sHtML

PHP:  strpos($s, "x");
来源：http://baike.hesvh.cn/Article/details/gvnrvlkev.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.zdbjq.cn/Article/details/gwwccalov.sHtML

TS:   s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gakngmbht.sHtML

Java: s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/goqgdpooe.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.hesvh.cn/Article/details/ginjhdsia.sHtML

Ruby: s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/ggvntwljg.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gxgcelmaq.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.zdbjq.cn/Article/details/gxrabssct.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.hesvh.cn/Article/details/gpswcuehy.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.fehbvm.com/Article/details/ghmuyppzu.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gpsgdntca.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.fehbvm.com/Article/details/gsctmxnqw.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gpkjqyzdc.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.zdbjq.cn/Article/details/gekrgyfxi.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.fehbvm.com/Article/details/gwvvlfvzt.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.fehbvm.com/Article/details/gjjexipxx.sHtML

[E06] 替换子串
来源：http://www.blog.zdbjq.cn/Article/details/gqmxrqemm.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gtcjgoqom.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.zdbjq.cn/Article/details/gcpceotim.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gsynppokp.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gdivhczug.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gzgfhpeso.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/gcsqfexoy.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gykknksou.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.hesvh.cn/Article/details/gxcvmuiwn.sHtML

[E07] 按分隔符拆分
来源：http://3g.hesvh.cn/Article/details/gippjjqoh.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.fehbvm.com/Article/details/gjopsperq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.hesvh.cn/Article/details/gmsninmeu.sHtML


<!-- 参考信息 -->