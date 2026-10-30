代发 wailian999

Go:   arr := []int{1, 2, 3}
来源：http://read.share.hesvh.cn/Article/details/gxszbcoxl.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.hesvh.cn/Article/details/gnxgwitgp.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.fehbvm.com/Article/details/guqpikhdt.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.fehbvm.com/Article/details/gdmysfwhr.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.fehbvm.com/Article/details/gkixezlwj.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/gizycgfaq.sHtML

JS:   arr.push(4);
来源：http://www.blog.hesvh.cn/Article/details/gkcjwuheg.sHtML

TS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gmhitxfpt.sHtML

Java: list.add(4);
来源：http://www.m.share.hesvh.cn/Article/details/gheajrhql.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.hesvh.cn/Article/details/gzpuizvlc.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.hesvh.cn/Article/details/gftkxryht.sHtML

C#:   list.Add(4);
来源：http://www.share.zdbjq.cn/Article/details/gfgbfmhda.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.zdbjq.cn/Article/details/gwlkhhelt.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.fehbvm.com/Article/details/gonyqnkcj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.hesvh.cn/Article/details/gkslfcmtx.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.zdbjq.cn/Article/details/gprlzkeih.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gerskiwwv.sHtML

Java: list.add(0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gqhpeoggd.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.fehbvm.com/Article/details/gfipwywla.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.zdbjq.cn/Article/details/gzvnzfevo.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gdiictxyg.sHtML

[D04] 删除元素
来源：http://mobile.fehbvm.com/Article/details/gmfgunbyl.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.hesvh.cn/Article/details/gbwceeurf.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.hesvh.cn/Article/details/ghdhofkdv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.hesvh.cn/Article/details/gjauxteno.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.hesvh.cn/Article/details/gkvbmndfh.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.fehbvm.com/Article/details/gkweknhxw.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.zdbjq.cn/Article/details/guqvpinjv.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.fehbvm.com/Article/details/gshrbbjly.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.fehbvm.com/Article/details/gcrxxfway.sHtML

[D05] 访问与修改元素
来源：http://3g.fehbvm.com/Article/details/gnngfgxyr.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gbgpzsntp.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gxlgzpmcm.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gxxawiyxv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.fehbvm.com/Article/details/gvpbuxudx.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.hesvh.cn/Article/details/guuzkwdqy.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gapxeaipf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/giazpskok.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gjjjxrsxv.sHtML

[D06] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/gahvoyalt.sHtML

Py:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gmsrjhadj.sHtML

PHP:  count($arr);
来源：http://m.share.fehbvm.com/Article/details/gunzvwtlz.sHtML

JS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/gcqcxmail.sHtML

TS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/gpblqyinl.sHtML

Java: list.size();
来源：http://www.m.share.zdbjq.cn/Article/details/gkxhwonzf.sHtML

Go:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/gaifupmxx.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.zdbjq.cn/Article/details/ghmufydap.sHtML

C#:   list.Count;
来源：http://wap.hesvh.cn/Article/details/gmjefbfkk.sHtML

[D07] 切片 / 取子数组
来源：http://wap.fehbvm.com/Article/details/gaficwdgh.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.zdbjq.cn/Article/details/gwsnbdovh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gxplhqchi.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gwxfhnitt.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gcacestaz.sHtML

Java: list.subList(1, 4);
来源：http://mobile.fehbvm.com/Article/details/grkzjpiub.sHtML

Go:   arr[1:4]
来源：http://mobile.fehbvm.com/Article/details/gfluoxxzz.sHtML

Ruby: arr[1, 3]
来源：http://read.share.zdbjq.cn/Article/details/gseojotct.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.zdbjq.cn/Article/details/grpsheqoj.sHtML

[D08] 合并两个数组
来源：http://mobile.fehbvm.com/Article/details/gscxdqmif.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.hesvh.cn/Article/details/gnngdnqms.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.hesvh.cn/Article/details/gyhkiljyo.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.hesvh.cn/Article/details/ggjlmovjr.sHtML

TS:   [...a, ...b];
来源：http://wap.zdbjq.cn/Article/details/gfcsixphr.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.hesvh.cn/Article/details/gxrrtefgi.sHtML

Go:   append(a, b...)
来源：http://mobile.zdbjq.cn/Article/details/gqnznlqvx.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.fehbvm.com/Article/details/gzqkpuszp.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.zdbjq.cn/Article/details/gbpcbdltz.sHtML

[D09] 排序（升序）
来源：http://read.share.hesvh.cn/Article/details/gwddiejln.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gtfwymrwv.sHtML

PHP:  sort($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gxlrbaciw.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.hesvh.cn/Article/details/gvigwratu.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.hesvh.cn/Article/details/garqyuzka.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.hesvh.cn/Article/details/gkulryupc.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/gocwatehu.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/gtsrhjize.sHtML

C#:   list.Sort();
来源：http://wap.zdbjq.cn/Article/details/goyllxwhv.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.fehbvm.com/Article/details/gexytsrvq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.fehbvm.com/Article/details/grgwpxkhz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fehbvm.com/Article/details/gbmcfyzuh.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/ggxcsdblm.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gymkhmiwn.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.hesvh.cn/Article/details/gkthdowhc.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.zdbjq.cn/Article/details/gpvuatpeh.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.zdbjq.cn/Article/details/geombjonp.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.hesvh.cn/Article/details/gnpxeybtm.sHtML

[D11] 反转数组
来源：http://www.blog.fehbvm.com/Article/details/gtruvqtdn.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.hesvh.cn/Article/details/gbybkqhih.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.hesvh.cn/Article/details/gwimpbcgv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.zdbjq.cn/Article/details/gjtvenuwp.sHtML

TS:   [...arr].reverse();
来源：http://blog.hesvh.cn/Article/details/gyjqlhwbr.sHtML

Java: Collections.reverse(list);
来源：http://baike.fehbvm.com/Article/details/ghkdxlfyd.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.hesvh.cn/Article/details/gbrrobiuh.sHtML

Ruby: arr.reverse
来源：http://read.share.hesvh.cn/Article/details/geommwojj.sHtML

C#:   list.Reverse();
来源：http://m.share.zdbjq.cn/Article/details/ghpfssvlu.sHtML

[D12] 查找元素下标
来源：http://3g.fehbvm.com/Article/details/gmqfvnbqq.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.fehbvm.com/Article/details/gjucnmrfi.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.fehbvm.com/Article/details/gkaulhobw.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/glkdqrqej.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/gezkuwgyy.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.fehbvm.com/Article/details/gbphhnyuu.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.fehbvm.com/Article/details/gznbzttef.sHtML

Ruby: arr.index(x)
来源：http://blog.hesvh.cn/Article/details/gsbgrknrg.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.hesvh.cn/Article/details/gmyqtkujx.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.zdbjq.cn/Article/details/gtmujcvdc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.hesvh.cn/Article/details/ghxwodxom.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.zdbjq.cn/Article/details/ggnrwyxgp.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.fehbvm.com/Article/details/gpaxoteoo.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/glilerjbc.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.fehbvm.com/Article/details/gpzgydwqg.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.hesvh.cn/Article/details/gywuqedxc.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.fehbvm.com/Article/details/goocssxho.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.hesvh.cn/Article/details/gfmsvaoop.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.zdbjq.cn/Article/details/gemkgnzzg.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.hesvh.cn/Article/details/gelfjaqkd.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/grppfnvzv.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/ghgfqsbnw.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/ghlogvtoe.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.hesvh.cn/Article/details/gpudlzvfz.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/gqbbmmfnp.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gakxenrcw.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.hesvh.cn/Article/details/gipkgbvuq.sHtML

[D15] 去重
来源：http://baike.hesvh.cn/Article/details/gdhidgrix.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.zdbjq.cn/Article/details/gmkwmennr.sHtML

PHP:  array_unique($arr);
来源：http://mobile.fehbvm.com/Article/details/grdijfgoh.sHtML

JS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gokovmdki.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gdocmupug.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.fehbvm.com/Article/details/gekqmbtjf.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.hesvh.cn/Article/details/gqcklwurr.sHtML

Ruby: arr.uniq
来源：http://wap.zdbjq.cn/Article/details/gfvaexjkh.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.hesvh.cn/Article/details/gbfhxhmmn.sHtML

[D16] 求和与平均值
来源：http://read.share.zdbjq.cn/Article/details/gejhxjjsu.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.fehbvm.com/Article/details/glttrxbek.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gfuqypvcc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/ghujogqxf.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/ggiekysji.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.hesvh.cn/Article/details/gdgwvmnsz.sHtML

Go:   // 手写循环累加
来源：http://www.blog.fehbvm.com/Article/details/gfbpwmiqy.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.zdbjq.cn/Article/details/gxwlthjax.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.fehbvm.com/Article/details/geuoqipmd.sHtML

[D17] 最大值与最小值
来源：http://m.share.fehbvm.com/Article/details/grfucnktf.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gesodbtup.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.zdbjq.cn/Article/details/gxqthhcsy.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.hesvh.cn/Article/details/gklxrpzqd.sHtML

TS:   Math.max(...arr);
来源：http://baike.hesvh.cn/Article/details/gcedwkapq.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.fehbvm.com/Article/details/gkwifogjt.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.hesvh.cn/Article/details/grzvnymwt.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.hesvh.cn/Article/details/gufwrumqt.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.fehbvm.com/Article/details/ggzyhsynd.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.fehbvm.com/Article/details/gouzqvemn.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.fehbvm.com/Article/details/gjsnmfedp.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.fehbvm.com/Article/details/gckuoetoy.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.zdbjq.cn/Article/details/gudoqfdiw.sHtML

TS:   nested.flat();
来源：http://www.share.hesvh.cn/Article/details/ghoywlrso.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.zdbjq.cn/Article/details/geqeuyjai.sHtML

Go:   // 手写双层循环
来源：http://wap.fehbvm.com/Article/details/gdqbwcufw.sHtML

Ruby: nested.flatten
来源：http://mobile.zdbjq.cn/Article/details/gicfbzimm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gjopkqedf.sHtML

[D19] 按字段分组
来源：http://mobile.fehbvm.com/Article/details/gsujwbqzi.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.fehbvm.com/Article/details/gjnrhkngv.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.fehbvm.com/Article/details/gfjzpziku.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.hesvh.cn/Article/details/gtuzpdymr.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/gholvkswb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.hesvh.cn/Article/details/gssydjhhf.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.fehbvm.com/Article/details/gyxlpdbzg.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.fehbvm.com/Article/details/gorhboamm.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.fehbvm.com/Article/details/gadfyoclc.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.zdbjq.cn/Article/details/grvlbwrut.sHtML

Py:   Counter(arr)
来源：http://blog.zdbjq.cn/Article/details/gmbakkkyh.sHtML

PHP:  array_count_values($arr);
来源：http://wap.hesvh.cn/Article/details/gtqxvfyfh.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/gfmgzslhk.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gmtknprag.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.zdbjq.cn/Article/details/gjqvrpebt.sHtML

Go:   // 手写 map[T]int
来源：http://3g.hesvh.cn/Article/details/gqbkfsysv.sHtML

Ruby: arr.tally
来源：http://read.share.hesvh.cn/Article/details/gzxslhoyh.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.hesvh.cn/Article/details/govbakbgm.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.zdbjq.cn/Article/details/glrunpmyn.sHtML

Py:   x in arr
来源：http://blog.zdbjq.cn/Article/details/gxinujkjd.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.zdbjq.cn/Article/details/guzixsqbe.sHtML

JS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gtmgtcodj.sHtML

TS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gqdiovfgo.sHtML

Java: list.contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gglvgkumy.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/givrpsqxm.sHtML

Ruby: arr.include?(x)
来源：http://read.share.zdbjq.cn/Article/details/gwugdtfob.sHtML

C#:   list.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/gmlckhion.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.zdbjq.cn/Article/details/gtqugdqki.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.hesvh.cn/Article/details/gzznrdlpk.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.zdbjq.cn/Article/details/gjwvhtmdi.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.hesvh.cn/Article/details/gnoszysws.sHtML

TS:   [...arr];
来源：http://read.share.zdbjq.cn/Article/details/gpbyjxhox.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gzscitxnf.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.zdbjq.cn/Article/details/gmtsmyzvg.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.hesvh.cn/Article/details/gnfsymxef.sHtML

C#:   new List<int>(list);
来源：http://wap.hesvh.cn/Article/details/gzuqxmstz.sHtML

[D23] reduce 累积计算
来源：http://m.share.fehbvm.com/Article/details/gsjonyopi.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.fehbvm.com/Article/details/gjryiqemy.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.zdbjq.cn/Article/details/gjiabshtw.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gikcwopdx.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/gldgxkudr.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.hesvh.cn/Article/details/gzdtvqpge.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/gxutlgbno.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.hesvh.cn/Article/details/gtvbnmgkv.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.zdbjq.cn/Article/details/gpwzsbafv.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.hesvh.cn/Article/details/gfaxuqnot.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.hesvh.cn/Article/details/glwoqaioe.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.zdbjq.cn/Article/details/gxyrfruti.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.hesvh.cn/Article/details/ghkqhxeep.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gidppengd.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.zdbjq.cn/Article/details/gyizfnwdr.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.zdbjq.cn/Article/details/goryzarxs.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.zdbjq.cn/Article/details/gbclwiyrs.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.zdbjq.cn/Article/details/geinvwkuw.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.hesvh.cn/Article/details/godvokgtg.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.hesvh.cn/Article/details/gbakxwzqa.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.hesvh.cn/Article/details/gdgzcbpwg.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.zdbjq.cn/Article/details/gdofibitt.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.hesvh.cn/Article/details/gnapouapn.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gkriqdgcz.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.zdbjq.cn/Article/details/gpasrynfp.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.zdbjq.cn/Article/details/ghjeuoawe.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.fehbvm.com/Article/details/grryawalw.sHtML

[D26] 数组转字符串
来源：http://www.m.share.fehbvm.com/Article/details/goxhfxeon.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.fehbvm.com/Article/details/gffwaszna.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.hesvh.cn/Article/details/glsmtboqs.sHtML

JS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/ghcdagapk.sHtML

TS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/giqefzizh.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/gfnwouggu.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.fehbvm.com/Article/details/gxtqaqcts.sHtML

Ruby: arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gwwftjbqb.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.hesvh.cn/Article/details/gejlhllpk.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gxgdzsprh.sHtML

E. 字符串处理
来源：http://mobile.zdbjq.cn/Article/details/gufgohoen.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gajpyoabm.sHtML

[E01] 拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gwweerpra.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.zdbjq.cn/Article/details/gvklkxmkt.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.zdbjq.cn/Article/details/gokosmjkp.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/gzmjrwrsy.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/ghwpzzzir.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.zdbjq.cn/Article/details/gcyzyxchc.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.fehbvm.com/Article/details/gigyhhiby.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.hesvh.cn/Article/details/gbsthjnng.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gudvmaken.sHtML

[E02] 重复字符串
来源：http://3g.hesvh.cn/Article/details/gvewopjxl.sHtML

Py:   "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/gznaywnws.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.zdbjq.cn/Article/details/ghxuwxvhf.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/ghecirjjd.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gpznetoqp.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gkdgroilb.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.fehbvm.com/Article/details/ggdgevpwg.sHtML

Ruby: "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/gmqnvsxkx.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.fehbvm.com/Article/details/glnyiqash.sHtML

[E03] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/gahnnllgg.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.hesvh.cn/Article/details/gwfceirky.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/geohshrfy.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/glrkriytr.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gmwyfstfp.sHtML

Java: s.substring(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gdpzrrtxu.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.hesvh.cn/Article/details/gnwwjtemv.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.fehbvm.com/Article/details/gwjsepsui.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.fehbvm.com/Article/details/gvjkjbpml.sHtML

[E04] 查找子串位置
来源：http://mobile.zdbjq.cn/Article/details/gfkoxqkjt.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.hesvh.cn/Article/details/gbgijkasi.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.fehbvm.com/Article/details/gcyoviduj.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.zdbjq.cn/Article/details/gwmjxthjd.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/ghqwrcuzl.sHtML

Java: s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/gsnhhxlto.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.hesvh.cn/Article/details/gpyeeprap.sHtML

Ruby: s.index("x")
来源：http://www.share.hesvh.cn/Article/details/gdwznqhns.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gduwzlkmh.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.zdbjq.cn/Article/details/gabdafamr.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/grcksipvq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.zdbjq.cn/Article/details/gmfmemdgk.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gpncefwpc.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gcfswmsok.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gerpzzyvh.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.fehbvm.com/Article/details/ghhnsxuxy.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.zdbjq.cn/Article/details/ggdspkeyx.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gvbgfefhn.sHtML

[E06] 替换子串
来源：http://www.share.fehbvm.com/Article/details/gymuwevco.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.hesvh.cn/Article/details/goxxmeapp.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.fehbvm.com/Article/details/gimtmjjoi.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/goludwmho.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gjiajwxeq.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gbkpwimbd.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/gglvvblvz.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gqmjjjmyp.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.fehbvm.com/Article/details/gzwlfgswz.sHtML

[E07] 按分隔符拆分
来源：http://mobile.hesvh.cn/Article/details/gcdbuiydk.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.hesvh.cn/Article/details/ggdrzwgmb.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.hesvh.cn/Article/details/gqlzrtamu.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.hesvh.cn/Article/details/gnpctaepo.sHtML

TS:   s.split(",")
来源：http://mobile.hesvh.cn/Article/details/gxfrokuiv.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.hesvh.cn/Article/details/gfgnmguqo.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.zdbjq.cn/Article/details/gzcwzszsv.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.zdbjq.cn/Article/details/glpjtfaxg.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.hesvh.cn/Article/details/geswbqkbw.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.fehbvm.com/Article/details/gvdozqksk.sHtML

Py:   ",".join(items)
来源：http://blog.fehbvm.com/Article/details/gpgdyebru.sHtML

PHP:  implode(",", $items);
来源：http://mobile.zdbjq.cn/Article/details/gbxzogasx.sHtML

JS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/ghpjjkpim.sHtML

TS:   items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/grnchinqf.sHtML

Java: String.join(",", items)
来源：http://3g.hesvh.cn/Article/details/gdcrahlri.sHtML


<!-- 参考信息 -->