代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.zdbjq.cn/Article/details/gqjhcknds.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.hesvh.cn/Article/details/ghwuuxqdg.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.hesvh.cn/Article/details/gtoqcoqzf.sHtML

Ruby: # 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gjbimftig.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.zdbjq.cn/Article/details/garsmgzjk.sHtML

[C15] 解构 / 展开参数
来源：http://blog.hesvh.cn/Article/details/guomigvot.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.hesvh.cn/Article/details/gnzbwhabv.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.hesvh.cn/Article/details/golrypwcm.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.hesvh.cn/Article/details/gqhtfzzlt.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.zdbjq.cn/Article/details/gpycqdesj.sHtML

Java: // 无解构
来源：http://wap.fehbvm.com/Article/details/gdvhivyxv.sHtML

Go:   // 无解构
来源：http://blog.zdbjq.cn/Article/details/gxvpkkfgr.sHtML

Ruby: a, b = pair
来源：http://mobile.fehbvm.com/Article/details/gerxnmdvp.sHtML

C#:   var (a, b) = pair;
来源：http://3g.zdbjq.cn/Article/details/gbwfsjqvu.sHtML

[C16] 函数 / 方法重载
来源：http://blog.fehbvm.com/Article/details/glagtypqf.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.fehbvm.com/Article/details/gwmepnber.sHtML

PHP:  // 无重载
来源：http://3g.fehbvm.com/Article/details/gdavfjnvo.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.zdbjq.cn/Article/details/gkesdbowa.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.hesvh.cn/Article/details/gnlxueron.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.zdbjq.cn/Article/details/gqwrjwzle.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.fehbvm.com/Article/details/givwrmnrf.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.hesvh.cn/Article/details/gmvwvxdsh.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.fehbvm.com/Article/details/gkpbljgvc.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gozjoyktd.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.zdbjq.cn/Article/details/ghfwqhtfj.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gwwhoeery.sHtML

[D01] 创建数组 / 列表
来源：http://baike.hesvh.cn/Article/details/gwczxzosq.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.fehbvm.com/Article/details/ggcpdeywl.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.zdbjq.cn/Article/details/ghnuyhxkl.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.hesvh.cn/Article/details/glckyyewo.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.hesvh.cn/Article/details/gyzqgccyw.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.hesvh.cn/Article/details/gqsevbecg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.hesvh.cn/Article/details/grevwnjdx.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.zdbjq.cn/Article/details/gcybwxdpg.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.hesvh.cn/Article/details/giuzcayki.sHtML

[D02] 追加元素到末尾
来源：http://baike.fehbvm.com/Article/details/gtyfrksmn.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.hesvh.cn/Article/details/gdjveuzfx.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.zdbjq.cn/Article/details/gaqbqzcum.sHtML

JS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/gizudbqah.sHtML

TS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/gtddgvrto.sHtML

Java: list.add(4);
来源：http://m.share.fehbvm.com/Article/details/gklqddwdt.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.zdbjq.cn/Article/details/glnvhdjdl.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.fehbvm.com/Article/details/gszqkjeoc.sHtML

C#:   list.Add(4);
来源：http://www.share.fehbvm.com/Article/details/gdcdgijul.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.zdbjq.cn/Article/details/gaeqlaonb.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.zdbjq.cn/Article/details/gtndvnayi.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.zdbjq.cn/Article/details/gewakpqgt.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.fehbvm.com/Article/details/gadleedxy.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.fehbvm.com/Article/details/gzsnqulwz.sHtML

Java: list.add(0, 0);
来源：http://baike.fehbvm.com/Article/details/gmeqqvhab.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.hesvh.cn/Article/details/gcnrpbufh.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.zdbjq.cn/Article/details/gjjwaqfkf.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.zdbjq.cn/Article/details/gfzcvudqr.sHtML

[D04] 删除元素
来源：http://blog.hesvh.cn/Article/details/gslfgiazc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.fehbvm.com/Article/details/glispluyd.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.hesvh.cn/Article/details/guwnrglxd.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.hesvh.cn/Article/details/gkgpfhhua.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.fehbvm.com/Article/details/goefurtdw.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.fehbvm.com/Article/details/gneljqkcs.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.fehbvm.com/Article/details/gpuyifetg.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.zdbjq.cn/Article/details/gkjumpoha.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.hesvh.cn/Article/details/gxqvydsdd.sHtML

[D05] 访问与修改元素
来源：http://www.blog.fehbvm.com/Article/details/gdjnqxjey.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gjuqtibpt.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gjiekiope.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gvdvumrtq.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.fehbvm.com/Article/details/gpyzsuqqi.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.fehbvm.com/Article/details/gjbdeuyfw.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gkrhpckfv.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gipstlbug.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gtyaoqobd.sHtML

[D06] 数组长度
来源：http://3g.zdbjq.cn/Article/details/gcapsppzg.sHtML

Py:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/gefsndcxg.sHtML

PHP:  count($arr);
来源：http://wap.fehbvm.com/Article/details/gqpkxuzod.sHtML

JS:   arr.length
来源：http://wap.hesvh.cn/Article/details/gdsfbwarb.sHtML

TS:   arr.length
来源：http://baike.fehbvm.com/Article/details/gzsbodyms.sHtML

Java: list.size();
来源：http://m.share.hesvh.cn/Article/details/gveomhafg.sHtML

Go:   len(arr)
来源：http://baike.fehbvm.com/Article/details/gvilhwwfx.sHtML

Ruby: arr.length; arr.size
来源：http://baike.zdbjq.cn/Article/details/gkakiezux.sHtML

C#:   list.Count;
来源：http://www.blog.fehbvm.com/Article/details/gvzkhkbtk.sHtML

[D07] 切片 / 取子数组
来源：http://wap.fehbvm.com/Article/details/gmcrqxbox.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.zdbjq.cn/Article/details/gqgopemgd.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gelmnqhul.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gnukeqewu.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gogtqpala.sHtML

Java: list.subList(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gkgvakfuu.sHtML

Go:   arr[1:4]
来源：http://www.blog.zdbjq.cn/Article/details/gekjilzqb.sHtML

Ruby: arr[1, 3]
来源：http://wap.fehbvm.com/Article/details/gnljmsgqo.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.hesvh.cn/Article/details/gswvuhqhb.sHtML

[D08] 合并两个数组
来源：http://3g.fehbvm.com/Article/details/gklntsjlw.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.hesvh.cn/Article/details/gptkvesph.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.zdbjq.cn/Article/details/gphjtljak.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.zdbjq.cn/Article/details/gkutdorgw.sHtML

TS:   [...a, ...b];
来源：http://mobile.hesvh.cn/Article/details/gtcezhsxd.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.fehbvm.com/Article/details/gjlfxznww.sHtML

Go:   append(a, b...)
来源：http://baike.fehbvm.com/Article/details/gcbwerqnm.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.hesvh.cn/Article/details/gbcrxubsc.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.fehbvm.com/Article/details/gytplppxg.sHtML

[D09] 排序（升序）
来源：http://blog.hesvh.cn/Article/details/gkblaiifj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.hesvh.cn/Article/details/gomtaacby.sHtML

PHP:  sort($arr);
来源：http://baike.hesvh.cn/Article/details/govyqngar.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.fehbvm.com/Article/details/gboehdvgw.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.fehbvm.com/Article/details/gsqhlsgyn.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.zdbjq.cn/Article/details/ghaacreiy.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gixyxlgfx.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/gmnaguyfi.sHtML

C#:   list.Sort();
来源：http://www.share.zdbjq.cn/Article/details/gvgujtaqh.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.zdbjq.cn/Article/details/gdrwhipob.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.fehbvm.com/Article/details/gruutfhmw.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/gsmsvdgju.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/gfbbpuwfa.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gueehdurd.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.zdbjq.cn/Article/details/ghfelaxdm.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.fehbvm.com/Article/details/glfymvpvq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.hesvh.cn/Article/details/glvokaxiw.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.zdbjq.cn/Article/details/gnapmxoaw.sHtML

[D11] 反转数组
来源：http://blog.fehbvm.com/Article/details/gelbwdpwd.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.fehbvm.com/Article/details/gfggfmdth.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.fehbvm.com/Article/details/griktypqy.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.zdbjq.cn/Article/details/ghufyzsty.sHtML

TS:   [...arr].reverse();
来源：http://www.share.hesvh.cn/Article/details/gdcybnpyn.sHtML

Java: Collections.reverse(list);
来源：http://mobile.zdbjq.cn/Article/details/gubttehcv.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.hesvh.cn/Article/details/gviarfftd.sHtML

Ruby: arr.reverse
来源：http://www.share.fehbvm.com/Article/details/giszmunzb.sHtML

C#:   list.Reverse();
来源：http://www.blog.hesvh.cn/Article/details/gnpyjcwmw.sHtML

[D12] 查找元素下标
来源：http://blog.zdbjq.cn/Article/details/gqcasycrh.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.hesvh.cn/Article/details/ghsgrnirb.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.fehbvm.com/Article/details/gdgzuffsj.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gjhnyiwln.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/gwkubtorf.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.fehbvm.com/Article/details/gwzflfxux.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gtauyusul.sHtML

Ruby: arr.index(x)
来源：http://wap.zdbjq.cn/Article/details/grqhzjjql.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.zdbjq.cn/Article/details/gziqnljzh.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.zdbjq.cn/Article/details/gykpnjgap.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.zdbjq.cn/Article/details/gjzzchyeh.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.zdbjq.cn/Article/details/gxhdgetui.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.fehbvm.com/Article/details/gzasskfqg.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/gxrcsgcug.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.zdbjq.cn/Article/details/gjuqlxnmo.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.hesvh.cn/Article/details/gmpgzbhto.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.fehbvm.com/Article/details/gifercwaq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.hesvh.cn/Article/details/ghvpttxpr.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.hesvh.cn/Article/details/ghpslnwsg.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.hesvh.cn/Article/details/gsssmmnqq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gwghfmbgp.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gbxoaqpiw.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/ggaotoiex.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.hesvh.cn/Article/details/gsilezdso.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/gzighngfd.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gkqqccyom.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.fehbvm.com/Article/details/gwbaraeeh.sHtML

[D15] 去重
来源：http://read.share.hesvh.cn/Article/details/gkbnsxvjc.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/gcsggxjox.sHtML

PHP:  array_unique($arr);
来源：http://mobile.hesvh.cn/Article/details/goolwwgyx.sHtML

JS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gemxwcvsv.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gklfolygb.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.fehbvm.com/Article/details/gxciahala.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.hesvh.cn/Article/details/gqklxaece.sHtML

Ruby: arr.uniq
来源：http://baike.zdbjq.cn/Article/details/gbzuqjclf.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.hesvh.cn/Article/details/gsnugzxzi.sHtML

[D16] 求和与平均值
来源：http://wap.hesvh.cn/Article/details/geyimaytl.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.zdbjq.cn/Article/details/gbbbxqlys.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.fehbvm.com/Article/details/griorxvid.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/gdtecockq.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/ggrfaomqe.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.zdbjq.cn/Article/details/geopukjyk.sHtML

Go:   // 手写循环累加
来源：http://m.share.fehbvm.com/Article/details/gjmyqsoca.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.hesvh.cn/Article/details/gvtonjtxu.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.zdbjq.cn/Article/details/gbdiorhai.sHtML

[D17] 最大值与最小值
来源：http://mobile.hesvh.cn/Article/details/gblmtwqjj.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gkxjlnaix.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gpcweqond.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.fehbvm.com/Article/details/gongbivsv.sHtML

TS:   Math.max(...arr);
来源：http://www.share.fehbvm.com/Article/details/gxahjpfrc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.zdbjq.cn/Article/details/gajadmvtz.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.zdbjq.cn/Article/details/grifsiudr.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.zdbjq.cn/Article/details/gpojqsjmu.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.zdbjq.cn/Article/details/guohajuht.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.fehbvm.com/Article/details/gataroyup.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.hesvh.cn/Article/details/gikeaytnd.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.hesvh.cn/Article/details/gjevxrase.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.zdbjq.cn/Article/details/gtgfmkqph.sHtML

TS:   nested.flat();
来源：http://mobile.zdbjq.cn/Article/details/gtyfsmjup.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.fehbvm.com/Article/details/gqdaeevvs.sHtML

Go:   // 手写双层循环
来源：http://www.share.fehbvm.com/Article/details/gowopewzr.sHtML

Ruby: nested.flatten
来源：http://www.m.share.fehbvm.com/Article/details/grazgpxgj.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.hesvh.cn/Article/details/gubunlpdp.sHtML

[D19] 按字段分组
来源：http://mobile.hesvh.cn/Article/details/gkwbbgqvf.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.hesvh.cn/Article/details/gudxxhcss.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.fehbvm.com/Article/details/gdfbxzflk.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.zdbjq.cn/Article/details/gsaosyfia.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/gcfsybtkk.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.hesvh.cn/Article/details/gozqbmzrt.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.zdbjq.cn/Article/details/gotwkmtrr.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.fehbvm.com/Article/details/gokrvrehf.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.hesvh.cn/Article/details/gxcxrwxtg.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.hesvh.cn/Article/details/gwyxsjejd.sHtML

Py:   Counter(arr)
来源：http://wap.zdbjq.cn/Article/details/gullegrel.sHtML

PHP:  array_count_values($arr);
来源：http://blog.zdbjq.cn/Article/details/gbbhhinod.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fehbvm.com/Article/details/glambdcne.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gaqjngona.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.hesvh.cn/Article/details/ggojmihvi.sHtML

Go:   // 手写 map[T]int
来源：http://baike.hesvh.cn/Article/details/gpjwugfda.sHtML

Ruby: arr.tally
来源：http://www.blog.zdbjq.cn/Article/details/gnvkznacs.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.fehbvm.com/Article/details/ggwofagsg.sHtML

[D21] 判断是否包含某元素
来源：http://blog.zdbjq.cn/Article/details/gddsddfph.sHtML

Py:   x in arr
来源：http://www.blog.zdbjq.cn/Article/details/gannlejma.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.hesvh.cn/Article/details/gfwisgmsu.sHtML

JS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gzjcrbbfk.sHtML

TS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/grikjwmaa.sHtML

Java: list.contains(x)
来源：http://mobile.fehbvm.com/Article/details/ghkekacfy.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.fehbvm.com/Article/details/gmdmmfdrk.sHtML

Ruby: arr.include?(x)
来源：http://blog.hesvh.cn/Article/details/gunuqesvv.sHtML

C#:   list.Contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gqbexyekn.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.fehbvm.com/Article/details/gspbvujkm.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gejdhdudv.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.zdbjq.cn/Article/details/ghpthxblq.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.hesvh.cn/Article/details/gwoxfvcdy.sHtML

TS:   [...arr];
来源：http://www.blog.fehbvm.com/Article/details/gsvpllpqk.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.zdbjq.cn/Article/details/girdpzhkg.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.hesvh.cn/Article/details/gwvlrpgev.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.hesvh.cn/Article/details/gjgjchxei.sHtML

C#:   new List<int>(list);
来源：http://www.blog.zdbjq.cn/Article/details/gtaxydqxr.sHtML

[D23] reduce 累积计算
来源：http://blog.zdbjq.cn/Article/details/gvqmjhusb.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.fehbvm.com/Article/details/glhmofjsd.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.fehbvm.com/Article/details/gexjnbvlq.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/gzuzpnuyn.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gfspwrkrf.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.zdbjq.cn/Article/details/gcygeqoih.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/gmqnnqemx.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.fehbvm.com/Article/details/gqzyyjzme.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.zdbjq.cn/Article/details/gbtzvrwwz.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.hesvh.cn/Article/details/ggmzriies.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.hesvh.cn/Article/details/gnqmmufxu.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.zdbjq.cn/Article/details/guihziyno.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.zdbjq.cn/Article/details/grwkwrtqc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.fehbvm.com/Article/details/gbddxhkxv.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.zdbjq.cn/Article/details/gbpxlyyhv.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.zdbjq.cn/Article/details/gvkadpcxf.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.hesvh.cn/Article/details/gxaxcngbo.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.zdbjq.cn/Article/details/gfvlsclio.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.zdbjq.cn/Article/details/gubaqljsn.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.fehbvm.com/Article/details/gqdtkzqrj.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.hesvh.cn/Article/details/gysjauhgx.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.fehbvm.com/Article/details/genezfnwy.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.fehbvm.com/Article/details/gbqslqaqp.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.hesvh.cn/Article/details/grfobrelh.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.zdbjq.cn/Article/details/gmintsyzp.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.fehbvm.com/Article/details/gvmgtakct.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.zdbjq.cn/Article/details/gqzcethal.sHtML

[D26] 数组转字符串
来源：http://3g.fehbvm.com/Article/details/gvmxtcqup.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.hesvh.cn/Article/details/gvylnuvkr.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gbvggjwub.sHtML

JS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gchzjsmuc.sHtML

TS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/ggkgsjbpq.sHtML

Java: String.join(", ", list)
来源：http://baike.fehbvm.com/Article/details/gihoxtsrt.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gfntexlis.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gzirpttfe.sHtML

C#:   string.Join(", ", list)
来源：http://blog.zdbjq.cn/Article/details/geatbzznu.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gkpyfcfcr.sHtML

E. 字符串处理
来源：http://3g.fehbvm.com/Article/details/ghsjvdtzd.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/giuucfdbg.sHtML

[E01] 拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gvreneduo.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.zdbjq.cn/Article/details/goguhvtzp.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.fehbvm.com/Article/details/gegwflivt.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/gitsbuaii.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gvsahudxp.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.hesvh.cn/Article/details/guttdoqee.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.fehbvm.com/Article/details/guvzlgubx.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.fehbvm.com/Article/details/gpxhbakkp.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gzusdbuyx.sHtML

[E02] 重复字符串
来源：http://www.share.zdbjq.cn/Article/details/gxkaoyfsp.sHtML

Py:   "ab" * 3
来源：http://wap.hesvh.cn/Article/details/gfgrtgogl.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.hesvh.cn/Article/details/gpckauvxf.sHtML

JS:   "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gmoulcavc.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gqqzzwwfs.sHtML

Java: "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gthvjgfhk.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.zdbjq.cn/Article/details/gclkxvhlf.sHtML

Ruby: "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/gmgnpdwft.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.zdbjq.cn/Article/details/gsxlyrjfa.sHtML

[E03] 截取子串
来源：http://www.share.hesvh.cn/Article/details/gkgtdgfbs.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.hesvh.cn/Article/details/gzdbkxsjf.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gyznmwbbx.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gwpyhmdyj.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gnutyhljs.sHtML

Java: s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gokilxktv.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.zdbjq.cn/Article/details/gcabuuxux.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.fehbvm.com/Article/details/ghrtzidqt.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.fehbvm.com/Article/details/gcwbzliol.sHtML

[E04] 查找子串位置
来源：http://www.blog.fehbvm.com/Article/details/gvpbtrgqr.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/gkqatxxaa.sHtML

PHP:  strpos($s, "x");
来源：http://3g.fehbvm.com/Article/details/gmkmokwpr.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.zdbjq.cn/Article/details/gjfolmvlf.sHtML

TS:   s.indexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gmrebsuib.sHtML

Java: s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/grgmggknm.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.zdbjq.cn/Article/details/gevsepiai.sHtML

Ruby: s.index("x")
来源：http://www.share.fehbvm.com/Article/details/gufrklbyx.sHtML

C#:   s.IndexOf("x")
来源：http://baike.hesvh.cn/Article/details/gbckvytaw.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.zdbjq.cn/Article/details/grmmwaume.sHtML


<!-- 参考信息 -->