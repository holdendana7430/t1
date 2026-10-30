代发 wailian999

Ruby: a, b = pair
来源：http://www.blog.hesvh.cn/Article/details/geqtxoxdo.sHtML

C#:   var (a, b) = pair;
来源：http://baike.fehbvm.com/Article/details/gzqvbpxfk.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.hesvh.cn/Article/details/gpkehabxx.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.hesvh.cn/Article/details/gxnpncmlq.sHtML

PHP:  // 无重载
来源：http://3g.hesvh.cn/Article/details/gjhrfuusu.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.fehbvm.com/Article/details/gmqorcthk.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.zdbjq.cn/Article/details/gvixzlsfv.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.zdbjq.cn/Article/details/gdpvfozxc.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.hesvh.cn/Article/details/glotmuinx.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.zdbjq.cn/Article/details/gjsqrevoa.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.zdbjq.cn/Article/details/gmeawmjwg.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gnvtxfigl.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.fehbvm.com/Article/details/goqcetvgy.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/glnfojusk.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.fehbvm.com/Article/details/gumlbyheh.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.zdbjq.cn/Article/details/gyzzbkfkm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.zdbjq.cn/Article/details/gfnnjoofe.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.hesvh.cn/Article/details/gnrvdvnxg.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.fehbvm.com/Article/details/gwvnxtrwd.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.zdbjq.cn/Article/details/gquqadotl.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.hesvh.cn/Article/details/gxlrvsjkx.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.fehbvm.com/Article/details/guwwunryf.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.hesvh.cn/Article/details/gxonmlsxb.sHtML

[D02] 追加元素到末尾
来源：http://mobile.zdbjq.cn/Article/details/ghvmguwxy.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.hesvh.cn/Article/details/gixezqotv.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.fehbvm.com/Article/details/gqpoxjvqu.sHtML

JS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/gigudlouc.sHtML

TS:   arr.push(4);
来源：http://www.blog.hesvh.cn/Article/details/gbxcpfnnc.sHtML

Java: list.add(4);
来源：http://read.share.fehbvm.com/Article/details/gvpqzbwms.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.fehbvm.com/Article/details/gaciwozvc.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.hesvh.cn/Article/details/gbmnrybsp.sHtML

C#:   list.Add(4);
来源：http://www.share.fehbvm.com/Article/details/gcrlvjrht.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.fehbvm.com/Article/details/gkfogwejq.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.hesvh.cn/Article/details/gefbguwxp.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.zdbjq.cn/Article/details/gkoijuiix.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.fehbvm.com/Article/details/gwntaamwc.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gxsbuybfe.sHtML

Java: list.add(0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gpxdaupat.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.hesvh.cn/Article/details/gsmcrnsnn.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.fehbvm.com/Article/details/gfbjpqwlb.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gomrrtszo.sHtML

[D04] 删除元素
来源：http://mobile.zdbjq.cn/Article/details/gxiunkdpr.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.fehbvm.com/Article/details/gmxgecgxi.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.fehbvm.com/Article/details/gdioumzqw.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.zdbjq.cn/Article/details/gabtyxfdm.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.zdbjq.cn/Article/details/gybepfzrs.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.hesvh.cn/Article/details/gqsjkvtrb.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.zdbjq.cn/Article/details/gzgbsygiz.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.hesvh.cn/Article/details/glzidnlsf.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.hesvh.cn/Article/details/grtpqvzwn.sHtML

[D05] 访问与修改元素
来源：http://m.share.zdbjq.cn/Article/details/grlpblobo.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gnyfaeasa.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/grbkjwlnh.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gzmqlubup.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.zdbjq.cn/Article/details/gxbekpylo.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.fehbvm.com/Article/details/gwkjufwqx.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gmoutqsqc.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/grmpxlwds.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gufkuwhqv.sHtML

[D06] 数组长度
来源：http://wap.hesvh.cn/Article/details/gijxavspx.sHtML

Py:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gscbsjdsu.sHtML

PHP:  count($arr);
来源：http://wap.fehbvm.com/Article/details/glpakajie.sHtML

JS:   arr.length
来源：http://wap.hesvh.cn/Article/details/gbqqygaox.sHtML

TS:   arr.length
来源：http://mobile.fehbvm.com/Article/details/gqcnirewm.sHtML

Java: list.size();
来源：http://www.m.share.fehbvm.com/Article/details/giylmnaek.sHtML

Go:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/ggadkryfk.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.hesvh.cn/Article/details/gjmjmfkdm.sHtML

C#:   list.Count;
来源：http://www.blog.fehbvm.com/Article/details/gwsfrregi.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.zdbjq.cn/Article/details/gbkmoigkp.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.fehbvm.com/Article/details/gecovzvzg.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gqomjyjxl.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gmsbybfig.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gjxkzyvtd.sHtML

Java: list.subList(1, 4);
来源：http://wap.fehbvm.com/Article/details/ggnbwidsp.sHtML

Go:   arr[1:4]
来源：http://read.share.hesvh.cn/Article/details/gbmodhedf.sHtML

Ruby: arr[1, 3]
来源：http://3g.hesvh.cn/Article/details/gyjstrlla.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gzxwvwmkp.sHtML

[D08] 合并两个数组
来源：http://read.share.hesvh.cn/Article/details/gioyciuus.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.zdbjq.cn/Article/details/gzmpqjghu.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.zdbjq.cn/Article/details/gjhhbvgjp.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.zdbjq.cn/Article/details/gdtysrvfz.sHtML

TS:   [...a, ...b];
来源：http://mobile.zdbjq.cn/Article/details/gagepjlrv.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.fehbvm.com/Article/details/gzwpfnpev.sHtML

Go:   append(a, b...)
来源：http://www.m.share.fehbvm.com/Article/details/gdyibyeam.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.zdbjq.cn/Article/details/gyrhvizpi.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.fehbvm.com/Article/details/gipxohoyt.sHtML

[D09] 排序（升序）
来源：http://blog.fehbvm.com/Article/details/gyoixpvmf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.zdbjq.cn/Article/details/gukowvwug.sHtML

PHP:  sort($arr);
来源：http://baike.zdbjq.cn/Article/details/grjskgymj.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.fehbvm.com/Article/details/giznsrsyz.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.hesvh.cn/Article/details/gbgmikylb.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.hesvh.cn/Article/details/gmlcimjye.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gooxmbvsk.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/ggqdinvvq.sHtML

C#:   list.Sort();
来源：http://blog.hesvh.cn/Article/details/gtgokdzwi.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.hesvh.cn/Article/details/gqgbinfdt.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.fehbvm.com/Article/details/gihqrkwjn.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/gjwbqybxw.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gvpofxttz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/glppburaa.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.zdbjq.cn/Article/details/gdtyxvlkt.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.hesvh.cn/Article/details/gzznyrssl.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.zdbjq.cn/Article/details/ggsforshi.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.zdbjq.cn/Article/details/glgnhhxzi.sHtML

[D11] 反转数组
来源：http://3g.fehbvm.com/Article/details/gdrzxrcbz.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.zdbjq.cn/Article/details/gqdqstltz.sHtML

PHP:  array_reverse($arr);
来源：http://baike.zdbjq.cn/Article/details/gkllpvfqh.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.zdbjq.cn/Article/details/getguuqfu.sHtML

TS:   [...arr].reverse();
来源：http://www.share.zdbjq.cn/Article/details/gtcuonrbr.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gpsbwewhg.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.zdbjq.cn/Article/details/gzvtxkbea.sHtML

Ruby: arr.reverse
来源：http://mobile.zdbjq.cn/Article/details/gudlayeqx.sHtML

C#:   list.Reverse();
来源：http://3g.hesvh.cn/Article/details/gkrpqvitu.sHtML

[D12] 查找元素下标
来源：http://mobile.hesvh.cn/Article/details/gcqqaoyaa.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.zdbjq.cn/Article/details/gccdhwdvn.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.hesvh.cn/Article/details/giuinacyt.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gmtpwjtot.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/gquqfzqki.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.hesvh.cn/Article/details/gtzrxvrms.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gapotsejq.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gxkrwrpyt.sHtML

C#:   list.IndexOf(x);
来源：http://blog.zdbjq.cn/Article/details/gleajoybm.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.hesvh.cn/Article/details/gjtpyfjqi.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.fehbvm.com/Article/details/gwhdqbgap.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.zdbjq.cn/Article/details/gizmtibeu.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gcfjsohfa.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gnwgsbwsl.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.fehbvm.com/Article/details/grccbumpp.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.zdbjq.cn/Article/details/gobxxzxrw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.hesvh.cn/Article/details/gnkerixuj.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.hesvh.cn/Article/details/grctraxhv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.hesvh.cn/Article/details/gtnspinjv.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gmqmjcdmd.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gcmfcujat.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/gegrtljuy.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/gioyeidhd.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.hesvh.cn/Article/details/gsnniuzjn.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/gvcsbdcuv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gbfckugny.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gklawwybg.sHtML

[D15] 去重
来源：http://mobile.zdbjq.cn/Article/details/ghqhhmdvg.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.hesvh.cn/Article/details/gyklzsnsx.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gkzilpjup.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gyajcssie.sHtML

TS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gfjoonszt.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.hesvh.cn/Article/details/gbizsunfx.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.fehbvm.com/Article/details/gzmtkgnmm.sHtML

Ruby: arr.uniq
来源：http://read.share.fehbvm.com/Article/details/gvzsasgip.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.hesvh.cn/Article/details/gyaqvirpa.sHtML

[D16] 求和与平均值
来源：http://read.share.zdbjq.cn/Article/details/gqraznyfp.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.fehbvm.com/Article/details/gekrafgef.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.hesvh.cn/Article/details/getiiioli.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/gticdbpxl.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gubkflrdk.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.hesvh.cn/Article/details/glbmpnygn.sHtML

Go:   // 手写循环累加
来源：http://read.share.fehbvm.com/Article/details/gxwevdfaz.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.fehbvm.com/Article/details/gxaqplbhd.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.hesvh.cn/Article/details/gprhjhngq.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.hesvh.cn/Article/details/glhsyksby.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.fehbvm.com/Article/details/gnnppkshw.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.fehbvm.com/Article/details/gmmtonefn.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.zdbjq.cn/Article/details/ggsimdoxz.sHtML

TS:   Math.max(...arr);
来源：http://baike.zdbjq.cn/Article/details/gfxtsoshz.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.zdbjq.cn/Article/details/gnypzockb.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.fehbvm.com/Article/details/gxukkbgnp.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.hesvh.cn/Article/details/ghqhlvxkw.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.zdbjq.cn/Article/details/gceaithnt.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.fehbvm.com/Article/details/gmhvqehjh.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.fehbvm.com/Article/details/gwuoqubtk.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.fehbvm.com/Article/details/gcvwfyehu.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.zdbjq.cn/Article/details/gthpudskz.sHtML

TS:   nested.flat();
来源：http://www.share.zdbjq.cn/Article/details/gitvhcfep.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.zdbjq.cn/Article/details/gbstlwieu.sHtML

Go:   // 手写双层循环
来源：http://www.share.zdbjq.cn/Article/details/grovnzvmf.sHtML

Ruby: nested.flatten
来源：http://m.share.hesvh.cn/Article/details/gvvpvuzsz.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.hesvh.cn/Article/details/gfbzxlumu.sHtML

[D19] 按字段分组
来源：http://read.share.fehbvm.com/Article/details/glupeyvnx.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.fehbvm.com/Article/details/gmibkhycj.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.zdbjq.cn/Article/details/gzxudwbfg.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.hesvh.cn/Article/details/gytfvgysg.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gzwxfpsae.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.zdbjq.cn/Article/details/grthdavmq.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.hesvh.cn/Article/details/geugczxxy.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.fehbvm.com/Article/details/ghspjuyoi.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.hesvh.cn/Article/details/ginqvrnbx.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.fehbvm.com/Article/details/gzptgzzst.sHtML

Py:   Counter(arr)
来源：http://mobile.hesvh.cn/Article/details/guaiuoupm.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.fehbvm.com/Article/details/gqkvzxutz.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/genqysjkb.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/gqosphsrv.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.fehbvm.com/Article/details/gvdsfludn.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.zdbjq.cn/Article/details/gtqfvspop.sHtML

Ruby: arr.tally
来源：http://read.share.zdbjq.cn/Article/details/gbkqsojfi.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.hesvh.cn/Article/details/gfbbcrfwc.sHtML

[D21] 判断是否包含某元素
来源：http://baike.zdbjq.cn/Article/details/gzwamefhi.sHtML

Py:   x in arr
来源：http://mobile.hesvh.cn/Article/details/ghhubqzgi.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.zdbjq.cn/Article/details/guiabcrnm.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gvjmddtwz.sHtML

TS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/gzfhjpuze.sHtML

Java: list.contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gqdlhzwky.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.hesvh.cn/Article/details/gechqezrz.sHtML

Ruby: arr.include?(x)
来源：http://mobile.zdbjq.cn/Article/details/gxmukoixh.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gixfwdlyz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.zdbjq.cn/Article/details/gyriptarp.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.hesvh.cn/Article/details/goavsioyv.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.fehbvm.com/Article/details/gnimybghk.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.hesvh.cn/Article/details/gpofnhksm.sHtML

TS:   [...arr];
来源：http://mobile.hesvh.cn/Article/details/gumkzfdco.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.fehbvm.com/Article/details/gbbcfzuon.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.fehbvm.com/Article/details/goyvntxms.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.hesvh.cn/Article/details/gaimscawv.sHtML

C#:   new List<int>(list);
来源：http://blog.fehbvm.com/Article/details/gihazkena.sHtML

[D23] reduce 累积计算
来源：http://blog.zdbjq.cn/Article/details/grczvxyek.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.hesvh.cn/Article/details/gmbaduuzc.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.fehbvm.com/Article/details/gfoabqqcw.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/gghlmpvrj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/gxdardrmv.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.fehbvm.com/Article/details/gjrjhlhyy.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/gwhjflbdm.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.hesvh.cn/Article/details/gikkmohua.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.fehbvm.com/Article/details/gfryfclgn.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.zdbjq.cn/Article/details/gvcpmxfnx.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.fehbvm.com/Article/details/gxknliiiq.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.fehbvm.com/Article/details/ghxabttlt.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.zdbjq.cn/Article/details/gasnzhcoo.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gwlzkrahp.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.zdbjq.cn/Article/details/gqcokavgt.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.hesvh.cn/Article/details/gtyossefj.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.zdbjq.cn/Article/details/gtqiqokom.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.zdbjq.cn/Article/details/gqsppgxdu.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.hesvh.cn/Article/details/gfidqnieg.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.fehbvm.com/Article/details/gvpdkonen.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.zdbjq.cn/Article/details/ggnbfdgsy.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.hesvh.cn/Article/details/gnscwuauu.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.hesvh.cn/Article/details/gothmcvtl.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.fehbvm.com/Article/details/ggixnglbf.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.zdbjq.cn/Article/details/gdhwitjxp.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.zdbjq.cn/Article/details/gvilyrmgr.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.zdbjq.cn/Article/details/gfjuysyss.sHtML

[D26] 数组转字符串
来源：http://baike.fehbvm.com/Article/details/gvlrdkfoo.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gjxaofuob.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.fehbvm.com/Article/details/gedmiauqz.sHtML

JS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gtwttcmjf.sHtML

TS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gleknxbjv.sHtML

Java: String.join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gamvjneyy.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.hesvh.cn/Article/details/gjnqedcoz.sHtML

Ruby: arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/grznwzwuu.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/gtfdxkjoq.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gyolxnjzi.sHtML

E. 字符串处理
来源：http://3g.fehbvm.com/Article/details/ggcukxidv.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gfwwlautc.sHtML

[E01] 拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gxthcviga.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.zdbjq.cn/Article/details/gbckownsj.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.fehbvm.com/Article/details/gyueujzjd.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/guxdjdjlj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/gplqawhwy.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.zdbjq.cn/Article/details/gimyfskjv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.zdbjq.cn/Article/details/gskraatjg.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.hesvh.cn/Article/details/gnodeegyz.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.hesvh.cn/Article/details/gqfojszbn.sHtML

[E02] 重复字符串
来源：http://www.blog.fehbvm.com/Article/details/grqtgmkrk.sHtML

Py:   "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/gftsxcqyk.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.zdbjq.cn/Article/details/gvebmfzxv.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gubfxvatu.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/ggnhtbucx.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gmzkwgzjo.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.fehbvm.com/Article/details/gqdtyriab.sHtML

Ruby: "ab" * 3
来源：http://blog.fehbvm.com/Article/details/gehxgncnm.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.hesvh.cn/Article/details/ggwbuppoo.sHtML

[E03] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gaqjwylbu.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.zdbjq.cn/Article/details/giskygqyw.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/glzljelkk.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gmqxzcdyk.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.hesvh.cn/Article/details/guntneywv.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gmarkdnih.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.zdbjq.cn/Article/details/ggvalthps.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.zdbjq.cn/Article/details/gvlqmmcxk.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.zdbjq.cn/Article/details/gqdjdfybr.sHtML

[E04] 查找子串位置
来源：http://baike.fehbvm.com/Article/details/gbgzouyfh.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gqeazqfxn.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.fehbvm.com/Article/details/gweifpzgs.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.fehbvm.com/Article/details/ggahgcbpf.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gcjgmnqgi.sHtML

Java: s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/ghvbsxwpr.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.zdbjq.cn/Article/details/goihmkmjl.sHtML

Ruby: s.index("x")
来源：http://3g.zdbjq.cn/Article/details/gbsyzvfik.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/gokcnpdir.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.fehbvm.com/Article/details/gkrirlgfk.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.zdbjq.cn/Article/details/giudeueop.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.hesvh.cn/Article/details/gezqjybcm.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/glixcugcp.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.fehbvm.com/Article/details/gqmkdoxrl.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/gfbkoazzz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.hesvh.cn/Article/details/gwlwzczrv.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.zdbjq.cn/Article/details/gfdvjdljh.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.fehbvm.com/Article/details/gmxbbhfds.sHtML

[E06] 替换子串
来源：http://read.share.zdbjq.cn/Article/details/ggpgoqdvp.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gqtjhybfr.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.hesvh.cn/Article/details/gpfhiwnhd.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/ghinfufzl.sHtML


<!-- 参考信息 -->