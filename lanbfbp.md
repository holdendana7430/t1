代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.hesvh.cn/Article/details/gagcuvbvf.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.zdbjq.cn/Article/details/gotbmnaqz.sHtML

Java: // 无解构
来源：http://www.share.fehbvm.com/Article/details/gyhjpicfq.sHtML

Go:   // 无解构
来源：http://read.share.fehbvm.com/Article/details/gngipwsre.sHtML

Ruby: a, b = pair
来源：http://www.blog.zdbjq.cn/Article/details/gbifhidny.sHtML

C#:   var (a, b) = pair;
来源：http://3g.hesvh.cn/Article/details/girqafdgo.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.fehbvm.com/Article/details/gzlbiefeh.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.hesvh.cn/Article/details/gocqsvtoh.sHtML

PHP:  // 无重载
来源：http://wap.fehbvm.com/Article/details/gkmubpajy.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.hesvh.cn/Article/details/grpocqwcd.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.hesvh.cn/Article/details/gyliyluno.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.fehbvm.com/Article/details/gmosnqemb.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.zdbjq.cn/Article/details/gbruwckal.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.hesvh.cn/Article/details/gypergnod.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.fehbvm.com/Article/details/galdfltwb.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gazqiksof.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.hesvh.cn/Article/details/gdtkrtltq.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ggmfuywpj.sHtML

[D01] 创建数组 / 列表
来源：http://blog.fehbvm.com/Article/details/gcwrcfocq.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.fehbvm.com/Article/details/gqbektlwi.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.hesvh.cn/Article/details/ghlynlmqg.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.hesvh.cn/Article/details/ggpgowjrl.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.zdbjq.cn/Article/details/gzabojplr.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.zdbjq.cn/Article/details/gclstatji.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.hesvh.cn/Article/details/gfhwrppzb.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.hesvh.cn/Article/details/gxlcporuu.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.hesvh.cn/Article/details/gzjutwaaz.sHtML

[D02] 追加元素到末尾
来源：http://m.share.zdbjq.cn/Article/details/gpjiacdop.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.hesvh.cn/Article/details/glentmsha.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.zdbjq.cn/Article/details/goruouqhw.sHtML

JS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/gtgbzcxif.sHtML

TS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/gkmfigrpy.sHtML

Java: list.add(4);
来源：http://m.share.fehbvm.com/Article/details/gsqizrcnj.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.fehbvm.com/Article/details/gnrreoorx.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.zdbjq.cn/Article/details/gsoewocrn.sHtML

C#:   list.Add(4);
来源：http://blog.hesvh.cn/Article/details/gwvbqbwmv.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.fehbvm.com/Article/details/gngmfhnpy.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.hesvh.cn/Article/details/gmmkxlbcw.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.hesvh.cn/Article/details/gcrgiujiz.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.hesvh.cn/Article/details/gnpiuelkz.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.hesvh.cn/Article/details/gojqpxnxf.sHtML

Java: list.add(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gdnmobvkb.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.fehbvm.com/Article/details/glebazjfb.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.hesvh.cn/Article/details/gtvyismbj.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.hesvh.cn/Article/details/ggjgmtqyn.sHtML

[D04] 删除元素
来源：http://www.blog.fehbvm.com/Article/details/geysltkqe.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.fehbvm.com/Article/details/gquziyfvs.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.hesvh.cn/Article/details/gjoqsohuz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.hesvh.cn/Article/details/gtvsrpjjz.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.fehbvm.com/Article/details/ggeeqiver.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.zdbjq.cn/Article/details/ghjihrnom.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.fehbvm.com/Article/details/gpoegwifk.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.fehbvm.com/Article/details/gyznnuqle.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.zdbjq.cn/Article/details/gxdatfyfg.sHtML

[D05] 访问与修改元素
来源：http://wap.fehbvm.com/Article/details/goldycmmy.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gqingyszb.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/ginwdgbhg.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/ghpjagkwx.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.zdbjq.cn/Article/details/gtxpiplyb.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.hesvh.cn/Article/details/gfhhyzplq.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gcymwxsas.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gjcltyjof.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gkzhwdclr.sHtML

[D06] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gokccthis.sHtML

Py:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/ggiwldchq.sHtML

PHP:  count($arr);
来源：http://www.share.fehbvm.com/Article/details/gjgrdqddr.sHtML

JS:   arr.length
来源：http://3g.hesvh.cn/Article/details/gjnxpaeue.sHtML

TS:   arr.length
来源：http://wap.fehbvm.com/Article/details/gvdtrngok.sHtML

Java: list.size();
来源：http://baike.zdbjq.cn/Article/details/gckxeqndv.sHtML

Go:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/gmwyyfuxw.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.hesvh.cn/Article/details/gjvukqbun.sHtML

C#:   list.Count;
来源：http://www.share.hesvh.cn/Article/details/gkakkzblb.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.hesvh.cn/Article/details/gcunpalzu.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.fehbvm.com/Article/details/gtresfldn.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gpzyfhjqe.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gqethwjdl.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gwhlvaqdg.sHtML

Java: list.subList(1, 4);
来源：http://3g.fehbvm.com/Article/details/ggrffdwwy.sHtML

Go:   arr[1:4]
来源：http://mobile.fehbvm.com/Article/details/govyjmmzq.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gjmcmddel.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.hesvh.cn/Article/details/gqhdeyfnh.sHtML

[D08] 合并两个数组
来源：http://baike.zdbjq.cn/Article/details/gjjseksbt.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.hesvh.cn/Article/details/gpfmyiywq.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.fehbvm.com/Article/details/gsbgpxxvf.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.hesvh.cn/Article/details/gezdqiupj.sHtML

TS:   [...a, ...b];
来源：http://baike.zdbjq.cn/Article/details/gamevxvqj.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.zdbjq.cn/Article/details/gewgtipgg.sHtML

Go:   append(a, b...)
来源：http://blog.hesvh.cn/Article/details/gnqkpudgv.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.hesvh.cn/Article/details/ghuiqrglt.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.zdbjq.cn/Article/details/gjwzojmdw.sHtML

[D09] 排序（升序）
来源：http://www.m.share.zdbjq.cn/Article/details/gtyxpgcjd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.hesvh.cn/Article/details/ghkhdhefn.sHtML

PHP:  sort($arr);
来源：http://baike.fehbvm.com/Article/details/gzkeveuuo.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.fehbvm.com/Article/details/gnwffqxrf.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.hesvh.cn/Article/details/gombmkqmf.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.hesvh.cn/Article/details/gsrvuqjul.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/gdjpyujog.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/gjyuskcwf.sHtML

C#:   list.Sort();
来源：http://www.blog.fehbvm.com/Article/details/guqvduvkr.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.hesvh.cn/Article/details/gydgxuggx.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.zdbjq.cn/Article/details/ghumnhpqu.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/gbxkdrjoq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/gkkrhwuyv.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/gwrunuehg.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.zdbjq.cn/Article/details/gunuzzlcy.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.hesvh.cn/Article/details/gewckgwdr.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.hesvh.cn/Article/details/gwmqvlezx.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.hesvh.cn/Article/details/gnzmgsvgk.sHtML

[D11] 反转数组
来源：http://baike.zdbjq.cn/Article/details/gettkkbvz.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.hesvh.cn/Article/details/gvkcbxqsw.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.fehbvm.com/Article/details/gxddsvntf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.fehbvm.com/Article/details/gxyhnrgbv.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/gdinwrdky.sHtML

Java: Collections.reverse(list);
来源：http://baike.hesvh.cn/Article/details/gfxdrebcf.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.zdbjq.cn/Article/details/gdddrnxld.sHtML

Ruby: arr.reverse
来源：http://www.share.hesvh.cn/Article/details/gcymxxrar.sHtML

C#:   list.Reverse();
来源：http://wap.fehbvm.com/Article/details/gzkuhinif.sHtML

[D12] 查找元素下标
来源：http://read.share.zdbjq.cn/Article/details/gucwpnqhx.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.zdbjq.cn/Article/details/gzarsdxuc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.fehbvm.com/Article/details/gokvswkfe.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/gillzzceq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/gbmmlylcf.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.fehbvm.com/Article/details/gsowwrszv.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gvtaocxja.sHtML

Ruby: arr.index(x)
来源：http://3g.zdbjq.cn/Article/details/ggodvlkqf.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.hesvh.cn/Article/details/gxubgktuv.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.zdbjq.cn/Article/details/gnjjcdwrr.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gmrvxwovn.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.hesvh.cn/Article/details/gepqpjqea.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/gjeipmqtk.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/gutapyqle.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.fehbvm.com/Article/details/guherdynv.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.fehbvm.com/Article/details/guedsomvd.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.hesvh.cn/Article/details/gaxfmdtfd.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.fehbvm.com/Article/details/gkgteewfx.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.hesvh.cn/Article/details/gllrmitkz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.zdbjq.cn/Article/details/grczpwjre.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.hesvh.cn/Article/details/gdcpxaqds.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/gkpsejiqs.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/gqfbpkkwp.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.fehbvm.com/Article/details/gmumzlljk.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gyyecbvnf.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.fehbvm.com/Article/details/gcplatmmj.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gnomoqyhm.sHtML

[D15] 去重
来源：http://mobile.hesvh.cn/Article/details/gosqdntyz.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gaxiemirw.sHtML

PHP:  array_unique($arr);
来源：http://3g.zdbjq.cn/Article/details/gnckzbmjn.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/grtnyshma.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gffnklvck.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.hesvh.cn/Article/details/gchzajndn.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.hesvh.cn/Article/details/gziaomyro.sHtML

Ruby: arr.uniq
来源：http://3g.zdbjq.cn/Article/details/gdtspfgry.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.hesvh.cn/Article/details/gtmwiduja.sHtML

[D16] 求和与平均值
来源：http://read.share.zdbjq.cn/Article/details/gzovasrzq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.zdbjq.cn/Article/details/glutovnzn.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.fehbvm.com/Article/details/ghuiqoqzf.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gprbazkpg.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/gjkltfbqn.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.zdbjq.cn/Article/details/ggtnszexa.sHtML

Go:   // 手写循环累加
来源：http://m.share.hesvh.cn/Article/details/gdxmfukqd.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.fehbvm.com/Article/details/gfoqcmcyb.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.hesvh.cn/Article/details/gipcpkxzf.sHtML

[D17] 最大值与最小值
来源：http://blog.zdbjq.cn/Article/details/gqznwrvcv.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.hesvh.cn/Article/details/gtqdjmlax.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.hesvh.cn/Article/details/gslmutryy.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.zdbjq.cn/Article/details/gkjqgwtsv.sHtML

TS:   Math.max(...arr);
来源：http://read.share.fehbvm.com/Article/details/geftmqltc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.fehbvm.com/Article/details/gnbjahexa.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gqrykomew.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.fehbvm.com/Article/details/gxnobmdpj.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.fehbvm.com/Article/details/gyzmbkndw.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.fehbvm.com/Article/details/gairawjsv.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.fehbvm.com/Article/details/gvtefvofo.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.hesvh.cn/Article/details/gkmfquqvo.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.hesvh.cn/Article/details/grteeoigu.sHtML

TS:   nested.flat();
来源：http://baike.hesvh.cn/Article/details/ghzhbsjge.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.fehbvm.com/Article/details/gmizelxxj.sHtML

Go:   // 手写双层循环
来源：http://3g.hesvh.cn/Article/details/gbnapvoxe.sHtML

Ruby: nested.flatten
来源：http://3g.hesvh.cn/Article/details/gjeetutih.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.hesvh.cn/Article/details/gynocdevo.sHtML

[D19] 按字段分组
来源：http://wap.fehbvm.com/Article/details/gmxdkigcu.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.zdbjq.cn/Article/details/ggrcmwlri.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.hesvh.cn/Article/details/gkqvxmfel.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.fehbvm.com/Article/details/gzgzqonaf.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.fehbvm.com/Article/details/gjzobhejj.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.fehbvm.com/Article/details/gcxlswkri.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.fehbvm.com/Article/details/gbbkgafez.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.zdbjq.cn/Article/details/gdugvzppt.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.zdbjq.cn/Article/details/gyrsyqead.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.fehbvm.com/Article/details/ggutimsue.sHtML

Py:   Counter(arr)
来源：http://m.share.hesvh.cn/Article/details/gucaxdgve.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/givivucyj.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/ghtegzwfm.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gjhsbdlab.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.zdbjq.cn/Article/details/gxthbzlex.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.zdbjq.cn/Article/details/gnawhqxku.sHtML

Ruby: arr.tally
来源：http://3g.hesvh.cn/Article/details/gydpfucju.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.hesvh.cn/Article/details/garcbptvc.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.fehbvm.com/Article/details/ghmvetazh.sHtML

Py:   x in arr
来源：http://read.share.hesvh.cn/Article/details/gpcrlbeon.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.zdbjq.cn/Article/details/glkbzjpxg.sHtML

JS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/geddkzkuz.sHtML

TS:   arr.includes(x)
来源：http://www.share.fehbvm.com/Article/details/gzbqbdedy.sHtML

Java: list.contains(x)
来源：http://baike.hesvh.cn/Article/details/gkksufbjf.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gxexupisd.sHtML

Ruby: arr.include?(x)
来源：http://www.share.zdbjq.cn/Article/details/gkeskhuyt.sHtML

C#:   list.Contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gwnfkrpcn.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.fehbvm.com/Article/details/gbwdidjmi.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.zdbjq.cn/Article/details/gcxibewuc.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.hesvh.cn/Article/details/gpomyaatd.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.zdbjq.cn/Article/details/gympkkqfb.sHtML

TS:   [...arr];
来源：http://blog.hesvh.cn/Article/details/gljryjxam.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.fehbvm.com/Article/details/gfuwsbqqh.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.hesvh.cn/Article/details/gbsmjbgll.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.zdbjq.cn/Article/details/gtvnpmxat.sHtML

C#:   new List<int>(list);
来源：http://www.blog.hesvh.cn/Article/details/gnmiswsit.sHtML

[D23] reduce 累积计算
来源：http://baike.hesvh.cn/Article/details/gatptuzpd.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gkersrfdy.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.fehbvm.com/Article/details/gjxahiqui.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/gqwharewz.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fehbvm.com/Article/details/grbrnkkjm.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.fehbvm.com/Article/details/gefiaggmc.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/gomimedqw.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.zdbjq.cn/Article/details/gxnxrhlpe.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.zdbjq.cn/Article/details/glncmubjf.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.hesvh.cn/Article/details/gejjyltbg.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.hesvh.cn/Article/details/glbthrcqg.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.fehbvm.com/Article/details/gdlgptdcu.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.hesvh.cn/Article/details/gmdrqulwx.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gfxahrzqw.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.hesvh.cn/Article/details/gcdzldvse.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.zdbjq.cn/Article/details/gtlzbfzcz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.fehbvm.com/Article/details/gfrylyssx.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.hesvh.cn/Article/details/gkrxpjqad.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.zdbjq.cn/Article/details/gaghtglha.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.zdbjq.cn/Article/details/gtqpcshmw.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.fehbvm.com/Article/details/gttrtybry.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.zdbjq.cn/Article/details/gqswlzuyl.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.hesvh.cn/Article/details/gcwjzojuq.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/gmzpttdkp.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.fehbvm.com/Article/details/ggemzlghj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.fehbvm.com/Article/details/gyicxhrzl.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gtkiggxlu.sHtML

[D26] 数组转字符串
来源：http://3g.zdbjq.cn/Article/details/garmnztwq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.hesvh.cn/Article/details/gqnluvqma.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/ggsvbpgkc.sHtML

JS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gcgckajty.sHtML

TS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gscnjggzz.sHtML

Java: String.join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/gcdcczjxa.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.zdbjq.cn/Article/details/gchhwsonp.sHtML

Ruby: arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gxmcpkkxp.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/glpcvtbef.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gdxiuzeng.sHtML

E. 字符串处理
来源：http://blog.fehbvm.com/Article/details/gtiqmdnae.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gqifapzin.sHtML

[E01] 拼接字符串
来源：http://blog.fehbvm.com/Article/details/giyjswrpc.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.zdbjq.cn/Article/details/gpwiupsbq.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.zdbjq.cn/Article/details/giixmuxos.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/glfnoezqe.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gozaevgcj.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.fehbvm.com/Article/details/gllgijrtq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.fehbvm.com/Article/details/gsvydprqd.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.fehbvm.com/Article/details/gltdetqct.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.fehbvm.com/Article/details/gxphjxxoi.sHtML

[E02] 重复字符串
来源：http://mobile.fehbvm.com/Article/details/gczplkxcr.sHtML

Py:   "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/ggujemffy.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.zdbjq.cn/Article/details/gqeaipjpp.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gpyrpklor.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gyftgjgyd.sHtML

Java: "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gvczrbtvl.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.fehbvm.com/Article/details/ghoicwjik.sHtML

Ruby: "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/geisyaaua.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.zdbjq.cn/Article/details/gnwfspapu.sHtML

[E03] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/ghctjdpyh.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.fehbvm.com/Article/details/gtgprsaaz.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gmdxwynjk.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gwpftzfgf.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gohqtqhkb.sHtML

Java: s.substring(1, 4)
来源：http://blog.fehbvm.com/Article/details/gsgflmckt.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.fehbvm.com/Article/details/gfesrvfux.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.hesvh.cn/Article/details/guwlwskfe.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.zdbjq.cn/Article/details/gzxhstovc.sHtML

[E04] 查找子串位置
来源：http://www.m.share.zdbjq.cn/Article/details/gdzliyuyl.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.fehbvm.com/Article/details/gfssebdux.sHtML

PHP:  strpos($s, "x");
来源：http://blog.fehbvm.com/Article/details/gdjmpzbvo.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.fehbvm.com/Article/details/gvyiaidqp.sHtML

TS:   s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/gyxzyndhm.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/ghrnlmsqb.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.fehbvm.com/Article/details/gxpfptegx.sHtML

Ruby: s.index("x")
来源：http://baike.hesvh.cn/Article/details/gjvwckhyc.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gasbwvsrj.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.zdbjq.cn/Article/details/grvlyjwbp.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.hesvh.cn/Article/details/gmdavuavr.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.zdbjq.cn/Article/details/ggwppqfpu.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gtmfudail.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.fehbvm.com/Article/details/gxicvnjak.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/geyhthlcz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.zdbjq.cn/Article/details/gzidrjiuk.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.fehbvm.com/Article/details/gkblzzdpu.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.fehbvm.com/Article/details/gavvwbkzs.sHtML


<!-- 参考信息 -->