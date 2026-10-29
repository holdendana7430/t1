代发 wailian999

PHP:  // 无重载
来源：http://3g.hesvh.cn/Article/details/goolwxowh.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.zdbjq.cn/Article/details/ggjgabbui.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.zdbjq.cn/Article/details/gelsqlvaj.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.zdbjq.cn/Article/details/gwdpubcko.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.zdbjq.cn/Article/details/gwbwrnhgw.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.hesvh.cn/Article/details/gkgskxlqu.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.hesvh.cn/Article/details/gacowcrsk.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ghgtqcurf.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.hesvh.cn/Article/details/giriippzg.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gyxfwlmpa.sHtML

[D01] 创建数组 / 列表
来源：http://wap.fehbvm.com/Article/details/giphnmbma.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.hesvh.cn/Article/details/gtlnfhnpx.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.zdbjq.cn/Article/details/gfgndaoao.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.zdbjq.cn/Article/details/gmhwdwvcu.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.hesvh.cn/Article/details/gyudufagg.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.zdbjq.cn/Article/details/gzpwzfoer.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.fehbvm.com/Article/details/grbymaooo.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.fehbvm.com/Article/details/gtwusxxhi.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.hesvh.cn/Article/details/gyhfpsitm.sHtML

[D02] 追加元素到末尾
来源：http://3g.hesvh.cn/Article/details/gnpcbohpd.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.hesvh.cn/Article/details/gnldptrcv.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.fehbvm.com/Article/details/gpupsgzhs.sHtML

JS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/ghzwsntsm.sHtML

TS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/gjlicjebc.sHtML

Java: list.add(4);
来源：http://mobile.zdbjq.cn/Article/details/gpwnbxhil.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.zdbjq.cn/Article/details/ghjucuuig.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.hesvh.cn/Article/details/gkthsjzjn.sHtML

C#:   list.Add(4);
来源：http://blog.zdbjq.cn/Article/details/gnyywbtvh.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.zdbjq.cn/Article/details/gohkbycym.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.zdbjq.cn/Article/details/gzvfggsfh.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.fehbvm.com/Article/details/ghrtqpiaz.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.hesvh.cn/Article/details/gcqnnkofi.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/giveduuvw.sHtML

Java: list.add(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gcmnmpdaw.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.zdbjq.cn/Article/details/gpccadexv.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.fehbvm.com/Article/details/gsidsknou.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gtihinlky.sHtML

[D04] 删除元素
来源：http://mobile.fehbvm.com/Article/details/gohcajijp.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.hesvh.cn/Article/details/ghycvwgiu.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.zdbjq.cn/Article/details/ghxzicuzh.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.fehbvm.com/Article/details/gdhxjtvvq.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.zdbjq.cn/Article/details/gatqngqbt.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.fehbvm.com/Article/details/gofspzueq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.fehbvm.com/Article/details/gywjlssdp.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.zdbjq.cn/Article/details/ggsmwxvyq.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.zdbjq.cn/Article/details/gxrcqyunw.sHtML

[D05] 访问与修改元素
来源：http://baike.fehbvm.com/Article/details/girmdevaj.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gbphbiswt.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gulzvnckn.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/glajwbreo.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.fehbvm.com/Article/details/gcwrytxzv.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.hesvh.cn/Article/details/gmwlrvhkn.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gsfdjltna.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/ghmirgqeq.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gtsagkyui.sHtML

[D06] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gapfzqlkb.sHtML

Py:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/gnzgkxqxn.sHtML

PHP:  count($arr);
来源：http://www.share.zdbjq.cn/Article/details/gpfhpedew.sHtML

JS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/gxttxcagc.sHtML

TS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/ghgqguxhl.sHtML

Java: list.size();
来源：http://www.share.fehbvm.com/Article/details/gmaizdllj.sHtML

Go:   len(arr)
来源：http://wap.zdbjq.cn/Article/details/gwcackajt.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.hesvh.cn/Article/details/gtqjmolgz.sHtML

C#:   list.Count;
来源：http://wap.fehbvm.com/Article/details/ggavozepb.sHtML

[D07] 切片 / 取子数组
来源：http://wap.zdbjq.cn/Article/details/goapcxloq.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.hesvh.cn/Article/details/gfpckgfkv.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gprosbrun.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/guypiuroz.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gurpuoaqm.sHtML

Java: list.subList(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gjsxldigb.sHtML

Go:   arr[1:4]
来源：http://blog.zdbjq.cn/Article/details/gglnynvwa.sHtML

Ruby: arr[1, 3]
来源：http://m.share.hesvh.cn/Article/details/gvnhbzjpi.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.fehbvm.com/Article/details/gdqudeybd.sHtML

[D08] 合并两个数组
来源：http://wap.zdbjq.cn/Article/details/gksnbbxdx.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.zdbjq.cn/Article/details/gcehvsofc.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.fehbvm.com/Article/details/gadkjlypq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.zdbjq.cn/Article/details/goydzvwmi.sHtML

TS:   [...a, ...b];
来源：http://mobile.hesvh.cn/Article/details/gnmdvllfe.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.hesvh.cn/Article/details/gljffodfd.sHtML

Go:   append(a, b...)
来源：http://mobile.fehbvm.com/Article/details/gooidhnkk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fehbvm.com/Article/details/gpqtdfypa.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.hesvh.cn/Article/details/galrwxsbe.sHtML

[D09] 排序（升序）
来源：http://www.share.hesvh.cn/Article/details/gskpccpba.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gxykaznxu.sHtML

PHP:  sort($arr);
来源：http://read.share.zdbjq.cn/Article/details/gosjvkoji.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.hesvh.cn/Article/details/gpjhvacfq.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.hesvh.cn/Article/details/gnlhnenem.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.zdbjq.cn/Article/details/ggnszynpg.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/gcqojnsfj.sHtML

Ruby: arr.sort
来源：http://www.m.share.hesvh.cn/Article/details/gxhpahhgo.sHtML

C#:   list.Sort();
来源：http://3g.zdbjq.cn/Article/details/grwsjizjf.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.fehbvm.com/Article/details/gsbaxlaop.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.hesvh.cn/Article/details/gcsiamrse.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/gilvdjinc.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/gqufxhenp.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gkeehdnwi.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.fehbvm.com/Article/details/getjpkgiu.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.zdbjq.cn/Article/details/gpudfbosr.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.fehbvm.com/Article/details/gszxoucwt.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.fehbvm.com/Article/details/grfncmeqt.sHtML

[D11] 反转数组
来源：http://wap.fehbvm.com/Article/details/grdolagjb.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.fehbvm.com/Article/details/gtjutkdkf.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.fehbvm.com/Article/details/gkjantmur.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.fehbvm.com/Article/details/grpbfhwae.sHtML

TS:   [...arr].reverse();
来源：http://wap.zdbjq.cn/Article/details/gmaswocvb.sHtML

Java: Collections.reverse(list);
来源：http://blog.fehbvm.com/Article/details/goahnigya.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.zdbjq.cn/Article/details/gpsokqckt.sHtML

Ruby: arr.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gdbsotamf.sHtML

C#:   list.Reverse();
来源：http://mobile.zdbjq.cn/Article/details/gmgggyidj.sHtML

[D12] 查找元素下标
来源：http://mobile.fehbvm.com/Article/details/glnbghrot.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.fehbvm.com/Article/details/gjuwqasrb.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.fehbvm.com/Article/details/gszekvlcp.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/gqqxockoj.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/gjtuubpma.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.zdbjq.cn/Article/details/golbhxnko.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gxfnenguv.sHtML

Ruby: arr.index(x)
来源：http://m.share.zdbjq.cn/Article/details/gggnufgah.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.zdbjq.cn/Article/details/gjxvxhofi.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.hesvh.cn/Article/details/gdxvdewsc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.fehbvm.com/Article/details/gojrhnvte.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.zdbjq.cn/Article/details/gojpgfuve.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/gobdrmyka.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gsfvptkmc.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.zdbjq.cn/Article/details/gsvjjiykp.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.zdbjq.cn/Article/details/gyrnuqwzk.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.zdbjq.cn/Article/details/grkhfuhld.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gbxyoantl.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.hesvh.cn/Article/details/gcuktipti.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.zdbjq.cn/Article/details/gfipvczcc.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.fehbvm.com/Article/details/guittcdkv.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.hesvh.cn/Article/details/grkhmcktq.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.hesvh.cn/Article/details/gdgoigfru.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.zdbjq.cn/Article/details/gefacuvld.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/gstkvnmza.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gwvovrixe.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.hesvh.cn/Article/details/goeagixrt.sHtML

[D15] 去重
来源：http://www.blog.fehbvm.com/Article/details/gmqwnpwqo.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/girwzsins.sHtML

PHP:  array_unique($arr);
来源：http://m.share.hesvh.cn/Article/details/gdhqksfoy.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gtktpclje.sHtML

TS:   [...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gdtulmnvm.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.zdbjq.cn/Article/details/gzwinzkgu.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.fehbvm.com/Article/details/gaexmngrz.sHtML

Ruby: arr.uniq
来源：http://3g.fehbvm.com/Article/details/gzutzciep.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.hesvh.cn/Article/details/gzvxmknym.sHtML

[D16] 求和与平均值
来源：http://mobile.zdbjq.cn/Article/details/gpgajfyll.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.fehbvm.com/Article/details/gmfrntxbp.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.hesvh.cn/Article/details/gfqotggkx.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/gxscmpjkr.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/gmtaugibg.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.fehbvm.com/Article/details/gqrkdmsix.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.zdbjq.cn/Article/details/ghxgevcqq.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.fehbvm.com/Article/details/gfoozmoyl.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.zdbjq.cn/Article/details/gbtbwhjas.sHtML

[D17] 最大值与最小值
来源：http://3g.zdbjq.cn/Article/details/galarbfhb.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.hesvh.cn/Article/details/gpegslngl.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.zdbjq.cn/Article/details/ghcphilhx.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.fehbvm.com/Article/details/geaatboaf.sHtML

TS:   Math.max(...arr);
来源：http://mobile.hesvh.cn/Article/details/gugivfnik.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.hesvh.cn/Article/details/gnnbubcnr.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.hesvh.cn/Article/details/gmlnqntbp.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.zdbjq.cn/Article/details/ghdmzdckj.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.zdbjq.cn/Article/details/gfesdxaql.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.fehbvm.com/Article/details/gajchjabn.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.hesvh.cn/Article/details/ginahzffb.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.fehbvm.com/Article/details/gkbxnaspr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.fehbvm.com/Article/details/grmxopgnz.sHtML

TS:   nested.flat();
来源：http://www.m.share.hesvh.cn/Article/details/gtvchuenc.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.hesvh.cn/Article/details/ggtgafhui.sHtML

Go:   // 手写双层循环
来源：http://3g.fehbvm.com/Article/details/gbmvlvedb.sHtML

Ruby: nested.flatten
来源：http://baike.hesvh.cn/Article/details/gdfywerhs.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.fehbvm.com/Article/details/gvnpreeqd.sHtML

[D19] 按字段分组
来源：http://www.share.hesvh.cn/Article/details/giabljrww.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.zdbjq.cn/Article/details/gutaozlrn.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.fehbvm.com/Article/details/ghrmhgypp.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.hesvh.cn/Article/details/gbvtxjswv.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/grvjwblen.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.hesvh.cn/Article/details/glaskxqga.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.hesvh.cn/Article/details/gtgplqoqk.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.fehbvm.com/Article/details/gdrpkuemt.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.fehbvm.com/Article/details/gzezyeutd.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.zdbjq.cn/Article/details/gfchaaejr.sHtML

Py:   Counter(arr)
来源：http://mobile.fehbvm.com/Article/details/ghpzoeujp.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.zdbjq.cn/Article/details/gffvszsor.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gjvcwdvxz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/gcmgphzud.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.zdbjq.cn/Article/details/gzhekaxip.sHtML

Go:   // 手写 map[T]int
来源：http://baike.zdbjq.cn/Article/details/gonibnnhd.sHtML

Ruby: arr.tally
来源：http://read.share.hesvh.cn/Article/details/gtjhnsiqv.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.fehbvm.com/Article/details/gdkkpszje.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.hesvh.cn/Article/details/gzkzkypwc.sHtML

Py:   x in arr
来源：http://www.blog.zdbjq.cn/Article/details/gibgwkeaz.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.zdbjq.cn/Article/details/gnccxemjc.sHtML

JS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gtihzrvaj.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/goblygdyh.sHtML

Java: list.contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gdvibadni.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.hesvh.cn/Article/details/geutggzrz.sHtML

Ruby: arr.include?(x)
来源：http://baike.zdbjq.cn/Article/details/gdwdtnyhx.sHtML

C#:   list.Contains(x)
来源：http://m.share.hesvh.cn/Article/details/ghffhfbow.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.hesvh.cn/Article/details/gzpllajwz.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.zdbjq.cn/Article/details/gmdtrqawo.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.hesvh.cn/Article/details/gnyyokrho.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.zdbjq.cn/Article/details/gkaizdzwj.sHtML

TS:   [...arr];
来源：http://www.m.share.fehbvm.com/Article/details/giyjsukov.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.fehbvm.com/Article/details/gxvaqjuyk.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.fehbvm.com/Article/details/gjrzqgvkp.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.fehbvm.com/Article/details/gktvaspwb.sHtML

C#:   new List<int>(list);
来源：http://wap.fehbvm.com/Article/details/gcjopfysq.sHtML

[D23] reduce 累积计算
来源：http://m.share.zdbjq.cn/Article/details/grdvnkgrj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.zdbjq.cn/Article/details/gitvxaiuu.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.zdbjq.cn/Article/details/gqiyerqjt.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/ggxvflncr.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gtmyeczzq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.fehbvm.com/Article/details/gyvayhrqn.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/gcufrtzey.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.fehbvm.com/Article/details/gkbcppnjy.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.fehbvm.com/Article/details/gpprhskre.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.zdbjq.cn/Article/details/gcwkvxdld.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.fehbvm.com/Article/details/ghsjlkmsw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.hesvh.cn/Article/details/gqevxrdyb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.zdbjq.cn/Article/details/gyyukdxdt.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.hesvh.cn/Article/details/gsmhspdpk.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.hesvh.cn/Article/details/ggelaczdk.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.hesvh.cn/Article/details/gnmflhvsr.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.fehbvm.com/Article/details/ghvtxtvph.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.fehbvm.com/Article/details/gadwebuez.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.hesvh.cn/Article/details/gjueqmcrd.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.hesvh.cn/Article/details/gbmrmaund.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.zdbjq.cn/Article/details/ggkrdorpl.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.zdbjq.cn/Article/details/gijueopqz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.hesvh.cn/Article/details/gsvlvkfmk.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.fehbvm.com/Article/details/gugbnnoxn.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.zdbjq.cn/Article/details/gxlsblndk.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.hesvh.cn/Article/details/guiuyhaab.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.hesvh.cn/Article/details/gsdalxoyo.sHtML

[D26] 数组转字符串
来源：http://3g.hesvh.cn/Article/details/gpwcsqtlr.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.hesvh.cn/Article/details/glblkihvp.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.zdbjq.cn/Article/details/gmxrqlzgf.sHtML

JS:   arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gmxigkoyo.sHtML

TS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gufgejpzt.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/gzplznpjm.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.zdbjq.cn/Article/details/gnejsqkjo.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gyjgkmezd.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/gmivdxdyz.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gsedtupnz.sHtML

E. 字符串处理
来源：http://www.blog.zdbjq.cn/Article/details/guoeimpra.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gxsbvsgft.sHtML

[E01] 拼接字符串
来源：http://read.share.fehbvm.com/Article/details/ghkheemwk.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.fehbvm.com/Article/details/govartuqq.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.zdbjq.cn/Article/details/gwynrzmmk.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/grgauqrpv.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/gqxipoycr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.zdbjq.cn/Article/details/gzmwtibxn.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.fehbvm.com/Article/details/gotvdpxre.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.zdbjq.cn/Article/details/gbzwbsjsf.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gmhqotkqj.sHtML

[E02] 重复字符串
来源：http://baike.hesvh.cn/Article/details/gptfcjkyt.sHtML

Py:   "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/gegckoink.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.fehbvm.com/Article/details/garjprnjn.sHtML

JS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gupnjtmfi.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gdyxaihkm.sHtML

Java: "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/ggvmjstsv.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.zdbjq.cn/Article/details/gscyydytm.sHtML

Ruby: "ab" * 3
来源：http://www.share.fehbvm.com/Article/details/gjvravmag.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.fehbvm.com/Article/details/gloyzzwre.sHtML

[E03] 截取子串
来源：http://baike.hesvh.cn/Article/details/gdthmdifs.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.fehbvm.com/Article/details/gtjmypyas.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gxnnopqre.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.fehbvm.com/Article/details/grtrfzgyj.sHtML

TS:   s.slice(1, 4)
来源：http://wap.hesvh.cn/Article/details/gflmbuxmk.sHtML

Java: s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gzyeilxxo.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.fehbvm.com/Article/details/gvxuvxvlt.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.zdbjq.cn/Article/details/grvochplc.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.hesvh.cn/Article/details/gmlntyhwz.sHtML

[E04] 查找子串位置
来源：http://blog.zdbjq.cn/Article/details/gewtmuqfb.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.fehbvm.com/Article/details/gjawwzeny.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.zdbjq.cn/Article/details/gwsebscop.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.fehbvm.com/Article/details/gxgiupcpt.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gyfcntqwx.sHtML

Java: s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/gijsnzphj.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.hesvh.cn/Article/details/gwbfghsyp.sHtML

Ruby: s.index("x")
来源：http://baike.hesvh.cn/Article/details/giqumjbzl.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gkgcaejce.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.zdbjq.cn/Article/details/gobpjpqgo.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.hesvh.cn/Article/details/gpjdegrjq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.zdbjq.cn/Article/details/ggowsnqju.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gswbbvfih.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.hesvh.cn/Article/details/gnjifpell.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gpncikyju.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.hesvh.cn/Article/details/gjqtrghxj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gqbgxriaa.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gfiqgdhbu.sHtML

[E06] 替换子串
来源：http://baike.fehbvm.com/Article/details/gzsvnjngq.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/gcokhxjgn.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.fehbvm.com/Article/details/gvfnmtejr.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gvwxljvis.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gutqylssa.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gkrsvspux.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/gffkewnvk.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.hesvh.cn/Article/details/glpgrgryx.sHtML


<!-- 参考信息 -->