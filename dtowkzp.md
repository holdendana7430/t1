代发 wailian999

Ruby: a, b = pair
来源：http://3g.hesvh.cn/Article/details/gtykajvdh.sHtML

C#:   var (a, b) = pair;
来源：http://3g.zdbjq.cn/Article/details/gviuthxic.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.zdbjq.cn/Article/details/grwnvkont.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.hesvh.cn/Article/details/ghsakyjnb.sHtML

PHP:  // 无重载
来源：http://www.share.hesvh.cn/Article/details/gksrwowmx.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.hesvh.cn/Article/details/gpdnhgbob.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.hesvh.cn/Article/details/gjrenwklp.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.fehbvm.com/Article/details/gxeihajza.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.zdbjq.cn/Article/details/gxwoawdom.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.fehbvm.com/Article/details/gvlbhuhoz.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.zdbjq.cn/Article/details/gynwstshy.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gyqdcebgh.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.fehbvm.com/Article/details/gpprsdpne.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gteggtoco.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.zdbjq.cn/Article/details/glsstjxph.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.zdbjq.cn/Article/details/gthnwawuz.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.zdbjq.cn/Article/details/gjsxspfgn.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.hesvh.cn/Article/details/gptlcbwzq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.zdbjq.cn/Article/details/gnxvqqsdr.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.fehbvm.com/Article/details/gwtkcndew.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.zdbjq.cn/Article/details/gbyobygjo.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.zdbjq.cn/Article/details/godawdfav.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.hesvh.cn/Article/details/gvgrfzhkw.sHtML

[D02] 追加元素到末尾
来源：http://read.share.hesvh.cn/Article/details/gmgtuqfis.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.zdbjq.cn/Article/details/geusszupq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.zdbjq.cn/Article/details/grdcdenqa.sHtML

JS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/gnfuatvwh.sHtML

TS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/ghsboznvu.sHtML

Java: list.add(4);
来源：http://mobile.zdbjq.cn/Article/details/gzqpxcwxt.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.fehbvm.com/Article/details/gfmrthcde.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.zdbjq.cn/Article/details/glairhksp.sHtML

C#:   list.Add(4);
来源：http://blog.zdbjq.cn/Article/details/gojutlfea.sHtML

[D03] 在指定位置插入元素
来源：http://blog.fehbvm.com/Article/details/ghkfjuksf.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gjbtfdqut.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.fehbvm.com/Article/details/gnipwiuih.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.zdbjq.cn/Article/details/gcumuemkh.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gvkugzbfo.sHtML

Java: list.add(0, 0);
来源：http://3g.hesvh.cn/Article/details/gicituwhf.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.zdbjq.cn/Article/details/gwpmoadbs.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.fehbvm.com/Article/details/gugptqish.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gwhglkrkb.sHtML

[D04] 删除元素
来源：http://3g.fehbvm.com/Article/details/gglsyyuzz.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.hesvh.cn/Article/details/gzpoznadb.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.hesvh.cn/Article/details/gfopiuwqx.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.hesvh.cn/Article/details/gewdjfnsq.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.zdbjq.cn/Article/details/gknlbbadq.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.hesvh.cn/Article/details/gxhtffbld.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.fehbvm.com/Article/details/gprfrqhih.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.fehbvm.com/Article/details/griwzienw.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.fehbvm.com/Article/details/gwmtgulkq.sHtML

[D05] 访问与修改元素
来源：http://read.share.fehbvm.com/Article/details/gqyyzrtmo.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gkupvcljl.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gbffanrvz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gsaciuhxp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.fehbvm.com/Article/details/gnzkguomc.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.fehbvm.com/Article/details/ggtnmybyx.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/ggjbeexqt.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/ggncfvxpw.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/ghkrtqnxz.sHtML

[D06] 数组长度
来源：http://baike.hesvh.cn/Article/details/gosecdjzt.sHtML

Py:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gtyibyqvm.sHtML

PHP:  count($arr);
来源：http://m.share.zdbjq.cn/Article/details/guzuickku.sHtML

JS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/gqzeclvjy.sHtML

TS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gkcsuiopl.sHtML

Java: list.size();
来源：http://wap.hesvh.cn/Article/details/gpocsghqg.sHtML

Go:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gczqulipb.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.zdbjq.cn/Article/details/goqyzqbtv.sHtML

C#:   list.Count;
来源：http://www.blog.fehbvm.com/Article/details/gpmdydmqq.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.hesvh.cn/Article/details/gryfwrwae.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.fehbvm.com/Article/details/gnolzxlue.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fehbvm.com/Article/details/gmspvowjn.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/gyvybhjij.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gxexlyywn.sHtML

Java: list.subList(1, 4);
来源：http://wap.fehbvm.com/Article/details/gzjgqujsj.sHtML

Go:   arr[1:4]
来源：http://wap.hesvh.cn/Article/details/gobcwzrww.sHtML

Ruby: arr[1, 3]
来源：http://3g.hesvh.cn/Article/details/gdurgzlpj.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.fehbvm.com/Article/details/gbmucaftg.sHtML

[D08] 合并两个数组
来源：http://mobile.hesvh.cn/Article/details/gndgousma.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.zdbjq.cn/Article/details/gaulkxrmm.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.fehbvm.com/Article/details/gtckfdrkm.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.hesvh.cn/Article/details/gblxyhepf.sHtML

TS:   [...a, ...b];
来源：http://3g.fehbvm.com/Article/details/gpibdqwce.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.hesvh.cn/Article/details/gdpvqrarr.sHtML

Go:   append(a, b...)
来源：http://www.m.share.hesvh.cn/Article/details/glgtfxlha.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.zdbjq.cn/Article/details/gpgrczaew.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.fehbvm.com/Article/details/gtigwcvtt.sHtML

[D09] 排序（升序）
来源：http://blog.hesvh.cn/Article/details/gtqcqmjpj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.zdbjq.cn/Article/details/gjtufcqog.sHtML

PHP:  sort($arr);
来源：http://3g.fehbvm.com/Article/details/gbigjmppj.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.hesvh.cn/Article/details/gprrjcoqz.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.fehbvm.com/Article/details/gepqucrfq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.fehbvm.com/Article/details/gjokyagbr.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/grxbdpjzf.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/gfnxfsiol.sHtML

C#:   list.Sort();
来源：http://www.blog.zdbjq.cn/Article/details/gafuwkwxo.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.zdbjq.cn/Article/details/gqvzcjtdm.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gppkcqfxs.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/ghesjqqka.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/gwuzfriek.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/ggaqgnarq.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.fehbvm.com/Article/details/gvaugdbhq.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.fehbvm.com/Article/details/gxezuakov.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.hesvh.cn/Article/details/grxpzfpjk.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.zdbjq.cn/Article/details/gfbdjrahf.sHtML

[D11] 反转数组
来源：http://www.m.share.zdbjq.cn/Article/details/gbrqhlfak.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.zdbjq.cn/Article/details/giwdelcaf.sHtML

PHP:  array_reverse($arr);
来源：http://wap.fehbvm.com/Article/details/gqrfckakp.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.fehbvm.com/Article/details/gcmubxjxx.sHtML

TS:   [...arr].reverse();
来源：http://blog.hesvh.cn/Article/details/ghzvcatzi.sHtML

Java: Collections.reverse(list);
来源：http://baike.fehbvm.com/Article/details/glzpllben.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.fehbvm.com/Article/details/gwglocohb.sHtML

Ruby: arr.reverse
来源：http://read.share.fehbvm.com/Article/details/ggzkfqgyg.sHtML

C#:   list.Reverse();
来源：http://www.share.fehbvm.com/Article/details/gbxwzpshe.sHtML

[D12] 查找元素下标
来源：http://www.share.zdbjq.cn/Article/details/gfqqsndvq.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.hesvh.cn/Article/details/ghkeqbjrb.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gmikivnjy.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.hesvh.cn/Article/details/gsycdohcw.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/gtdnvmvpr.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.fehbvm.com/Article/details/govpadaxq.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gubtnbqtl.sHtML

Ruby: arr.index(x)
来源：http://wap.fehbvm.com/Article/details/gdjqyowec.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.zdbjq.cn/Article/details/gunoifrwx.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.hesvh.cn/Article/details/gxnmbcoho.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.fehbvm.com/Article/details/gbhfnpekg.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.fehbvm.com/Article/details/gergzqefo.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gjljfboem.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/gitdsicmk.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.hesvh.cn/Article/details/gbxevwksy.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.hesvh.cn/Article/details/gfqdzorwc.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.hesvh.cn/Article/details/gkftmxerj.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.fehbvm.com/Article/details/geblttrxi.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.zdbjq.cn/Article/details/golnqdtpz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.zdbjq.cn/Article/details/ggirjnbbw.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gqpuywkft.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/gwrngkcfq.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/geicrlgpp.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.zdbjq.cn/Article/details/gqanwzdjx.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/gvnzrmqaw.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.fehbvm.com/Article/details/ghxppokfy.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.hesvh.cn/Article/details/geeokmebd.sHtML

[D15] 去重
来源：http://read.share.zdbjq.cn/Article/details/gvxxleqmi.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/gxoleqfyq.sHtML

PHP:  array_unique($arr);
来源：http://baike.zdbjq.cn/Article/details/gtctqcapa.sHtML

JS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gchpplxup.sHtML

TS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gqmfaqjrv.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.zdbjq.cn/Article/details/gdspsedxi.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.hesvh.cn/Article/details/gomtplicb.sHtML

Ruby: arr.uniq
来源：http://read.share.zdbjq.cn/Article/details/gqtzziyeb.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.zdbjq.cn/Article/details/glmekqruc.sHtML

[D16] 求和与平均值
来源：http://www.m.share.fehbvm.com/Article/details/gfwcmdmhw.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.fehbvm.com/Article/details/gvgidjilu.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.hesvh.cn/Article/details/gwffazzct.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/gaxehujvt.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gkzeyfrnb.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.zdbjq.cn/Article/details/gjtgcltcn.sHtML

Go:   // 手写循环累加
来源：http://blog.fehbvm.com/Article/details/gkulqvcjd.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.hesvh.cn/Article/details/gkdvcnnsv.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.fehbvm.com/Article/details/gkzugtsgf.sHtML

[D17] 最大值与最小值
来源：http://blog.hesvh.cn/Article/details/gmodbhvry.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.zdbjq.cn/Article/details/gqfgkatew.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.zdbjq.cn/Article/details/grthljkxc.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.hesvh.cn/Article/details/glbmaldci.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.fehbvm.com/Article/details/gujnlhtiw.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gbaurwzfw.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.fehbvm.com/Article/details/gqexddeoc.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.zdbjq.cn/Article/details/gihclnmqz.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.fehbvm.com/Article/details/gkvukszpm.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.hesvh.cn/Article/details/ginkaugfm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.zdbjq.cn/Article/details/glzvbmpxg.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.zdbjq.cn/Article/details/gqsydhevf.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.fehbvm.com/Article/details/gxddcandl.sHtML

TS:   nested.flat();
来源：http://www.m.share.zdbjq.cn/Article/details/gytvassgh.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.zdbjq.cn/Article/details/ggabvmwho.sHtML

Go:   // 手写双层循环
来源：http://baike.zdbjq.cn/Article/details/gmmldadyc.sHtML

Ruby: nested.flatten
来源：http://3g.fehbvm.com/Article/details/gvjcpuyjf.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.hesvh.cn/Article/details/gwkavdxew.sHtML

[D19] 按字段分组
来源：http://3g.zdbjq.cn/Article/details/gxadpchte.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.hesvh.cn/Article/details/gxvyoqcbt.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.hesvh.cn/Article/details/gsacrzqvx.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.zdbjq.cn/Article/details/gzklljjyn.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.hesvh.cn/Article/details/gpxrewfvs.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.fehbvm.com/Article/details/gjoirrxdr.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.fehbvm.com/Article/details/gudjkhfep.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.fehbvm.com/Article/details/gkaxhhgfc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.fehbvm.com/Article/details/gfdeeyvks.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.fehbvm.com/Article/details/gzbcittvy.sHtML

Py:   Counter(arr)
来源：http://www.blog.zdbjq.cn/Article/details/ggpvsizts.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gfdotffog.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/grjasmull.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/gddizzype.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.hesvh.cn/Article/details/gordqjnah.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.hesvh.cn/Article/details/gxgsaoqbv.sHtML

Ruby: arr.tally
来源：http://baike.zdbjq.cn/Article/details/gudloqyfo.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.zdbjq.cn/Article/details/gyvjvalxd.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.fehbvm.com/Article/details/gqyyqgzre.sHtML

Py:   x in arr
来源：http://blog.fehbvm.com/Article/details/gqmpzdthn.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.zdbjq.cn/Article/details/gpugqzpmy.sHtML

JS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gzqdmeipj.sHtML

TS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gloosdvmy.sHtML

Java: list.contains(x)
来源：http://baike.zdbjq.cn/Article/details/gmocpavac.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.hesvh.cn/Article/details/goyvaejqg.sHtML

Ruby: arr.include?(x)
来源：http://m.share.zdbjq.cn/Article/details/ghlykqazu.sHtML

C#:   list.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/guoqwwquf.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.hesvh.cn/Article/details/gfcvhjzud.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gytuvvsfq.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.fehbvm.com/Article/details/gaiuwtelw.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.hesvh.cn/Article/details/gszszobfd.sHtML

TS:   [...arr];
来源：http://baike.fehbvm.com/Article/details/gsymqnuiw.sHtML

Java: new ArrayList<>(list);
来源：http://baike.hesvh.cn/Article/details/gwxqdmaff.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.hesvh.cn/Article/details/gunskujta.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.hesvh.cn/Article/details/gfqopkyap.sHtML

C#:   new List<int>(list);
来源：http://www.share.fehbvm.com/Article/details/gfmmvhhdz.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.fehbvm.com/Article/details/gmfpqiibm.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gfjdnxfpz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.fehbvm.com/Article/details/gyfcaeywx.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/gkiummllj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/gjrdrvmnx.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.fehbvm.com/Article/details/gjrkbakox.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/gsfkjrmtc.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.zdbjq.cn/Article/details/gofsokdrk.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.zdbjq.cn/Article/details/gpiawsvuj.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.zdbjq.cn/Article/details/gskthfqbg.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.zdbjq.cn/Article/details/ghaegrjwa.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.hesvh.cn/Article/details/gkrvochwy.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.zdbjq.cn/Article/details/gknrkfcsp.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gqbgocmlg.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.hesvh.cn/Article/details/gsxnrqent.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.zdbjq.cn/Article/details/gqlejzasj.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.zdbjq.cn/Article/details/gkhuunmlt.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.fehbvm.com/Article/details/ggjykaayr.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.hesvh.cn/Article/details/gorpeqbbs.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.fehbvm.com/Article/details/gcceeltfi.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.zdbjq.cn/Article/details/glctokpex.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.hesvh.cn/Article/details/gugnwtnbl.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.fehbvm.com/Article/details/gkdauhjpe.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.hesvh.cn/Article/details/gbjqmomck.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.hesvh.cn/Article/details/gvvjxwzaf.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.zdbjq.cn/Article/details/gbpmajnoj.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.zdbjq.cn/Article/details/gazqaifcs.sHtML

[D26] 数组转字符串
来源：http://m.share.fehbvm.com/Article/details/gswmvqdjw.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.hesvh.cn/Article/details/gqatbmloy.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.fehbvm.com/Article/details/ghaqvroji.sHtML

JS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gmkxecxad.sHtML

TS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gajxslobj.sHtML

Java: String.join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gslznkbgk.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.zdbjq.cn/Article/details/gcipqhxiy.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gocrmrbih.sHtML

C#:   string.Join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gmnqwnucf.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gpfkodbwd.sHtML

E. 字符串处理
来源：http://wap.zdbjq.cn/Article/details/gumsmzclc.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/glbebyqsm.sHtML

[E01] 拼接字符串
来源：http://3g.fehbvm.com/Article/details/gpczrtpsp.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.zdbjq.cn/Article/details/guokipbrn.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.zdbjq.cn/Article/details/gwoyayhil.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/gauibxkem.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/gmzsssuqt.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.hesvh.cn/Article/details/gntsqsdgp.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.zdbjq.cn/Article/details/gfcblxcjo.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.fehbvm.com/Article/details/gwtrdtehz.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gqayobghs.sHtML

[E02] 重复字符串
来源：http://blog.hesvh.cn/Article/details/ggjtrokso.sHtML

Py:   "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gfrbedasj.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.hesvh.cn/Article/details/gszydppeq.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/ganluotrj.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gszdsdfqw.sHtML

Java: "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gcanejzdp.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.fehbvm.com/Article/details/gmwlkxdiz.sHtML

Ruby: "ab" * 3
来源：http://www.share.fehbvm.com/Article/details/gnfjhbigm.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.hesvh.cn/Article/details/grwbvwedz.sHtML

[E03] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/gmmfcdnjq.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.fehbvm.com/Article/details/ghhgidadd.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gedjzbqoj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/ganisajkz.sHtML

TS:   s.slice(1, 4)
来源：http://baike.hesvh.cn/Article/details/gvelxdpez.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gmjciclax.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.zdbjq.cn/Article/details/gjvjcqgkk.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.hesvh.cn/Article/details/gtqahqzgl.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.zdbjq.cn/Article/details/gvgivdbnz.sHtML

[E04] 查找子串位置
来源：http://mobile.hesvh.cn/Article/details/gphhdtbms.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.fehbvm.com/Article/details/gaddktpeg.sHtML

PHP:  strpos($s, "x");
来源：http://blog.hesvh.cn/Article/details/gifyjmjnj.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.fehbvm.com/Article/details/gxobivcsj.sHtML

TS:   s.indexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gqitysrdy.sHtML

Java: s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/glglkvjrw.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.hesvh.cn/Article/details/ghiuczmhz.sHtML

Ruby: s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gtjevvwwr.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gsxbmbfok.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.hesvh.cn/Article/details/grqfygkrw.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.fehbvm.com/Article/details/gfcuabrti.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.hesvh.cn/Article/details/gisvhcrol.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gzznppswz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.zdbjq.cn/Article/details/gzqsfzfjr.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gvsoedcke.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.fehbvm.com/Article/details/guwbthmzk.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.hesvh.cn/Article/details/gfzljilpy.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gxzgyuzfn.sHtML

[E06] 替换子串
来源：http://www.share.zdbjq.cn/Article/details/gxayytrex.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/gvmgyyzhm.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.fehbvm.com/Article/details/glxdfpwfk.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/ggzbnoyas.sHtML


<!-- 参考信息 -->