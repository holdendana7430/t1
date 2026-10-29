代发 wailian999

PHP:  // 无重载
来源：http://3g.fehbvm.com/Article/details/gduuwovcy.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.zdbjq.cn/Article/details/gudzdvrpe.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.zdbjq.cn/Article/details/gpncsqgnx.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.fehbvm.com/Article/details/gzorrltko.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.hesvh.cn/Article/details/gbgdxhvya.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.hesvh.cn/Article/details/gshsueuuw.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.fehbvm.com/Article/details/gbklpggpx.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gybdphbpo.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.hesvh.cn/Article/details/gfgfxfyde.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gruexqcbq.sHtML

[D01] 创建数组 / 列表
来源：http://baike.hesvh.cn/Article/details/gzktoyhev.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.zdbjq.cn/Article/details/gvtgzladq.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/gnxdjakrj.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.hesvh.cn/Article/details/ggtsspqkh.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.hesvh.cn/Article/details/gtwoczrjv.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.zdbjq.cn/Article/details/gpfsehyuv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.fehbvm.com/Article/details/gocfkryra.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.fehbvm.com/Article/details/gibpufbpq.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.fehbvm.com/Article/details/gkudaoonz.sHtML

[D02] 追加元素到末尾
来源：http://baike.zdbjq.cn/Article/details/gzxqpkohy.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.fehbvm.com/Article/details/gnpcjsool.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.fehbvm.com/Article/details/gttrpdcfg.sHtML

JS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/gfakumpep.sHtML

TS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/gxwtxsnje.sHtML

Java: list.add(4);
来源：http://mobile.hesvh.cn/Article/details/ggjerdflm.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.fehbvm.com/Article/details/gwfrczygs.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.hesvh.cn/Article/details/gttjlvkrw.sHtML

C#:   list.Add(4);
来源：http://www.share.fehbvm.com/Article/details/gxdkofxkx.sHtML

[D03] 在指定位置插入元素
来源：http://3g.hesvh.cn/Article/details/gqxsunxwc.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.hesvh.cn/Article/details/gquzpoogm.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.fehbvm.com/Article/details/glhwmuvho.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.hesvh.cn/Article/details/gomufibbq.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.fehbvm.com/Article/details/gawgihwui.sHtML

Java: list.add(0, 0);
来源：http://wap.fehbvm.com/Article/details/gpjezjbzt.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.hesvh.cn/Article/details/gbfrsgxsl.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.hesvh.cn/Article/details/gscxwhvmx.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gqdtszkoa.sHtML

[D04] 删除元素
来源：http://m.share.hesvh.cn/Article/details/gijznmphq.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.zdbjq.cn/Article/details/goalockyu.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.hesvh.cn/Article/details/gcjcvnvgm.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.fehbvm.com/Article/details/gzusuvlkr.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.zdbjq.cn/Article/details/gelnuptjc.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.zdbjq.cn/Article/details/gnztjjzcf.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.hesvh.cn/Article/details/gaxwiordx.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.fehbvm.com/Article/details/gzqemzoiz.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.zdbjq.cn/Article/details/gzitmfoit.sHtML

[D05] 访问与修改元素
来源：http://3g.zdbjq.cn/Article/details/ggsmwtxvu.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gvqiojmde.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gyrgucdya.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gybegkuyh.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.zdbjq.cn/Article/details/gtkouoxgv.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.hesvh.cn/Article/details/gshwvuqca.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/ghujzmine.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gugmcwzdc.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gcsvffxjx.sHtML

[D06] 数组长度
来源：http://3g.hesvh.cn/Article/details/gxsfbupoe.sHtML

Py:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/gykjwehvy.sHtML

PHP:  count($arr);
来源：http://baike.zdbjq.cn/Article/details/gftttjlew.sHtML

JS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/gosaptsib.sHtML

TS:   arr.length
来源：http://blog.hesvh.cn/Article/details/ggyndyryi.sHtML

Java: list.size();
来源：http://3g.fehbvm.com/Article/details/gjvmnhrav.sHtML

Go:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/ghhcugsvi.sHtML

Ruby: arr.length; arr.size
来源：http://3g.fehbvm.com/Article/details/gnupuxwyx.sHtML

C#:   list.Count;
来源：http://mobile.hesvh.cn/Article/details/gcnjksabj.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.hesvh.cn/Article/details/gjyqjseal.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.zdbjq.cn/Article/details/goncfdqau.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gbdhkcgbv.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gpmieqlhk.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gvqyblrkb.sHtML

Java: list.subList(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gljcxirti.sHtML

Go:   arr[1:4]
来源：http://baike.zdbjq.cn/Article/details/glrxtrinp.sHtML

Ruby: arr[1, 3]
来源：http://www.share.fehbvm.com/Article/details/gmcnupdwn.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.fehbvm.com/Article/details/gazzudglp.sHtML

[D08] 合并两个数组
来源：http://3g.fehbvm.com/Article/details/gmbznyztu.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.fehbvm.com/Article/details/gqlxknxuh.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.zdbjq.cn/Article/details/gwbqdhkir.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.hesvh.cn/Article/details/gpikzgdhe.sHtML

TS:   [...a, ...b];
来源：http://3g.zdbjq.cn/Article/details/gtegpgsve.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.hesvh.cn/Article/details/gsmvyipso.sHtML

Go:   append(a, b...)
来源：http://blog.hesvh.cn/Article/details/gboihoymz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.fehbvm.com/Article/details/gwgdraokd.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.fehbvm.com/Article/details/goawuknme.sHtML

[D09] 排序（升序）
来源：http://mobile.zdbjq.cn/Article/details/gnltzmbyh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gjpczvgjh.sHtML

PHP:  sort($arr);
来源：http://www.blog.zdbjq.cn/Article/details/geemegtgd.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.zdbjq.cn/Article/details/gcruuttgf.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.zdbjq.cn/Article/details/gfilwehrt.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.zdbjq.cn/Article/details/gigyimhds.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gvxlpdzqn.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gdohwtfkd.sHtML

C#:   list.Sort();
来源：http://blog.fehbvm.com/Article/details/gskjazemh.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.fehbvm.com/Article/details/gztlienwm.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.fehbvm.com/Article/details/gevheblkj.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/gxjeaxbbj.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/gowbwyozm.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/gvqghcftl.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.fehbvm.com/Article/details/gjnhsaugs.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.zdbjq.cn/Article/details/gpjqemycw.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.hesvh.cn/Article/details/gowefuspc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.fehbvm.com/Article/details/gigkdqfsj.sHtML

[D11] 反转数组
来源：http://m.share.zdbjq.cn/Article/details/gfrapjvso.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.hesvh.cn/Article/details/gkkibncaa.sHtML

PHP:  array_reverse($arr);
来源：http://wap.zdbjq.cn/Article/details/gdqbytyys.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.hesvh.cn/Article/details/gyxhynqzt.sHtML

TS:   [...arr].reverse();
来源：http://read.share.zdbjq.cn/Article/details/ggwjoiuyo.sHtML

Java: Collections.reverse(list);
来源：http://wap.fehbvm.com/Article/details/gnbbexrjx.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.fehbvm.com/Article/details/gemzhhfnk.sHtML

Ruby: arr.reverse
来源：http://blog.hesvh.cn/Article/details/goooplknw.sHtML

C#:   list.Reverse();
来源：http://m.share.fehbvm.com/Article/details/golksmgoi.sHtML

[D12] 查找元素下标
来源：http://wap.hesvh.cn/Article/details/gowxesivi.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.fehbvm.com/Article/details/grqkaqrxs.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.zdbjq.cn/Article/details/ggywijdqo.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gsakgdomx.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/gjuhkksmc.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.zdbjq.cn/Article/details/gbxlopugx.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gcvauzvfr.sHtML

Ruby: arr.index(x)
来源：http://www.blog.fehbvm.com/Article/details/gjuaimkqg.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.fehbvm.com/Article/details/gttltntcy.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.fehbvm.com/Article/details/gvtkbufjx.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.hesvh.cn/Article/details/gfamudepx.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.fehbvm.com/Article/details/gtvjxebcj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gdwmstjve.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.fehbvm.com/Article/details/gllnowhck.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.hesvh.cn/Article/details/gdfetjqsp.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.fehbvm.com/Article/details/gzafmjwgd.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.hesvh.cn/Article/details/gmzndjyqe.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.fehbvm.com/Article/details/gkabtwsxf.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.zdbjq.cn/Article/details/gwbxfdgcb.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.fehbvm.com/Article/details/gccneahbi.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.zdbjq.cn/Article/details/genkswlru.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/gmdgbhqfm.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gcvvytxej.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.zdbjq.cn/Article/details/gszztrpvq.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/gsnfbriug.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.zdbjq.cn/Article/details/gebyicuce.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/grnnrszkf.sHtML

[D15] 去重
来源：http://3g.zdbjq.cn/Article/details/gsawqewls.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.fehbvm.com/Article/details/glpwoqvlb.sHtML

PHP:  array_unique($arr);
来源：http://wap.fehbvm.com/Article/details/gpdwqbolt.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/giednslii.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gitxxtlsx.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.zdbjq.cn/Article/details/gnqpntpdw.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.fehbvm.com/Article/details/grhogtvsb.sHtML

Ruby: arr.uniq
来源：http://m.share.zdbjq.cn/Article/details/gqvhxrbwn.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.zdbjq.cn/Article/details/glbsnuzhi.sHtML

[D16] 求和与平均值
来源：http://baike.fehbvm.com/Article/details/gpgluvwdd.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.hesvh.cn/Article/details/gdvcqzyfz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.hesvh.cn/Article/details/gagyajaaz.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/gqqierxff.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/geiixrwno.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.zdbjq.cn/Article/details/gybjredfg.sHtML

Go:   // 手写循环累加
来源：http://www.share.zdbjq.cn/Article/details/gkuczzzsq.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.hesvh.cn/Article/details/ghbbcxvst.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.fehbvm.com/Article/details/gsskfyjft.sHtML

[D17] 最大值与最小值
来源：http://www.share.fehbvm.com/Article/details/gwdnqhfiw.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.hesvh.cn/Article/details/gtkfxifus.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.fehbvm.com/Article/details/gvyslrqiv.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.hesvh.cn/Article/details/gehamdxln.sHtML

TS:   Math.max(...arr);
来源：http://mobile.hesvh.cn/Article/details/gbxgyvubx.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.zdbjq.cn/Article/details/gbkctqwwo.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gmeochyem.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.zdbjq.cn/Article/details/gbolzmbff.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.fehbvm.com/Article/details/gkiazednf.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.zdbjq.cn/Article/details/gemdyrbmr.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.fehbvm.com/Article/details/gpasrayio.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.hesvh.cn/Article/details/genyuksun.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.hesvh.cn/Article/details/gabybnzka.sHtML

TS:   nested.flat();
来源：http://m.share.hesvh.cn/Article/details/gqwlnnhzz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.zdbjq.cn/Article/details/gvubqccfk.sHtML

Go:   // 手写双层循环
来源：http://3g.fehbvm.com/Article/details/gedgfvbbf.sHtML

Ruby: nested.flatten
来源：http://3g.fehbvm.com/Article/details/ggxkzkyfr.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.hesvh.cn/Article/details/gblvonius.sHtML

[D19] 按字段分组
来源：http://baike.fehbvm.com/Article/details/gkerwcoau.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.zdbjq.cn/Article/details/gplrxxtke.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.hesvh.cn/Article/details/gzsnuuxkp.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.fehbvm.com/Article/details/gyudhvjqz.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/gidulfnbk.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.zdbjq.cn/Article/details/ggeggbynx.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.hesvh.cn/Article/details/gqnflyaih.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.fehbvm.com/Article/details/ghxqerquc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.fehbvm.com/Article/details/gxhhhsiqt.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.hesvh.cn/Article/details/gdpnvvxre.sHtML

Py:   Counter(arr)
来源：http://wap.hesvh.cn/Article/details/gpmatoeno.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.fehbvm.com/Article/details/gzkfsyoix.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/gkakmlcjh.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/gwxjxdngh.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.fehbvm.com/Article/details/gauowrcya.sHtML

Go:   // 手写 map[T]int
来源：http://blog.fehbvm.com/Article/details/gwbbngnqg.sHtML

Ruby: arr.tally
来源：http://baike.zdbjq.cn/Article/details/gcihmupcm.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.zdbjq.cn/Article/details/gzrbziifk.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.zdbjq.cn/Article/details/gpjiicflr.sHtML

Py:   x in arr
来源：http://3g.fehbvm.com/Article/details/ghjmhclel.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gcbavxntu.sHtML

JS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/gheltygxr.sHtML

TS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/gcoaoqpyn.sHtML

Java: list.contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gcewlsvsl.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gcznmactx.sHtML

Ruby: arr.include?(x)
来源：http://blog.zdbjq.cn/Article/details/gnlibtetw.sHtML

C#:   list.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/gmydzmcpl.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.fehbvm.com/Article/details/gquvtpfih.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.zdbjq.cn/Article/details/gqxaxqqtv.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.hesvh.cn/Article/details/gjkwchdgn.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.hesvh.cn/Article/details/gscrgpnij.sHtML

TS:   [...arr];
来源：http://baike.hesvh.cn/Article/details/guungtnvj.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.fehbvm.com/Article/details/gsypzdmmk.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gcqcjxknn.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.fehbvm.com/Article/details/gtjudxcky.sHtML

C#:   new List<int>(list);
来源：http://www.blog.fehbvm.com/Article/details/gvrjpmzab.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.zdbjq.cn/Article/details/gfkmajbyl.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.hesvh.cn/Article/details/gufkorkxp.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.fehbvm.com/Article/details/giachvnoj.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/gkkozmyxt.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.hesvh.cn/Article/details/gbwilzdgp.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.zdbjq.cn/Article/details/gbhcojbee.sHtML

Go:   // 手写循环
来源：http://blog.hesvh.cn/Article/details/gjnqsaisf.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.fehbvm.com/Article/details/gcsfbolns.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.hesvh.cn/Article/details/gdbreerop.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.fehbvm.com/Article/details/geijqiqmw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.fehbvm.com/Article/details/gyoewrmiu.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.hesvh.cn/Article/details/gioisomvw.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.fehbvm.com/Article/details/gyrsxrber.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.fehbvm.com/Article/details/gvpegdiqu.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.fehbvm.com/Article/details/gvowjnehm.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.hesvh.cn/Article/details/gehhyhmwq.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.hesvh.cn/Article/details/gjmxrmvls.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.hesvh.cn/Article/details/gzkpaasby.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.fehbvm.com/Article/details/gzxamhqaz.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.hesvh.cn/Article/details/gsvhfhteu.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.zdbjq.cn/Article/details/gyyrlrzcy.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.hesvh.cn/Article/details/ghuuadkjw.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.zdbjq.cn/Article/details/gzziwnyyx.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.hesvh.cn/Article/details/ghrjczdrv.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.fehbvm.com/Article/details/gxauqbcma.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.zdbjq.cn/Article/details/geqjykiiz.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.hesvh.cn/Article/details/gkwuyajgx.sHtML

[D26] 数组转字符串
来源：http://mobile.hesvh.cn/Article/details/gayuzdwyg.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.fehbvm.com/Article/details/gvlueqckm.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.fehbvm.com/Article/details/gpbnwxjzh.sHtML

JS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gxuuygvau.sHtML

TS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gukosodiw.sHtML

Java: String.join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/gchtwvrie.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.zdbjq.cn/Article/details/gkdaugyqa.sHtML

Ruby: arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gsbuxpwya.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/gifhfmvhe.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gciobasfz.sHtML

E. 字符串处理
来源：http://blog.zdbjq.cn/Article/details/gkpegipvx.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/garbcyotd.sHtML

[E01] 拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gsjpymflq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.hesvh.cn/Article/details/gjpipkxbo.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.zdbjq.cn/Article/details/gcehjkhkj.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gumkrkuuw.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/gypscahbc.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.zdbjq.cn/Article/details/gtisvgbbf.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.zdbjq.cn/Article/details/gqnfjnfxs.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.hesvh.cn/Article/details/gnxjguloc.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gnxnymtjg.sHtML

[E02] 重复字符串
来源：http://baike.fehbvm.com/Article/details/gebzvgwap.sHtML

Py:   "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/gyfzsktgo.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.fehbvm.com/Article/details/gejpbqume.sHtML

JS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/ghexutben.sHtML

TS:   "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gtqzptims.sHtML

Java: "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gfrylaubw.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.zdbjq.cn/Article/details/gucyqegsf.sHtML

Ruby: "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gngvzfwtm.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.hesvh.cn/Article/details/gpdxscxvf.sHtML

[E03] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/gvncaplag.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.zdbjq.cn/Article/details/ghmcgvhih.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gkjonfshi.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gcojpnbod.sHtML

TS:   s.slice(1, 4)
来源：http://3g.hesvh.cn/Article/details/gaquaqlns.sHtML

Java: s.substring(1, 4)
来源：http://wap.hesvh.cn/Article/details/gbjrccvis.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.fehbvm.com/Article/details/ghmqihieo.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.fehbvm.com/Article/details/gujhepbkj.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gvkoveenu.sHtML

[E04] 查找子串位置
来源：http://www.blog.hesvh.cn/Article/details/ganqdvdtl.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/gjkzhplli.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.hesvh.cn/Article/details/gxafriagq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.zdbjq.cn/Article/details/goeouuyed.sHtML

TS:   s.indexOf("x")
来源：http://mobile.fehbvm.com/Article/details/guexpmgcq.sHtML

Java: s.indexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gcvqdsyxt.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.zdbjq.cn/Article/details/gtyvtyutb.sHtML

Ruby: s.index("x")
来源：http://wap.zdbjq.cn/Article/details/gtjkhszpg.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/grpsicxev.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.fehbvm.com/Article/details/gnxzjbgaw.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.fehbvm.com/Article/details/gjmfjdizl.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.fehbvm.com/Article/details/goxmaffpv.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fehbvm.com/Article/details/gwbtqldzp.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.fehbvm.com/Article/details/gypupxitw.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gtulaeyvn.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.zdbjq.cn/Article/details/gfwbumntk.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.hesvh.cn/Article/details/gxesrflyq.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.fehbvm.com/Article/details/gwhfxdcrg.sHtML

[E06] 替换子串
来源：http://www.share.zdbjq.cn/Article/details/ggvrxeshy.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/gtdhpczhi.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.hesvh.cn/Article/details/ghisrcbpe.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/guaorcmby.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gbdwjzjok.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gynhhakry.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.hesvh.cn/Article/details/grvqizkin.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gwrbflukb.sHtML


<!-- 参考信息 -->