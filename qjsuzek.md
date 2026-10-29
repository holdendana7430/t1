代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.fehbvm.com/Article/details/gokqdsagw.sHtML

[C15] 解构 / 展开参数
来源：http://blog.hesvh.cn/Article/details/gtdczdels.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.zdbjq.cn/Article/details/gunlxhuqp.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.zdbjq.cn/Article/details/gjelvfved.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/gqyhjnplv.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.fehbvm.com/Article/details/gulmtrbjj.sHtML

Java: // 无解构
来源：http://wap.zdbjq.cn/Article/details/gaurgnbgs.sHtML

Go:   // 无解构
来源：http://blog.hesvh.cn/Article/details/gcqgrrarv.sHtML

Ruby: a, b = pair
来源：http://wap.zdbjq.cn/Article/details/garjseend.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.hesvh.cn/Article/details/gfzkbqrfw.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.fehbvm.com/Article/details/gikreovpo.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.fehbvm.com/Article/details/gtkihxfnk.sHtML

PHP:  // 无重载
来源：http://blog.hesvh.cn/Article/details/gmummsunx.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.fehbvm.com/Article/details/gtxpnasua.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.fehbvm.com/Article/details/gbueqxkor.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.zdbjq.cn/Article/details/gpdallklg.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.hesvh.cn/Article/details/gxucypgev.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.hesvh.cn/Article/details/gudfdzhip.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.fehbvm.com/Article/details/gcbtwfbki.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/glitzhsui.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.fehbvm.com/Article/details/ghuevvqaw.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ghlvamprw.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.fehbvm.com/Article/details/gzvplyeke.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.hesvh.cn/Article/details/gswjdjbel.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.zdbjq.cn/Article/details/gmhvsxoiq.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.fehbvm.com/Article/details/gkibebupt.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.zdbjq.cn/Article/details/gonkjrzem.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.zdbjq.cn/Article/details/gzbbpgmus.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.zdbjq.cn/Article/details/gwuqyyvtx.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.hesvh.cn/Article/details/gotykeggw.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.zdbjq.cn/Article/details/gvqzremby.sHtML

[D02] 追加元素到末尾
来源：http://m.share.hesvh.cn/Article/details/gtoufwglz.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.hesvh.cn/Article/details/gjkubkwia.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.fehbvm.com/Article/details/gglobfkap.sHtML

JS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/gptklkkbo.sHtML

TS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/gmqggkjsk.sHtML

Java: list.add(4);
来源：http://blog.zdbjq.cn/Article/details/gvwnqngbs.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.hesvh.cn/Article/details/gfnrdpvqo.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.fehbvm.com/Article/details/gqbyfczzl.sHtML

C#:   list.Add(4);
来源：http://wap.hesvh.cn/Article/details/gwlmtwgrv.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.fehbvm.com/Article/details/gfmkbyqtg.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.zdbjq.cn/Article/details/gayujczcx.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.zdbjq.cn/Article/details/gjgpostgl.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.zdbjq.cn/Article/details/grfxmbgli.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.zdbjq.cn/Article/details/ggjvhzycn.sHtML

Java: list.add(0, 0);
来源：http://wap.hesvh.cn/Article/details/gzkujgpfd.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.fehbvm.com/Article/details/gtrkipikz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.zdbjq.cn/Article/details/gxrkhzrpf.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.fehbvm.com/Article/details/gcgucifuz.sHtML

[D04] 删除元素
来源：http://baike.hesvh.cn/Article/details/gyipgwmfk.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.hesvh.cn/Article/details/gvgvdicji.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.fehbvm.com/Article/details/gewceiefc.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.fehbvm.com/Article/details/gyfpytsjo.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.fehbvm.com/Article/details/glszigoru.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.fehbvm.com/Article/details/gvctgxlyy.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.hesvh.cn/Article/details/ggzctiokn.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.zdbjq.cn/Article/details/gjgqabhfj.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.fehbvm.com/Article/details/gyelqipkn.sHtML

[D05] 访问与修改元素
来源：http://mobile.fehbvm.com/Article/details/gfloecgdj.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gvvsougfc.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gpwlnnduu.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gtwwzmqfs.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.hesvh.cn/Article/details/gbedmxsxt.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.zdbjq.cn/Article/details/gplotyewo.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gjcxvblhw.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gccbjklvy.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/ggyxdgeic.sHtML

[D06] 数组长度
来源：http://read.share.hesvh.cn/Article/details/girvqttga.sHtML

Py:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/gjwzokehg.sHtML

PHP:  count($arr);
来源：http://baike.zdbjq.cn/Article/details/gtmkacoko.sHtML

JS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/gcchaxptc.sHtML

TS:   arr.length
来源：http://www.m.share.hesvh.cn/Article/details/gpbwiahnc.sHtML

Java: list.size();
来源：http://m.share.fehbvm.com/Article/details/grylniadu.sHtML

Go:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gdmhymijx.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.hesvh.cn/Article/details/gswrtauvg.sHtML

C#:   list.Count;
来源：http://baike.hesvh.cn/Article/details/glrxapkuq.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.zdbjq.cn/Article/details/guknjeqok.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.fehbvm.com/Article/details/gziypqsnx.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.fehbvm.com/Article/details/gkfukhnrx.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gnqlsptgx.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gbddjjsie.sHtML

Java: list.subList(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/ghmelobar.sHtML

Go:   arr[1:4]
来源：http://3g.fehbvm.com/Article/details/goraozqby.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.hesvh.cn/Article/details/grxwegaub.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.zdbjq.cn/Article/details/gznzaqnls.sHtML

[D08] 合并两个数组
来源：http://www.m.share.fehbvm.com/Article/details/gdvanxtao.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.hesvh.cn/Article/details/geyqwpwck.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.zdbjq.cn/Article/details/gdaxlibse.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.hesvh.cn/Article/details/gvxwfqlsj.sHtML

TS:   [...a, ...b];
来源：http://blog.fehbvm.com/Article/details/gdsekvfgt.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.zdbjq.cn/Article/details/gvgcoczap.sHtML

Go:   append(a, b...)
来源：http://3g.fehbvm.com/Article/details/gkygvyrby.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.hesvh.cn/Article/details/ggtbeymiy.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.hesvh.cn/Article/details/grzzkkstt.sHtML

[D09] 排序（升序）
来源：http://read.share.zdbjq.cn/Article/details/gcobgxlea.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/guphcbioc.sHtML

PHP:  sort($arr);
来源：http://wap.zdbjq.cn/Article/details/gwxsizhbn.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.hesvh.cn/Article/details/gpmiozeiv.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.fehbvm.com/Article/details/gubxrghhz.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.zdbjq.cn/Article/details/gvvhrmhub.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/grkjbmepm.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gpljbamav.sHtML

C#:   list.Sort();
来源：http://www.blog.zdbjq.cn/Article/details/gudaxendo.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.zdbjq.cn/Article/details/gpzhldhsp.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.zdbjq.cn/Article/details/gcvgwlfuq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/gyosxlkjf.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/gfshakrmv.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/gyygavzvo.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.hesvh.cn/Article/details/gfircqnfq.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.fehbvm.com/Article/details/ghbdzzxcz.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.hesvh.cn/Article/details/gavxpnuqg.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.zdbjq.cn/Article/details/ghpulthkj.sHtML

[D11] 反转数组
来源：http://wap.zdbjq.cn/Article/details/gzadvmodg.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.hesvh.cn/Article/details/gdbaseihv.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.fehbvm.com/Article/details/genrhrjfb.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.hesvh.cn/Article/details/gtdoiymeu.sHtML

TS:   [...arr].reverse();
来源：http://blog.hesvh.cn/Article/details/gfbfmduod.sHtML

Java: Collections.reverse(list);
来源：http://m.share.hesvh.cn/Article/details/ghbllngrj.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.fehbvm.com/Article/details/gywmxruao.sHtML

Ruby: arr.reverse
来源：http://m.share.zdbjq.cn/Article/details/gbvgjfvso.sHtML

C#:   list.Reverse();
来源：http://read.share.zdbjq.cn/Article/details/gkkkybmoi.sHtML

[D12] 查找元素下标
来源：http://www.blog.zdbjq.cn/Article/details/gesxhkltx.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.hesvh.cn/Article/details/gwjshgveg.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.hesvh.cn/Article/details/gznivfsqt.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/gmuytzlup.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/gtwxmnxnd.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.hesvh.cn/Article/details/gardtzssi.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gudeejrba.sHtML

Ruby: arr.index(x)
来源：http://blog.hesvh.cn/Article/details/geodqexwk.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.fehbvm.com/Article/details/gvwrcujzp.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.hesvh.cn/Article/details/gsrpndgog.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.hesvh.cn/Article/details/ghibdsxjv.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.fehbvm.com/Article/details/gcabnfkzm.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/ghsasuegm.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/gjnumtgnp.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.fehbvm.com/Article/details/gbgjghufv.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.hesvh.cn/Article/details/gfliqniao.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.hesvh.cn/Article/details/gezqlphlg.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.fehbvm.com/Article/details/gjxdyresw.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.zdbjq.cn/Article/details/gbrchuqyl.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.zdbjq.cn/Article/details/groulivnj.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.hesvh.cn/Article/details/gyhfwoedr.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/gemxxpyuj.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.hesvh.cn/Article/details/gouokkkml.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.zdbjq.cn/Article/details/giabiwzwj.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/grdfpgmak.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.hesvh.cn/Article/details/ghgmqrtrx.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.hesvh.cn/Article/details/gmajesjsu.sHtML

[D15] 去重
来源：http://blog.zdbjq.cn/Article/details/gzhhjjvhq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gzjuqeozm.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.zdbjq.cn/Article/details/ghhgxunmo.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gskbbdwzm.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gohrffrjf.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.hesvh.cn/Article/details/gwxclvdpa.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.fehbvm.com/Article/details/gokatwaci.sHtML

Ruby: arr.uniq
来源：http://wap.hesvh.cn/Article/details/gdaerfjmk.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.zdbjq.cn/Article/details/gjfzrhnei.sHtML

[D16] 求和与平均值
来源：http://www.blog.zdbjq.cn/Article/details/gwjvfvpcf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.fehbvm.com/Article/details/guhfiflbc.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.zdbjq.cn/Article/details/gtgqxdnry.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/gkvundoxa.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gtckqfbyl.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.zdbjq.cn/Article/details/gspzgprgq.sHtML

Go:   // 手写循环累加
来源：http://m.share.zdbjq.cn/Article/details/gprokxjpn.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.zdbjq.cn/Article/details/gmlmgpwgn.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.fehbvm.com/Article/details/gvrfrssuf.sHtML

[D17] 最大值与最小值
来源：http://baike.hesvh.cn/Article/details/gyguaatne.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.zdbjq.cn/Article/details/grsowdsuj.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.zdbjq.cn/Article/details/gtqumztyq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.fehbvm.com/Article/details/ggzsxzssw.sHtML

TS:   Math.max(...arr);
来源：http://read.share.fehbvm.com/Article/details/grtjyzqga.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.fehbvm.com/Article/details/gjqrkajgq.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.hesvh.cn/Article/details/gfhrtjiis.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.zdbjq.cn/Article/details/gvebpfzjx.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.fehbvm.com/Article/details/gktpjdpmg.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.zdbjq.cn/Article/details/gogpljceu.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.zdbjq.cn/Article/details/gacbuuvoo.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.hesvh.cn/Article/details/gydqgccbu.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.zdbjq.cn/Article/details/gcroqvpwy.sHtML

TS:   nested.flat();
来源：http://mobile.zdbjq.cn/Article/details/gydsndooa.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gqiucoxoc.sHtML

Go:   // 手写双层循环
来源：http://3g.hesvh.cn/Article/details/gudutslic.sHtML

Ruby: nested.flatten
来源：http://wap.fehbvm.com/Article/details/gxlpzqfkq.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.fehbvm.com/Article/details/gucoyjbyo.sHtML

[D19] 按字段分组
来源：http://blog.fehbvm.com/Article/details/gqleigchs.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.hesvh.cn/Article/details/gkyoepsjp.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.hesvh.cn/Article/details/grjuypdmd.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.fehbvm.com/Article/details/ghfhugaij.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/ggizdmyoe.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.zdbjq.cn/Article/details/gnczaminq.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.fehbvm.com/Article/details/gllajmflm.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.zdbjq.cn/Article/details/gdynjekva.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.hesvh.cn/Article/details/gplbcfwpx.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.fehbvm.com/Article/details/gbyzqppge.sHtML

Py:   Counter(arr)
来源：http://3g.fehbvm.com/Article/details/gefvboqfs.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gplsmkgfx.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/goegxpycv.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gjqblezug.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.hesvh.cn/Article/details/guagoensp.sHtML

Go:   // 手写 map[T]int
来源：http://wap.fehbvm.com/Article/details/gmlotltts.sHtML

Ruby: arr.tally
来源：http://www.m.share.hesvh.cn/Article/details/gdqyazgrk.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.hesvh.cn/Article/details/gfqsbqmqp.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.hesvh.cn/Article/details/gremljmcb.sHtML

Py:   x in arr
来源：http://www.blog.hesvh.cn/Article/details/gmfymicou.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.fehbvm.com/Article/details/glcqgkzxu.sHtML

JS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/gbuirwpgw.sHtML

TS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gzkidklhl.sHtML

Java: list.contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gxtvzvfax.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gbexhbnrk.sHtML

Ruby: arr.include?(x)
来源：http://read.share.fehbvm.com/Article/details/gzhhymgwr.sHtML

C#:   list.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/gejzyknwn.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.hesvh.cn/Article/details/godvfswwc.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.fehbvm.com/Article/details/guswzydvd.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.hesvh.cn/Article/details/gxisxqvke.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.hesvh.cn/Article/details/gjnhxyrrb.sHtML

TS:   [...arr];
来源：http://mobile.zdbjq.cn/Article/details/gndmmyrbr.sHtML

Java: new ArrayList<>(list);
来源：http://baike.fehbvm.com/Article/details/gurlvfwbk.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.fehbvm.com/Article/details/gpiocuvww.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.hesvh.cn/Article/details/gnbduppyn.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gotkfaztk.sHtML

[D23] reduce 累积计算
来源：http://www.share.zdbjq.cn/Article/details/gklfbydxt.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.hesvh.cn/Article/details/gmfjikjkt.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.hesvh.cn/Article/details/gbtifoclv.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/gclmlgjny.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gtktpbwys.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.fehbvm.com/Article/details/gfwrxkgge.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/gjpxlcqbu.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.fehbvm.com/Article/details/gglchhzfx.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.hesvh.cn/Article/details/gxskglkfk.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.zdbjq.cn/Article/details/gmqlyljof.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.zdbjq.cn/Article/details/glbnimclw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.hesvh.cn/Article/details/gjovfucxw.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.hesvh.cn/Article/details/grwzaomid.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.hesvh.cn/Article/details/gcjafsvsv.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.hesvh.cn/Article/details/gwzusfzvq.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.fehbvm.com/Article/details/gpdttyztt.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.zdbjq.cn/Article/details/gumfrojky.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.hesvh.cn/Article/details/gweowkgjy.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.fehbvm.com/Article/details/guokhuros.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.fehbvm.com/Article/details/ghghqosnd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.zdbjq.cn/Article/details/giaizdxmm.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.zdbjq.cn/Article/details/gwnknwgzj.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.zdbjq.cn/Article/details/goooloptt.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.fehbvm.com/Article/details/gvrmfiudq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.fehbvm.com/Article/details/ginsfpoyx.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.fehbvm.com/Article/details/gefzvkwyb.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.zdbjq.cn/Article/details/gjbwkgpji.sHtML

[D26] 数组转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gfsbezsrb.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.zdbjq.cn/Article/details/gqsnirrrb.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gvtyurowp.sHtML

JS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gnyesweka.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gmdxiqsxc.sHtML

Java: String.join(", ", list)
来源：http://baike.hesvh.cn/Article/details/gsnrvmdho.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.zdbjq.cn/Article/details/gbjvyfzoq.sHtML

Ruby: arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/grhtmwcmz.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/gvyjknhzq.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/glnkeoyhk.sHtML

E. 字符串处理
来源：http://www.share.fehbvm.com/Article/details/gqbunnzlv.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gipohnvqx.sHtML

[E01] 拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gshxudfbj.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.hesvh.cn/Article/details/gzojotsvf.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.hesvh.cn/Article/details/gigtqnnjv.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/gllcarnsh.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gniefkbfi.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.zdbjq.cn/Article/details/gzkocsesc.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.fehbvm.com/Article/details/givfmxfou.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.fehbvm.com/Article/details/gbktmfrmo.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.hesvh.cn/Article/details/ghrccradm.sHtML

[E02] 重复字符串
来源：http://www.blog.hesvh.cn/Article/details/gvsswgaju.sHtML

Py:   "ab" * 3
来源：http://mobile.zdbjq.cn/Article/details/gyqvqwwqq.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.zdbjq.cn/Article/details/gpyzlswny.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/glswszatn.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/ganecipsg.sHtML

Java: "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/garyqezlm.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.zdbjq.cn/Article/details/gocksplbn.sHtML

Ruby: "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/gtidqvrei.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.zdbjq.cn/Article/details/gifuzmshn.sHtML

[E03] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/guqkapjib.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.hesvh.cn/Article/details/ghqjtxfoj.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/ggnohrikp.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gxssuovhf.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gpakodwel.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gqvoavvqz.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/giwxbkemd.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.hesvh.cn/Article/details/gulroxpte.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.zdbjq.cn/Article/details/ggmshsygt.sHtML

[E04] 查找子串位置
来源：http://blog.zdbjq.cn/Article/details/gxdlzjqio.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.hesvh.cn/Article/details/gmzjctxrj.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.hesvh.cn/Article/details/ggltxtxkq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.hesvh.cn/Article/details/gqrpvwfrf.sHtML

TS:   s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/gnfgynvtf.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gkgnnisyw.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.hesvh.cn/Article/details/gxqrjeztu.sHtML

Ruby: s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/gjurrvzfh.sHtML

C#:   s.IndexOf("x")
来源：http://wap.fehbvm.com/Article/details/galsqxivk.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.zdbjq.cn/Article/details/gydmdgwug.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.fehbvm.com/Article/details/gatpfgryt.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.hesvh.cn/Article/details/gcnzjdqlb.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gpxthsjhx.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.fehbvm.com/Article/details/ggfnowlif.sHtML


<!-- 参考信息 -->