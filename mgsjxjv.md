代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.zdbjq.cn/Article/details/gdbgjqkyb.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.hesvh.cn/Article/details/gjbckgbcx.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.hesvh.cn/Article/details/gfrdaxaoj.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.zdbjq.cn/Article/details/gbmigzgac.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.hesvh.cn/Article/details/gvxreqwgo.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.zdbjq.cn/Article/details/gaidebxfe.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.fehbvm.com/Article/details/godqtwmwt.sHtML

[D02] 追加元素到末尾
来源：http://mobile.fehbvm.com/Article/details/gjspjkgfu.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.hesvh.cn/Article/details/gsuqgrihw.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.fehbvm.com/Article/details/gzjndlgei.sHtML

JS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gdjnnsocg.sHtML

TS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/ghzxwhbnv.sHtML

Java: list.add(4);
来源：http://baike.fehbvm.com/Article/details/gxhubczzd.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.fehbvm.com/Article/details/golmdyael.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.zdbjq.cn/Article/details/gywcfzbzu.sHtML

C#:   list.Add(4);
来源：http://read.share.zdbjq.cn/Article/details/gebctgzor.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.hesvh.cn/Article/details/gkcjksatr.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.zdbjq.cn/Article/details/gcpedgbkp.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.hesvh.cn/Article/details/goasvbaax.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.fehbvm.com/Article/details/gbxiwzktn.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.fehbvm.com/Article/details/gosmruwcl.sHtML

Java: list.add(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/ggdtdclps.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.hesvh.cn/Article/details/gakudfquo.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.fehbvm.com/Article/details/gviethihd.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.hesvh.cn/Article/details/gzsncbinn.sHtML

[D04] 删除元素
来源：http://mobile.hesvh.cn/Article/details/gwqddknfb.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.hesvh.cn/Article/details/gsqdbnsvr.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.fehbvm.com/Article/details/guoieyupg.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.fehbvm.com/Article/details/gkvuywbih.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gobtwbuge.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.fehbvm.com/Article/details/gpdtaitep.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.hesvh.cn/Article/details/gbytrfwlv.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.zdbjq.cn/Article/details/gyxotyjaq.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.zdbjq.cn/Article/details/gljszbtnj.sHtML

[D05] 访问与修改元素
来源：http://mobile.hesvh.cn/Article/details/gxiyqmkxl.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gbwrcacdx.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gecjoazly.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gkocythxk.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.fehbvm.com/Article/details/gizdqfbac.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.zdbjq.cn/Article/details/gdltbsell.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gkmbutxfl.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gkfblwrua.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gsiumiqyt.sHtML

[D06] 数组长度
来源：http://baike.hesvh.cn/Article/details/gpitjvoxf.sHtML

Py:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gcxqontqe.sHtML

PHP:  count($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gvlqymcrv.sHtML

JS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/gqiidhwxd.sHtML

TS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gixrnenef.sHtML

Java: list.size();
来源：http://mobile.zdbjq.cn/Article/details/gngmnrdnm.sHtML

Go:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/ggpljnolc.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.zdbjq.cn/Article/details/gbglrjfqj.sHtML

C#:   list.Count;
来源：http://www.blog.hesvh.cn/Article/details/gugdofmqr.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.fehbvm.com/Article/details/gmdwdjtsh.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.hesvh.cn/Article/details/gaebxnrmz.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.zdbjq.cn/Article/details/gouooclyf.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gesytxtfu.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/ggczkeyna.sHtML

Java: list.subList(1, 4);
来源：http://3g.hesvh.cn/Article/details/gdarzagxr.sHtML

Go:   arr[1:4]
来源：http://blog.fehbvm.com/Article/details/gcudhrwky.sHtML

Ruby: arr[1, 3]
来源：http://mobile.fehbvm.com/Article/details/gncqpurdr.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gonbhcpjh.sHtML

[D08] 合并两个数组
来源：http://www.m.share.hesvh.cn/Article/details/gpaqginrm.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.hesvh.cn/Article/details/gsekgetzb.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.zdbjq.cn/Article/details/gnzsuimqk.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.hesvh.cn/Article/details/gctdvnipr.sHtML

TS:   [...a, ...b];
来源：http://blog.zdbjq.cn/Article/details/gkzpeztqb.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.hesvh.cn/Article/details/gfjarrkyf.sHtML

Go:   append(a, b...)
来源：http://blog.fehbvm.com/Article/details/ginnhafku.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.zdbjq.cn/Article/details/gbelkbpbj.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.hesvh.cn/Article/details/gcszstung.sHtML

[D09] 排序（升序）
来源：http://www.m.share.hesvh.cn/Article/details/gcylotbsw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.zdbjq.cn/Article/details/gavvvohku.sHtML

PHP:  sort($arr);
来源：http://baike.hesvh.cn/Article/details/grlwyvexw.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.hesvh.cn/Article/details/gsjmgbfix.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.fehbvm.com/Article/details/gsrsunjvk.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.zdbjq.cn/Article/details/gnycsnuii.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/gxqpsebyu.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gyozwbwwq.sHtML

C#:   list.Sort();
来源：http://m.share.fehbvm.com/Article/details/gmrszddzh.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.hesvh.cn/Article/details/gmfqdrgfs.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.hesvh.cn/Article/details/gvneqmbso.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/gxsfbeeug.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/ggoeovrwp.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gmfcqsrpg.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.zdbjq.cn/Article/details/glxdvfnxl.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.hesvh.cn/Article/details/gitwtxxok.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.hesvh.cn/Article/details/glxzudela.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.fehbvm.com/Article/details/glbnbrfii.sHtML

[D11] 反转数组
来源：http://read.share.fehbvm.com/Article/details/gamvrzdea.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.zdbjq.cn/Article/details/gxmyxdeqq.sHtML

PHP:  array_reverse($arr);
来源：http://baike.hesvh.cn/Article/details/gpxikdxai.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.hesvh.cn/Article/details/gpounfaqz.sHtML

TS:   [...arr].reverse();
来源：http://mobile.hesvh.cn/Article/details/gvjfbbmig.sHtML

Java: Collections.reverse(list);
来源：http://baike.fehbvm.com/Article/details/grvscwjqr.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.zdbjq.cn/Article/details/gtcmkzlak.sHtML

Ruby: arr.reverse
来源：http://m.share.hesvh.cn/Article/details/gmrxscldn.sHtML

C#:   list.Reverse();
来源：http://www.blog.hesvh.cn/Article/details/gdlpwsroo.sHtML

[D12] 查找元素下标
来源：http://mobile.hesvh.cn/Article/details/gwlwvacbr.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.hesvh.cn/Article/details/ghkomhowr.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.fehbvm.com/Article/details/ggrcizrxm.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/gysguywzy.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fehbvm.com/Article/details/grslrrpja.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.zdbjq.cn/Article/details/gkvqegtqd.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.hesvh.cn/Article/details/gcttqsyoo.sHtML

Ruby: arr.index(x)
来源：http://mobile.zdbjq.cn/Article/details/gfjnfevad.sHtML

C#:   list.IndexOf(x);
来源：http://baike.hesvh.cn/Article/details/gsbtbvijj.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.hesvh.cn/Article/details/gfvjibbjh.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.hesvh.cn/Article/details/gmlmfccet.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.fehbvm.com/Article/details/gqjqvmlgm.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/ghmhnwgcs.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gnzutkpen.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.zdbjq.cn/Article/details/gccawneld.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.hesvh.cn/Article/details/gfsamujis.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.zdbjq.cn/Article/details/gskysejho.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gnuapjzmi.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.zdbjq.cn/Article/details/gtdfosaek.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.hesvh.cn/Article/details/gzkopsung.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.fehbvm.com/Article/details/gvcqlhqme.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/gctctglcn.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gksedqcoo.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.fehbvm.com/Article/details/glspjqeix.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gfrnmkayd.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/glgzcefmq.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.fehbvm.com/Article/details/gextyulua.sHtML

[D15] 去重
来源：http://wap.hesvh.cn/Article/details/gykopfvji.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/gjpctgbmz.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gzvubqlle.sHtML

JS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gdvpbdogb.sHtML

TS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/goqasozpi.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.zdbjq.cn/Article/details/glnikmjfe.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.hesvh.cn/Article/details/gjlhkyaii.sHtML

Ruby: arr.uniq
来源：http://mobile.zdbjq.cn/Article/details/gywpnarvx.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/giciupsxn.sHtML

[D16] 求和与平均值
来源：http://blog.zdbjq.cn/Article/details/gadyfljab.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.fehbvm.com/Article/details/gvtfuljlw.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.zdbjq.cn/Article/details/gvresvsil.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/gvcdtftbu.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/gvarytydh.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.fehbvm.com/Article/details/gogvnzlrg.sHtML

Go:   // 手写循环累加
来源：http://wap.zdbjq.cn/Article/details/gxgjwobzn.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.zdbjq.cn/Article/details/grhqtmytm.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.fehbvm.com/Article/details/gsslwwygd.sHtML

[D17] 最大值与最小值
来源：http://wap.hesvh.cn/Article/details/glzfjqsdj.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gecsbovzp.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.fehbvm.com/Article/details/gvdknunsq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.zdbjq.cn/Article/details/gmdbwriap.sHtML

TS:   Math.max(...arr);
来源：http://www.share.hesvh.cn/Article/details/gmsfefjub.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.zdbjq.cn/Article/details/guheicdcf.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.zdbjq.cn/Article/details/grlgxgwsl.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.hesvh.cn/Article/details/gigptdeez.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.hesvh.cn/Article/details/gytlkeybq.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.zdbjq.cn/Article/details/gvpguaola.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.fehbvm.com/Article/details/gkrfgnqid.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.zdbjq.cn/Article/details/gsmzikkbp.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.hesvh.cn/Article/details/gjpnsnclb.sHtML

TS:   nested.flat();
来源：http://www.blog.zdbjq.cn/Article/details/ggznczbvy.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gatiskrah.sHtML

Go:   // 手写双层循环
来源：http://mobile.hesvh.cn/Article/details/gtbeasqzx.sHtML

Ruby: nested.flatten
来源：http://wap.hesvh.cn/Article/details/gebzrwstu.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.fehbvm.com/Article/details/gqiskqbxq.sHtML

[D19] 按字段分组
来源：http://www.share.hesvh.cn/Article/details/gztfitbis.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.fehbvm.com/Article/details/glgzmaqlp.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.hesvh.cn/Article/details/geshvljbu.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.zdbjq.cn/Article/details/gvhvkphxb.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.fehbvm.com/Article/details/gaguxwlat.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.fehbvm.com/Article/details/gydmuhntw.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.fehbvm.com/Article/details/gjhxdbuiz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.zdbjq.cn/Article/details/ggehneued.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.zdbjq.cn/Article/details/gmekvnbhm.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.fehbvm.com/Article/details/gngnkmvpm.sHtML

Py:   Counter(arr)
来源：http://mobile.hesvh.cn/Article/details/ggiacwsna.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.zdbjq.cn/Article/details/gdacbdwgu.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/gujcwmzak.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/gvvefdeto.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.hesvh.cn/Article/details/gbtbjzyin.sHtML

Go:   // 手写 map[T]int
来源：http://blog.zdbjq.cn/Article/details/gdelvmfuq.sHtML

Ruby: arr.tally
来源：http://mobile.hesvh.cn/Article/details/gqgqxhwmo.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.hesvh.cn/Article/details/gmxroldpb.sHtML

[D21] 判断是否包含某元素
来源：http://3g.hesvh.cn/Article/details/gadikggxh.sHtML

Py:   x in arr
来源：http://www.share.zdbjq.cn/Article/details/gelsdjfwn.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.hesvh.cn/Article/details/gthdqzaiu.sHtML

JS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/godkjpmrp.sHtML

TS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gzifcytza.sHtML

Java: list.contains(x)
来源：http://blog.zdbjq.cn/Article/details/gbplsrbmp.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gijebznai.sHtML

Ruby: arr.include?(x)
来源：http://baike.zdbjq.cn/Article/details/gsaalexbz.sHtML

C#:   list.Contains(x)
来源：http://read.share.fehbvm.com/Article/details/gpwwbkwpt.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.zdbjq.cn/Article/details/ghghdjriz.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.hesvh.cn/Article/details/gqsevtpan.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.zdbjq.cn/Article/details/gittgatnk.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.hesvh.cn/Article/details/guuimwjdf.sHtML

TS:   [...arr];
来源：http://read.share.zdbjq.cn/Article/details/glziqafia.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.zdbjq.cn/Article/details/gicwxukaq.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.hesvh.cn/Article/details/gdfmxcdex.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.fehbvm.com/Article/details/gjgtwjwmd.sHtML

C#:   new List<int>(list);
来源：http://blog.zdbjq.cn/Article/details/gtqwoswmi.sHtML

[D23] reduce 累积计算
来源：http://wap.zdbjq.cn/Article/details/gwwahtyfa.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.hesvh.cn/Article/details/glsagzhiu.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.zdbjq.cn/Article/details/gccydnprb.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.hesvh.cn/Article/details/gnzkqazoj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gtnjtlfur.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.fehbvm.com/Article/details/ggpnfdofg.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/gcatrxjpx.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.zdbjq.cn/Article/details/gczneqrsb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.hesvh.cn/Article/details/gvuvsyqdc.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.zdbjq.cn/Article/details/gtsxpdaez.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.fehbvm.com/Article/details/gwrxcabuv.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.fehbvm.com/Article/details/gkxmlgmsd.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.hesvh.cn/Article/details/gxtmiknlx.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.hesvh.cn/Article/details/gtdtyflkh.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.hesvh.cn/Article/details/gbbwnbedu.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.hesvh.cn/Article/details/ghljgsxfq.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.zdbjq.cn/Article/details/gymfycvmy.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.fehbvm.com/Article/details/givgdwttv.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.fehbvm.com/Article/details/guqbaeprs.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.zdbjq.cn/Article/details/guqyytzkn.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.fehbvm.com/Article/details/gqysbhmvh.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.zdbjq.cn/Article/details/gphxbipul.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.fehbvm.com/Article/details/gcazxmfud.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.hesvh.cn/Article/details/gliowmnqp.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.hesvh.cn/Article/details/gpvytdeoc.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gsolgatxx.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gulikaaxz.sHtML

[D26] 数组转字符串
来源：http://3g.zdbjq.cn/Article/details/gvgrbbvss.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.zdbjq.cn/Article/details/gknchmvez.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.hesvh.cn/Article/details/gipysklwf.sHtML

JS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gujkjgxxu.sHtML

TS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/giwzsnubr.sHtML

Java: String.join(", ", list)
来源：http://blog.hesvh.cn/Article/details/gmhjlcyvf.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.fehbvm.com/Article/details/gttohgafq.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gqydphvci.sHtML

C#:   string.Join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/ghzvgqgxb.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gawyappdr.sHtML

E. 字符串处理
来源：http://read.share.fehbvm.com/Article/details/gmhwgxsya.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gbkazteul.sHtML

[E01] 拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/giuweeyab.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.hesvh.cn/Article/details/globbkdsy.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.hesvh.cn/Article/details/gmgwvundl.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/gifntbuqi.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gzxsjqtdx.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.hesvh.cn/Article/details/gpsqsmein.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.zdbjq.cn/Article/details/gywwnqlfv.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.fehbvm.com/Article/details/gsrfphihn.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.hesvh.cn/Article/details/gnehfeyxj.sHtML

[E02] 重复字符串
来源：http://www.blog.hesvh.cn/Article/details/gpueyokik.sHtML

Py:   "ab" * 3
来源：http://3g.hesvh.cn/Article/details/gewfkmqwc.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.zdbjq.cn/Article/details/gqhxteltf.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gedqykzgm.sHtML

TS:   "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gbqowvtkz.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gjvhuixty.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.hesvh.cn/Article/details/giqqmtbrx.sHtML

Ruby: "ab" * 3
来源：http://www.share.hesvh.cn/Article/details/ghuwwltrl.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.hesvh.cn/Article/details/gwvojpcnf.sHtML

[E03] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/gyvbcqlrt.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.hesvh.cn/Article/details/gpnkyhhes.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gidbhjvqv.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gtzgxftqr.sHtML

TS:   s.slice(1, 4)
来源：http://blog.hesvh.cn/Article/details/gxucagoqd.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gakylfart.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.hesvh.cn/Article/details/gqapyudva.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.fehbvm.com/Article/details/gfocnzrgx.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.zdbjq.cn/Article/details/gzfnzfwwy.sHtML

[E04] 查找子串位置
来源：http://www.blog.hesvh.cn/Article/details/ggahhmijv.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.fehbvm.com/Article/details/gwvdsdfzk.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.hesvh.cn/Article/details/gqwrekxst.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.fehbvm.com/Article/details/gbapaqhvz.sHtML

TS:   s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gpgzojgfh.sHtML

Java: s.indexOf("x")
来源：http://3g.fehbvm.com/Article/details/gntbtzbht.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.hesvh.cn/Article/details/gptpozira.sHtML

Ruby: s.index("x")
来源：http://www.blog.hesvh.cn/Article/details/gypakupip.sHtML

C#:   s.IndexOf("x")
来源：http://blog.hesvh.cn/Article/details/ghgpklrel.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.fehbvm.com/Article/details/gyuynabrp.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.hesvh.cn/Article/details/gosiymdjv.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.hesvh.cn/Article/details/gudvsjvhw.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/grjvxeiqd.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.zdbjq.cn/Article/details/ggypwigcc.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/gbsnaytpa.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.hesvh.cn/Article/details/gznhycrmy.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.fehbvm.com/Article/details/gdvrdutuf.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.fehbvm.com/Article/details/ghfcrpgld.sHtML

[E06] 替换子串
来源：http://baike.zdbjq.cn/Article/details/gjembcupe.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/gstfaxccd.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.hesvh.cn/Article/details/gmebiqjod.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/ggvacarbc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gnizjjwmh.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gffjwzmrg.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/gjwgjubvp.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gegzrsjla.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gvliwcdej.sHtML

[E07] 按分隔符拆分
来源：http://blog.hesvh.cn/Article/details/gxijfqcvf.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.zdbjq.cn/Article/details/gafytxuxt.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.hesvh.cn/Article/details/gqhlavgsj.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.zdbjq.cn/Article/details/guxmdzelp.sHtML

TS:   s.split(",")
来源：http://read.share.hesvh.cn/Article/details/gmtubflnt.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.zdbjq.cn/Article/details/gehaeysei.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.zdbjq.cn/Article/details/grwwsypoo.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.hesvh.cn/Article/details/goltgttkc.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.zdbjq.cn/Article/details/gfvhscmgy.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.hesvh.cn/Article/details/gmhfjejek.sHtML

Py:   ",".join(items)
来源：http://www.blog.hesvh.cn/Article/details/gpynaqchw.sHtML


<!-- 参考信息 -->