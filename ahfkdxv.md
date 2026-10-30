代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.hesvh.cn/Article/details/glrmpbuon.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.fehbvm.com/Article/details/gvcpyfptg.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.hesvh.cn/Article/details/gglbavnat.sHtML

Ruby: # 无泛型
来源：http://3g.zdbjq.cn/Article/details/grumkqgdw.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.zdbjq.cn/Article/details/gbwumojpp.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.zdbjq.cn/Article/details/gaiyawkmb.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.zdbjq.cn/Article/details/glnwydbgq.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fehbvm.com/Article/details/glszucwkk.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.zdbjq.cn/Article/details/gcoaslubr.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.zdbjq.cn/Article/details/gkhquxjem.sHtML

Java: // 无解构
来源：http://www.blog.fehbvm.com/Article/details/gkdfptowa.sHtML

Go:   // 无解构
来源：http://read.share.fehbvm.com/Article/details/gbtbdxriz.sHtML

Ruby: a, b = pair
来源：http://blog.hesvh.cn/Article/details/gtdcxsuwp.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.zdbjq.cn/Article/details/grqdiwomj.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.hesvh.cn/Article/details/gyykkhorq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.hesvh.cn/Article/details/gtdoawuqd.sHtML

PHP:  // 无重载
来源：http://www.m.share.fehbvm.com/Article/details/gcxjtlsjg.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.zdbjq.cn/Article/details/gjodiqcnn.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.fehbvm.com/Article/details/gxvqxzsoe.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.fehbvm.com/Article/details/gxeeqkqck.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.hesvh.cn/Article/details/gpgwngqyw.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.hesvh.cn/Article/details/gcyiarpoz.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.hesvh.cn/Article/details/gnvwgwwhc.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gtjbwrruh.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.fehbvm.com/Article/details/gtmxmffto.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gmzvuowah.sHtML

[D01] 创建数组 / 列表
来源：http://blog.hesvh.cn/Article/details/grfsaizyk.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.zdbjq.cn/Article/details/gohcemmjx.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.zdbjq.cn/Article/details/geyfbyvpg.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.hesvh.cn/Article/details/grvhlsyru.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.hesvh.cn/Article/details/gahnhxzeh.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.fehbvm.com/Article/details/gzdmiivze.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.zdbjq.cn/Article/details/gwzetirex.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.fehbvm.com/Article/details/gvtxpfjoj.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.fehbvm.com/Article/details/ggjnfpqpe.sHtML

[D02] 追加元素到末尾
来源：http://mobile.hesvh.cn/Article/details/gdgrldmmt.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.zdbjq.cn/Article/details/giosddjbr.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.zdbjq.cn/Article/details/gsgjbdfad.sHtML

JS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/gtsachklq.sHtML

TS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/gacgidmjn.sHtML

Java: list.add(4);
来源：http://www.share.fehbvm.com/Article/details/gsjjakjia.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.zdbjq.cn/Article/details/gonzjixsh.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.zdbjq.cn/Article/details/gtndpdciu.sHtML

C#:   list.Add(4);
来源：http://www.m.share.fehbvm.com/Article/details/gqsckgzwh.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.fehbvm.com/Article/details/grmeymuse.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.zdbjq.cn/Article/details/guwgiwpyh.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.zdbjq.cn/Article/details/gfyfmxnox.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.hesvh.cn/Article/details/gpekvxbob.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.fehbvm.com/Article/details/gwcipvycg.sHtML

Java: list.add(0, 0);
来源：http://wap.zdbjq.cn/Article/details/gyopkugbw.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.fehbvm.com/Article/details/gsdutxiot.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.zdbjq.cn/Article/details/gkefwjxpx.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.zdbjq.cn/Article/details/gsmpxtyzd.sHtML

[D04] 删除元素
来源：http://www.blog.hesvh.cn/Article/details/gcmwckdss.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.hesvh.cn/Article/details/ggxpilias.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.zdbjq.cn/Article/details/gfctqizkb.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.zdbjq.cn/Article/details/gtatbvrzy.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.fehbvm.com/Article/details/giyvfqhdf.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.hesvh.cn/Article/details/glutyjjix.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.hesvh.cn/Article/details/gdysnrfhl.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.fehbvm.com/Article/details/gjfkqgosq.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.hesvh.cn/Article/details/grsnjeyot.sHtML

[D05] 访问与修改元素
来源：http://read.share.zdbjq.cn/Article/details/gdyniiuox.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gsajinbgz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gkebfoaaq.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gdifowikh.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.fehbvm.com/Article/details/gkoeoyfia.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.hesvh.cn/Article/details/gyygxszuy.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gcttgadsr.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gvrdbckqp.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.hesvh.cn/Article/details/grzdxntwm.sHtML

[D06] 数组长度
来源：http://read.share.fehbvm.com/Article/details/gfaiflzwd.sHtML

Py:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/gurnjfciy.sHtML

PHP:  count($arr);
来源：http://www.share.zdbjq.cn/Article/details/gpxkedyfo.sHtML

JS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/gphueayoh.sHtML

TS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gkypakpwh.sHtML

Java: list.size();
来源：http://baike.fehbvm.com/Article/details/gqndvtqqq.sHtML

Go:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/gvlxkqhnc.sHtML

Ruby: arr.length; arr.size
来源：http://3g.zdbjq.cn/Article/details/gvpilowry.sHtML

C#:   list.Count;
来源：http://www.blog.zdbjq.cn/Article/details/gsnmlofrd.sHtML

[D07] 切片 / 取子数组
来源：http://wap.hesvh.cn/Article/details/gcacbkezy.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.zdbjq.cn/Article/details/glwblgkyh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fehbvm.com/Article/details/ghcvxijin.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/ggieppmdn.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/gebekrgpl.sHtML

Java: list.subList(1, 4);
来源：http://3g.hesvh.cn/Article/details/gvhviyksd.sHtML

Go:   arr[1:4]
来源：http://blog.hesvh.cn/Article/details/ggwlgrxit.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.fehbvm.com/Article/details/gimfukvfy.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.hesvh.cn/Article/details/gmoubrosx.sHtML

[D08] 合并两个数组
来源：http://www.share.fehbvm.com/Article/details/ghcgyfjwz.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.zdbjq.cn/Article/details/gqrvxdcxj.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.hesvh.cn/Article/details/gkupgyrvx.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.zdbjq.cn/Article/details/ghpdiqcuf.sHtML

TS:   [...a, ...b];
来源：http://mobile.zdbjq.cn/Article/details/grvbfauuu.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gfparlvdw.sHtML

Go:   append(a, b...)
来源：http://www.m.share.zdbjq.cn/Article/details/gbbqcqycl.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.zdbjq.cn/Article/details/gqbnugyuz.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.fehbvm.com/Article/details/gnoaoyufv.sHtML

[D09] 排序（升序）
来源：http://baike.hesvh.cn/Article/details/gyrlhgnmq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.hesvh.cn/Article/details/gjanvizvt.sHtML

PHP:  sort($arr);
来源：http://mobile.zdbjq.cn/Article/details/gkcocclol.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.fehbvm.com/Article/details/gzvvduura.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.zdbjq.cn/Article/details/gtlbivuzm.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.zdbjq.cn/Article/details/gfdfspssb.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gikoiotmy.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/guftdasqz.sHtML

C#:   list.Sort();
来源：http://baike.fehbvm.com/Article/details/gflirqycf.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.zdbjq.cn/Article/details/gqwoogokm.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gzcgemumm.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.hesvh.cn/Article/details/gwkuehbai.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/gpwhvxfsq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/ggodbgver.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.hesvh.cn/Article/details/gdmnfhowi.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.fehbvm.com/Article/details/gmkgnvqvb.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.hesvh.cn/Article/details/gyvbylubk.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.fehbvm.com/Article/details/grqnmpzsn.sHtML

[D11] 反转数组
来源：http://m.share.fehbvm.com/Article/details/gvuoswdef.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.fehbvm.com/Article/details/gsdyxbvii.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.zdbjq.cn/Article/details/gijpquopk.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.fehbvm.com/Article/details/gecptkvsc.sHtML

TS:   [...arr].reverse();
来源：http://mobile.hesvh.cn/Article/details/gbriyyoqy.sHtML

Java: Collections.reverse(list);
来源：http://www.share.fehbvm.com/Article/details/gmjzhfnqx.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.fehbvm.com/Article/details/guysfvtio.sHtML

Ruby: arr.reverse
来源：http://mobile.fehbvm.com/Article/details/gnvctxima.sHtML

C#:   list.Reverse();
来源：http://www.m.share.hesvh.cn/Article/details/gtnukgews.sHtML

[D12] 查找元素下标
来源：http://mobile.fehbvm.com/Article/details/gouejokgp.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.hesvh.cn/Article/details/gveootlpo.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.hesvh.cn/Article/details/gowfpcrnb.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/gqttptrxm.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/gesfsiyeo.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.hesvh.cn/Article/details/ghbprooer.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gjgdtkcft.sHtML

Ruby: arr.index(x)
来源：http://blog.zdbjq.cn/Article/details/gyjffadwo.sHtML

C#:   list.IndexOf(x);
来源：http://baike.zdbjq.cn/Article/details/gmcixplud.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.zdbjq.cn/Article/details/gkhrhfwll.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.hesvh.cn/Article/details/gseixmcyx.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.hesvh.cn/Article/details/gfitpzbhb.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/gwfpknqpr.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gktnufxqx.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gqtlouvow.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.zdbjq.cn/Article/details/gggssfhuz.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.zdbjq.cn/Article/details/gvldhbgwa.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.hesvh.cn/Article/details/gwnitwwhy.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.hesvh.cn/Article/details/gtywaffzm.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/grseatots.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.zdbjq.cn/Article/details/gtagjemgo.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/gmjtunwlm.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/gqkhebxvu.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.fehbvm.com/Article/details/gylfqeeji.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/ggjgjkmwt.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gjwpkqjvi.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.hesvh.cn/Article/details/ghktdeaxt.sHtML

[D15] 去重
来源：http://mobile.fehbvm.com/Article/details/gfhglsfcm.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.zdbjq.cn/Article/details/gelrebdrd.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gwkvustqj.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/ghhbvyjqm.sHtML

TS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gwsxwegar.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.zdbjq.cn/Article/details/goncbgocz.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.zdbjq.cn/Article/details/gvxpyqqve.sHtML

Ruby: arr.uniq
来源：http://www.blog.hesvh.cn/Article/details/gvpynvpxh.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.zdbjq.cn/Article/details/gktgtwlqi.sHtML

[D16] 求和与平均值
来源：http://www.share.zdbjq.cn/Article/details/ggdofcxld.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.zdbjq.cn/Article/details/gwnooobap.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.zdbjq.cn/Article/details/gdfgpadyg.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/gyprmtrhg.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/gsyobhhgc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.zdbjq.cn/Article/details/gicufnbcb.sHtML

Go:   // 手写循环累加
来源：http://m.share.hesvh.cn/Article/details/gkkvsituv.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.hesvh.cn/Article/details/gxscsatmu.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.fehbvm.com/Article/details/gedhihqdf.sHtML

[D17] 最大值与最小值
来源：http://read.share.fehbvm.com/Article/details/gapcsxagl.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.fehbvm.com/Article/details/gbqenzfwu.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.zdbjq.cn/Article/details/gakhgwqrv.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.hesvh.cn/Article/details/gagmkoabz.sHtML

TS:   Math.max(...arr);
来源：http://m.share.fehbvm.com/Article/details/gjqxwjkmt.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gqkuqbqnc.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gudyhnsus.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.hesvh.cn/Article/details/gsrxiygfg.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.zdbjq.cn/Article/details/gmvwzjlch.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.fehbvm.com/Article/details/glceypawr.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.hesvh.cn/Article/details/guddivixn.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.hesvh.cn/Article/details/gqvqohneo.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.zdbjq.cn/Article/details/grusvzcuv.sHtML

TS:   nested.flat();
来源：http://www.m.share.hesvh.cn/Article/details/gtqmyjefs.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.fehbvm.com/Article/details/gzymqaitx.sHtML

Go:   // 手写双层循环
来源：http://m.share.hesvh.cn/Article/details/gtzjrizdw.sHtML

Ruby: nested.flatten
来源：http://blog.hesvh.cn/Article/details/gxdjlxhjc.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gwxtcfgyl.sHtML

[D19] 按字段分组
来源：http://www.share.fehbvm.com/Article/details/gbbcklwoe.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.hesvh.cn/Article/details/gowpvnzlt.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.hesvh.cn/Article/details/gyzrpiobw.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.fehbvm.com/Article/details/ggeayyuvi.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.hesvh.cn/Article/details/gyofwkpgt.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.zdbjq.cn/Article/details/gsicuhhhp.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.zdbjq.cn/Article/details/gwutyolch.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.fehbvm.com/Article/details/gqxaxclap.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.fehbvm.com/Article/details/ghqkkexte.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.hesvh.cn/Article/details/gvbnkpqqj.sHtML

Py:   Counter(arr)
来源：http://blog.hesvh.cn/Article/details/gwncfktse.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.hesvh.cn/Article/details/giavljrvg.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/geiruunfp.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/ghglhrnys.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.zdbjq.cn/Article/details/gogwqrpoz.sHtML

Go:   // 手写 map[T]int
来源：http://3g.fehbvm.com/Article/details/gjfwptbzt.sHtML

Ruby: arr.tally
来源：http://baike.fehbvm.com/Article/details/gysjvvhev.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.hesvh.cn/Article/details/gygugamdp.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.zdbjq.cn/Article/details/gbnkmsccb.sHtML

Py:   x in arr
来源：http://wap.fehbvm.com/Article/details/gewxbxwsb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.hesvh.cn/Article/details/gyazkwtgv.sHtML

JS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/gbkxigilt.sHtML

TS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/gcitpgjip.sHtML

Java: list.contains(x)
来源：http://wap.zdbjq.cn/Article/details/giknoqpfm.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gnxxnhgcj.sHtML

Ruby: arr.include?(x)
来源：http://read.share.zdbjq.cn/Article/details/gdgcgupbv.sHtML

C#:   list.Contains(x)
来源：http://blog.hesvh.cn/Article/details/gllnproet.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.hesvh.cn/Article/details/ghgernsaf.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.fehbvm.com/Article/details/gkpqjbjla.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.fehbvm.com/Article/details/grzhjcefe.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.hesvh.cn/Article/details/gyhxtvmyc.sHtML

TS:   [...arr];
来源：http://3g.fehbvm.com/Article/details/glksreeyw.sHtML

Java: new ArrayList<>(list);
来源：http://baike.zdbjq.cn/Article/details/gkpkuekdz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.hesvh.cn/Article/details/gmgzxcmyc.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.fehbvm.com/Article/details/gkwcfenud.sHtML

C#:   new List<int>(list);
来源：http://mobile.zdbjq.cn/Article/details/ggmpuejmi.sHtML

[D23] reduce 累积计算
来源：http://www.blog.fehbvm.com/Article/details/gfnkujdlr.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.zdbjq.cn/Article/details/gonlgbvli.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.fehbvm.com/Article/details/gpnujghhf.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/glfnwemsf.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gxxpkexly.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.fehbvm.com/Article/details/gadnmyeik.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/gcmicrnmy.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.hesvh.cn/Article/details/gwclimelh.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.zdbjq.cn/Article/details/gvehkxokn.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.zdbjq.cn/Article/details/govwifkcu.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.zdbjq.cn/Article/details/govngxmee.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.hesvh.cn/Article/details/gggngaurp.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.zdbjq.cn/Article/details/gnwalvmhm.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gwbxjwxiw.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.fehbvm.com/Article/details/gxbrptnhc.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.fehbvm.com/Article/details/guqjzruno.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.zdbjq.cn/Article/details/gvkxsxtty.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.hesvh.cn/Article/details/gzpfrxhzt.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.hesvh.cn/Article/details/gymceqsps.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.hesvh.cn/Article/details/gimmweeru.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.fehbvm.com/Article/details/gjnxzhgfa.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.fehbvm.com/Article/details/gbsrieqte.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.zdbjq.cn/Article/details/gfupbobnt.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gbbqkrvxi.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.zdbjq.cn/Article/details/ghcqsgalg.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.zdbjq.cn/Article/details/gmldorpvp.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.fehbvm.com/Article/details/gozmfnicy.sHtML

[D26] 数组转字符串
来源：http://mobile.zdbjq.cn/Article/details/geoacewxj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.hesvh.cn/Article/details/gxtxdbmfr.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.zdbjq.cn/Article/details/gndgapwzz.sHtML

JS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gpbqxeckz.sHtML

TS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gjysxtgjw.sHtML

Java: String.join(", ", list)
来源：http://www.share.hesvh.cn/Article/details/gzgfgujbg.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.zdbjq.cn/Article/details/gcujebqut.sHtML

Ruby: arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/grrtefqgs.sHtML

C#:   string.Join(", ", list)
来源：http://baike.fehbvm.com/Article/details/gdhoskhlf.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gxsbastwm.sHtML

E. 字符串处理
来源：http://baike.hesvh.cn/Article/details/guxjmnmhv.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gqlzmpmtc.sHtML

[E01] 拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gcpqndcaz.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.fehbvm.com/Article/details/giagxbgpu.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.fehbvm.com/Article/details/gvqvmwmdl.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.hesvh.cn/Article/details/gvlmoqvdy.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gwxldjffi.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.zdbjq.cn/Article/details/gokfhodjs.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.hesvh.cn/Article/details/gvlbmpycl.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.zdbjq.cn/Article/details/gjaakpyhm.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.hesvh.cn/Article/details/gvnsgqldr.sHtML

[E02] 重复字符串
来源：http://baike.fehbvm.com/Article/details/gskqqhymc.sHtML

Py:   "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/gczqffhvv.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.zdbjq.cn/Article/details/gmlyzcmxw.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gzukepecf.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gdiqrjacr.sHtML

Java: "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gnpdfyarc.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.hesvh.cn/Article/details/gzxneggjr.sHtML

Ruby: "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gefjcdhts.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.fehbvm.com/Article/details/gcnqsxzkq.sHtML

[E03] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/gsxfhymjl.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.hesvh.cn/Article/details/gnqzmpfsc.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gafkvxwyx.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/ghtxmlqvy.sHtML

TS:   s.slice(1, 4)
来源：http://wap.fehbvm.com/Article/details/gbvgchkir.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gtbeuvfhx.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.fehbvm.com/Article/details/gyehjbwvg.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.zdbjq.cn/Article/details/gmruajosk.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.fehbvm.com/Article/details/gfqohyivt.sHtML

[E04] 查找子串位置
来源：http://read.share.hesvh.cn/Article/details/gzwbkclbw.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.hesvh.cn/Article/details/ghaerfxor.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.fehbvm.com/Article/details/gzpvlvrtv.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.zdbjq.cn/Article/details/grprprjzg.sHtML

TS:   s.indexOf("x")
来源：http://baike.hesvh.cn/Article/details/gpwdmsnoo.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gksnlywcw.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.zdbjq.cn/Article/details/gizrtuudd.sHtML

Ruby: s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/gzcqmyrny.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gbfmoaspl.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.zdbjq.cn/Article/details/glzspontu.sHtML


<!-- 参考信息 -->