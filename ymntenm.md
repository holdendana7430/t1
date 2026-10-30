代发 wailian999

Go:   arr := []int{1, 2, 3}
来源：http://blog.hesvh.cn/Article/details/guhhryuhj.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.fehbvm.com/Article/details/gekxnbkqx.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.zdbjq.cn/Article/details/grdbwihbd.sHtML

[D02] 追加元素到末尾
来源：http://wap.zdbjq.cn/Article/details/garixtjmt.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.zdbjq.cn/Article/details/gdfexsxzk.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.fehbvm.com/Article/details/guirsnkzu.sHtML

JS:   arr.push(4);
来源：http://baike.hesvh.cn/Article/details/gbvzigglt.sHtML

TS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/gaohtvgbl.sHtML

Java: list.add(4);
来源：http://www.blog.hesvh.cn/Article/details/gueohcndm.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.zdbjq.cn/Article/details/gynpodpjj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.fehbvm.com/Article/details/gylnemtzn.sHtML

C#:   list.Add(4);
来源：http://www.blog.hesvh.cn/Article/details/gdyirckid.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.fehbvm.com/Article/details/goxtegpzo.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.hesvh.cn/Article/details/gnarqauqh.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.hesvh.cn/Article/details/gbjoilclc.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.fehbvm.com/Article/details/gyynjblnq.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.hesvh.cn/Article/details/gwcswykrt.sHtML

Java: list.add(0, 0);
来源：http://www.share.fehbvm.com/Article/details/gjguhktgr.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.fehbvm.com/Article/details/gvpoygwiw.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.fehbvm.com/Article/details/gjhaomxsa.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/ghnwfbubd.sHtML

[D04] 删除元素
来源：http://baike.fehbvm.com/Article/details/gqcizydxu.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.hesvh.cn/Article/details/gqowtjwpy.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gwafbeamj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.hesvh.cn/Article/details/gchafjfxx.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.zdbjq.cn/Article/details/gvqmyalaz.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.zdbjq.cn/Article/details/gvyxsmafs.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.hesvh.cn/Article/details/ghzogmhiz.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.zdbjq.cn/Article/details/gkeelpxjr.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.hesvh.cn/Article/details/gdnbucqtq.sHtML

[D05] 访问与修改元素
来源：http://read.share.hesvh.cn/Article/details/gesvucvxp.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gyuzfpuih.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gmlbxknzg.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/grrmkipfe.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.fehbvm.com/Article/details/gesaligsm.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.fehbvm.com/Article/details/gnrarwhtw.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/ggiofbxgr.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gmtslkxjy.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gmchkwwoc.sHtML

[D06] 数组长度
来源：http://3g.fehbvm.com/Article/details/gmyqtncrq.sHtML

Py:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/gzzqafxgv.sHtML

PHP:  count($arr);
来源：http://3g.fehbvm.com/Article/details/gawncrdpv.sHtML

JS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/giswjekdd.sHtML

TS:   arr.length
来源：http://3g.fehbvm.com/Article/details/ghqqzwbld.sHtML

Java: list.size();
来源：http://www.share.fehbvm.com/Article/details/ghkjttbvi.sHtML

Go:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/gocbumjmv.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.fehbvm.com/Article/details/gnlmzesxr.sHtML

C#:   list.Count;
来源：http://www.share.zdbjq.cn/Article/details/gomgtgaij.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.fehbvm.com/Article/details/gmfoyprlz.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.fehbvm.com/Article/details/gkrldcocz.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.hesvh.cn/Article/details/gitkzgxzw.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gwttdfwcw.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/gcgykitax.sHtML

Java: list.subList(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gqvuluwte.sHtML

Go:   arr[1:4]
来源：http://www.share.fehbvm.com/Article/details/ghhytdyax.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.zdbjq.cn/Article/details/glfteogke.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gexdxctoe.sHtML

[D08] 合并两个数组
来源：http://blog.fehbvm.com/Article/details/giwjtscdu.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.hesvh.cn/Article/details/gtqbyutmf.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.fehbvm.com/Article/details/glspzyjmj.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.hesvh.cn/Article/details/guwmcbjbt.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.fehbvm.com/Article/details/gcojemphf.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.hesvh.cn/Article/details/gjkewbupv.sHtML

Go:   append(a, b...)
来源：http://www.blog.zdbjq.cn/Article/details/gllteouks.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.hesvh.cn/Article/details/gudpsvtrx.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.hesvh.cn/Article/details/grucapbaf.sHtML

[D09] 排序（升序）
来源：http://baike.hesvh.cn/Article/details/goqjmjsdk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gxrnlqjhw.sHtML

PHP:  sort($arr);
来源：http://wap.zdbjq.cn/Article/details/geltdcvhd.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.zdbjq.cn/Article/details/gxzwrfvez.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.hesvh.cn/Article/details/gwjtbacyg.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.hesvh.cn/Article/details/gdjmlnjsv.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gljwdusuv.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/gwtlilcci.sHtML

C#:   list.Sort();
来源：http://blog.zdbjq.cn/Article/details/gowyqtpao.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.zdbjq.cn/Article/details/gudvvjyjx.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.zdbjq.cn/Article/details/gvopnntio.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.hesvh.cn/Article/details/goljxhjgf.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.zdbjq.cn/Article/details/ggodmesws.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/gbscjpuqy.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.hesvh.cn/Article/details/gujxwrbrt.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.hesvh.cn/Article/details/gcqzkvsqp.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.hesvh.cn/Article/details/gqvcqherj.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.fehbvm.com/Article/details/gtjbhauiv.sHtML

[D11] 反转数组
来源：http://www.blog.zdbjq.cn/Article/details/giishhtnq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.hesvh.cn/Article/details/gwnlsccij.sHtML

PHP:  array_reverse($arr);
来源：http://3g.fehbvm.com/Article/details/gveiekydf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.hesvh.cn/Article/details/gbqroikhp.sHtML

TS:   [...arr].reverse();
来源：http://baike.hesvh.cn/Article/details/ghwafsscy.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.hesvh.cn/Article/details/ghndnanih.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.zdbjq.cn/Article/details/givdwgjga.sHtML

Ruby: arr.reverse
来源：http://mobile.fehbvm.com/Article/details/ggmkmkkou.sHtML

C#:   list.Reverse();
来源：http://www.share.hesvh.cn/Article/details/gfkwygkvw.sHtML

[D12] 查找元素下标
来源：http://www.blog.hesvh.cn/Article/details/gizfyyhnz.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.fehbvm.com/Article/details/goiejpnzw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.hesvh.cn/Article/details/gejpkysxm.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/gnhzfgkif.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/gptbhpjhg.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.fehbvm.com/Article/details/giclrzgqk.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/glcgmqvmb.sHtML

Ruby: arr.index(x)
来源：http://blog.hesvh.cn/Article/details/gvocafczk.sHtML

C#:   list.IndexOf(x);
来源：http://blog.hesvh.cn/Article/details/gjpmiphoj.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.hesvh.cn/Article/details/gsrdcwapt.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.hesvh.cn/Article/details/grbgirxzh.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.hesvh.cn/Article/details/gbqdflngx.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gztufykhe.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/gypzyzdks.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.zdbjq.cn/Article/details/gquojzmlj.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.zdbjq.cn/Article/details/gjphqieqt.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.zdbjq.cn/Article/details/ghcharcge.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.zdbjq.cn/Article/details/gkjbzpmut.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.hesvh.cn/Article/details/ghghtwlld.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gwaqrflai.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gxayuwvup.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.hesvh.cn/Article/details/ggrctxaxa.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/gtaoirzxr.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.fehbvm.com/Article/details/gronyurqx.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/gemyhfckb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.fehbvm.com/Article/details/gaedvabrj.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.zdbjq.cn/Article/details/gncyhqjsa.sHtML

[D15] 去重
来源：http://m.share.fehbvm.com/Article/details/gxpuvoitj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/gwheaxdqp.sHtML

PHP:  array_unique($arr);
来源：http://www.share.fehbvm.com/Article/details/gsrzjiupe.sHtML

JS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/ghpolwcal.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gvgfucwbf.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.hesvh.cn/Article/details/gbfasmzuy.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.hesvh.cn/Article/details/gukuthbbb.sHtML

Ruby: arr.uniq
来源：http://m.share.zdbjq.cn/Article/details/gifcspphl.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.zdbjq.cn/Article/details/gxrfiodoz.sHtML

[D16] 求和与平均值
来源：http://read.share.zdbjq.cn/Article/details/gvotjirrf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.hesvh.cn/Article/details/gwvweyqsy.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.hesvh.cn/Article/details/gmoftrjos.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/gfbxnwjhm.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gqnewxphd.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.hesvh.cn/Article/details/guidmviho.sHtML

Go:   // 手写循环累加
来源：http://read.share.fehbvm.com/Article/details/gkwymsiaf.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.fehbvm.com/Article/details/ghhrdfkba.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.hesvh.cn/Article/details/gkkxvxyry.sHtML

[D17] 最大值与最小值
来源：http://read.share.zdbjq.cn/Article/details/grvelnumb.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.hesvh.cn/Article/details/gfgzifglq.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.fehbvm.com/Article/details/gmaxcwwrd.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.hesvh.cn/Article/details/giifxjimo.sHtML

TS:   Math.max(...arr);
来源：http://wap.fehbvm.com/Article/details/glmuakxuc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.fehbvm.com/Article/details/gfbrhvvpd.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.hesvh.cn/Article/details/gzadjcqdh.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.zdbjq.cn/Article/details/gjyarlzpa.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.zdbjq.cn/Article/details/gbundeiui.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.zdbjq.cn/Article/details/gdvqgdfvz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.zdbjq.cn/Article/details/gsviojrej.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.hesvh.cn/Article/details/gttstbvfg.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.hesvh.cn/Article/details/gpaoookck.sHtML

TS:   nested.flat();
来源：http://www.m.share.fehbvm.com/Article/details/gehqtbwdr.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.zdbjq.cn/Article/details/getxaorpi.sHtML

Go:   // 手写双层循环
来源：http://mobile.fehbvm.com/Article/details/gyemlcwbe.sHtML

Ruby: nested.flatten
来源：http://mobile.fehbvm.com/Article/details/guuuzupqg.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.zdbjq.cn/Article/details/gpszqyaio.sHtML

[D19] 按字段分组
来源：http://www.m.share.zdbjq.cn/Article/details/gpnbrvbxo.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.fehbvm.com/Article/details/grvmiuugs.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.hesvh.cn/Article/details/glduduhjr.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.zdbjq.cn/Article/details/ghsnvrkvo.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/gnyhojnqr.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.fehbvm.com/Article/details/gqzpmgasp.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.zdbjq.cn/Article/details/ggzkwoncn.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.zdbjq.cn/Article/details/gequnuvjm.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.fehbvm.com/Article/details/grfgtormc.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.hesvh.cn/Article/details/gbiitxbsv.sHtML

Py:   Counter(arr)
来源：http://read.share.hesvh.cn/Article/details/gdxphnbfl.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.fehbvm.com/Article/details/grbcylkwu.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gounfudjj.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/ggwzraxxi.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.zdbjq.cn/Article/details/giiaxnrgl.sHtML

Go:   // 手写 map[T]int
来源：http://3g.zdbjq.cn/Article/details/gojlpwfmf.sHtML

Ruby: arr.tally
来源：http://read.share.fehbvm.com/Article/details/gsgokfulq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.hesvh.cn/Article/details/gyxqylnth.sHtML

[D21] 判断是否包含某元素
来源：http://baike.zdbjq.cn/Article/details/gswmiuzjw.sHtML

Py:   x in arr
来源：http://blog.hesvh.cn/Article/details/gxpfiwhbe.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.zdbjq.cn/Article/details/gaoidvdib.sHtML

JS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gngulzbdb.sHtML

TS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/gjfjlfnql.sHtML

Java: list.contains(x)
来源：http://3g.zdbjq.cn/Article/details/gdntivkvo.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gzcyscpxf.sHtML

Ruby: arr.include?(x)
来源：http://baike.zdbjq.cn/Article/details/gzqkiampl.sHtML

C#:   list.Contains(x)
来源：http://www.share.zdbjq.cn/Article/details/ghwcrejkd.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.fehbvm.com/Article/details/gvolywvxa.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.hesvh.cn/Article/details/gxkbnjvvu.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.hesvh.cn/Article/details/gmywflqxe.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gahltqmqt.sHtML

TS:   [...arr];
来源：http://read.share.fehbvm.com/Article/details/gsgfhbueu.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.hesvh.cn/Article/details/grpetrzyo.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.hesvh.cn/Article/details/gxfihxgqk.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.hesvh.cn/Article/details/goiusphxo.sHtML

C#:   new List<int>(list);
来源：http://3g.hesvh.cn/Article/details/gdhszvqac.sHtML

[D23] reduce 累积计算
来源：http://read.share.hesvh.cn/Article/details/ghbzbqmot.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.hesvh.cn/Article/details/gvjcxpzvj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.zdbjq.cn/Article/details/gfgcapvom.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gdyasctel.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.hesvh.cn/Article/details/gdggrfdak.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.zdbjq.cn/Article/details/gjuwjkaqx.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gefpnfhqe.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.hesvh.cn/Article/details/gnthtokfd.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.zdbjq.cn/Article/details/gkdqauawn.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.zdbjq.cn/Article/details/gbkwtylbn.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.hesvh.cn/Article/details/giizxtpny.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.hesvh.cn/Article/details/gldqsxbuo.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.zdbjq.cn/Article/details/gozdlgcia.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/ggfdimpui.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.fehbvm.com/Article/details/gmqbipqbd.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.hesvh.cn/Article/details/garxumlvv.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.zdbjq.cn/Article/details/gtvnheqsn.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.fehbvm.com/Article/details/gymjtmupj.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.zdbjq.cn/Article/details/gyohwuzot.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.hesvh.cn/Article/details/gskqaabsf.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.fehbvm.com/Article/details/gdlleumyj.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.hesvh.cn/Article/details/ghyamxcfb.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.fehbvm.com/Article/details/gcjxrnlvj.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.fehbvm.com/Article/details/gbqshupvi.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.zdbjq.cn/Article/details/gygkciomu.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.fehbvm.com/Article/details/gfqztpgop.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.hesvh.cn/Article/details/grzhaljki.sHtML

[D26] 数组转字符串
来源：http://m.share.zdbjq.cn/Article/details/gzuewfjwx.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gpfcvucfr.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.zdbjq.cn/Article/details/geuzbtlbq.sHtML

JS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gqyyjfyzc.sHtML

TS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gzfqtskhy.sHtML

Java: String.join(", ", list)
来源：http://www.blog.hesvh.cn/Article/details/gjjziyxhn.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.hesvh.cn/Article/details/gxngkrmzo.sHtML

Ruby: arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gbvdjweue.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/gfooayrpj.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gzhkcfsud.sHtML

E. 字符串处理
来源：http://mobile.zdbjq.cn/Article/details/gvlvibbuf.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/grfvxvgnf.sHtML

[E01] 拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gradbdfgj.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.hesvh.cn/Article/details/gejnzikad.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gaigvrcxs.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.hesvh.cn/Article/details/guvfdlsin.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/gtqdswxyb.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.fehbvm.com/Article/details/guozyvopu.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.fehbvm.com/Article/details/gnzbnzfun.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.hesvh.cn/Article/details/ghjdrmixv.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gwdopdrrl.sHtML

[E02] 重复字符串
来源：http://www.m.share.fehbvm.com/Article/details/gdjkwlfqu.sHtML

Py:   "ab" * 3
来源：http://m.share.hesvh.cn/Article/details/gmwjeygui.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.zdbjq.cn/Article/details/gnrnojeph.sHtML

JS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gvrkckana.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gdixkzdlq.sHtML

Java: "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gsiepjuln.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.zdbjq.cn/Article/details/grahkxeuf.sHtML

Ruby: "ab" * 3
来源：http://wap.fehbvm.com/Article/details/gwbwmjdfn.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.fehbvm.com/Article/details/gyshfzmta.sHtML

[E03] 截取子串
来源：http://wap.hesvh.cn/Article/details/gitcdmzdl.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.zdbjq.cn/Article/details/gjvfvoseh.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gohgnllol.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/glzcanhra.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gtfoswoxd.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/ggfbrdjla.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.fehbvm.com/Article/details/gsuzideob.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.hesvh.cn/Article/details/ggcumgthn.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.hesvh.cn/Article/details/gaiywblko.sHtML

[E04] 查找子串位置
来源：http://read.share.fehbvm.com/Article/details/gygstclct.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gdzfzjhvm.sHtML

PHP:  strpos($s, "x");
来源：http://3g.hesvh.cn/Article/details/gzhzsahuq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.fehbvm.com/Article/details/gnjjmcpjk.sHtML

TS:   s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gtdmmcijv.sHtML

Java: s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/genpgqecu.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.hesvh.cn/Article/details/gscmftrss.sHtML

Ruby: s.index("x")
来源：http://m.share.fehbvm.com/Article/details/gbrflwofb.sHtML

C#:   s.IndexOf("x")
来源：http://blog.fehbvm.com/Article/details/gtmxackmu.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.fehbvm.com/Article/details/gfbnknjkb.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.zdbjq.cn/Article/details/gmcpgnpmh.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.hesvh.cn/Article/details/gmdwpptjq.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.hesvh.cn/Article/details/gwjeciltf.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.zdbjq.cn/Article/details/gyqdbhtzn.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/gfwvtosxf.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.zdbjq.cn/Article/details/gwlkeevmk.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.zdbjq.cn/Article/details/gvstzvhzs.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.fehbvm.com/Article/details/gwzujnvit.sHtML

[E06] 替换子串
来源：http://3g.zdbjq.cn/Article/details/glmovykmq.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/ghbrqyfcw.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.fehbvm.com/Article/details/gjbvkvglm.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gqlgenbwt.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/glenylprb.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/guhehxbas.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/gmxdmscew.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.hesvh.cn/Article/details/giieqanpm.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.hesvh.cn/Article/details/gnfiewubl.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.hesvh.cn/Article/details/gimpwvrww.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.fehbvm.com/Article/details/grajtcvaa.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gnvausmwj.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.zdbjq.cn/Article/details/geptpqkjq.sHtML

TS:   s.split(",")
来源：http://www.share.zdbjq.cn/Article/details/girkflrgx.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.hesvh.cn/Article/details/gjjaridle.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.fehbvm.com/Article/details/gqauzuoie.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.hesvh.cn/Article/details/gwzzkmnsz.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.fehbvm.com/Article/details/gfkgudnip.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.fehbvm.com/Article/details/gxzyogtfx.sHtML

Py:   ",".join(items)
来源：http://mobile.zdbjq.cn/Article/details/gvpccobju.sHtML

PHP:  implode(",", $items);
来源：http://www.share.zdbjq.cn/Article/details/gkztbejew.sHtML

JS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/gyjjvfrjo.sHtML

TS:   items.join(",")
来源：http://www.share.hesvh.cn/Article/details/glhhowjdj.sHtML

Java: String.join(",", items)
来源：http://m.share.fehbvm.com/Article/details/gvzgggctu.sHtML


<!-- 参考信息 -->