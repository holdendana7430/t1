代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.hesvh.cn/Article/details/gyqtgidce.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.zdbjq.cn/Article/details/gmqsswsxw.sHtML

Java: // 无解构
来源：http://blog.fehbvm.com/Article/details/gcdptpbhs.sHtML

Go:   // 无解构
来源：http://baike.zdbjq.cn/Article/details/gjeojrjts.sHtML

Ruby: a, b = pair
来源：http://baike.hesvh.cn/Article/details/ggbagwnvh.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.zdbjq.cn/Article/details/giwltnoyh.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.zdbjq.cn/Article/details/gxksublbm.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.zdbjq.cn/Article/details/goznpfmhv.sHtML

PHP:  // 无重载
来源：http://m.share.zdbjq.cn/Article/details/ghxcrjdvh.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.fehbvm.com/Article/details/gcdxbqyqg.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.zdbjq.cn/Article/details/gpmaqseof.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.zdbjq.cn/Article/details/gljfmbwgx.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.hesvh.cn/Article/details/glcfgttja.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.zdbjq.cn/Article/details/gygkwwlzh.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fehbvm.com/Article/details/gccqmdhpg.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/graiizcbl.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.zdbjq.cn/Article/details/gkaxrckda.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ggvnagaul.sHtML

[D01] 创建数组 / 列表
来源：http://blog.hesvh.cn/Article/details/ggupxzrtc.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.zdbjq.cn/Article/details/gvjdscgll.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.hesvh.cn/Article/details/gviducycb.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.zdbjq.cn/Article/details/gyrtihcyd.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.hesvh.cn/Article/details/ghicjmebi.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.hesvh.cn/Article/details/gpdizawrj.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.zdbjq.cn/Article/details/gdgxomqqz.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.fehbvm.com/Article/details/gdfefrmhn.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.fehbvm.com/Article/details/gcfjcvten.sHtML

[D02] 追加元素到末尾
来源：http://3g.zdbjq.cn/Article/details/gmvhwzrgn.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.fehbvm.com/Article/details/gymeaxbuc.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.fehbvm.com/Article/details/glwcvpfjr.sHtML

JS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/gognslnuw.sHtML

TS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/gnhrmdvpo.sHtML

Java: list.add(4);
来源：http://blog.hesvh.cn/Article/details/gndtqeiyx.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.fehbvm.com/Article/details/grzxkywxg.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.fehbvm.com/Article/details/gloidbitu.sHtML

C#:   list.Add(4);
来源：http://3g.zdbjq.cn/Article/details/gcnziiwbl.sHtML

[D03] 在指定位置插入元素
来源：http://baike.fehbvm.com/Article/details/gzvugduvc.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.zdbjq.cn/Article/details/ginetiuqs.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.hesvh.cn/Article/details/goknrvina.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.fehbvm.com/Article/details/ghjisbajs.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.zdbjq.cn/Article/details/gsdfrwvht.sHtML

Java: list.add(0, 0);
来源：http://mobile.zdbjq.cn/Article/details/ggetstwpo.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.fehbvm.com/Article/details/gilhnbqyk.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.zdbjq.cn/Article/details/gzogypypc.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.fehbvm.com/Article/details/ghwusquqh.sHtML

[D04] 删除元素
来源：http://read.share.hesvh.cn/Article/details/gebvkhtrb.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.hesvh.cn/Article/details/glfqbuhaq.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.hesvh.cn/Article/details/gtzqhoywb.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.zdbjq.cn/Article/details/gpvzjrzbv.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.zdbjq.cn/Article/details/ghzlqykna.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.hesvh.cn/Article/details/gfynjomnx.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.fehbvm.com/Article/details/ggxkbwldx.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.hesvh.cn/Article/details/gfjonymwc.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.fehbvm.com/Article/details/gzqjoxfaq.sHtML

[D05] 访问与修改元素
来源：http://3g.fehbvm.com/Article/details/ghtnwhexx.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gsdchenqi.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/guizeazzz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/ggsnewhoa.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.hesvh.cn/Article/details/gmlgioaow.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.fehbvm.com/Article/details/gglosdyjt.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gnrxgavng.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/glhgxstwy.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gbmhdaozw.sHtML

[D06] 数组长度
来源：http://wap.zdbjq.cn/Article/details/gqpvmtubn.sHtML

Py:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gxtwsqqvt.sHtML

PHP:  count($arr);
来源：http://m.share.hesvh.cn/Article/details/gashcmwfh.sHtML

JS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gpblaoikl.sHtML

TS:   arr.length
来源：http://wap.fehbvm.com/Article/details/gaaokzumb.sHtML

Java: list.size();
来源：http://www.m.share.fehbvm.com/Article/details/ggqmiefmu.sHtML

Go:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gjxinpmiq.sHtML

Ruby: arr.length; arr.size
来源：http://wap.fehbvm.com/Article/details/gihecpfqu.sHtML

C#:   list.Count;
来源：http://m.share.fehbvm.com/Article/details/gjzcvbfjn.sHtML

[D07] 切片 / 取子数组
来源：http://baike.hesvh.cn/Article/details/gjdrizvbw.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.hesvh.cn/Article/details/gozlizxje.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gonxuscei.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/glxxhxbif.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gsrlpnxwy.sHtML

Java: list.subList(1, 4);
来源：http://wap.hesvh.cn/Article/details/gfbukuhbq.sHtML

Go:   arr[1:4]
来源：http://www.share.hesvh.cn/Article/details/gzrczvnlm.sHtML

Ruby: arr[1, 3]
来源：http://3g.hesvh.cn/Article/details/gecdbiuik.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.fehbvm.com/Article/details/gknzosyop.sHtML

[D08] 合并两个数组
来源：http://www.share.zdbjq.cn/Article/details/gpriuufxm.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.zdbjq.cn/Article/details/gcsmwetay.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.fehbvm.com/Article/details/gxzannjzs.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.zdbjq.cn/Article/details/gikrnwfpw.sHtML

TS:   [...a, ...b];
来源：http://m.share.zdbjq.cn/Article/details/gquvnrmzb.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.fehbvm.com/Article/details/grggluakj.sHtML

Go:   append(a, b...)
来源：http://wap.hesvh.cn/Article/details/gsioyswbf.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fehbvm.com/Article/details/gzxndpzgt.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.hesvh.cn/Article/details/ghujlnyuo.sHtML

[D09] 排序（升序）
来源：http://mobile.zdbjq.cn/Article/details/gronfwzqj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/ghjsjyjnw.sHtML

PHP:  sort($arr);
来源：http://www.share.fehbvm.com/Article/details/goppzcqxn.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.zdbjq.cn/Article/details/gibdindbe.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.fehbvm.com/Article/details/gpswuulca.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.fehbvm.com/Article/details/glnaaafst.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gamhcrama.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/ghpmtsjmr.sHtML

C#:   list.Sort();
来源：http://www.m.share.hesvh.cn/Article/details/gsngzkxco.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.hesvh.cn/Article/details/gwcdzapis.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.hesvh.cn/Article/details/gkotwwhth.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/gagbfkcpp.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/gxynvbpsm.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/ghvocovfs.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.hesvh.cn/Article/details/gstwtmkbz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.hesvh.cn/Article/details/ggossfzml.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.fehbvm.com/Article/details/gknaeklun.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.hesvh.cn/Article/details/ggaybfghw.sHtML

[D11] 反转数组
来源：http://www.blog.fehbvm.com/Article/details/gqtlqkfjx.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.fehbvm.com/Article/details/gaylqbftg.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.fehbvm.com/Article/details/gvirqctnf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.zdbjq.cn/Article/details/gqqcbpzds.sHtML

TS:   [...arr].reverse();
来源：http://www.share.zdbjq.cn/Article/details/guturiarc.sHtML

Java: Collections.reverse(list);
来源：http://baike.fehbvm.com/Article/details/gpirqtizo.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gcoakmdhz.sHtML

Ruby: arr.reverse
来源：http://baike.hesvh.cn/Article/details/gtovsblwz.sHtML

C#:   list.Reverse();
来源：http://www.blog.zdbjq.cn/Article/details/gjreajxaa.sHtML

[D12] 查找元素下标
来源：http://m.share.hesvh.cn/Article/details/gzwzkrfja.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.fehbvm.com/Article/details/glmsousez.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.zdbjq.cn/Article/details/gjjvrgeiu.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/gcviynqdw.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/glauwqzgg.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.zdbjq.cn/Article/details/glvuhzpif.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gtorfrhot.sHtML

Ruby: arr.index(x)
来源：http://blog.fehbvm.com/Article/details/ghjfxjcgn.sHtML

C#:   list.IndexOf(x);
来源：http://3g.fehbvm.com/Article/details/gdwqndczb.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.hesvh.cn/Article/details/gqtqsepxr.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.hesvh.cn/Article/details/gtfowpzoa.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.fehbvm.com/Article/details/gfgckirba.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gzuccahjz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/gtvaegnwq.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.hesvh.cn/Article/details/gobinygyr.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.hesvh.cn/Article/details/gwtqzzyer.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.fehbvm.com/Article/details/gtpjabnxk.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.hesvh.cn/Article/details/gsufooqkt.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.hesvh.cn/Article/details/gyfmkvuxu.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.hesvh.cn/Article/details/gjirttwyr.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.zdbjq.cn/Article/details/gcywicvgz.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/grxoudmcs.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/getltrhfx.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.hesvh.cn/Article/details/geypmzpjr.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/gysetztqv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.fehbvm.com/Article/details/gmihdknpk.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fehbvm.com/Article/details/gilgdcpgu.sHtML

[D15] 去重
来源：http://mobile.fehbvm.com/Article/details/gtgszlhat.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/goxxbsbts.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gjahvlnvt.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gsjodiqst.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/guyykcibl.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.hesvh.cn/Article/details/gbexelmlo.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.hesvh.cn/Article/details/gyvskureh.sHtML

Ruby: arr.uniq
来源：http://blog.hesvh.cn/Article/details/giuqmyoug.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.fehbvm.com/Article/details/grdnowmhc.sHtML

[D16] 求和与平均值
来源：http://baike.zdbjq.cn/Article/details/gdaaiwoky.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.hesvh.cn/Article/details/gnixlnwgf.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.fehbvm.com/Article/details/gssywofmj.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/gguyljzhb.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/gzddvhjue.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.zdbjq.cn/Article/details/guqojadtg.sHtML

Go:   // 手写循环累加
来源：http://wap.hesvh.cn/Article/details/gqgcookpy.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.hesvh.cn/Article/details/gwcqthsqp.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.hesvh.cn/Article/details/gulnrblte.sHtML

[D17] 最大值与最小值
来源：http://www.share.hesvh.cn/Article/details/gghqnvznl.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.hesvh.cn/Article/details/gambmkhyg.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gctsiaufs.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.zdbjq.cn/Article/details/glajrvagx.sHtML

TS:   Math.max(...arr);
来源：http://mobile.hesvh.cn/Article/details/gzrlckgcw.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.fehbvm.com/Article/details/gasrnoesj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.zdbjq.cn/Article/details/ggskhtbdn.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.hesvh.cn/Article/details/gowqnvwzc.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.hesvh.cn/Article/details/gpblnjceu.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.zdbjq.cn/Article/details/gxjbddacv.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.fehbvm.com/Article/details/gqtjrwjtt.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.fehbvm.com/Article/details/gffuxlynw.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.fehbvm.com/Article/details/gujalxkyk.sHtML

TS:   nested.flat();
来源：http://m.share.fehbvm.com/Article/details/gbuuojngh.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.zdbjq.cn/Article/details/glnibhvox.sHtML

Go:   // 手写双层循环
来源：http://www.share.hesvh.cn/Article/details/gjkvpaidu.sHtML

Ruby: nested.flatten
来源：http://3g.hesvh.cn/Article/details/gabeuyyhj.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.fehbvm.com/Article/details/gwedmxqej.sHtML

[D19] 按字段分组
来源：http://www.blog.hesvh.cn/Article/details/gqefpxwvu.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.hesvh.cn/Article/details/goflfhbuv.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.fehbvm.com/Article/details/gedhjlvfh.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.hesvh.cn/Article/details/ghgqscuxo.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.hesvh.cn/Article/details/gcbdzeffr.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.hesvh.cn/Article/details/gfriuuwyt.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.hesvh.cn/Article/details/gvcijwkbx.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.fehbvm.com/Article/details/gomtwswgw.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.hesvh.cn/Article/details/gqnrvpjkp.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.zdbjq.cn/Article/details/ghdijofyu.sHtML

Py:   Counter(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/giwuoqhqg.sHtML

PHP:  array_count_values($arr);
来源：http://wap.hesvh.cn/Article/details/gxrzqdkei.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gzhykgtkt.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/gsevyepgr.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.fehbvm.com/Article/details/gtoruhbau.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.hesvh.cn/Article/details/gvrjrehoq.sHtML

Ruby: arr.tally
来源：http://mobile.fehbvm.com/Article/details/gvocubdlt.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.fehbvm.com/Article/details/glubmqxnw.sHtML

[D21] 判断是否包含某元素
来源：http://wap.zdbjq.cn/Article/details/glykjortf.sHtML

Py:   x in arr
来源：http://www.blog.fehbvm.com/Article/details/gjdbngmfw.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.fehbvm.com/Article/details/giysnqlxo.sHtML

JS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/gymbtuiqz.sHtML

TS:   arr.includes(x)
来源：http://read.share.hesvh.cn/Article/details/glwelvaqj.sHtML

Java: list.contains(x)
来源：http://read.share.fehbvm.com/Article/details/gzjfnhmya.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gevrbbxop.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.hesvh.cn/Article/details/gbljlyplg.sHtML

C#:   list.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gkorkljck.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.fehbvm.com/Article/details/gsekqgqhd.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.hesvh.cn/Article/details/giseplitk.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.zdbjq.cn/Article/details/givcmsykl.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.fehbvm.com/Article/details/giekzqxmq.sHtML

TS:   [...arr];
来源：http://wap.hesvh.cn/Article/details/gcufutwbm.sHtML

Java: new ArrayList<>(list);
来源：http://baike.hesvh.cn/Article/details/gsoorbvma.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gzyfmnzez.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.hesvh.cn/Article/details/gipsrrhfq.sHtML

C#:   new List<int>(list);
来源：http://mobile.hesvh.cn/Article/details/gqocacijh.sHtML

[D23] reduce 累积计算
来源：http://read.share.zdbjq.cn/Article/details/glziclbfq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.hesvh.cn/Article/details/gjeuyuoxp.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.hesvh.cn/Article/details/gtcubsveo.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gbweiypji.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/gdbwgpfhz.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.fehbvm.com/Article/details/gvdgnfcvo.sHtML

Go:   // 手写循环
来源：http://blog.hesvh.cn/Article/details/gcxrfjlnv.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.fehbvm.com/Article/details/gzubppntz.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.hesvh.cn/Article/details/gpzkhqiwv.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.zdbjq.cn/Article/details/gcjkcjgtc.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.hesvh.cn/Article/details/gjdbvfvcw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.fehbvm.com/Article/details/gtrdhjtuo.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.fehbvm.com/Article/details/gvjjeowhf.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/georucwkz.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.zdbjq.cn/Article/details/guhxiyqqz.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.fehbvm.com/Article/details/gsrjgacwu.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.fehbvm.com/Article/details/ggyryyjyp.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.hesvh.cn/Article/details/gqjmoawkn.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.fehbvm.com/Article/details/ggpypwdzb.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.hesvh.cn/Article/details/gwzyrfuwv.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.fehbvm.com/Article/details/guazzboto.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.fehbvm.com/Article/details/gewxyyvsn.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.hesvh.cn/Article/details/grhdddsne.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.fehbvm.com/Article/details/gkxwjmsty.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.hesvh.cn/Article/details/gygllwfbq.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.fehbvm.com/Article/details/gxflazszm.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.zdbjq.cn/Article/details/ghznzhklk.sHtML

[D26] 数组转字符串
来源：http://www.share.fehbvm.com/Article/details/gjnkiqakn.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.fehbvm.com/Article/details/girbtarkb.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.zdbjq.cn/Article/details/gxzebrrgw.sHtML

JS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gwsmjirfe.sHtML

TS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/ggwhzmovl.sHtML

Java: String.join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/gnucybrch.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gwofprspm.sHtML

Ruby: arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gickiqheb.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/gjfnrohyz.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gqbstipvr.sHtML

E. 字符串处理
来源：http://wap.zdbjq.cn/Article/details/grxktmdji.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gmzrmiopz.sHtML

[E01] 拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gtzinlzdc.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.zdbjq.cn/Article/details/ghykemrqb.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.hesvh.cn/Article/details/gixqzzcoj.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/gxnqlzxhq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/gvzqmtkdo.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.hesvh.cn/Article/details/gzotahwuf.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.fehbvm.com/Article/details/gisumeytd.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.hesvh.cn/Article/details/gxhrrfkuz.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/glzmufbgm.sHtML

[E02] 重复字符串
来源：http://blog.fehbvm.com/Article/details/gvxrklchh.sHtML

Py:   "ab" * 3
来源：http://baike.hesvh.cn/Article/details/gklcfgavt.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.hesvh.cn/Article/details/glsudywwq.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/ggasolfeu.sHtML

TS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gbbvsruvo.sHtML

Java: "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gqjohkgeh.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.fehbvm.com/Article/details/glayvpaor.sHtML

Ruby: "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gwnraaoqk.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.hesvh.cn/Article/details/gjfntvutq.sHtML

[E03] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/gnpqxhvvv.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.zdbjq.cn/Article/details/gtwmgzlih.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gnlpkpmpw.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/grewyfxpx.sHtML

TS:   s.slice(1, 4)
来源：http://blog.hesvh.cn/Article/details/gufxnasst.sHtML

Java: s.substring(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gxdvnmyxl.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.zdbjq.cn/Article/details/gdsfkjgad.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.zdbjq.cn/Article/details/gruougkom.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.fehbvm.com/Article/details/gpueznjuh.sHtML

[E04] 查找子串位置
来源：http://baike.fehbvm.com/Article/details/gomgwxwlg.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.fehbvm.com/Article/details/gvgtsnxhd.sHtML

PHP:  strpos($s, "x");
来源：http://baike.zdbjq.cn/Article/details/gnyvpbgla.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.fehbvm.com/Article/details/gkbnovzeh.sHtML

TS:   s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/goqxfxwuy.sHtML

Java: s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gmwxbtsjz.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.fehbvm.com/Article/details/ggkqrbxdl.sHtML

Ruby: s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gymibedfo.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gdvnzofrr.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.hesvh.cn/Article/details/guuhonisr.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gsgtlzkaw.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.hesvh.cn/Article/details/gpjfvxeuo.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gynwdzbiw.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.fehbvm.com/Article/details/goujafiil.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gdmjqnejs.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.hesvh.cn/Article/details/gwwqxtlfe.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.hesvh.cn/Article/details/gxepxkedj.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gnrijhouq.sHtML


<!-- 参考信息 -->