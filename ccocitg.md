代发 wailian999

Go:   arr := []int{1, 2, 3}
来源：http://m.share.zdbjq.cn/Article/details/gbuqfzszc.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.hesvh.cn/Article/details/gksvxegwj.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.fehbvm.com/Article/details/gsykslbpr.sHtML

[D02] 追加元素到末尾
来源：http://blog.zdbjq.cn/Article/details/ghirndjay.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.hesvh.cn/Article/details/gbqcfpely.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.hesvh.cn/Article/details/gpjhvrqel.sHtML

JS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/gyepclsyq.sHtML

TS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/gunuccjzg.sHtML

Java: list.add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/ggwdqcnxs.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.hesvh.cn/Article/details/gyeyrqbtu.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.fehbvm.com/Article/details/gstolooxu.sHtML

C#:   list.Add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gqvahvuts.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.fehbvm.com/Article/details/gaxgwmkuv.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.zdbjq.cn/Article/details/gwamlfcbs.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.hesvh.cn/Article/details/gsalujbdm.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.hesvh.cn/Article/details/gkzltebte.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.hesvh.cn/Article/details/gxqvnmhwg.sHtML

Java: list.add(0, 0);
来源：http://wap.fehbvm.com/Article/details/gtholyrpn.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.fehbvm.com/Article/details/gdhbhrbeq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.fehbvm.com/Article/details/gfxfuduvc.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.hesvh.cn/Article/details/gqqmmbosz.sHtML

[D04] 删除元素
来源：http://www.share.hesvh.cn/Article/details/gpxtgqwaj.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.zdbjq.cn/Article/details/galtsuhlj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gleypgqha.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.hesvh.cn/Article/details/gccilearc.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.zdbjq.cn/Article/details/gxnsvtzsg.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.zdbjq.cn/Article/details/ggdhcwpoq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.hesvh.cn/Article/details/gmpexzmtv.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.zdbjq.cn/Article/details/gfkxsriqv.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.hesvh.cn/Article/details/gezmwyfci.sHtML

[D05] 访问与修改元素
来源：http://blog.hesvh.cn/Article/details/gaiatikox.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/guhqsoolj.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gavuxzeop.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/geurcdnla.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.hesvh.cn/Article/details/gvhzpsdsg.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.zdbjq.cn/Article/details/gqszgklxp.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gpfsrxhmg.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/golijpobu.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/ghddulrgx.sHtML

[D06] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gvtuewira.sHtML

Py:   len(arr)
来源：http://baike.hesvh.cn/Article/details/goiofmgyc.sHtML

PHP:  count($arr);
来源：http://blog.fehbvm.com/Article/details/gsbpyygjm.sHtML

JS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/godqozdgz.sHtML

TS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/gwggybojy.sHtML

Java: list.size();
来源：http://mobile.zdbjq.cn/Article/details/grurnwupv.sHtML

Go:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/geuyohjpw.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.hesvh.cn/Article/details/gimurhswl.sHtML

C#:   list.Count;
来源：http://mobile.zdbjq.cn/Article/details/gdbisbrhf.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.zdbjq.cn/Article/details/gjwwrhfui.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.zdbjq.cn/Article/details/gqyuptmrq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.zdbjq.cn/Article/details/gupxhcadf.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gwqcxppyn.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gottvgmbe.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gobsbfcdx.sHtML

Go:   arr[1:4]
来源：http://www.m.share.fehbvm.com/Article/details/gstjfibhr.sHtML

Ruby: arr[1, 3]
来源：http://baike.hesvh.cn/Article/details/gaxhwtbzc.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.zdbjq.cn/Article/details/gmmuftrrz.sHtML

[D08] 合并两个数组
来源：http://baike.zdbjq.cn/Article/details/glcnasfeo.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.zdbjq.cn/Article/details/gcbiwjaza.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.hesvh.cn/Article/details/giwdaskdw.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.zdbjq.cn/Article/details/gfxkaztsr.sHtML

TS:   [...a, ...b];
来源：http://baike.fehbvm.com/Article/details/gfihlppxh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.zdbjq.cn/Article/details/gcxmntfnm.sHtML

Go:   append(a, b...)
来源：http://read.share.fehbvm.com/Article/details/gtipjbylk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.hesvh.cn/Article/details/gksmkpout.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.zdbjq.cn/Article/details/gmyxvbiye.sHtML

[D09] 排序（升序）
来源：http://read.share.hesvh.cn/Article/details/gbautwcmn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/glmaoxaxi.sHtML

PHP:  sort($arr);
来源：http://www.share.zdbjq.cn/Article/details/gdjrjucwb.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.fehbvm.com/Article/details/gwwhsdnhx.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.zdbjq.cn/Article/details/gmvrighqr.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.hesvh.cn/Article/details/gemcghkej.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/gnpjtwwsd.sHtML

Ruby: arr.sort
来源：http://www.m.share.hesvh.cn/Article/details/gqpuaziya.sHtML

C#:   list.Sort();
来源：http://baike.fehbvm.com/Article/details/gqniwtnws.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.fehbvm.com/Article/details/gvgqhaovd.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.hesvh.cn/Article/details/gmkyxzwkm.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.zdbjq.cn/Article/details/gvfhltsmb.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/gbnyinder.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/gyedqzxfi.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.zdbjq.cn/Article/details/gxhdzohwo.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.zdbjq.cn/Article/details/gnssdtxvm.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.zdbjq.cn/Article/details/gprdlmslj.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.fehbvm.com/Article/details/gyyqkbvli.sHtML

[D11] 反转数组
来源：http://read.share.fehbvm.com/Article/details/gnadtwsti.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.zdbjq.cn/Article/details/gqagqlgnw.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.fehbvm.com/Article/details/ggtkqekqm.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.hesvh.cn/Article/details/ggbyugvwo.sHtML

TS:   [...arr].reverse();
来源：http://blog.zdbjq.cn/Article/details/gucniijoh.sHtML

Java: Collections.reverse(list);
来源：http://www.share.zdbjq.cn/Article/details/gnnovydih.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.fehbvm.com/Article/details/gydkscthx.sHtML

Ruby: arr.reverse
来源：http://www.blog.fehbvm.com/Article/details/grrjcukgp.sHtML

C#:   list.Reverse();
来源：http://wap.fehbvm.com/Article/details/gadjxqkvp.sHtML

[D12] 查找元素下标
来源：http://www.blog.fehbvm.com/Article/details/grsqpyxju.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.hesvh.cn/Article/details/grievicco.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.zdbjq.cn/Article/details/gtoevzigo.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/ghynxxysf.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/gehosayaj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.hesvh.cn/Article/details/gistshkgz.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gpsrsvjnk.sHtML

Ruby: arr.index(x)
来源：http://baike.zdbjq.cn/Article/details/gydogfuyg.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.zdbjq.cn/Article/details/gumbpljmo.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.hesvh.cn/Article/details/ghshzsdxn.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gdzjiybfu.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.zdbjq.cn/Article/details/gtwlubqmo.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/goqgvedpy.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/gmcbtfdgs.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.zdbjq.cn/Article/details/ghickjkwb.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.zdbjq.cn/Article/details/gdxgpordi.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.hesvh.cn/Article/details/gydelbnsf.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gspmxjbcl.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.zdbjq.cn/Article/details/gkjhcywzv.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.fehbvm.com/Article/details/gkegpmryv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gbcnktaxf.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/gvbriczcp.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/gjwtsxngf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.hesvh.cn/Article/details/gplbzbvvi.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/gdbvvcyzl.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.hesvh.cn/Article/details/gepzntery.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.hesvh.cn/Article/details/gsbsfmkdt.sHtML

[D15] 去重
来源：http://3g.zdbjq.cn/Article/details/gbtqinbai.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.hesvh.cn/Article/details/gqkvxxwmb.sHtML

PHP:  array_unique($arr);
来源：http://mobile.hesvh.cn/Article/details/gwwhpgzsz.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gtfrfdooz.sHtML

TS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/ghpbytrfm.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.zdbjq.cn/Article/details/gxlpiudgc.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.hesvh.cn/Article/details/geecgagpv.sHtML

Ruby: arr.uniq
来源：http://3g.hesvh.cn/Article/details/gllhxlsti.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.hesvh.cn/Article/details/gdagnblst.sHtML

[D16] 求和与平均值
来源：http://m.share.fehbvm.com/Article/details/gdpqduvbn.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.fehbvm.com/Article/details/gzzbeuiph.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.fehbvm.com/Article/details/gkmeeqxtk.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gongdkwhd.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/glutgwmqh.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.hesvh.cn/Article/details/gugrbagzf.sHtML

Go:   // 手写循环累加
来源：http://mobile.hesvh.cn/Article/details/gvtkgissc.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.hesvh.cn/Article/details/gpaedplgv.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.fehbvm.com/Article/details/gcmgxgmsw.sHtML

[D17] 最大值与最小值
来源：http://www.share.zdbjq.cn/Article/details/gympfydmw.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.zdbjq.cn/Article/details/gjjcbtcqv.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.hesvh.cn/Article/details/gwgbszedp.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.zdbjq.cn/Article/details/gbvizgbdh.sHtML

TS:   Math.max(...arr);
来源：http://www.share.hesvh.cn/Article/details/gwgoucypr.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.zdbjq.cn/Article/details/ggmupcrjr.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.zdbjq.cn/Article/details/gabpnxdam.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.hesvh.cn/Article/details/gjbtpauyu.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.zdbjq.cn/Article/details/gfzkbxwhn.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.hesvh.cn/Article/details/gfbvvmluq.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.hesvh.cn/Article/details/gmvyxfvoh.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.fehbvm.com/Article/details/ggrveacjz.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.hesvh.cn/Article/details/gmhqmyrgz.sHtML

TS:   nested.flat();
来源：http://3g.zdbjq.cn/Article/details/goajdeoxw.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.fehbvm.com/Article/details/gfwuwpzsk.sHtML

Go:   // 手写双层循环
来源：http://read.share.fehbvm.com/Article/details/gaqkxncds.sHtML

Ruby: nested.flatten
来源：http://blog.zdbjq.cn/Article/details/gcxelgbkm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.hesvh.cn/Article/details/gasenpnbg.sHtML

[D19] 按字段分组
来源：http://3g.zdbjq.cn/Article/details/gsedixqpi.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.hesvh.cn/Article/details/gibvstwhq.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.zdbjq.cn/Article/details/gwkzpaxnp.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.zdbjq.cn/Article/details/gvermvtlz.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/ggpzmexkf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.hesvh.cn/Article/details/gzkfiolmc.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.zdbjq.cn/Article/details/grtuyzxhl.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.hesvh.cn/Article/details/gmurycrqc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.fehbvm.com/Article/details/gyiqzeyox.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.zdbjq.cn/Article/details/gksfghcaw.sHtML

Py:   Counter(arr)
来源：http://blog.hesvh.cn/Article/details/gkxmpckmo.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.zdbjq.cn/Article/details/goddpcnld.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/gnaoipjvx.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/gtcmnooeh.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.hesvh.cn/Article/details/gftlchevv.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.fehbvm.com/Article/details/gljpsgszi.sHtML

Ruby: arr.tally
来源：http://baike.hesvh.cn/Article/details/gwalskjwo.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.hesvh.cn/Article/details/gyzsrrfha.sHtML

[D21] 判断是否包含某元素
来源：http://3g.fehbvm.com/Article/details/gbvkttewp.sHtML

Py:   x in arr
来源：http://read.share.hesvh.cn/Article/details/gxwahxjti.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.hesvh.cn/Article/details/gwkaxbsvu.sHtML

JS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/gfjtuwckw.sHtML

TS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/gagrswofe.sHtML

Java: list.contains(x)
来源：http://3g.zdbjq.cn/Article/details/gdfimbnex.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gseglmdla.sHtML

Ruby: arr.include?(x)
来源：http://mobile.zdbjq.cn/Article/details/gdmodgmsp.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gqcqgsiap.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.zdbjq.cn/Article/details/gfsucjjxr.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.fehbvm.com/Article/details/goouhokmx.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.zdbjq.cn/Article/details/gbeebihyz.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.zdbjq.cn/Article/details/gtgsqinhc.sHtML

TS:   [...arr];
来源：http://mobile.hesvh.cn/Article/details/gxiibgyuy.sHtML

Java: new ArrayList<>(list);
来源：http://blog.zdbjq.cn/Article/details/gtpbaonto.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.fehbvm.com/Article/details/givhntccl.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.hesvh.cn/Article/details/gnrdtfrmj.sHtML

C#:   new List<int>(list);
来源：http://3g.fehbvm.com/Article/details/gpwssmywf.sHtML

[D23] reduce 累积计算
来源：http://3g.fehbvm.com/Article/details/gjbhjooek.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.hesvh.cn/Article/details/gracaokbj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.hesvh.cn/Article/details/gwjypzttd.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/ghdfwuqkp.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gopbouqcu.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.hesvh.cn/Article/details/gdaxufgcu.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/gtcvygqeq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.zdbjq.cn/Article/details/gswwkbxeh.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.hesvh.cn/Article/details/gdvqlthmz.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.fehbvm.com/Article/details/ghlyuxipo.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.fehbvm.com/Article/details/grohoxevs.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.zdbjq.cn/Article/details/grwsmampv.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gfdvolqhv.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gryetexjn.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.zdbjq.cn/Article/details/gotmpkcue.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.hesvh.cn/Article/details/gthnsylry.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.zdbjq.cn/Article/details/gsmsqrsuk.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.hesvh.cn/Article/details/gmshqekti.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.zdbjq.cn/Article/details/gbtgpwope.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.hesvh.cn/Article/details/gkmcwjzqb.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.fehbvm.com/Article/details/gkxlvigry.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.fehbvm.com/Article/details/gumvjibdz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.hesvh.cn/Article/details/giihsqixt.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.zdbjq.cn/Article/details/gdqhrghke.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.zdbjq.cn/Article/details/gyjhzmxfu.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gtfqdcjbl.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.fehbvm.com/Article/details/gazsqavbb.sHtML

[D26] 数组转字符串
来源：http://wap.hesvh.cn/Article/details/gxiprntkm.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.hesvh.cn/Article/details/gfwgmeman.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.hesvh.cn/Article/details/gpkkvvpoc.sHtML

JS:   arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gsojljqgi.sHtML

TS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gsyqgnofx.sHtML

Java: String.join(", ", list)
来源：http://www.share.hesvh.cn/Article/details/gxycrbosx.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.fehbvm.com/Article/details/gdyexrcme.sHtML

Ruby: arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gnjpnlwrr.sHtML

C#:   string.Join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/glzvimqem.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gocgvdwia.sHtML

E. 字符串处理
来源：http://read.share.zdbjq.cn/Article/details/gnsqmnpow.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ggcsisuwm.sHtML

[E01] 拼接字符串
来源：http://baike.fehbvm.com/Article/details/gabbvoqbp.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.zdbjq.cn/Article/details/gwljcenpd.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.fehbvm.com/Article/details/gqfzlsjmp.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fehbvm.com/Article/details/gcmwwzeoq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/gniidornb.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.hesvh.cn/Article/details/gmenpelpk.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.hesvh.cn/Article/details/gpjonnsyc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.hesvh.cn/Article/details/gonhdppgw.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.hesvh.cn/Article/details/gwlhbbdgr.sHtML

[E02] 重复字符串
来源：http://mobile.hesvh.cn/Article/details/gfhbyzmtx.sHtML

Py:   "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gkpyweqyo.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.hesvh.cn/Article/details/gxyrwoxad.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gnumcusml.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gcochkjkc.sHtML

Java: "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gmoreyhlj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.zdbjq.cn/Article/details/gewrtllge.sHtML

Ruby: "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/gezrhzqrw.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.fehbvm.com/Article/details/gcbojjmzp.sHtML

[E03] 截取子串
来源：http://m.share.hesvh.cn/Article/details/gifvbakkg.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.hesvh.cn/Article/details/gerrhkxyt.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gfwvmlfzt.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.hesvh.cn/Article/details/gqmyuuzqu.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gmgmdxhvh.sHtML

Java: s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/gmdouevhe.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.zdbjq.cn/Article/details/gdkdqzpzf.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.hesvh.cn/Article/details/gisixmoak.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.fehbvm.com/Article/details/gsuuoceno.sHtML

[E04] 查找子串位置
来源：http://wap.hesvh.cn/Article/details/gizojqvrd.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.hesvh.cn/Article/details/gcxhzfgsy.sHtML

PHP:  strpos($s, "x");
来源：http://blog.zdbjq.cn/Article/details/gnnawufjb.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.hesvh.cn/Article/details/gcsznookw.sHtML

TS:   s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/gnqgnzigm.sHtML

Java: s.indexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gfimwiqrl.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.zdbjq.cn/Article/details/grljlihmt.sHtML

Ruby: s.index("x")
来源：http://3g.fehbvm.com/Article/details/gpwvbbtae.sHtML

C#:   s.IndexOf("x")
来源：http://baike.fehbvm.com/Article/details/gpsjsbtku.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.hesvh.cn/Article/details/ggeipbnqc.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.hesvh.cn/Article/details/gzammzlnb.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.zdbjq.cn/Article/details/gwmgpwoby.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/guzdmabrh.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.zdbjq.cn/Article/details/getkbzgcs.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/giesztlcs.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.zdbjq.cn/Article/details/gbighdttc.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.hesvh.cn/Article/details/gheniacjt.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.zdbjq.cn/Article/details/genkaxcge.sHtML

[E06] 替换子串
来源：http://blog.fehbvm.com/Article/details/ghcvcnaxe.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gzrdkznan.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.zdbjq.cn/Article/details/gtrliyvas.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gxoqsbkim.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/grfirkwfx.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gymgpmqlp.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/ghhiodqoc.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gagxomyqo.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.fehbvm.com/Article/details/gwrflcefv.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.zdbjq.cn/Article/details/gmbjfnbsp.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.fehbvm.com/Article/details/gdaxnlvuw.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.fehbvm.com/Article/details/gzebjsfls.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.hesvh.cn/Article/details/gpkwrqrop.sHtML

TS:   s.split(",")
来源：http://baike.zdbjq.cn/Article/details/gqwrhkvzh.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.hesvh.cn/Article/details/gbbogqjou.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.zdbjq.cn/Article/details/gmkhrhzgh.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.hesvh.cn/Article/details/gtequqsbh.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.fehbvm.com/Article/details/gkgzsppkp.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.fehbvm.com/Article/details/gnokjzxob.sHtML

Py:   ",".join(items)
来源：http://3g.hesvh.cn/Article/details/gtjqdcifb.sHtML

PHP:  implode(",", $items);
来源：http://m.share.zdbjq.cn/Article/details/gkfrubkno.sHtML

JS:   items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gechfegrd.sHtML

TS:   items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gbyfmqivu.sHtML

Java: String.join(",", items)
来源：http://blog.hesvh.cn/Article/details/gkgskqudx.sHtML


<!-- 参考信息 -->