代发 wailian999

Go:   // 无重载：用不同函数名
来源：http://www.blog.fehbvm.com/Article/details/gyrqmltzc.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.zdbjq.cn/Article/details/gbeeuxpzn.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.fehbvm.com/Article/details/guoseczfz.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghkngmxul.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.hesvh.cn/Article/details/gksaggrxg.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gfgjcfpoj.sHtML

[D01] 创建数组 / 列表
来源：http://wap.fehbvm.com/Article/details/gamrgipdb.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.hesvh.cn/Article/details/gtvbsvuky.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.hesvh.cn/Article/details/gcuucmoen.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.hesvh.cn/Article/details/gmcfpfpfu.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.hesvh.cn/Article/details/gacobkbum.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.zdbjq.cn/Article/details/gwwvzxgzk.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.hesvh.cn/Article/details/goereptmh.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.hesvh.cn/Article/details/ggweoblcn.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.hesvh.cn/Article/details/ghatuvyrq.sHtML

[D02] 追加元素到末尾
来源：http://m.share.fehbvm.com/Article/details/ghvpnisgn.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.zdbjq.cn/Article/details/grdpomjdc.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.zdbjq.cn/Article/details/gmteeyuuk.sHtML

JS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gmtkilwty.sHtML

TS:   arr.push(4);
来源：http://baike.hesvh.cn/Article/details/gsgfltjnx.sHtML

Java: list.add(4);
来源：http://www.blog.zdbjq.cn/Article/details/gvasennkj.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.fehbvm.com/Article/details/grpbahnyi.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.zdbjq.cn/Article/details/gdytboexa.sHtML

C#:   list.Add(4);
来源：http://blog.hesvh.cn/Article/details/glnzncbob.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.hesvh.cn/Article/details/gjpeehcqu.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.fehbvm.com/Article/details/gmvesichk.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.fehbvm.com/Article/details/gkdfphjkb.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.fehbvm.com/Article/details/gyyellmbw.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gjmmbajhe.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gqaxrodji.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.hesvh.cn/Article/details/glxstlyga.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.zdbjq.cn/Article/details/grwnuzhoc.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.fehbvm.com/Article/details/gwjbgodls.sHtML

[D04] 删除元素
来源：http://m.share.zdbjq.cn/Article/details/gbbvrpeac.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.fehbvm.com/Article/details/gmgdhwwfk.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gvsmtocgo.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.zdbjq.cn/Article/details/geltdijba.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.zdbjq.cn/Article/details/gghkmmfbd.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.hesvh.cn/Article/details/gnmhcdfor.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.hesvh.cn/Article/details/gjzvpyecu.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.hesvh.cn/Article/details/gjsnglczd.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.zdbjq.cn/Article/details/grdwgaxqg.sHtML

[D05] 访问与修改元素
来源：http://www.blog.fehbvm.com/Article/details/gojjzslno.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gwuftyxgh.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gwyfndabj.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gowhpheqw.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.hesvh.cn/Article/details/gxoswpbnz.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.fehbvm.com/Article/details/gobmjhpsk.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/ggbzycmpt.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gsmgnndur.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gthbvgnaj.sHtML

[D06] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/gcmnlidze.sHtML

Py:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/ggifdszlr.sHtML

PHP:  count($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gmexieoej.sHtML

JS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/ghvfxpqhb.sHtML

TS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/gselvzzyi.sHtML

Java: list.size();
来源：http://www.share.hesvh.cn/Article/details/gvsbvzulj.sHtML

Go:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/gnrqyadah.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.fehbvm.com/Article/details/glswsswzr.sHtML

C#:   list.Count;
来源：http://wap.zdbjq.cn/Article/details/gzlxtqvxh.sHtML

[D07] 切片 / 取子数组
来源：http://wap.hesvh.cn/Article/details/gbzxjvwfx.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.fehbvm.com/Article/details/gbkgeqlww.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.fehbvm.com/Article/details/guuheudtk.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/ghpzyplra.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/gmunjdlxf.sHtML

Java: list.subList(1, 4);
来源：http://3g.fehbvm.com/Article/details/gpshyzruo.sHtML

Go:   arr[1:4]
来源：http://blog.hesvh.cn/Article/details/gyxaiqalv.sHtML

Ruby: arr[1, 3]
来源：http://mobile.hesvh.cn/Article/details/gankaolxa.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.fehbvm.com/Article/details/gomjmixpl.sHtML

[D08] 合并两个数组
来源：http://baike.fehbvm.com/Article/details/grbotnjds.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.hesvh.cn/Article/details/gvrpqoeia.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.hesvh.cn/Article/details/gvtpxnwjo.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.hesvh.cn/Article/details/gfnnpfchz.sHtML

TS:   [...a, ...b];
来源：http://blog.fehbvm.com/Article/details/gactpihjw.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gtdfuuckz.sHtML

Go:   append(a, b...)
来源：http://www.blog.fehbvm.com/Article/details/gedoqtchi.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.zdbjq.cn/Article/details/gaupaliaj.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.zdbjq.cn/Article/details/gskpsoaoy.sHtML

[D09] 排序（升序）
来源：http://blog.fehbvm.com/Article/details/gnocptnnk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gfoudcshk.sHtML

PHP:  sort($arr);
来源：http://read.share.fehbvm.com/Article/details/gzmhtjaeq.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.fehbvm.com/Article/details/gxlnecdkj.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.zdbjq.cn/Article/details/gpzvcxqpc.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.fehbvm.com/Article/details/gzqwtcyig.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gloosdrjz.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/gzvwldkff.sHtML

C#:   list.Sort();
来源：http://read.share.hesvh.cn/Article/details/grrdkigdc.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.fehbvm.com/Article/details/gftuiabwz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.fehbvm.com/Article/details/gwhhwdqwq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/giydtfurr.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fehbvm.com/Article/details/gaosprkdy.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fehbvm.com/Article/details/gnmephlxb.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.hesvh.cn/Article/details/ghzfwytqp.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.zdbjq.cn/Article/details/gepctcfre.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.zdbjq.cn/Article/details/ggjyhzcww.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.hesvh.cn/Article/details/gyxmvdrgk.sHtML

[D11] 反转数组
来源：http://mobile.zdbjq.cn/Article/details/gdvmgtpty.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.fehbvm.com/Article/details/gxgtvlqva.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.hesvh.cn/Article/details/gvlxfaphi.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.hesvh.cn/Article/details/gmkwmbriq.sHtML

TS:   [...arr].reverse();
来源：http://blog.zdbjq.cn/Article/details/gbjltnthr.sHtML

Java: Collections.reverse(list);
来源：http://baike.hesvh.cn/Article/details/gmxxivges.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.fehbvm.com/Article/details/gplspyzmg.sHtML

Ruby: arr.reverse
来源：http://www.blog.hesvh.cn/Article/details/giouovtji.sHtML

C#:   list.Reverse();
来源：http://read.share.fehbvm.com/Article/details/gtpidmbwj.sHtML

[D12] 查找元素下标
来源：http://3g.zdbjq.cn/Article/details/gxbliuiiy.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.hesvh.cn/Article/details/gdnxqpfhb.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gcvjopsux.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/ghpxhhgbm.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/gyapxbgth.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.fehbvm.com/Article/details/guiztjcqj.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gqmturowx.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.fehbvm.com/Article/details/gddkhnepy.sHtML

C#:   list.IndexOf(x);
来源：http://baike.hesvh.cn/Article/details/gcsrvjwrw.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.fehbvm.com/Article/details/gomzximjm.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.hesvh.cn/Article/details/gdfbsibck.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.zdbjq.cn/Article/details/gdpvfzkwf.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/gqzxzvrxy.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/gtxgyghmu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.zdbjq.cn/Article/details/gptqmdtlg.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.hesvh.cn/Article/details/glnmxgyyp.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.zdbjq.cn/Article/details/gccpwieue.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gmswkkhjs.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.hesvh.cn/Article/details/glbgrpqap.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.zdbjq.cn/Article/details/gbazoaehi.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.fehbvm.com/Article/details/gqoowrzfs.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gtpbbghta.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/gowbsckjf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gzqebiola.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/gamvoaivl.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gatjhyacz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.zdbjq.cn/Article/details/gntpbxbin.sHtML

[D15] 去重
来源：http://www.blog.hesvh.cn/Article/details/gttergeys.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.zdbjq.cn/Article/details/gcdkeuwaw.sHtML

PHP:  array_unique($arr);
来源：http://blog.fehbvm.com/Article/details/gowrdispk.sHtML

JS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gjbanhefy.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gxoxrluer.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.zdbjq.cn/Article/details/gnettevea.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.zdbjq.cn/Article/details/goifivwws.sHtML

Ruby: arr.uniq
来源：http://wap.zdbjq.cn/Article/details/gexoqosmp.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gijpztitf.sHtML

[D16] 求和与平均值
来源：http://www.m.share.fehbvm.com/Article/details/gypqfawdl.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.fehbvm.com/Article/details/gqkvgdofs.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.fehbvm.com/Article/details/gfotygvax.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gaotzrysq.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fehbvm.com/Article/details/gdshtjisf.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.fehbvm.com/Article/details/ghjpfgine.sHtML

Go:   // 手写循环累加
来源：http://www.share.hesvh.cn/Article/details/gotoyzqut.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.fehbvm.com/Article/details/gawlwqjmr.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.zdbjq.cn/Article/details/ggslhqeuj.sHtML

[D17] 最大值与最小值
来源：http://mobile.hesvh.cn/Article/details/gzaplamin.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.fehbvm.com/Article/details/genhgygeo.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.fehbvm.com/Article/details/gwntroljn.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.hesvh.cn/Article/details/ghnbkzsqn.sHtML

TS:   Math.max(...arr);
来源：http://m.share.fehbvm.com/Article/details/ghuxrozpf.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.fehbvm.com/Article/details/gnyuufkxa.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.fehbvm.com/Article/details/gfrncfgmr.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.fehbvm.com/Article/details/gtvupdoop.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.zdbjq.cn/Article/details/gbmvvelep.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.fehbvm.com/Article/details/gtlxfybam.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.fehbvm.com/Article/details/ggilonceh.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.fehbvm.com/Article/details/goxdxhyjf.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.hesvh.cn/Article/details/gfpzmnhns.sHtML

TS:   nested.flat();
来源：http://wap.zdbjq.cn/Article/details/ggplzirrf.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.hesvh.cn/Article/details/gxyrlaxjw.sHtML

Go:   // 手写双层循环
来源：http://3g.fehbvm.com/Article/details/gbgflvcqo.sHtML

Ruby: nested.flatten
来源：http://wap.zdbjq.cn/Article/details/gbxwwzgfm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gdqcxvsbi.sHtML

[D19] 按字段分组
来源：http://3g.zdbjq.cn/Article/details/gixjhqcnk.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.hesvh.cn/Article/details/gjcogcitb.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.zdbjq.cn/Article/details/gguvujtso.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.zdbjq.cn/Article/details/gfjiaxccj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/grmrpotvh.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.zdbjq.cn/Article/details/gnnnkkknu.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.hesvh.cn/Article/details/gwudpbgtg.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.hesvh.cn/Article/details/gnjyqihmi.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.hesvh.cn/Article/details/gxqznjzlf.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.zdbjq.cn/Article/details/gvhyhbjii.sHtML

Py:   Counter(arr)
来源：http://blog.zdbjq.cn/Article/details/gmxvyfyru.sHtML

PHP:  array_count_values($arr);
来源：http://baike.hesvh.cn/Article/details/glomeroaa.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/gnaywxamn.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/gxhugplnb.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.fehbvm.com/Article/details/gguhvspzp.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.fehbvm.com/Article/details/guexiznuu.sHtML

Ruby: arr.tally
来源：http://3g.fehbvm.com/Article/details/gegknocis.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.fehbvm.com/Article/details/gtmjovans.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.zdbjq.cn/Article/details/gpcnhpiyx.sHtML

Py:   x in arr
来源：http://www.blog.zdbjq.cn/Article/details/gawmtbaxp.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.zdbjq.cn/Article/details/gqoozlcbd.sHtML

JS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/glztqzfrk.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gmnwermxj.sHtML

Java: list.contains(x)
来源：http://mobile.hesvh.cn/Article/details/gvrgymbyx.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gvkabytzw.sHtML

Ruby: arr.include?(x)
来源：http://baike.zdbjq.cn/Article/details/gtbsbjiax.sHtML

C#:   list.Contains(x)
来源：http://m.share.hesvh.cn/Article/details/gvucijore.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.zdbjq.cn/Article/details/guobkagth.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.hesvh.cn/Article/details/gstyrjbso.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.zdbjq.cn/Article/details/gewqlepfh.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.hesvh.cn/Article/details/gzlkqieuu.sHtML

TS:   [...arr];
来源：http://wap.hesvh.cn/Article/details/glbhlzauz.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.zdbjq.cn/Article/details/ghoukbbej.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.fehbvm.com/Article/details/gyxwbrakk.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.hesvh.cn/Article/details/gvkbafgfa.sHtML

C#:   new List<int>(list);
来源：http://wap.zdbjq.cn/Article/details/gfstzrfqd.sHtML

[D23] reduce 累积计算
来源：http://baike.hesvh.cn/Article/details/guznkpatb.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gjjxghlwr.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.hesvh.cn/Article/details/gbkmfttfv.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/gquojxjmn.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gnhszpsza.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.fehbvm.com/Article/details/gtuamvpjd.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/gdsvpwfpx.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.hesvh.cn/Article/details/gezpqsyrs.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.hesvh.cn/Article/details/gmjlryqpb.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.zdbjq.cn/Article/details/glvfqppnu.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.zdbjq.cn/Article/details/gejxcbgkw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.hesvh.cn/Article/details/ggiwwjnfu.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gsdqflpxz.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.hesvh.cn/Article/details/gsydsbqqt.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.hesvh.cn/Article/details/gthetfsyr.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.hesvh.cn/Article/details/gubolaona.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.hesvh.cn/Article/details/ghrvsmgdq.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.zdbjq.cn/Article/details/gdxgjcget.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.fehbvm.com/Article/details/gjehowmml.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.zdbjq.cn/Article/details/giwzfavic.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.fehbvm.com/Article/details/gjjinujyv.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.zdbjq.cn/Article/details/gjixbcwzd.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.fehbvm.com/Article/details/gdecepvlz.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/ggyxriljb.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.zdbjq.cn/Article/details/gbjtadvgu.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.zdbjq.cn/Article/details/gjqffdjih.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.zdbjq.cn/Article/details/gaowpkhkc.sHtML

[D26] 数组转字符串
来源：http://3g.zdbjq.cn/Article/details/gsqpkhjad.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.hesvh.cn/Article/details/gitpkqnln.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.hesvh.cn/Article/details/gddhhrjbp.sHtML

JS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gchzyclvf.sHtML

TS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gwtrlnuqt.sHtML

Java: String.join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/gktardtxd.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.hesvh.cn/Article/details/grkzubyyo.sHtML

Ruby: arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gdyaoqeks.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/gbdpgugpm.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gjctpgebu.sHtML

E. 字符串处理
来源：http://3g.hesvh.cn/Article/details/gqprntmce.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gpwmjycwx.sHtML

[E01] 拼接字符串
来源：http://3g.fehbvm.com/Article/details/gpuynsbrm.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.hesvh.cn/Article/details/goqocchhh.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.fehbvm.com/Article/details/gsuiqtaye.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.hesvh.cn/Article/details/gmkmaolpb.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/guxwoueqj.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.fehbvm.com/Article/details/gchkwxcfu.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.hesvh.cn/Article/details/gnforfidp.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.fehbvm.com/Article/details/glzwoybzh.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gsmjebscw.sHtML

[E02] 重复字符串
来源：http://mobile.zdbjq.cn/Article/details/goqpbrgcn.sHtML

Py:   "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/grpppajxq.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.hesvh.cn/Article/details/glgfanghv.sHtML

JS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gpuebcujr.sHtML

TS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gwgilwnom.sHtML

Java: "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gxbhwfmwb.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.zdbjq.cn/Article/details/grzehawfe.sHtML

Ruby: "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/gtqecmufk.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.zdbjq.cn/Article/details/gwpdvyabe.sHtML

[E03] 截取子串
来源：http://baike.hesvh.cn/Article/details/gmclhqktf.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.zdbjq.cn/Article/details/gobecomfx.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gvdnpwwau.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gjjmspqsq.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gyltptlzi.sHtML

Java: s.substring(1, 4)
来源：http://wap.hesvh.cn/Article/details/gxmaeaagu.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/glprwloyr.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.fehbvm.com/Article/details/gbmjjkzpy.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.fehbvm.com/Article/details/gghugkvvh.sHtML

[E04] 查找子串位置
来源：http://baike.hesvh.cn/Article/details/gzadnipva.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/ghhwhiezp.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.zdbjq.cn/Article/details/gbhztrurc.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.hesvh.cn/Article/details/ghrmudikm.sHtML

TS:   s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gsxwhvdjk.sHtML

Java: s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/glpdftndu.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.hesvh.cn/Article/details/gacyohlub.sHtML

Ruby: s.index("x")
来源：http://3g.zdbjq.cn/Article/details/ghdngtnrd.sHtML

C#:   s.IndexOf("x")
来源：http://blog.fehbvm.com/Article/details/gmkxwnzmy.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.zdbjq.cn/Article/details/gbmvhjwsn.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.fehbvm.com/Article/details/gjugxhwes.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.fehbvm.com/Article/details/glrzbfedx.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.hesvh.cn/Article/details/gnndhoimu.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.hesvh.cn/Article/details/gfdbpmhzf.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/geunycanc.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.fehbvm.com/Article/details/gudytmqdm.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.hesvh.cn/Article/details/gitibegee.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gxsftullu.sHtML

[E06] 替换子串
来源：http://read.share.zdbjq.cn/Article/details/gldmgzsue.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/gpyzwtdho.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gkkouxihq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gzuadgsuk.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gqdnbycsa.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gumhvznvc.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/gcbcqeaiv.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gcrghdlxh.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gbsmgilvo.sHtML

[E07] 按分隔符拆分
来源：http://m.share.zdbjq.cn/Article/details/gsbmlfilk.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.fehbvm.com/Article/details/gkgxuaxqa.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.zdbjq.cn/Article/details/gafqgyyax.sHtML


<!-- 参考信息 -->