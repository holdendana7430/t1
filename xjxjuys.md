代发 wailian999

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.hesvh.cn/Article/details/ghuikvcgq.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.hesvh.cn/Article/details/geynzucoa.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.fehbvm.com/Article/details/gpoyjybvr.sHtML

[D02] 追加元素到末尾
来源：http://3g.zdbjq.cn/Article/details/gshbvuhuv.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.zdbjq.cn/Article/details/gotinjncf.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.hesvh.cn/Article/details/grdemtevb.sHtML

JS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/ghbopusie.sHtML

TS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/gwzcklnjq.sHtML

Java: list.add(4);
来源：http://wap.hesvh.cn/Article/details/guqxpnosl.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.zdbjq.cn/Article/details/gbrtawdep.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.zdbjq.cn/Article/details/gzygbppoj.sHtML

C#:   list.Add(4);
来源：http://wap.hesvh.cn/Article/details/gjrvsoedo.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.fehbvm.com/Article/details/gmkzwbawa.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.fehbvm.com/Article/details/gozvzoweg.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.hesvh.cn/Article/details/gqukvpqvc.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.fehbvm.com/Article/details/gfcjvuezh.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.zdbjq.cn/Article/details/gwuhagtvl.sHtML

Java: list.add(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/grjzgsofk.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gehzjpihn.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.fehbvm.com/Article/details/gwnrmzisf.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.fehbvm.com/Article/details/gqspipqxw.sHtML

[D04] 删除元素
来源：http://3g.hesvh.cn/Article/details/gfrizbftx.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.zdbjq.cn/Article/details/gsbqpnjmm.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.fehbvm.com/Article/details/gzvkobcby.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.zdbjq.cn/Article/details/gdjjqstce.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.hesvh.cn/Article/details/ghzihpvsz.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.fehbvm.com/Article/details/gfuglqdvg.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.hesvh.cn/Article/details/gtppjnxmp.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.zdbjq.cn/Article/details/gbpboyfei.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.fehbvm.com/Article/details/glgryejlm.sHtML

[D05] 访问与修改元素
来源：http://3g.zdbjq.cn/Article/details/gayqulwad.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gnpwchzvg.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/getyshsaw.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gyfwynrbr.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.zdbjq.cn/Article/details/gmpevjneh.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.hesvh.cn/Article/details/gwqmukzcy.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gbuwrmrmm.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gmyneyubu.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gqvxbxkwh.sHtML

[D06] 数组长度
来源：http://www.share.fehbvm.com/Article/details/gzocaiyae.sHtML

Py:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gwdbkbgji.sHtML

PHP:  count($arr);
来源：http://mobile.fehbvm.com/Article/details/ggmpmaplk.sHtML

JS:   arr.length
来源：http://mobile.fehbvm.com/Article/details/gjqqsstsh.sHtML

TS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/gtjtluemb.sHtML

Java: list.size();
来源：http://baike.hesvh.cn/Article/details/gaflpfwnb.sHtML

Go:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gnrecbgji.sHtML

Ruby: arr.length; arr.size
来源：http://blog.zdbjq.cn/Article/details/gkgvdepla.sHtML

C#:   list.Count;
来源：http://www.m.share.zdbjq.cn/Article/details/gkgapsxkv.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.zdbjq.cn/Article/details/ggvzbpfac.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.hesvh.cn/Article/details/gveiebbzt.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.hesvh.cn/Article/details/gchejwbvz.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/giqycdofd.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/ggrrefttj.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gljbdaflx.sHtML

Go:   arr[1:4]
来源：http://mobile.hesvh.cn/Article/details/gwotecsua.sHtML

Ruby: arr[1, 3]
来源：http://mobile.zdbjq.cn/Article/details/gwrftsalv.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.fehbvm.com/Article/details/gbauumxgl.sHtML

[D08] 合并两个数组
来源：http://read.share.hesvh.cn/Article/details/gvqodpytn.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.hesvh.cn/Article/details/gdjhnafgk.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.zdbjq.cn/Article/details/gtklodbhr.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.fehbvm.com/Article/details/gqlnxeour.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.fehbvm.com/Article/details/ghatkkkwn.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.zdbjq.cn/Article/details/gnwtslhzx.sHtML

Go:   append(a, b...)
来源：http://www.share.hesvh.cn/Article/details/gcldaxvhu.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.zdbjq.cn/Article/details/gjnwehbyx.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.fehbvm.com/Article/details/gisvnlkbk.sHtML

[D09] 排序（升序）
来源：http://3g.hesvh.cn/Article/details/gsdaqbvna.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/gwsqrqeqn.sHtML

PHP:  sort($arr);
来源：http://blog.zdbjq.cn/Article/details/gmnewivte.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.zdbjq.cn/Article/details/gaockxtcj.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.fehbvm.com/Article/details/gxelkyrqv.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.hesvh.cn/Article/details/gngqxeypb.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gxcbnvuut.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gmdpxfbnw.sHtML

C#:   list.Sort();
来源：http://mobile.hesvh.cn/Article/details/gtbecndiq.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.fehbvm.com/Article/details/gjespshhu.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.zdbjq.cn/Article/details/gqmlbmoxx.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/gmcewotef.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/ggjunkgvx.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/gbdaniiov.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.hesvh.cn/Article/details/ggfhneypx.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.fehbvm.com/Article/details/gsduthbwn.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.hesvh.cn/Article/details/gnwmeyxld.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.fehbvm.com/Article/details/gaphlkpoy.sHtML

[D11] 反转数组
来源：http://blog.zdbjq.cn/Article/details/gbojdhjmi.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.fehbvm.com/Article/details/gjaikalmb.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.zdbjq.cn/Article/details/gkrvqdazt.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.hesvh.cn/Article/details/ghveijlmy.sHtML

TS:   [...arr].reverse();
来源：http://www.share.hesvh.cn/Article/details/gwmovuykc.sHtML

Java: Collections.reverse(list);
来源：http://baike.zdbjq.cn/Article/details/geobneohc.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.fehbvm.com/Article/details/ggkrkdmsn.sHtML

Ruby: arr.reverse
来源：http://read.share.hesvh.cn/Article/details/gtnttsger.sHtML

C#:   list.Reverse();
来源：http://mobile.fehbvm.com/Article/details/gaoxsxped.sHtML

[D12] 查找元素下标
来源：http://wap.hesvh.cn/Article/details/gydlyzryj.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.hesvh.cn/Article/details/gbupixldy.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.fehbvm.com/Article/details/golzawdck.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/guoxcsnfs.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gvshmyxkl.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.fehbvm.com/Article/details/grpmuhwba.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gvpulepnu.sHtML

Ruby: arr.index(x)
来源：http://read.share.zdbjq.cn/Article/details/gjdmgvsal.sHtML

C#:   list.IndexOf(x);
来源：http://wap.zdbjq.cn/Article/details/gywefphpj.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.fehbvm.com/Article/details/gigxbxscy.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.zdbjq.cn/Article/details/gkhonnues.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.zdbjq.cn/Article/details/ggdcdeolc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/govpvcoas.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gkurzhqwq.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.fehbvm.com/Article/details/gqvfznfyv.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.fehbvm.com/Article/details/gwwrclczf.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.fehbvm.com/Article/details/gndxaxlwb.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.hesvh.cn/Article/details/gtjnqrxxr.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.zdbjq.cn/Article/details/gqssrlsin.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gcbqkvwcw.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.hesvh.cn/Article/details/ghwxuxmhl.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.hesvh.cn/Article/details/gqfhmupmu.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gdfbmscgu.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.fehbvm.com/Article/details/gdnxntzxg.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gqsvuaqbf.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gafhgdbqf.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gwlhejyna.sHtML

[D15] 去重
来源：http://baike.hesvh.cn/Article/details/gsfhuwkxj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/gechdhcbp.sHtML

PHP:  array_unique($arr);
来源：http://read.share.hesvh.cn/Article/details/gaebexiot.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gxztjfkns.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/guktojvkn.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.zdbjq.cn/Article/details/gaqqbuvfm.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.hesvh.cn/Article/details/ghttkoqsu.sHtML

Ruby: arr.uniq
来源：http://www.share.fehbvm.com/Article/details/gsadojkar.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.hesvh.cn/Article/details/gwzmbtxda.sHtML

[D16] 求和与平均值
来源：http://3g.hesvh.cn/Article/details/gchejhfkj.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.hesvh.cn/Article/details/gotuetmes.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gdafskytx.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/gbeicsebf.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/grhbxxbuy.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.zdbjq.cn/Article/details/gdkczcwec.sHtML

Go:   // 手写循环累加
来源：http://m.share.fehbvm.com/Article/details/gopmmwadd.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.zdbjq.cn/Article/details/geukqvyxp.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.zdbjq.cn/Article/details/gyenjcezh.sHtML

[D17] 最大值与最小值
来源：http://read.share.hesvh.cn/Article/details/glgurpgpi.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.zdbjq.cn/Article/details/gvhvvnxbg.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.hesvh.cn/Article/details/gatbxlroi.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.zdbjq.cn/Article/details/gxqzfnskl.sHtML

TS:   Math.max(...arr);
来源：http://read.share.zdbjq.cn/Article/details/gdgqgtrgl.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.fehbvm.com/Article/details/gwhgpxobg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.hesvh.cn/Article/details/glioambat.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.fehbvm.com/Article/details/gvumdgwhs.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.hesvh.cn/Article/details/gqknypffr.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.hesvh.cn/Article/details/gotoowtwa.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.fehbvm.com/Article/details/gpkhncsmx.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.fehbvm.com/Article/details/geprnwkdk.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.zdbjq.cn/Article/details/gqspumkiy.sHtML

TS:   nested.flat();
来源：http://mobile.zdbjq.cn/Article/details/gokltzdhz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.fehbvm.com/Article/details/ggoxapmyb.sHtML

Go:   // 手写双层循环
来源：http://wap.zdbjq.cn/Article/details/gxlthdkvj.sHtML

Ruby: nested.flatten
来源：http://baike.fehbvm.com/Article/details/gxsspctaq.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gzixnqbwi.sHtML

[D19] 按字段分组
来源：http://blog.hesvh.cn/Article/details/gemjnfnre.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.hesvh.cn/Article/details/gucpzslof.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.fehbvm.com/Article/details/gzsaxpkda.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.zdbjq.cn/Article/details/gnhrbeqph.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.zdbjq.cn/Article/details/gqinlrxql.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.fehbvm.com/Article/details/gqogpgwpf.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.zdbjq.cn/Article/details/gngeyevpt.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.zdbjq.cn/Article/details/gghnaxhgo.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.hesvh.cn/Article/details/ghokogmji.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.hesvh.cn/Article/details/gjikslnpp.sHtML

Py:   Counter(arr)
来源：http://www.share.fehbvm.com/Article/details/geqvinrim.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gqttwcbiq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gciqpmpsa.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/gaxxjopks.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.zdbjq.cn/Article/details/giovhmaoc.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.fehbvm.com/Article/details/gnqjkpzuq.sHtML

Ruby: arr.tally
来源：http://www.m.share.hesvh.cn/Article/details/gebkjibtc.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.hesvh.cn/Article/details/glalxusat.sHtML

[D21] 判断是否包含某元素
来源：http://wap.zdbjq.cn/Article/details/gksfbebss.sHtML

Py:   x in arr
来源：http://mobile.zdbjq.cn/Article/details/gkjzxjivk.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.fehbvm.com/Article/details/gsfxaegzc.sHtML

JS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gkihmqqfq.sHtML

TS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gfjxppbel.sHtML

Java: list.contains(x)
来源：http://www.share.hesvh.cn/Article/details/gugvoregn.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gcqxmyltq.sHtML

Ruby: arr.include?(x)
来源：http://read.share.fehbvm.com/Article/details/gghychvpg.sHtML

C#:   list.Contains(x)
来源：http://3g.zdbjq.cn/Article/details/gqdhovvxx.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.fehbvm.com/Article/details/gedlixvgs.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.fehbvm.com/Article/details/gxwsunozk.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.hesvh.cn/Article/details/gjzpyfhfi.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.zdbjq.cn/Article/details/gxteipswv.sHtML

TS:   [...arr];
来源：http://blog.hesvh.cn/Article/details/gljketjik.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.fehbvm.com/Article/details/gwxvyuguw.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.hesvh.cn/Article/details/ganupeqvo.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.fehbvm.com/Article/details/gukliuebt.sHtML

C#:   new List<int>(list);
来源：http://wap.hesvh.cn/Article/details/gpofuwpma.sHtML

[D23] reduce 累积计算
来源：http://wap.hesvh.cn/Article/details/gtoimnhsx.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.fehbvm.com/Article/details/gcqbrqbjk.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.hesvh.cn/Article/details/gklcbmnrm.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/gvgtlmsee.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/gvshouslc.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.fehbvm.com/Article/details/gzuzzfgby.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/gxwtumxyh.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.hesvh.cn/Article/details/gjyvotjlt.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fehbvm.com/Article/details/gbmylyspo.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.hesvh.cn/Article/details/gjangxmck.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.zdbjq.cn/Article/details/gfmgoqcgu.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.zdbjq.cn/Article/details/gidfhwfre.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.hesvh.cn/Article/details/gbbfwgtlm.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.hesvh.cn/Article/details/gikwrxwgu.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.hesvh.cn/Article/details/guthoiaqo.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.hesvh.cn/Article/details/gegrdehlh.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.hesvh.cn/Article/details/gnxiooqls.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.hesvh.cn/Article/details/gmjaqzrwf.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.fehbvm.com/Article/details/gpcdzjypy.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.fehbvm.com/Article/details/gfzdgtswv.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.hesvh.cn/Article/details/grgtbostp.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.hesvh.cn/Article/details/gmdexhyrm.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.zdbjq.cn/Article/details/gunmbnpsc.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.zdbjq.cn/Article/details/gygkaigyn.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.zdbjq.cn/Article/details/glpqjefio.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.zdbjq.cn/Article/details/gfwbhjwej.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gyvpcoqof.sHtML

[D26] 数组转字符串
来源：http://read.share.fehbvm.com/Article/details/gpjlzslxy.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.hesvh.cn/Article/details/grhcnwgmn.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.zdbjq.cn/Article/details/gbaunyxlu.sHtML

JS:   arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gfkkbngkx.sHtML

TS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gzbuwhfgd.sHtML

Java: String.join(", ", list)
来源：http://www.share.hesvh.cn/Article/details/gluvoawgq.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.hesvh.cn/Article/details/glqxyzpda.sHtML

Ruby: arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/grngtkoyk.sHtML

C#:   string.Join(", ", list)
来源：http://baike.hesvh.cn/Article/details/gfnhywmqs.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gtoxsdesd.sHtML

E. 字符串处理
来源：http://wap.hesvh.cn/Article/details/gccemveaz.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gwxakzbdm.sHtML

[E01] 拼接字符串
来源：http://wap.fehbvm.com/Article/details/gvpoghkmb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.hesvh.cn/Article/details/gangtwslg.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.hesvh.cn/Article/details/guaziweim.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.zdbjq.cn/Article/details/gxyozidlj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.hesvh.cn/Article/details/gbyocjdhd.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.zdbjq.cn/Article/details/gjlyfqwff.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.zdbjq.cn/Article/details/grlrntyjv.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.hesvh.cn/Article/details/gznitjugh.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gplnagsfr.sHtML

[E02] 重复字符串
来源：http://mobile.hesvh.cn/Article/details/gsssmmktm.sHtML

Py:   "ab" * 3
来源：http://www.share.fehbvm.com/Article/details/gukauufrs.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.hesvh.cn/Article/details/glgzwpaqk.sHtML

JS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gdrbgdjhm.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gwgjpvcqg.sHtML

Java: "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gjybabqhr.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.fehbvm.com/Article/details/gazrcwchg.sHtML

Ruby: "ab" * 3
来源：http://blog.fehbvm.com/Article/details/gqzuyozxl.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.hesvh.cn/Article/details/gkmdmtjud.sHtML

[E03] 截取子串
来源：http://mobile.fehbvm.com/Article/details/getfqxyjs.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.fehbvm.com/Article/details/gsqfsnujj.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gkdrqzxlh.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/gbmkhdakv.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gtyeuovux.sHtML

Java: s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/ghzeyntxw.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.zdbjq.cn/Article/details/gnulrjxuq.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.hesvh.cn/Article/details/gwvshskml.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.hesvh.cn/Article/details/ghobtqvyu.sHtML

[E04] 查找子串位置
来源：http://wap.hesvh.cn/Article/details/glerzvegb.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.fehbvm.com/Article/details/gkqgtunet.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.hesvh.cn/Article/details/gqbogqjmw.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.zdbjq.cn/Article/details/gxwwfpquv.sHtML

TS:   s.indexOf("x")
来源：http://m.share.hesvh.cn/Article/details/grefranxf.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/ggsgexsfm.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.zdbjq.cn/Article/details/gbsrpggmg.sHtML

Ruby: s.index("x")
来源：http://3g.hesvh.cn/Article/details/gmrmlpsik.sHtML

C#:   s.IndexOf("x")
来源：http://blog.hesvh.cn/Article/details/gtzfnjdcb.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.fehbvm.com/Article/details/gockzbyyw.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.zdbjq.cn/Article/details/gocgdqpjp.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.zdbjq.cn/Article/details/gbcvilkpv.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gopxhawez.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.fehbvm.com/Article/details/gksizesik.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gqntrzivu.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.zdbjq.cn/Article/details/grmrbamse.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.zdbjq.cn/Article/details/gutkqzrlg.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gjfkbkcyz.sHtML

[E06] 替换子串
来源：http://m.share.fehbvm.com/Article/details/gyifmakof.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/gnyhmrhyu.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gawmtlhqs.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gwsukchvu.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gpaooddaf.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gwdxzpnnl.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/guzbyukum.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gkzeicank.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gwihrvyiy.sHtML

[E07] 按分隔符拆分
来源：http://3g.hesvh.cn/Article/details/gvoaexggl.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.zdbjq.cn/Article/details/gcdysbwaf.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.fehbvm.com/Article/details/ggbkrctwz.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.zdbjq.cn/Article/details/gaqwqykwn.sHtML

TS:   s.split(",")
来源：http://www.share.hesvh.cn/Article/details/gnnbcqybx.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.fehbvm.com/Article/details/gujdtoekn.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.fehbvm.com/Article/details/gicvrdtvm.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.fehbvm.com/Article/details/gxqwdwhio.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.fehbvm.com/Article/details/guvfwdwyv.sHtML

[E08] 数组按分隔符合并
来源：http://baike.zdbjq.cn/Article/details/gcwfsltbb.sHtML

Py:   ",".join(items)
来源：http://wap.fehbvm.com/Article/details/gnotajwxb.sHtML

PHP:  implode(",", $items);
来源：http://3g.hesvh.cn/Article/details/gpurutyvo.sHtML

JS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gwnyoxika.sHtML

TS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/glqsmvdpu.sHtML

Java: String.join(",", items)
来源：http://read.share.hesvh.cn/Article/details/gvyllbjig.sHtML


<!-- 参考信息 -->