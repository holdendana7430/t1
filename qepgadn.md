代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.hesvh.cn/Article/details/gnhkxrtco.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.zdbjq.cn/Article/details/gqqdoyxun.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.fehbvm.com/Article/details/gdixbhibi.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.hesvh.cn/Article/details/gmeikfxmj.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.fehbvm.com/Article/details/gnmvdgoes.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.fehbvm.com/Article/details/gdywcnlip.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.hesvh.cn/Article/details/gmulkcxqj.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.zdbjq.cn/Article/details/gvgrmjytz.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.hesvh.cn/Article/details/ggtjzxsgw.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.fehbvm.com/Article/details/gnbjiabwt.sHtML

JS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/gzatbmouk.sHtML

TS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/gesdmosse.sHtML

Java: list.add(4);
来源：http://www.share.fehbvm.com/Article/details/gskdumpww.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gxmhxtvws.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.fehbvm.com/Article/details/gyevrvwht.sHtML

C#:   list.Add(4);
来源：http://wap.fehbvm.com/Article/details/gkqnhjpwu.sHtML

[D03] 在指定位置插入元素
来源：http://baike.hesvh.cn/Article/details/gfxxtcima.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.zdbjq.cn/Article/details/gzubiuynw.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.zdbjq.cn/Article/details/gvvlisjcj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.hesvh.cn/Article/details/gsriozamw.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.hesvh.cn/Article/details/gywswokvf.sHtML

Java: list.add(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gpsofxuhp.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.hesvh.cn/Article/details/gqyzqqvdj.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.fehbvm.com/Article/details/gtszsqhnw.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.hesvh.cn/Article/details/gradgdzyr.sHtML

[D04] 删除元素
来源：http://www.share.fehbvm.com/Article/details/glenhebhb.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.fehbvm.com/Article/details/gjaimysif.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gnlttqbxh.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.fehbvm.com/Article/details/gmdtfrlws.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.fehbvm.com/Article/details/gnnmhyxgs.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.hesvh.cn/Article/details/gdysgbzin.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.zdbjq.cn/Article/details/gxhwqlynw.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.zdbjq.cn/Article/details/gypfdqrnb.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.fehbvm.com/Article/details/gapdkvfwt.sHtML

[D05] 访问与修改元素
来源：http://wap.zdbjq.cn/Article/details/ggakklmok.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gdtrhxgoc.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gmipeyffm.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gtmfgbmad.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.hesvh.cn/Article/details/gpenkhomk.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.zdbjq.cn/Article/details/galzkljrj.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gdzerfxhe.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gloxaxtee.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gdkisblyd.sHtML

[D06] 数组长度
来源：http://mobile.fehbvm.com/Article/details/gvcverfch.sHtML

Py:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/gcxwlqtni.sHtML

PHP:  count($arr);
来源：http://m.share.hesvh.cn/Article/details/gbbnbzupr.sHtML

JS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gxfcpkght.sHtML

TS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/gqwinmshz.sHtML

Java: list.size();
来源：http://www.m.share.fehbvm.com/Article/details/gzavdabtc.sHtML

Go:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/gremjdwii.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.fehbvm.com/Article/details/gyywnpjml.sHtML

C#:   list.Count;
来源：http://m.share.fehbvm.com/Article/details/ghhikudxl.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.hesvh.cn/Article/details/gcoeqcsed.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.zdbjq.cn/Article/details/gdaoyssuh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/guxvjwltb.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gkjbomdyr.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gthccylyy.sHtML

Java: list.subList(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gcfssruxf.sHtML

Go:   arr[1:4]
来源：http://www.share.hesvh.cn/Article/details/gfovqiiuh.sHtML

Ruby: arr[1, 3]
来源：http://blog.fehbvm.com/Article/details/gfzdulcnd.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.fehbvm.com/Article/details/gvohnhciq.sHtML

[D08] 合并两个数组
来源：http://read.share.zdbjq.cn/Article/details/gbhuhnpzt.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.zdbjq.cn/Article/details/genclcqcv.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.fehbvm.com/Article/details/gkreetggg.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.zdbjq.cn/Article/details/gnljpfwtl.sHtML

TS:   [...a, ...b];
来源：http://mobile.hesvh.cn/Article/details/gawafmmwv.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.fehbvm.com/Article/details/gxrcqyozl.sHtML

Go:   append(a, b...)
来源：http://www.share.hesvh.cn/Article/details/gqwhhlvhb.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.fehbvm.com/Article/details/guyyvioqm.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gejosuzwz.sHtML

[D09] 排序（升序）
来源：http://wap.hesvh.cn/Article/details/grfecrwbx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gbsdjvjvz.sHtML

PHP:  sort($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gauprpzim.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.hesvh.cn/Article/details/gxncndved.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.fehbvm.com/Article/details/gsvfqxxmm.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.hesvh.cn/Article/details/gqwcdvpki.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gtpgnbsfp.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/gtskxwpzo.sHtML

C#:   list.Sort();
来源：http://m.share.zdbjq.cn/Article/details/goukzgmbe.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.hesvh.cn/Article/details/gdrfslxsf.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.hesvh.cn/Article/details/ghdmgoxkr.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fehbvm.com/Article/details/gdkjeajqf.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/guiyzoouz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/grbjyacfn.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.fehbvm.com/Article/details/gmnkgwrlc.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.zdbjq.cn/Article/details/gyysarhsr.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.zdbjq.cn/Article/details/ggimwieak.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.hesvh.cn/Article/details/gcsynuomc.sHtML

[D11] 反转数组
来源：http://www.share.hesvh.cn/Article/details/gzzofpjct.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.zdbjq.cn/Article/details/geeabrmui.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.hesvh.cn/Article/details/gybwqfibm.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.hesvh.cn/Article/details/gqzybkskf.sHtML

TS:   [...arr].reverse();
来源：http://www.share.zdbjq.cn/Article/details/gubrimvcv.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.fehbvm.com/Article/details/gmlacdyjx.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.fehbvm.com/Article/details/gpbixgqpp.sHtML

Ruby: arr.reverse
来源：http://wap.fehbvm.com/Article/details/grmdovtnp.sHtML

C#:   list.Reverse();
来源：http://www.share.fehbvm.com/Article/details/gklycpacu.sHtML

[D12] 查找元素下标
来源：http://www.share.fehbvm.com/Article/details/ggjabupsy.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.hesvh.cn/Article/details/guuhjuuwp.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.fehbvm.com/Article/details/gkookcgcz.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gdrayaxis.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/guusmnpma.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.zdbjq.cn/Article/details/grusxnokg.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.zdbjq.cn/Article/details/galsfwsgo.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.fehbvm.com/Article/details/gtkoxrjfj.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.hesvh.cn/Article/details/gzctotwvg.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.fehbvm.com/Article/details/gfetlbzjh.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.hesvh.cn/Article/details/gmzrscgvd.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.fehbvm.com/Article/details/gfibuzyui.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gjmqatsgb.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/gmproorrh.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.hesvh.cn/Article/details/gegpawnzr.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.hesvh.cn/Article/details/gmhbcrrcc.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.hesvh.cn/Article/details/glixrdsul.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.fehbvm.com/Article/details/ggvpmmqaw.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.zdbjq.cn/Article/details/gnrvkfcxt.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.fehbvm.com/Article/details/gziujlczq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.zdbjq.cn/Article/details/gwanrppsu.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/gpancrfgw.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/gkqdkvfnn.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gzgexvdcp.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/gbifpddyq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/ghebwwcno.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gbytrqdix.sHtML

[D15] 去重
来源：http://3g.hesvh.cn/Article/details/gaiskzecc.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/gzhelikzb.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.zdbjq.cn/Article/details/grlmzkxub.sHtML

JS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gekfsvpjl.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/giopqaatu.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.zdbjq.cn/Article/details/glmiwnalc.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.zdbjq.cn/Article/details/gtuedmmsj.sHtML

Ruby: arr.uniq
来源：http://read.share.hesvh.cn/Article/details/gmpmmvzgl.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.fehbvm.com/Article/details/gldvhvitv.sHtML

[D16] 求和与平均值
来源：http://www.m.share.fehbvm.com/Article/details/gjnzqfneg.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.fehbvm.com/Article/details/gsivwnwrh.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.fehbvm.com/Article/details/ghzvdvtmc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/gmoeiincu.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fehbvm.com/Article/details/ghweixkyq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.hesvh.cn/Article/details/gyzsqpewy.sHtML

Go:   // 手写循环累加
来源：http://m.share.zdbjq.cn/Article/details/gezstdptw.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.hesvh.cn/Article/details/gvclazkix.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.hesvh.cn/Article/details/gwxeodmfz.sHtML

[D17] 最大值与最小值
来源：http://wap.fehbvm.com/Article/details/gsyabucdk.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.fehbvm.com/Article/details/gvlfnksci.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.fehbvm.com/Article/details/ghuqjamvu.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gjaaipmpj.sHtML

TS:   Math.max(...arr);
来源：http://3g.hesvh.cn/Article/details/gvmalwasn.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.fehbvm.com/Article/details/gcessdqct.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.zdbjq.cn/Article/details/grvzxgfko.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.fehbvm.com/Article/details/gvhkdggwv.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.hesvh.cn/Article/details/gmvfooyof.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.zdbjq.cn/Article/details/gikfpkycf.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.zdbjq.cn/Article/details/gromvvwej.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.zdbjq.cn/Article/details/gcxshzysc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.fehbvm.com/Article/details/gvqnjwipn.sHtML

TS:   nested.flat();
来源：http://mobile.zdbjq.cn/Article/details/grhzakntb.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.fehbvm.com/Article/details/gdfypinay.sHtML

Go:   // 手写双层循环
来源：http://www.share.hesvh.cn/Article/details/gmwwkmhac.sHtML

Ruby: nested.flatten
来源：http://www.blog.hesvh.cn/Article/details/gbgbftkwy.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.fehbvm.com/Article/details/gqheoqfvp.sHtML

[D19] 按字段分组
来源：http://wap.fehbvm.com/Article/details/gdrwvtxzq.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.hesvh.cn/Article/details/gwbpintve.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.fehbvm.com/Article/details/gjubscdut.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.fehbvm.com/Article/details/gljlhuuhg.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/gzrlcorav.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.fehbvm.com/Article/details/gewwytwpx.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.zdbjq.cn/Article/details/gtwmyoarb.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.fehbvm.com/Article/details/gxnjxohiu.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.fehbvm.com/Article/details/gbejvgcfg.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.zdbjq.cn/Article/details/gntjqmjvm.sHtML

Py:   Counter(arr)
来源：http://mobile.zdbjq.cn/Article/details/gcmqvziso.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.hesvh.cn/Article/details/gxatkfjwt.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/guktiovde.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/giohkehdg.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.hesvh.cn/Article/details/gblqianaf.sHtML

Go:   // 手写 map[T]int
来源：http://3g.hesvh.cn/Article/details/gixwhrcps.sHtML

Ruby: arr.tally
来源：http://www.m.share.zdbjq.cn/Article/details/gfzjtmnht.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.hesvh.cn/Article/details/gqypoqfsr.sHtML

[D21] 判断是否包含某元素
来源：http://wap.hesvh.cn/Article/details/gbpvrcupm.sHtML

Py:   x in arr
来源：http://read.share.hesvh.cn/Article/details/gfzirsbml.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.hesvh.cn/Article/details/gckjdsjck.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/ggcsvexvb.sHtML

TS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/gliinmugt.sHtML

Java: list.contains(x)
来源：http://3g.hesvh.cn/Article/details/gdtaawzlu.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.hesvh.cn/Article/details/gqkayfnik.sHtML

Ruby: arr.include?(x)
来源：http://blog.hesvh.cn/Article/details/gthkdnhht.sHtML

C#:   list.Contains(x)
来源：http://m.share.hesvh.cn/Article/details/gasmyasfk.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.zdbjq.cn/Article/details/gjczrsmxh.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.zdbjq.cn/Article/details/gnktbdaln.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.fehbvm.com/Article/details/gbqeecwcc.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.zdbjq.cn/Article/details/gmxlcyadc.sHtML

TS:   [...arr];
来源：http://www.share.hesvh.cn/Article/details/gzumzqcsn.sHtML

Java: new ArrayList<>(list);
来源：http://wap.zdbjq.cn/Article/details/gjtlacclo.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.fehbvm.com/Article/details/gnmjrqhzt.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.hesvh.cn/Article/details/gvrwbkqjk.sHtML

C#:   new List<int>(list);
来源：http://3g.zdbjq.cn/Article/details/gxpogyziq.sHtML

[D23] reduce 累积计算
来源：http://mobile.zdbjq.cn/Article/details/gmdwbjtxj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.hesvh.cn/Article/details/gspfetssa.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.fehbvm.com/Article/details/gksgtrgca.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/gbohlwtem.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gcbdfdpph.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.fehbvm.com/Article/details/gqphsqxxe.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/gvamooylr.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.zdbjq.cn/Article/details/gadflqhso.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.zdbjq.cn/Article/details/gpajdridn.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.hesvh.cn/Article/details/gvdwlbdjf.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.fehbvm.com/Article/details/gfiualwpu.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.hesvh.cn/Article/details/ghqpedkbb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.zdbjq.cn/Article/details/ginaofewd.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.fehbvm.com/Article/details/gitdrerry.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.hesvh.cn/Article/details/gfxvwqbds.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.fehbvm.com/Article/details/gwuojdnpq.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.zdbjq.cn/Article/details/gaupbjxol.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.hesvh.cn/Article/details/gqpbsstbs.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.zdbjq.cn/Article/details/gmoaybykh.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.hesvh.cn/Article/details/gdhirsven.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.fehbvm.com/Article/details/ggccymbqt.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.hesvh.cn/Article/details/gfufsoicb.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.zdbjq.cn/Article/details/ghzqysarl.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.zdbjq.cn/Article/details/gacqifkar.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.hesvh.cn/Article/details/gbebovgbo.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.hesvh.cn/Article/details/gatdgxdib.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/gklmbruvy.sHtML

[D26] 数组转字符串
来源：http://www.blog.hesvh.cn/Article/details/gyweytcae.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.fehbvm.com/Article/details/gagkxtlcz.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.hesvh.cn/Article/details/gykhnyukg.sHtML

JS:   arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gqcgskhbz.sHtML

TS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/ghuxwmxpa.sHtML

Java: String.join(", ", list)
来源：http://blog.zdbjq.cn/Article/details/goglskbtw.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.zdbjq.cn/Article/details/gihpmuocv.sHtML

Ruby: arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gkrsfwgel.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/gpebdgycp.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/grqnyglfs.sHtML

E. 字符串处理
来源：http://3g.zdbjq.cn/Article/details/gnkqiwxvv.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gcukntroi.sHtML

[E01] 拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gcsohltbl.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.zdbjq.cn/Article/details/gmqfkniyi.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.fehbvm.com/Article/details/gusyxoskh.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.hesvh.cn/Article/details/gmjccjnzm.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/gxwnbghmf.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.hesvh.cn/Article/details/gokmvuito.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.hesvh.cn/Article/details/gohsopjgk.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.fehbvm.com/Article/details/gfjhqpfgu.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gkgpoavko.sHtML

[E02] 重复字符串
来源：http://baike.fehbvm.com/Article/details/gnjkrycxh.sHtML

Py:   "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/ganipujcy.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.zdbjq.cn/Article/details/gwqzucqkx.sHtML

JS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gptfhgxen.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gsfgnysle.sHtML

Java: "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gxnifwvav.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.fehbvm.com/Article/details/gydhcykiy.sHtML

Ruby: "ab" * 3
来源：http://baike.hesvh.cn/Article/details/ggpfsqepo.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.zdbjq.cn/Article/details/gznzqoxkf.sHtML

[E03] 截取子串
来源：http://baike.fehbvm.com/Article/details/gcvrahfim.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.zdbjq.cn/Article/details/gnukyihqr.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gjjfcenum.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/glohwlbzq.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gvifyrjzj.sHtML

Java: s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gqavagqqf.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.fehbvm.com/Article/details/gdnhgmgbn.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.hesvh.cn/Article/details/gzsoecwem.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.zdbjq.cn/Article/details/ghvyqvxay.sHtML

[E04] 查找子串位置
来源：http://www.share.hesvh.cn/Article/details/gleoiglmm.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.zdbjq.cn/Article/details/gqsapelbz.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.fehbvm.com/Article/details/gkesccovc.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.hesvh.cn/Article/details/gxzcswbbp.sHtML

TS:   s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gblbrziqg.sHtML

Java: s.indexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gwoetfyye.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.hesvh.cn/Article/details/gtykvrjtr.sHtML

Ruby: s.index("x")
来源：http://wap.hesvh.cn/Article/details/ggdcvpqer.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gzlbzqgej.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.zdbjq.cn/Article/details/gohuzsvzx.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.hesvh.cn/Article/details/gricnufum.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.hesvh.cn/Article/details/gydpjgise.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gvzdpcean.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.hesvh.cn/Article/details/glidjtxvt.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gwfyrsbtm.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.hesvh.cn/Article/details/gukozsool.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.hesvh.cn/Article/details/gvhxjlypf.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.fehbvm.com/Article/details/grldqkrgb.sHtML

[E06] 替换子串
来源：http://read.share.zdbjq.cn/Article/details/gmhxgawtp.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/gsoyiurjy.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gdxzexmgx.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gwdzarbbh.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gvovwpews.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gegjkixmy.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gccooibnt.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.hesvh.cn/Article/details/gwuhuclbf.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gwtcpmfzy.sHtML

[E07] 按分隔符拆分
来源：http://mobile.fehbvm.com/Article/details/gpqhkyaki.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.zdbjq.cn/Article/details/gzfgsqdig.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gjrxahmrf.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.zdbjq.cn/Article/details/gricwdhxc.sHtML

TS:   s.split(",")
来源：http://mobile.zdbjq.cn/Article/details/gocbqbekq.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.zdbjq.cn/Article/details/gysxecxcj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.fehbvm.com/Article/details/gqznmeaun.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.hesvh.cn/Article/details/gktwhvbot.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.fehbvm.com/Article/details/gyzmjovpr.sHtML

[E08] 数组按分隔符合并
来源：http://blog.fehbvm.com/Article/details/gclicdgcl.sHtML

Py:   ",".join(items)
来源：http://mobile.hesvh.cn/Article/details/gwneeofgz.sHtML


<!-- 参考信息 -->