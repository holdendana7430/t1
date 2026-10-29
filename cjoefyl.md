代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gwgfrlblb.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.hesvh.cn/Article/details/gytqwikkd.sHtML

Java: // 无解构
来源：http://read.share.fehbvm.com/Article/details/gdhvuabqg.sHtML

Go:   // 无解构
来源：http://www.blog.hesvh.cn/Article/details/gxiwqvlbl.sHtML

Ruby: a, b = pair
来源：http://www.blog.zdbjq.cn/Article/details/gkmpehcqc.sHtML

C#:   var (a, b) = pair;
来源：http://3g.hesvh.cn/Article/details/gfukstior.sHtML

[C16] 函数 / 方法重载
来源：http://blog.fehbvm.com/Article/details/gyxowisad.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.fehbvm.com/Article/details/ganebrdka.sHtML

PHP:  // 无重载
来源：http://baike.zdbjq.cn/Article/details/grcyzvfhm.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.hesvh.cn/Article/details/gdvgepakf.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.zdbjq.cn/Article/details/glegkqhrc.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.fehbvm.com/Article/details/ghjoiofzy.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.fehbvm.com/Article/details/gezjsskcr.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.fehbvm.com/Article/details/grkyforzv.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.hesvh.cn/Article/details/guyeugwku.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gpfkonxst.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.hesvh.cn/Article/details/gkasbqgbh.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gnjxdltof.sHtML

[D01] 创建数组 / 列表
来源：http://baike.fehbvm.com/Article/details/gzbjfmoah.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.fehbvm.com/Article/details/glzaxswjx.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.fehbvm.com/Article/details/gqtgdkocj.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.fehbvm.com/Article/details/gjzcrnane.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.hesvh.cn/Article/details/gykdxnyht.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.fehbvm.com/Article/details/gluekagux.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.zdbjq.cn/Article/details/ghecrqygr.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.fehbvm.com/Article/details/gpdhkebgf.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.fehbvm.com/Article/details/gshwzadti.sHtML

[D02] 追加元素到末尾
来源：http://mobile.zdbjq.cn/Article/details/giwixaeow.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.hesvh.cn/Article/details/gfhjkckqq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.fehbvm.com/Article/details/gmvzcomgv.sHtML

JS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/grhebwkff.sHtML

TS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gvatfcmra.sHtML

Java: list.add(4);
来源：http://wap.zdbjq.cn/Article/details/gvjwnxxwy.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.hesvh.cn/Article/details/ghgqoyrek.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.zdbjq.cn/Article/details/gkbjdqidf.sHtML

C#:   list.Add(4);
来源：http://3g.fehbvm.com/Article/details/gxqlthcyh.sHtML

[D03] 在指定位置插入元素
来源：http://wap.fehbvm.com/Article/details/gmjjnizmt.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.fehbvm.com/Article/details/gbtbtjwoz.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.zdbjq.cn/Article/details/gatzfmxqh.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.zdbjq.cn/Article/details/gvzjsieij.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gsntzwlgv.sHtML

Java: list.add(0, 0);
来源：http://baike.hesvh.cn/Article/details/gyodqxfpl.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.fehbvm.com/Article/details/grcwwfyup.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.zdbjq.cn/Article/details/gepszajth.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gbnlpmqra.sHtML

[D04] 删除元素
来源：http://read.share.zdbjq.cn/Article/details/gkihhpoth.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.zdbjq.cn/Article/details/gkkqxtbdf.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.hesvh.cn/Article/details/gipwlimqc.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.zdbjq.cn/Article/details/gleqtuypo.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.hesvh.cn/Article/details/glluuusll.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.zdbjq.cn/Article/details/guobqgvsr.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.zdbjq.cn/Article/details/gnlsqhkhf.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.hesvh.cn/Article/details/gmajmctgb.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.hesvh.cn/Article/details/gpfdonyvq.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.hesvh.cn/Article/details/gzbqbtepi.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gyzmaohoh.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/goquvhkmf.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gkeagdhpk.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.fehbvm.com/Article/details/gwfxwxsub.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.hesvh.cn/Article/details/gdjtctuww.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gtfkkczmx.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gyniltmuz.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.fehbvm.com/Article/details/grpjkkvys.sHtML

[D06] 数组长度
来源：http://mobile.fehbvm.com/Article/details/guqyddjhi.sHtML

Py:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gfxnwkjla.sHtML

PHP:  count($arr);
来源：http://m.share.zdbjq.cn/Article/details/gadnwefii.sHtML

JS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/gnwytasfk.sHtML

TS:   arr.length
来源：http://3g.fehbvm.com/Article/details/grkglswvh.sHtML

Java: list.size();
来源：http://baike.zdbjq.cn/Article/details/gwadstaug.sHtML

Go:   len(arr)
来源：http://blog.hesvh.cn/Article/details/gtgyfhxph.sHtML

Ruby: arr.length; arr.size
来源：http://3g.zdbjq.cn/Article/details/gvmykbrpt.sHtML

C#:   list.Count;
来源：http://read.share.zdbjq.cn/Article/details/gunkdvlzl.sHtML

[D07] 切片 / 取子数组
来源：http://3g.hesvh.cn/Article/details/gixqeyjht.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.hesvh.cn/Article/details/gbklxshvg.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.fehbvm.com/Article/details/gemhmbnpx.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/gilrpswhp.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gqugcztbp.sHtML

Java: list.subList(1, 4);
来源：http://wap.hesvh.cn/Article/details/gunidscfg.sHtML

Go:   arr[1:4]
来源：http://baike.hesvh.cn/Article/details/gexrtebcc.sHtML

Ruby: arr[1, 3]
来源：http://read.share.fehbvm.com/Article/details/gtinexwea.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.hesvh.cn/Article/details/gogxeebki.sHtML

[D08] 合并两个数组
来源：http://read.share.zdbjq.cn/Article/details/gnsfvhefr.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.fehbvm.com/Article/details/gspjoduwq.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.hesvh.cn/Article/details/gmcmwyozw.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.hesvh.cn/Article/details/gzacccjen.sHtML

TS:   [...a, ...b];
来源：http://mobile.fehbvm.com/Article/details/gzomkecxn.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.zdbjq.cn/Article/details/gfklarpzp.sHtML

Go:   append(a, b...)
来源：http://mobile.hesvh.cn/Article/details/ghgoauigx.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.hesvh.cn/Article/details/gcixiklos.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.zdbjq.cn/Article/details/gvdyqynfi.sHtML

[D09] 排序（升序）
来源：http://baike.hesvh.cn/Article/details/gdlorvigi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/gekbbasne.sHtML

PHP:  sort($arr);
来源：http://wap.fehbvm.com/Article/details/gfxdcnpcw.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.fehbvm.com/Article/details/ghkdrhepo.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.hesvh.cn/Article/details/gadspvftw.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.fehbvm.com/Article/details/gcclgzqqk.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/glifxygqm.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/gevcnrcpp.sHtML

C#:   list.Sort();
来源：http://www.share.fehbvm.com/Article/details/ggddovuva.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.zdbjq.cn/Article/details/gzwajpswn.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.fehbvm.com/Article/details/gtigxbdqh.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gcnojghtt.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/gqrrkbrxy.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gaxmvyjsk.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.zdbjq.cn/Article/details/ghqpvxxiz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.fehbvm.com/Article/details/glrluvfum.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.fehbvm.com/Article/details/gdtyxunta.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.fehbvm.com/Article/details/gzbngxeyq.sHtML

[D11] 反转数组
来源：http://read.share.hesvh.cn/Article/details/gbybizmxn.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.hesvh.cn/Article/details/ghgkenzda.sHtML

PHP:  array_reverse($arr);
来源：http://wap.hesvh.cn/Article/details/gxokzoikx.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.fehbvm.com/Article/details/gatqpdbkh.sHtML

TS:   [...arr].reverse();
来源：http://read.share.zdbjq.cn/Article/details/ghvwffmvu.sHtML

Java: Collections.reverse(list);
来源：http://blog.hesvh.cn/Article/details/gckoljgdf.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.fehbvm.com/Article/details/gbhybvytx.sHtML

Ruby: arr.reverse
来源：http://blog.hesvh.cn/Article/details/goikovjvp.sHtML

C#:   list.Reverse();
来源：http://blog.hesvh.cn/Article/details/gpfgakqhu.sHtML

[D12] 查找元素下标
来源：http://m.share.fehbvm.com/Article/details/gilqhrxlg.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.hesvh.cn/Article/details/gzkocaoco.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.zdbjq.cn/Article/details/gkvrguwgk.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/gznhcewgh.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/gmdvvrkdz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.zdbjq.cn/Article/details/gthfdecih.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gdzumbzet.sHtML

Ruby: arr.index(x)
来源：http://read.share.hesvh.cn/Article/details/gnhunyxbf.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.fehbvm.com/Article/details/gmlootrru.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.zdbjq.cn/Article/details/gwmkhpvce.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.hesvh.cn/Article/details/gfkbonbqi.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.hesvh.cn/Article/details/gmkihqihm.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gvattjkbf.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/geoxeyarl.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.zdbjq.cn/Article/details/gqoeudspd.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.fehbvm.com/Article/details/getorxvzq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.zdbjq.cn/Article/details/gqngdldhw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.hesvh.cn/Article/details/gtdsdcayj.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.fehbvm.com/Article/details/gujqepuzc.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.hesvh.cn/Article/details/gbxttcdqf.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.fehbvm.com/Article/details/gbwfhxziq.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/ggsrqkjxe.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.hesvh.cn/Article/details/gscpylzvd.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.hesvh.cn/Article/details/gkcgqcbdm.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/glfuyhaip.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.fehbvm.com/Article/details/gddpiicqx.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.fehbvm.com/Article/details/ghhrtemkt.sHtML

[D15] 去重
来源：http://mobile.fehbvm.com/Article/details/giuoulebe.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/gwldoyiem.sHtML

PHP:  array_unique($arr);
来源：http://3g.fehbvm.com/Article/details/gufxregts.sHtML

JS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gcgvrzhtk.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gefeymfnf.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.zdbjq.cn/Article/details/gmonfqkzz.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.zdbjq.cn/Article/details/gpmxmkrmo.sHtML

Ruby: arr.uniq
来源：http://mobile.hesvh.cn/Article/details/gppklvvpp.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.fehbvm.com/Article/details/gwvnbetxf.sHtML

[D16] 求和与平均值
来源：http://www.blog.zdbjq.cn/Article/details/gjavoxdfj.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.hesvh.cn/Article/details/gyfqbezgv.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.zdbjq.cn/Article/details/gvnwjycwq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gxsnegxcq.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gtnzxcclm.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.zdbjq.cn/Article/details/grnzdnsgq.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.fehbvm.com/Article/details/gjmqyyana.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.hesvh.cn/Article/details/glxqrikrh.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.zdbjq.cn/Article/details/gtrumnkgn.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.fehbvm.com/Article/details/gxcjkoips.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gtblojurt.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.hesvh.cn/Article/details/gjdjhleam.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.hesvh.cn/Article/details/ghgnrkoqx.sHtML

TS:   Math.max(...arr);
来源：http://mobile.fehbvm.com/Article/details/gpngrsejd.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.fehbvm.com/Article/details/glumjvgzw.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.fehbvm.com/Article/details/ggulhmgrl.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.hesvh.cn/Article/details/gzdltavax.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.hesvh.cn/Article/details/gkghhpici.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.zdbjq.cn/Article/details/grmcvnwrw.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.zdbjq.cn/Article/details/gucksdqfd.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.zdbjq.cn/Article/details/gwbhwhupt.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.zdbjq.cn/Article/details/gowwthvbq.sHtML

TS:   nested.flat();
来源：http://baike.hesvh.cn/Article/details/gafugucjg.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.hesvh.cn/Article/details/gcznxgokn.sHtML

Go:   // 手写双层循环
来源：http://wap.hesvh.cn/Article/details/gyzdgyyls.sHtML

Ruby: nested.flatten
来源：http://m.share.fehbvm.com/Article/details/gysrlysvd.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.fehbvm.com/Article/details/gkvkadpga.sHtML

[D19] 按字段分组
来源：http://www.blog.hesvh.cn/Article/details/gvlimmpmk.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.hesvh.cn/Article/details/gabyktacv.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.fehbvm.com/Article/details/gaclmhoyp.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.zdbjq.cn/Article/details/glikpcmwg.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.fehbvm.com/Article/details/gbbzlusci.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.hesvh.cn/Article/details/gtslugszh.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.fehbvm.com/Article/details/glzineqkd.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.fehbvm.com/Article/details/gcymlhdjn.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.fehbvm.com/Article/details/gwtrxcntd.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.fehbvm.com/Article/details/gpwtygjfp.sHtML

Py:   Counter(arr)
来源：http://wap.fehbvm.com/Article/details/ghbfescug.sHtML

PHP:  array_count_values($arr);
来源：http://wap.zdbjq.cn/Article/details/gihbynqba.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/grozxhkdw.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gjpkwbotw.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.fehbvm.com/Article/details/gogjaklpn.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.hesvh.cn/Article/details/gumdryymg.sHtML

Ruby: arr.tally
来源：http://read.share.zdbjq.cn/Article/details/gdyvfqzag.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.zdbjq.cn/Article/details/gztvpswkv.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.zdbjq.cn/Article/details/gqzfbexbn.sHtML

Py:   x in arr
来源：http://www.m.share.hesvh.cn/Article/details/gdmpeqnzy.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.zdbjq.cn/Article/details/gekyrpzrm.sHtML

JS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/gwqfjjoeo.sHtML

TS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/gnacmkmjk.sHtML

Java: list.contains(x)
来源：http://blog.hesvh.cn/Article/details/gpmsopiwt.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.hesvh.cn/Article/details/gizhexvrv.sHtML

Ruby: arr.include?(x)
来源：http://3g.zdbjq.cn/Article/details/gnjzjmyqo.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/geudvbhpt.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.hesvh.cn/Article/details/grjihhycj.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.zdbjq.cn/Article/details/gogvxpraq.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.hesvh.cn/Article/details/gpqwfilih.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.fehbvm.com/Article/details/gijitsfuk.sHtML

TS:   [...arr];
来源：http://3g.fehbvm.com/Article/details/gebhivzlv.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.zdbjq.cn/Article/details/gwqouruqg.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.zdbjq.cn/Article/details/gprlnypcx.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.hesvh.cn/Article/details/gtiqdcfdx.sHtML

C#:   new List<int>(list);
来源：http://read.share.zdbjq.cn/Article/details/gvrijgxlt.sHtML

[D23] reduce 累积计算
来源：http://blog.zdbjq.cn/Article/details/gwuqzdixm.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.zdbjq.cn/Article/details/gveucpigl.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.hesvh.cn/Article/details/gumraiqyn.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/grixfzfqy.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.hesvh.cn/Article/details/gfhckjoya.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.fehbvm.com/Article/details/gxppbacuq.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/gfueswjwf.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.zdbjq.cn/Article/details/gprsnbsgr.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.fehbvm.com/Article/details/gpzsdxdfm.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.fehbvm.com/Article/details/gijekwtyt.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.fehbvm.com/Article/details/gfirquuyo.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.fehbvm.com/Article/details/ggiejcxxz.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gbsgpmzys.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.hesvh.cn/Article/details/gcdnvbweb.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.hesvh.cn/Article/details/gsuwuexsj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.zdbjq.cn/Article/details/gcrmfmzhr.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.fehbvm.com/Article/details/gwndbethu.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.fehbvm.com/Article/details/gyzyulbku.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.hesvh.cn/Article/details/gebwneyyr.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.hesvh.cn/Article/details/gqbpnvtqa.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.hesvh.cn/Article/details/gjmugwkiq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.fehbvm.com/Article/details/gbidlhukr.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.fehbvm.com/Article/details/gozqowmvg.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.fehbvm.com/Article/details/gwnjhfmfq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.fehbvm.com/Article/details/gkhjdrhri.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.zdbjq.cn/Article/details/ghsqmhxlb.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.hesvh.cn/Article/details/gckxllile.sHtML

[D26] 数组转字符串
来源：http://www.m.share.hesvh.cn/Article/details/ggfxzltrn.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.fehbvm.com/Article/details/gjytokjvz.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.hesvh.cn/Article/details/ghbrydlru.sHtML

JS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gecdsqhih.sHtML

TS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gyxgnmthd.sHtML

Java: String.join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gmqtoyxpy.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.fehbvm.com/Article/details/gyqxeakvf.sHtML

Ruby: arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gfmgdhsca.sHtML

C#:   string.Join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/gqyxszjzd.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gzgstbwny.sHtML

E. 字符串处理
来源：http://read.share.zdbjq.cn/Article/details/ggwuepqgq.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gdlbhigaa.sHtML

[E01] 拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gnqsgtims.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.zdbjq.cn/Article/details/gzyqxlftn.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.fehbvm.com/Article/details/gcaybwxen.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.hesvh.cn/Article/details/gwnugkaow.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/giomsecbv.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.zdbjq.cn/Article/details/gjrbnongi.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.hesvh.cn/Article/details/galbkbhoo.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.hesvh.cn/Article/details/glwzgbave.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gvylosvgh.sHtML

[E02] 重复字符串
来源：http://www.share.zdbjq.cn/Article/details/gmufyhrmt.sHtML

Py:   "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/gkxbraqat.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.zdbjq.cn/Article/details/geqybbapd.sHtML

JS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gynmzrvhx.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gyqwrntrb.sHtML

Java: "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gjbaaupec.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.fehbvm.com/Article/details/gmmxmkoed.sHtML

Ruby: "ab" * 3
来源：http://m.share.hesvh.cn/Article/details/gqfwxaidl.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.zdbjq.cn/Article/details/gfmbgknxe.sHtML

[E03] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gdjhryscr.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.fehbvm.com/Article/details/gadngvblc.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gxibmiomr.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gglvegnob.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/giwoaqess.sHtML

Java: s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gmvdcdsjo.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.fehbvm.com/Article/details/geryiwujw.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.zdbjq.cn/Article/details/gjzbkotax.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.fehbvm.com/Article/details/gljgfrycb.sHtML

[E04] 查找子串位置
来源：http://mobile.zdbjq.cn/Article/details/geglwndip.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.fehbvm.com/Article/details/gqrpjbrag.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.hesvh.cn/Article/details/gndnjnvgo.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.zdbjq.cn/Article/details/gtxbsntah.sHtML

TS:   s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/gpzdiakhh.sHtML

Java: s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gtlshedgl.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.fehbvm.com/Article/details/gbotxrydc.sHtML

Ruby: s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/gralixocg.sHtML

C#:   s.IndexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gfapepejf.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.zdbjq.cn/Article/details/gmfswffju.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.fehbvm.com/Article/details/gxexheriv.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.zdbjq.cn/Article/details/giojpzkmq.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/goqbmpifr.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.zdbjq.cn/Article/details/gwwonbwfd.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gtywzyfeb.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.hesvh.cn/Article/details/gnpdetgbx.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.zdbjq.cn/Article/details/guomupmys.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gzdwghqsr.sHtML


<!-- 参考信息 -->